
<h2>Image Steganography Tool</h2>

A browser-based tool that hides a secret text message inside an image and reads it back later. It is a single HTML file with no server and no external libraries.
This project is a browser-based image steganography tool that hides a secret text message inside an ordinary-looking image. Plain text is easy to read if it is intercepted, and an encrypted string looks suspicious. This tool does both jobs: it scrambles the message and hides that it exists at all.

The sender enters a number and the tool creates a matching Lock Key and Unlock Key. The message is scrambled with a Caesar shift cipher, and a `###STOP###` marker is added to show where it ends. The scrambled bits are then stored in the Least Significant Bit (LSB) of each pixel's Red, Green and Blue values. This changes the image so slightly that the human eye cannot see it, and the result is downloaded as a lossless PNG. The receiver uploads that PNG and enters the Unlock Key. The tool reads the hidden bits, reverses the shift, and shows the original message.

The whole tool is one HTML file built with HTML, CSS and JavaScript. It runs locally in the browser with no server and no external libraries, so no image or message is ever uploaded anywhere.

This is an individual learning project that demonstrates how key generation, a simple cipher and pixel-level bit manipulation work together. It is not meant to protect real confidential data.


**Student:** Gaurang Khare | **Class:** ELCE-1 | **Roll No:** 2026B02310077|
**Faculty:** Mr. Pushparaj Dora | **Institute:** ABES Engineering College, Ghaziabad
