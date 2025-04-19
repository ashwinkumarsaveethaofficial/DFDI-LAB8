# EXP8:DETECTING STEGANOGRAPHY WITH TOOLS  LIKE STEGEXPOSE,ANALYSING FILE SIGNATURES

## AIM:
To hide and extract secret information (e.g., text files) inside a cover file (e.g., JPEG image) using the steganography tool `steghide` in Kali Linux.

EQUIPMENTS REQUIRED:
●	Hardware: PCs

```
Register Number: 212222040121
Name: Praveen V
```

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROCEDURE:
### Step 1: Download Image and Create Secret Message File
  •	Download a .jpeg image (e.g., praveen.jpeg) from a trusted website or use own image.
  
  ![image](https://github.com/user-attachments/assets/4450ad9a-6810-4393-884d-fdcaf074d740)
  
  •	Create a text file named secret with a confidential message:
  
  ![image](https://github.com/user-attachments/assets/50b131bf-9090-4b58-9d9d-9d0482562578)
  ![image](https://github.com/user-attachments/assets/a352aa29-11e7-4071-9798-d9e44a53b1d1)


### Step 2: Install and Verify Steghide Tool
  •	To install Steghide on Kali linux,run:
  
  ![image](https://github.com/user-attachments/assets/a5d4bd21-52af-4713-b9fb-0a92efae25b0)
  
  •	Confirm the installation by checking its version:
  
  ![image](https://github.com/user-attachments/assets/b4f90361-9f9f-49b6-b8b4-865c8f3c8703)

 
### Step 3: Embed the Secret Message into the Image
  •	Use the following command to embed secret into praveen.jpeg:
  
  ![image](https://github.com/user-attachments/assets/7d545e46-2984-43e9-a3a6-7ee77e94c226)


### Step 4: Delete the Original Secret File
  •	After embedding, delete the plaintext file:
  
  ![image](https://github.com/user-attachments/assets/3fdd3aa0-37c2-42c2-8440-3e23c9b9814c)


### Step 5: Extract the Embedded Secret from the Image
  •	To retrieve the hidden file:
  
  ![image](https://github.com/user-attachments/assets/71100795-e4a7-491b-a005-80eb3c1cf1bd)

  •	Enter the same passphrase used during embedding.
  
  ![image](https://github.com/user-attachments/assets/55a3d6cb-6606-40dc-ae53-2a385ecd63da)

## OUTPUT:
### Step 1: Verify the Extracted Message

  •	Display the extracted file content to verify:
  
  ![image](https://github.com/user-attachments/assets/6fab15a7-706b-4c44-8d30-8418d57634b4)
  
  •	Ensure the message matches the original secret content.
  
  •	Another command to see the same secret message is
  
  ![image](https://github.com/user-attachments/assets/5e478ee7-baae-4b20-b2c3-8ed1b41f3d69)

 
### Step 2: Retrieve Information About the Embedded Data
  •	To gather details about embedded content in the image:
  
  ![image](https://github.com/user-attachments/assets/2a559d4f-e5e2-4567-9573-aa1e6ce873af)
  
   
  •	This will display file type, size, and whether data is embedded.

 
## RESULT:
Embedded "secret" into praveen.jpeg successfully using Steghide with passphrase 12345.Extracted and verified hidden message
