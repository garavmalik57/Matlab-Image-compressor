# Wavelet DWT Image Compression (MATLAB)

This MATLAB project implements **image compression using 2D Discrete Wavelet Transform (DWT)** with the **Haar wavelet**. The program performs compression on a batch of images from a specified folder, calculates compression ratios, and evaluates the quality of decompressed images using **PSNR (Peak Signal-to-Noise Ratio)**.

---

## Features

- **Batch image compression** using Haar wavelet (DWT2).
- Handles both **grayscale and RGB images**.
- Computes:
  - Compression Ratio
  - PSNR (Image quality)
- Visual comparison between:
  - Original Image
  - Compressed Approximation (coefficients)
  - Decompressed Image (after inverse DWT)

---

## Outputs

- **Compression ratio** for each image.
- **PSNR** value to measure reconstruction quality.
- Visualization of original, compressed, and decompressed images side by side.

---

## How to Use

1. Set the path to your image folder in the script:

   ```matlab
   folder_path = 'C:\Path\To\Your\Images';
   ```

2. Run the MATLAB script to process all `.jpg` images (or modify the extension to `.png`, etc.).

3. Review compression statistics and visual comparisons in MATLAB figures.

---

## Dependencies

- MATLAB (with Wavelet Toolbox)

---

## Notes

- Compression is performed by **retaining only approximation coefficients** (`cA`) and discarding detail coefficients (`cH`, `cV`, `cD`).
- Compressed size is estimated assuming **64 bits per double coefficient**.
- No quantization or entropy encoding applied — this can be added for real-world compression applications.

---

## Example Output

- **Original Image**
- **Compressed Approximation**
- **Decompressed Image**

Each displayed in a side-by-side figure for easy comparison.

---

## Contributors

- [@ayush126kashyap](https://github.com/ayush126kashyap)
- [@garavmalik57](https://github.com/garavmalik57)

---

## License

This project is shared for educational purposes. Feel free to modify and extend it.

