---
layout: default
title: Compression Quality
nav_order: 3
---

# Compression Quality

The quality slider is where most file-size savings come from. This page explains what it changes and how to pick a good value.

---

## What the quality slider does

For **JPG** and **WebP** output, the quality slider controls the tradeoff between visual fidelity and file size.

- **Higher quality** means fewer visible artifacts and larger files
- **Lower quality** means smaller files and more visible compression damage

The slider ranges from **1** to **100**.

---

## When the slider applies

| Output mode | Does quality apply? |
|---|---|
| **JPG** | Yes |
| **WebP** | Yes |
| **PNG** | No - PNG export is lossless |
| **Same as Input** | Only for JPEG and WebP source files |

If you switch output to **PNG**, the app disables the quality slider because PNG compression is lossless.

---

## Recommended starting points

| Quality | Typical use |
|---|---|
| **90-100** | Minimal quality loss, larger files |
| **80-89** | Best default balance for most photos |
| **65-79** | Stronger compression when file size matters |
| **1-64** | Aggressive compression, usually only for throwaway previews or web thumbnails |

The default value in BatchCompress Image is **80**.

---

## What artifacts to look for

When quality is too low, you may notice:

- Blockiness in detailed textures
- Smearing in foliage, hair, or fabric
- Haloing around sharp edges
- Text or UI elements becoming fuzzy
- Banding in gradients or skies

The live preview is the fastest way to catch these issues before you process the whole batch.

---

## Photo vs graphic content

### Photos

Photographs usually compress well as **JPG** or **WebP**. Start around **80** and only move lower if the preview still looks clean.

### Graphics, logos, screenshots, and text

These often look worse at low JPG quality because hard edges show artifacts quickly. Prefer **PNG** for these images when preserving crisp edges matters more than file size.

---

## Why preview matters

Different images react differently to the same quality value. A portrait with a soft background may still look excellent at 70, while a screenshot full of fine text may look poor even at 90.

BatchCompress Image previews one file from the folder using your current settings so you can tune the tradeoff before running the full batch.
