---
layout: default
title: Troubleshooting
nav_order: 5
---

# Troubleshooting

---

## "No supported images found"

The app only processes **JPG, PNG, WebP, and TIFF** files.

If your folder contains HEIC, GIF, BMP, RAW, or other formats, they will not be counted. Convert them first before running compression.

---

## The Compress button stays disabled

The button is disabled until:

- An input folder is selected
- The selected folder contains at least one supported image
- A batch is not already running

If the image count is 0, the app found no supported files in that folder.

---

## Some files were skipped

This usually happens when **Skip already compressed files** is turned on and a file with the same output name already exists in the output folder.

Turn the switch off if you want to overwrite or regenerate those outputs.

---

## The preview does not match the final file exactly

The preview is a reduced-resolution proof designed to help you judge settings quickly. It is not intended to be a byte-for-byte copy of the final exported image.

Use it to evaluate quality direction, visible artifacts, and format behavior before the full run.

---

## Output images are still too large

Try one or more of these:

- Lower the quality value for JPG or WebP output
- Convert photographic images to **WebP** instead of PNG
- Use **JPG** instead of **Same as Input** if the source folder contains many PNG or TIFF files
- Turn on **Strip EXIF metadata** if embedded metadata is unnecessary

---

## Output images look blurry or blocky

That usually means compression is too aggressive for the content.

- Raise the quality value
- Try **PNG** for screenshots, text, graphics, or logos
- Compare **Original** and **Split** preview modes before running the full batch

---

## The app reports errors for some files

Open the **Activity Logs** panel to see the filename and error.

Common causes:

| Error type | Likely cause |
|---|---|
| Unsupported image data | File extension looks valid but the file is corrupt or not really an image |
| Read error | Source file was moved, locked, or deleted during processing |
| Write error | Output folder is unavailable, read-only, or blocked by permissions |

---

## Output folder will not open

The **Open Output Folder** button uses Windows Explorer. If Explorer does not open, navigate manually to the output subfolder inside your selected input folder.

---

## Still stuck?

Email [hello@3thousand30.com](mailto:hello@3thousand30.com) or [open an issue](https://github.com/3thousand30/batchcompressimage-docs/issues) on GitHub.
