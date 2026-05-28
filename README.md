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
**Check file type**
```bash
file image.jpg
```
or view magic bytes:
```
xxd image.jpg | head
```

<img width="591" height="341" alt="image" src="https://github.com/user-attachments/assets/b3cee605-31eb-44bb-b6e7-adda75315bc4" />

**Run StegExpose**
```bash
java -jar StegExpose.jar suspect.jpg
```
instead of StegExpose an alternative tool binwalk is used
```
binwalk wallpaper.jpg
```
<img width="743" height="126" alt="image" src="https://github.com/user-attachments/assets/643114f6-0688-406d-9753-4c0d23b4bb74" />

## OUTPUT:

List of Images with Steganography Detection Scores and File Signature Details

<img width="942" height="266" alt="image" src="https://github.com/user-attachments/assets/1bb409a4-3e2b-422d-ab89-ce1f489bb4d9" />



## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
