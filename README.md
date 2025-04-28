# NAME:T.KAVINAJAI
# REGISTER NO: 212223100020
# Detecting-steganography-with-tools-like-StegExpose-analyzing-file-signatures
## AIM:
To detect hidden data using steganography detection tools like StegExpose and analyze file signatures for authenticity and manipulation.

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROGRAM:
StegExpose and File Signature Analysis Commands
# Install and Verify Steghide Tool
```
sudo apt update
sudo apt install steghide
steghide --version 
```

# Embed the Secret Message into the image
```
steghide embed -cf image.jpg -ef hidden.txt
```
# Extract the Hidden Secret from Image and Verify the Extracted Message
```
steghide extract -sf image.jpg
 cat hidden.txt
```
# Retrieve Information About the Embedded Data
```
 steghide info image.jpg
```

# Analyze File SignatureL
```
  file image.jpg
  binwalk image.jpg
```
## OUTPUT:
# Install and Verify Steghide Tool
![image](https://github.com/user-attachments/assets/451b76eb-16d1-4dff-8446-dec47c300613)
![Screenshot 2025-04-28 132936](https://github.com/user-attachments/assets/ab93cff7-7f87-4560-b332-35daa2b00aae)

# Embed the Secret Message into the Image
![Screenshot 2025-04-28 133316](https://github.com/user-attachments/assets/25241afe-4f74-4fbc-a5a6-82de992e2e26)

# Delete Original Secret File

![Screenshot 2025-04-28 133435](https://github.com/user-attachments/assets/cf536fcc-7ad7-4ac0-ae70-0f4f7f47ab73)

# Extract the Hidden Secret from Image:
![Screenshot 2025-04-28 133435](https://github.com/user-attachments/assets/af801fae-1c10-4dd7-971d-eb5643b65711)

# Retrieve information from the image:

![Screenshot 2025-04-28 133651](https://github.com/user-attachments/assets/5c05935e-9230-4f55-a7de-b169d8bb3cea)

# ANALYSE IMAGE USING BINWALKER:
![Screenshot 2025-04-28 133828](https://github.com/user-attachments/assets/4eb3bd11-b8cf-4407-a1c2-5c92669cfa05)

## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
