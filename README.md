# Image Compression Using 2D DCT

## Overview

This project implements a simple image compression technique using **2D Discrete Cosine Transform (DCT)**. The compression is achieved by reducing the frequency components of **8x8 pixel blocks** in an image, retaining only the most important parts.

The goal is to explore the balance between image quality and compression, by adjusting the number of DCT coefficients retained.

## Results

- The value of **m** (size of retained DCT coefficients) impacts the compression level:
  - **m = 1**: Highest compression, but lowest image quality.
  - **m = 4**: Lower compression, but better image quality.

**original image**:<br>![image](https://github.com/user-attachments/assets/e8c07e2b-478c-4bec-b6b2-8b8f6b645fe1)
<br>
**sample images compressed(m=1)**:<br>![image](https://github.com/user-attachments/assets/98ebc90e-8629-4ec3-bd49-5174af96c67c)
<br>
**sample images decompressed(m=1)**:<br>![image](https://github.com/user-attachments/assets/c33db77f-acc0-44fb-8b6c-9bde9ef2c4a8)


- The **PSNR (Peak Signal-to-Noise Ratio)** curve shows how image quality improves as `m` increases, with a tradeoff in compression.




## Conclusion

This project demonstrates how the **2D DCT** can be used to achieve image compression while balancing between file size and quality. 
