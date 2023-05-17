# Color Range

Range is a concept that describes the valid values for a pixel. Typically, RGB will use full range and YUV will use limited range.

What does this mean?

For 8-bit video, full range indicates that all values between 0-255 may be used to represent a color value. On the other hand, limited range indicates that only values between 16-235, or 16-240 for chroma, are valid, and any values outside that range will be clamped to fit in that range. These ranges do expand appropriately for high bit depth videos as well.

Why is limited range a thing that exists? Essentially, it's due to historical reasons, but it's a convention that we are stuck with today. Even though full range may provide slightly better color accuracy, it is far less meaningful for high bit depth content, and even HDR blu-rays use limited color range. Therefore, it is recommended to follow existing conventions.
