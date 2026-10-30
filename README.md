# Image Compressor

Compress JPG, PNG and WebP images free online. Reduce photo size to an exact target such as 20KB, 50KB or 100KB for exam and job forms, or shrink images for websites and WhatsApp.

**Live demo:** https://harikabehara247.github.io/image-compressor/

## About

Online application forms for exams, jobs and government services often reject photos and signatures above a size limit such as 20 KB or 50 KB. Large phone photos are several megabytes, and resizing them by trial and error wastes time.

Turn on Target size, type the limit, and the compressor tries quality levels (and, if needed, slightly smaller dimensions) until the file fits. For websites and WhatsApp, the quality slider with a maximum width gives much smaller files that still look sharp. To set exact pixel dimensions first, use the Image Resizer.

## Features

- **Exact KB targets** — Perfect for exam, job and government forms that need photos under 20 KB, 50 KB or 100 KB.
- **Batch compression** — Compress many photos together and download them as one ZIP.
- **Optional resize** — Limit the longest side, for example to 1,600 pixels, for much smaller files.
- **Private and instant** — Compression runs on your device; nothing is uploaded.

## How to use

1. **Add images** — Drop JPG, PNG or WebP files, or choose them from your device.
2. **Choose how small** — Use the quality slider, or switch on “Target size” and enter the KB limit your form asks for.
3. **Compress** — Each file shows its old and new size and how much was saved.
4. **Download** — Save one file or all of them as a ZIP.

## Tech

- Plain HTML, CSS and JavaScript (ES modules), no build step
- Runs entirely in the browser: files and inputs never leave the device
- Third-party libraries:
  - fflate 0.8.3 MIT

## Run locally

Serve the folder with any static server, for example `python3 -m http.server`, then open http://localhost:8000. (ES modules do not load from `file://`.)

## FAQ

**How do I compress a photo to 50 KB?**  
Add the photo, switch on Target size, enter 50 and click Compress. The tool saves the best-quality JPG that is 50 KB or smaller.

**Will compression reduce the quality?**  
A little. At quality 70 to 80 most people cannot see a difference, while the file is often 60 to 80 percent smaller.

**Why did my PNG become a JPG?**  
PNG cannot be compressed by quality, so for real savings the tool saves photos as JPG. Choose WebP if you need a small file that keeps transparency.

**What if the target size cannot be reached?**  
The tool also reduces the dimensions step by step. If it still cannot fit, it tells you the smallest size it reached.

**Are my images uploaded?**  
No. Everything happens in your browser.

## Author

Built by **[Harika Behara](https://github.com/harikabehara247)**.

## Licence

Code: [MIT](LICENSE) © 2026 Harika Behara. Bundled third-party libraries keep their own licences — see `assets/tools/vendor/LICENSES.txt`.
