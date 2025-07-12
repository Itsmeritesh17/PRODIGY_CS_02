# PRODIGY_CS_02

## Image Pixel Manipulation for Encryption and Decryption

This project demonstrates a basic approach to image-based encryption and decryption by scrambling and unscrambling pixel positions using a user-defined key. It leverages a graphical interface to allow users to interactively process image files.

## Description

The core concept is to manipulate the pixel data of an image based on a pseudo-random pattern generated using a user-provided key. The same key is required to revert (unscramble) the image to its original form, ensuring basic confidentiality through controlled randomness.

## Features

- Load and view an image file
- Enter a key to control the pixel shuffling
- Encrypt (scramble) image pixels
- Decrypt (unscramble) image using the same key
- Save the encrypted or decrypted image to disk
- Simple and intuitive GUI interface

## Technologies Used

- Python
- Tkinter (for GUI)
- Pillow (for image processing)
- Random (for seeded shuffling based on key)

## How It Works

1. **Encryption**:
   - Pixels are rearranged in a pseudo-random order using a seeded shuffle based on the input key.
   - The scrambled image is visually unrecognizable.

2. **Decryption**:
   - Using the same key, the pixel positions are deterministically restored to their original order.
   - The decrypted image matches the original.

## Usage Instructions

1. Run the script using Python.
2. Select an image (supported formats: PNG, JPG, BMP).
3. Enter a key (string).
4. Click on "Scramble Image" to encrypt or "Unscramble Image" to decrypt.
5. Save the output image when prompted.

## File Structure

- `cs_task2.py`: Main application script with GUI and logic for scrambling and unscrambling image pixels.

## Notes

- The encryption is reversible only with the exact same key.
- This is a conceptual demonstration and not suitable for secure image encryption in real-world cryptographic applications.
