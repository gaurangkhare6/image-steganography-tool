Secret Message in Image - Image Steganography Tool

A browser-based tool that hides a secret text message inside an image and reads it back later. It is a single HTML file with no server and no external libraries.

Student: Gaurang Khare | Class: ELCE-2 | Roll No: 2026B02310077
Faculty: Mr. Pushparaj Dora | Institute: ABES Engineering College, Ghaziabad

Features
Generates a paired Lock Key and Unlock Key from any number
Scrambles the message with a Caesar shift cipher
Hides the message in the Least Significant Bits (LSB) of the image's Red, Green and Blue values
Downloads the result as a lossless PNG (secret_photo.png)
Shows image size, capacity and a live character counter
Copy and Clear buttons; everything runs locally in your browser
How it works
Key Generator: Lock Key = number x 5, Unlock Key = number x 9
Encode: the message is shifted, ###STOP### is added at the end, and the bits go into the image pixels (even value = 0, odd value = 1)
Decode: the bits are read back until ###STOP### is found, then the shift is reversed
How to use
Open image steganography tool.html in any browser
Enter a number and click Make Keys
Choose a cover photo, paste the Lock Key, type a message and click Hide & Download Photo
To read it, upload secret_photo.png, paste the Unlock Key and click Unlock & Show Message
Limitations
Send the PNG as a file. JPEG conversion or messaging-app compression destroys the hidden message
The key formula and Caesar cipher are for learning only; do not hide real passwords or private data
Technologies

HTML5, CSS3, JavaScript, Canvas API, FileReader API
