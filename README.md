# CODECRAFT_CS_02
1. This code creates a simple image encryption tool that:

 - Takes an image file, applies a random pixel swap (mixes the positions of the pixels) to encrypt the image.
 - Applies a mathematical transformation (adds a key to the pixel values) for encryption.
 - Decrypts the image by reversing both the pixel swap and the mathematical transformation, returning the image to its original form.

2. Process
  a. User Input:

   - The user is prompted to enter the path to the image they want to encrypt and a key (a number).
   - The key is used to modify pixel values in a reversible way.

  b. Pixel Swapping:

  -  The image is converted into a list of pixels (RGB values).
  -  The pixels are shuffled randomly to encrypt the image, and the order of this shuffle is saved so it can be reversed later.
  -  During decryption, the code uses the saved shuffle order to put the pixels back into their original positions.

  c. Mathematical Transformation:

  - For encryption, the key is added to each pixel’s RGB values (with wrapping at 256, so values stay within color limits).
  - For decryption, the key is subtracted from each pixel’s RGB values to restore the original colors.
  
  d. Saving Files:

  - The encrypted image is saved with a default name (e.g., encrypted_image.jpg).
  - The decrypted image is saved with a default name (e.g., decrypted_image.jpg).

IN SIMPLE TERMS
1. Encrypt:
- Shuffle pixel positions.
- Add key to pixel values.
- Save encrypted image.
2. Decrypt:
- Reverse the addition of the key.
- Reverse the pixel shuffle using stored indices.
- Save decrypted image.

   
