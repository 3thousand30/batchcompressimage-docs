---
layout: default
title: Getting Started
nav_order: 2
---

# Getting Started

This guide walks you through compressing your first batch of images.

---

## 1. Install the app

Download and install **BatchCompress Image** from the Microsoft Store. Once installed, launch it from the Start menu.

---

## 2. Select your input folder

Click **Browse** next to **Input Folder** and choose a folder containing your source images.

Supported formats: **JPG, PNG, WebP, TIFF**

The app scans the folder, counts supported images, and loads sample files for the preview panel.

---

## 3. Choose your output format

You can keep each file in its original format or convert the whole batch.

| Format | Best for |
|---|---|
| **Same as Input** | Keep the current format of each image |
| **JPG** | Small files for photographs and general sharing |
| **PNG** | Lossless output for graphics, screenshots, and transparency |
| **WebP** | Strong compression with good quality for modern workflows |

See [Output Formats](output-formats) for the details.

---

## 4. Set compression quality

Use the **Quality** slider to control how aggressively the app compresses the images.

- **Higher values** keep more detail and produce larger files
- **Lower values** create smaller files but may add visible artifacts
- The slider applies to **JPG** and **WebP** output
- **PNG** output is lossless, so the slider does not apply
- In **Same as Input** mode, quality only affects JPEG and WebP source files

A good starting point is **80%**, which is the app default.

---

## 5. Configure output options

The **Output** card lets you control where the compressed files go and how they are named.

- **Folder** - subfolder created inside the input folder. Default: `compressed`
- **Suffix** - optional text added before the file extension
- **Skip already compressed files** - prevents reprocessing files that already exist in the output folder

Example:

```text
photo.jpg -> compressed\photo.jpg
photo.jpg with suffix _web -> compressed\photo_web.jpg
```

---

## 6. Decide whether to strip EXIF metadata

Turn on **Strip EXIF metadata** if you want to remove embedded metadata such as camera details, timestamps, and GPS data from exported files.

Leave it off if you want to preserve the original metadata.

---

## 7. Check the preview

The preview panel shows a sample image from the selected folder using your current settings.

- **Compressed** shows the exported result
- **Original** shows the source image
- **Split** shows both side by side

Use **Previous**, **Next**, and **Refresh** to inspect other files before running the full batch.

---

## 8. Compress the folder

Click **Compress Images** to start.

While running:
- A progress bar shows overall completion
- The current filename is displayed
- You can cancel the batch at any time
- Errors are logged in the **Activity Logs** panel

When the run finishes, click **Open Output Folder** to see the results.

---

## Tips

- Start with **80% quality** and preview a few representative files before compressing a large folder
- Use **PNG** for screenshots, UI captures, logos, or text-heavy graphics
- Use **JPG** or **WebP** for photographic content
- Turn on **Skip already compressed files** if you are retrying a partially completed batch
