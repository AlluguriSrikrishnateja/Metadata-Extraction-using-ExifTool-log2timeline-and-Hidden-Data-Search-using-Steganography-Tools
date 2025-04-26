# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools

# AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.

# DESIGN STEPS:
## Step 1:
Use exiftool to extract metadata from files such as images, documents, and videos.

## Step 2:
Use log2timeline and plaso to create and analyze event timelines from system logs and file metadata.

## Step 3:
Apply steganography detection tools like steghide, zsteg, or binwalk to uncover hidden data in media files.

# PROGRAM:
Metadata and Timeline Forensics, Steganography Analysis Steps

# OUTPUT:

# Using ExifTool – for file metadata

* Install the tool:

```
sudo apt update
sudo apt install exiftool -y
```
*  Extract metadata from a file:
```
exiftool image.jpg
```
*  Batch process a folder:
```
exiftool -r /path/to/folder
```


* Useful flags:

-G: Show metadata group

-time:all: Show only timestamps

-GPSLatitude -GPSLongitude: Extract GPS data


<img width="461" alt="image" src="https://github.com/user-attachments/assets/1853aa3d-b7f2-4f52-b05b-b79e72af004d" />


# install log2timeline

```
sudo apt install plaso -y
```

```
sudo apt install steghide -y
```

* Embed data
```
steghide embed -cf /home/kali/Downloads/wallpaper.jpg -ef /home/kali/Downloads/sec

```

<img width="475" alt="image" src="https://github.com/user-attachments/assets/a9d66203-47e2-4028-a602-6bb903ebba6d" />

* Extract hidden data:
```
steghide extract -sf hidden.jpg

```
<img width="476" alt="image" src="https://github.com/user-attachments/assets/08c23224-7459-4127-8cfa-8c26a70b3a01" />

* Using binwalk – for file analysis
```
sudo apt install binwalk -y
```

```
binwalk /home/kali/Downloads/wallpaper.jpg
```
<img width="475" alt="image" src="https://github.com/user-attachments/assets/a78009c8-4092-4de2-bdf9-2aab52a75318" />

# RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.

