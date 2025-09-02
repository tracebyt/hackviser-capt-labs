# Hackviser CAPT Labs – Cryptanalysis & Encoding Techniques

This document provides **conceptual understanding** of common encoding and cryptanalysis techniques used in cybersecurity labs. It complements the practical exercises in `encoding_techniques_lab.txt`.

---

## 1. ASCII Encoding
**Overview:**  
ASCII (American Standard Code for Information Interchange) is a character encoding standard mapping characters to numbers between 0 and 127. It includes uppercase and lowercase letters, digits, punctuation, and control characters. ASCII forms the foundation for most modern character encodings.

**Use Cases:**  
- Text representation in computers and networking protocols  
- File and data transfer between different systems

---

## 2. Base64 Encoding
**Overview:**  
Base64 is a binary-to-text encoding scheme converting binary data into 64 printable ASCII characters. It ensures data remains intact during transport over media that are designed to handle text, such as email or JSON.  

**Use Cases:**  
- Encoding images, documents, or binary files in text-based formats  
- Embedding data in XML, JSON, or HTML

---

## 3. URL Encoding
**Overview:**  
URL encoding converts characters not allowed in URLs into `%hex` notation, where `hex` represents the ASCII value. Reserved characters, unsafe characters, and non-ASCII characters are encoded for compatibility with all browsers and servers.

**Use Cases:**  
- Safe transmission of query parameters in web URLs  
- Avoiding misinterpretation of special characters

---

## 4. Hex Encoding
**Overview:**  
Hexadecimal encoding represents binary data as a sequence of two-digit hex numbers. This is human-readable and commonly used in debugging, memory dumps, or cryptography.

**Use Cases:**  
- Binary-to-text conversion for safe display or storage  
- Representing cryptographic keys and hashes

---

## 5. Binary Encoding
**Overview:**  
Binary encoding expresses each byte as a sequence of 8 bits (0s and 1s). It is the lowest-level representation of data in computing systems.

**Use Cases:**  
- Teaching fundamental computing concepts  
- Direct bit-level manipulation

---

## 6. Base32 Encoding
**Overview:**  
Base32 encoding is similar to Base64 but uses 32 characters (A–Z, 2–7). It is useful when fewer characters are needed or to avoid visually similar characters.

**Use Cases:**  
- Encoding secret keys for QR codes and authentication tokens  
- Reducing errors in manual transcription

---

## 7. Quoted-printable Encoding
**Overview:**  
Quoted-printable converts 8-bit text into 7-bit ASCII. Special characters are represented as `=XX`, where `XX` is the hexadecimal code.  

**Use Cases:**  
- Email transmission (MIME)  
- Preserving accented or special characters

---

## 8. HTML Character Entities
**Overview:**  
HTML entities represent special characters using numeric codes (`&#NNN;`) or named codes (`&name;`). This allows reserved or invisible characters to render properly in web browsers.

**Use Cases:**  
- Web page content with special symbols  
- Ensuring cross-browser compatibility

---

## 9. Uuencoding
**Overview:**  
Uuencoding converts binary files to 7-bit ASCII text for transfer across systems that may not support binary data. It was originally used for email and Unix-to-Unix file transfer.  

**Use Cases:**  
- Legacy file transfer via email  
- Preserving binary files in text-only systems

---

### **References & Further Reading**
- [ASCII Table](https://www.asciitable.com/)  
- [Base64 Encoding on Wikipedia](https://en.wikipedia.org/wiki/Base64)  
- [URL Encoding](https://www.w3schools.com/tags/ref_urlencode.ASP)  
- [Hexadecimal Encoding](https://en.wikipedia.org/wiki/Hexadecimal)  
- [Quoted-Printable](https://en.wikipedia.org/wiki/Quoted-printable)  
- [HTML Character Entities](https://www.w3schools.com/html/html_entities.asp)  
- [Uuencode](https://en.wikipedia.org/wiki/Uuencoding)

---

**Note:**  
This theory document is intended to provide context and understanding for the practical labs. All practical exercises, commands, and answers are in `encoding_techniques_lab.txt`.
