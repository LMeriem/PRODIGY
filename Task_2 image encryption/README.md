# Pixel Manipulation for Image Encryption

This repository contains a Python-based tool for **image encryption and decryption** using pixel manipulation. The project demonstrates how basic mathematical operations can be applied to an image's pixel values to achieve encryption and decryption, making it suitable for learning purposes.

---

## **Solution Approach**

### **Problem Statement**
The goal is to develop an encryption and decryption mechanism for images using pixel manipulation techniques. Users should be able to encrypt an image such that its pixel values are modified, rendering it unrecognizable, and then decrypt it back to its original state.

### **Approach**

1. **Image Loading**:
   - The input image is loaded using the Python `Pillow` library, which allows easy access to pixel data.
   - The image is converted into a NumPy array for efficient manipulation of pixel values.

2. **Encryption**:
   - A user-provided integer key is used to modify each pixel's value using the formula:
     ```
     encrypted_pixel = (pixel_value + key) % 256
     ```
   - This operation ensures that pixel values remain within the valid range (0-255), as required for images.

3. **Decryption**:
   - The encrypted image is restored to its original form by reversing the encryption operation:
     ```
     decrypted_pixel = (pixel_value - key) % 256
     ```
   - This operation undoes the modification applied during encryption.

4. **Image Reconstruction**:
   - After modifying the pixel values, the NumPy array is converted back into an image using `Pillow`.
   - The resulting encrypted or decrypted image is displayed using `Matplotlib`.

---

## **Features**

- **Encryption and Decryption**:
  - Users can encrypt any image using a custom key.
  - The same key is required to decrypt the image.

- **Pixel Manipulation**:
  - All pixels, including all channels (e.g., RGB or RGBA), are processed.
  - Operations ensure data integrity by keeping values within the range of 0-255.

- **Cross-Platform**:
  - The tool works on any system with Python installed.

---

## **Requirements**

- Python 3.7+
- Libraries:
  - `Pillow` (for image handling)
  - `NumPy` (for efficient pixel manipulation)
  - `Matplotlib` (for displaying images inline)

Install the required libraries using:
```bash
pip install pillow numpy matplotlib
```

---

## **Usage**

### **Step 1: Clone the Repository**
```bash
git clone https://github.com/your-username/image-encryption-tool.git
cd image-encryption-tool
```

### **Step 2: Upload Your Image**
- Place the image you want to encrypt or decrypt in the project folder, or use an absolute path.

### **Step 3: Run the Script**
Execute the Python script in your terminal or Colab:
```bash
python image_encryption.py
```

### **Step 4: Interact with the Program**
- Choose an option:
  1. Encrypt an image.
  2. Decrypt an image.
- Provide the image path and an integer key for encryption/decryption.

### **Step 5: View the Result**
- The encrypted or decrypted image will be displayed directly.

---

## **Limitations**

- **Educational Purpose**:
  - The encryption method is basic and not suitable for securing sensitive data.

- **Key Dependency**:
  - The same key must be used for encryption and decryption.
