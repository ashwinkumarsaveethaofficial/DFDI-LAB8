# EXP8:DETECTING STEGANOGRAPHY WITH TOOLS  LIKE STEGEXPOSE,ANALYSING FILE SIGNATURES

## AIM:
To hide and extract secret information (e.g., text files) inside a cover file (e.g., JPEG image) using the steganography tool `steghide` in Kali Linux.

EQUIPMENTS REQUIRED:
●	Hardware: PCs

```
Register Number: 212222040020
Name: Ashwinkumar S
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
  
![Screenshot 2025-04-22 210915](https://github.com/user-attachments/assets/e5d98043-19fd-44e1-987f-c202bdfbb267)

  
  •	Create a text file named secret with a confidential message:
  
 ![Screenshot 2025-04-22 213925](https://github.com/user-attachments/assets/40904222-99bb-4fe6-bfe4-ca8ef79d801d)

![Screenshot 2025-04-22 211107](https://github.com/user-attachments/assets/35535d4e-5c28-4e86-8335-856c6e7c33bb)



### Step 2: Install and Verify Steghide Tool
  •	To install Steghide on Kali linux,run:
  
![Screenshot 2025-04-22 211233](https://github.com/user-attachments/assets/020e523d-a1fc-48b8-b1b6-786af9d96e95)

  
  •	Confirm the installation by checking its version:
  
![Screenshot 2025-04-22 211244](https://github.com/user-attachments/assets/f3fc8819-5cf0-4935-9611-2a3f938ee908)


 
### Step 3: Embed the Secret Message into the Image
  •	Use the following command to embed secret into praveen.jpeg:
  ![Screenshot 2025-04-22 212850](https://github.com/user-attachments/assets/ba0c2dbc-b199-4390-b167-cabe6f48bd3f)



### Step 4: Delete the Original Secret File
  •	After embedding, delete the plaintext file:
  
 ![Screenshot 2025-04-22 213936](https://github.com/user-attachments/assets/1480e1b3-12d9-43df-a9fa-cb405d75661f)

## OUTPUT:
### Step 1: Extract the Embedded Secret from the Image
  •	To retrieve the hidden file:
  
  ![Screenshot 2025-04-22 213023](https://github.com/user-attachments/assets/50ef56a2-a3dd-4221-ab75-334cbb11e0db)

  •	Enter the same passphrase used during embedding.
  
  ![Screenshot 2025-04-22 213046](https://github.com/user-attachments/assets/c63bcd37-b4b8-4794-a886-40a9fef23e20)


### Step 2: Verify the Extracted Message

  •	Display the extracted file content to verify:
  
![Screenshot 2025-04-22 213113](https://github.com/user-attachments/assets/5cf364bd-fb8e-42ed-956a-faab1af88cdd)

  
  •	Ensure the message matches the original secret content.
  
  •	Another command to see the same secret message is
  
![Screenshot 2025-04-22 213212](https://github.com/user-attachments/assets/b4c64c19-6fd8-485b-875a-43db39d520a4)

 
### Step 3: Retrieve Information About the Embedded Data
  •	To gather details about embedded content in the image:
  
![Screenshot 2025-04-22 213302](https://github.com/user-attachments/assets/bc44b6c3-68e0-4fa7-94f2-5e53c40a0289)

   
  •	This will display file type, size, and whether data is embedded.

 
## RESULT:
Embedded "secret" into praveen.jpeg successfully using Steghide with passphrase 12345.Extracted and verified hidden message
