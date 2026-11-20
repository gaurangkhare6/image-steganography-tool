<h1 align="center">🔐 SECRET MESSAGE IN IMAGE</h1>
<h2 align="center">Image Steganography Tool</h2>

<p align="center"><b>Hide text inside a photo using LSB steganography and a Caesar cipher</b></p>

---

A browser-based tool that hides a secret text message inside an image and reads it back later. It is a single HTML file with no server and no external libraries.

**Student:** Gaurang Khare | **Class:** ELCE-1 | **Roll No:** 2026B02310077
**Faculty:** Mr. Pushparaj Dora | **Institute:** ABES Engineering College, Ghaziabad

## Features
- Generates a paired **Lock Key** and **Unlock Key** from any number
- Scrambles the message with a **Caesar shift cipher**
- Hides the message in the **Least Significant Bits (LSB)** of the image's Red, Green and Blue values
- Downloads the result as a lossless PNG (`secret_photo.png`)
- Shows image size, capacity and a live character counter
- Copy and Clear buttons; everything runs locally in your browser

## How it works
1. **Key Generator:** Lock Key = number x 5, Unlock Key = number x 9
2. **Encode:** the message is shifted, `###STOP###` is added at the end, and the bits go into the image pixels (even value = 0, odd value = 1)
3. **Decode:** the bits are read back until `###STOP###` is found, then the shift is reversed

## How to use
1. Open `image steganography tool.html` in any browser
2. Enter a number and click **Make Keys**
3. Choose a cover photo, paste the Lock Key, type a message and click **Hide & Download Photo**
4. To read it, upload `secret_photo.png`, paste the Unlock Key and click **Unlock & Show Message**

## Limitations
- Send the PNG as a file. JPEG conversion or messaging-app compression destroys the hidden message
- The key formula and Caesar cipher are for learning only; do not hide real passwords or private data

## Technologies
HTML5, CSS3, JavaScript, Canvas API, FileReader API
