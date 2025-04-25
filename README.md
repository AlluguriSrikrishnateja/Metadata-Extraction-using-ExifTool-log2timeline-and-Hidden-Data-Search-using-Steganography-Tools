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




