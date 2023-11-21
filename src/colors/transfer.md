# Transfer Functions

Transfer functions, also known as transfer characteristics, represent the gamma function of a video--that is, how to convert from a gamma-compressed video to one that is in linear light. These are sometimes also called EOTF and OETF functions. The following values are available:

### 1: BT.1886

BT.1886 is the standard used for most modern, SDR video, and is a safe default assumption.

This transfer function is used in the following standards:

- Rec. ITU-R BT.709-6
- Rec. ITU-R BT.1361-0 conventional
  colour gamut system (historical)

### 2: Unspecified

This value indicates that no transfer function is set for the video, and the player must decide which value to use.

mpv will always assume BT.1886 in this case.

### 4: BT.470M

BT.470M is a standard that was used in analog television systems in the United States. This transfer represents a power function with a gamma of 2.2.

This transfer function is used in the following standards:

- Rec. ITU-R BT.470-6 System M
  (historical)
- United States National Television
  System Committee 1953
  Recommendation for transmission
  standards for color television
- United States Federal Communications
  Commission (2003) Title 47 Code of
  Federal Regulations 73.682 (a) (20)
- Rec. ITU-R BT.1700-0 625 PAL and
  625 SECAM

### 5: BT.470BG

BT.470BG is a standard that was used for European (PAL) television systems and DVDs. This transfer represents a power function with a gamma of 2.8.

### 6: SMPTE 170M

SMPTE 170M is a stanrard that was used for NTSC television systems and DVDs. Its transfer function is equivalent to BT.1886.

This transfer function is used in the following standards:

- Rec. ITU-R BT.601-7 525 or 625
- Rec. ITU-R BT.1358-1 525 or 625
  (historical)
- Rec. ITU-R BT.1700-0 NTSC
- SMPTE ST 170 (2004)

### 7: SMPTE 240M

SMPTE 240M was an interim standard used during the early days of HDTV (1988-1998).

### 8: Linear

This value indicates that the content is already in linear light.

### 9: Logarithmic 100

Indicates a logarithmic transfer function with a 100:1 range.

### 10: Logarithmic 316

Indicates a logarithmic transfer function with a (100 \* sqrt(10)):1 range.

### 11: XVYCC

Used in standard IEC 61966-2-4. I have no idea what this actually is.

### 12: BT.1361E

This was intended to be a standard for "future" television systems, but it never really came into use.

### 13: sRGB

Represents the sRGB colorspace.

This transfer function is used in the following standards:

- IEC 61966-2-1 sRGB (with
  MatrixCoefficients equal to 0)
- IEC 61966-2-1 sYCC (with
  MatrixCoefficients equal to 5)

### 14: BT.2020 10-bit

Typically used with ultra-high-definition 10-bit SDR video. Its transfer function is equivalent to BT.1886.

### 15: BT.2020 12-bit

Typically used with ultra-high-definition 12-bit SDR video. Its transfer function is equivalent to BT.1886.

### 16: PQ aka SMPTE 2084

PQ is the most widely used transfer function for HDR content. It allows for a wider range of luminance to be represented than conventional transfer functions.

This transfer function is used in the following standards:

- SMPTE ST 2084 (2014) for 10-, 12-,
  14- and 16-bit systems
- Rec. ITU-R BT.2100-2 perceptual
  quantization (PQ) system

### 17: SMPTE 428

SMPTE 428 is used for D-Cinema Distribution Masters, aka DCDM.

### 18: HLG aka Hybrid Log-Gamma

HLG is an alternative transfer function for HDR content used by some televisions.

This transfer function is used in the following standards:

- ARIB STD-B67 (2015)
- Rec. ITU-R BT.2100-2 hybrid log-
  gamma (HLG) system
