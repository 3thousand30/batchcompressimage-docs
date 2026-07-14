---
layout: default
title: Output Formats
nav_order: 4
---

# Output Formats

Batch Compress Image can keep the original format of each file or convert the batch to JPG, PNG, or WebP.

---

## Same as Input (default)

Keeps each image in its original format where practical.

- JPG stays JPG
- PNG stays PNG
- WebP stays WebP
- TIFF input is flattened to JPG output

**Use this when:** You want the simplest workflow and do not need a format conversion.

Note: In this mode, the quality slider only affects JPEG and WebP source files.

---

## JPG

JPEG uses lossy compression and is usually the best choice for photographs.

**Pros:**
- Small file sizes
- Universal compatibility
- Good choice for photo-heavy folders

**Cons:**
- Lossy compression artifacts at lower quality values
- No transparency support

**Use JPG when:** You are compressing photos for email, upload, archive reduction, or general sharing.

---

## PNG

PNG uses lossless compression.

**Pros:**
- No lossy artifacts
- Supports transparency
- Excellent for screenshots, UI captures, logos, and text

**Cons:**
- Larger file sizes than JPG or WebP for photographic images
- Quality slider does not apply

**Use PNG when:** You want to preserve exact pixels or maintain transparency.

---

## WebP

WebP is a modern format that often compresses better than JPG at similar visual quality.

**Pros:**
- Very efficient compression
- Supports transparency
- Good balance of quality and size

**Cons:**
- Compatibility can be weaker than JPG in some older tools
- Not every workflow expects WebP files

**Use WebP when:** You want smaller files and you know the destination apps or websites support WebP.

---

## Format comparison at a glance

| | Same as Input | JPG | PNG | WebP |
|---|---|---|---|---|
| Compression | Follows source/output rules | Lossy | Lossless | Usually lossy |
| Transparency | Original | No | Yes | Yes |
| File size | Often reduced | Small | Large | Smallest in many cases |
| Best for | Simple batch runs | Photos | Graphics / text / transparency | Web and compact archives |

---

## What about TIFF?

Batch Compress Image accepts **TIFF** as an input format, but there is no direct TIFF output button.

If you choose **Same as Input**, TIFF files are exported as **JPG**. If you choose **JPG**, **PNG**, or **WebP**, TIFF files are converted to that selected format.
