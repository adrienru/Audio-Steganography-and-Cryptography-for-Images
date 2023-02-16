# Audio-Steganography-Cryptography-for-Images
2-LSB Audio Steganography with Encryption &amp; Decryption Codes

About:
In the attached code, I am encoding an encrypted image inside an audio file using 2-LSB (least significant bits) of the cover medium. I have also provided code for decryption process. 
Note: Since I am using symmetric encryption in the code. The encryption key generated during encryption must be shared while implementing decryption.

Methodology:

Encryption:
1. Import 'Fernet' module of 'cryptography' package and generate a symmetric encryption key
2. Load sample image and convert into bites format 
3. Encrypt the images bites string using the encryption key
4. Import sample audio and encode the encrypted bites string in the last 2 LSB of the cover audio
5. Share the encoded audio and encryption key with the receiver

Decryption:
1. Create a decrypter object with the encryption key generated during encryption
2. Extract the last 2 LSB from the shared cover medium
3. Use the decrypter to decrypt the encrypted bites images
4. Convert the bites image back into original format

Conclusion:
Audio steganography had various use cases in domains like secure communication and copyrights. This is a small project to showcase the utility of such such techniques.
