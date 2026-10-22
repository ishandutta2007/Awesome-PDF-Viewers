# Awesome-PDF-Viewers

## Top PDF Viewers Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Lightweight Rendering, Annotation Support & Browser-Native Viewing*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **PDF Viewers**. These tools render, navigate, and annotate PDF documents — from featherweight desktop readers that open instantly to JavaScript libraries that embed PDF viewing directly into web applications without plugins.

**Examples** include SumatraPDF, Okular, MuPDF, PDF.js, Sioyek, Zathura, qpdfview, Evince, Adobe Acrobat Reader, and Foxit Reader (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, browser-native rendering, and transparent document handling — ideal for users who want fast, private PDF viewing without subscription bloat, and developers embedding PDF rendering into their applications.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Adobe Acrobat Reader](https://acrobat.adobe.com/)**  
  **The reference commercial PDF viewer** with form filling, annotation, and cloud integration. **Adobe Acrobat's standard pricing runs at $12.99 per month or $155.88 annually**; Pro goes as high as **$19.99 per month** . **Trade-offs**: notoriously slow and resource-hungry, with background processes for collaboration, cloud sync, and AI features compounding performance issues . **Best for users locked into Adobe's ecosystem** needing enterprise form workflows.

- **[Foxit PDF Reader](https://www.foxit.com/)**  
  **Lightweight commercial alternative to Adobe Reader** with fast rendering, annotation tools, and form filling. Free version available with paid Pro upgrade. **Best for Windows users wanting Adobe compatibility** without Adobe's resource footprint.

- **[Google Drive PDF Viewer](https://drive.google.com/)**  
  **Browser-native PDF viewing** within Google Drive. No installation required; works across devices signed into a Google account. **Trade-offs**: requires uploading documents to Google's cloud. **Best for users already storing documents in Google Drive.**

## Open-Source GitHub Projects

- **[PDF.js](https://github.com/mozilla/pdf.js)**  
  **The browser-native PDF standard** — Apache-2.0 licensed, maintained by Mozilla . **A general-purpose, web standards-based platform for parsing and rendering PDFs** using HTML5 and JavaScript, without requiring a browser plugin . **Three layers**: **Core** (binary PDF parsing and interpretation), **Display** (easier-to-use API for rendering), and **Viewer** (the UI powering Firefox's built-in PDF viewer) . **Prebuilt stable release v6.3.289** available, plus source via `git clone` . **Can be embedded via CDN** or built into custom applications . **Mozilla asks that if you embed the viewer, you re-skin it or build upon it rather than using an unmodified version** . **Best for web applications needing PDF rendering** without server-side conversion or native dependencies.

- **[SumatraPDF](https://github.com/sumatrapdfreader/sumatrapdf)**  
  **The lightweight Windows champion** — (A)GPLv3 licensed, **opens documents instantly with minimal memory use** . **Supports PDF, EPUB, MOBI, comic books (CBZ/CBR), DjVu, XPS, CHM, and images** . **Portable option** — run from a USB drive without installation . **Highly customizable** keyboard shortcuts, themes, and toolbar layouts . **Windows 7, 8, 10, and 11** with 32-bit, 64-bit, and ARM64 builds . **"One of those amazing open source programs that does everything a closed-source and/or commercial product does, but better in every way"** — described as **"small, svelte, lightweight and lightning fast"** compared to Adobe Reader . **Trade-offs**: **Windows-only** — no Mac or Linux version . **Best for Windows users wanting the fastest possible PDF viewing** with zero bloat.

- **[Okular](https://github.com/KDE/okular)**  
  **The universal document viewer from KDE** — GPL-2.0+ licensed . **Supports PDF, PostScript, DjVu, CHM, XPS, ePub, comic books, TIFF, DVI, Markdown, and more** . **Annotation capabilities rival or surpass Adobe's**: highlight, underline, strikethrough, pop-up notes, freehand drawing, text boxes, stamps, geometric shapes, and typewriter tool for forms . **Annotations stored separately from the original PDF by default**, keeping source files intact, with option to save directly into the PDF . **Tabs for multiple documents**, sidebar navigation, text selection, text-to-speech, magnifier, search, and dark mode . **Performance tuning** lets you choose low, normal, or aggressive memory usage . **Installed size under 300 MB on Windows**, smaller on Linux . **Available on Linux, Windows (Microsoft Store), and macOS (MacPorts/Homebrew)** . **No user data collection, no ads, no registration** . **Best for cross-platform users wanting a full-featured, privacy-respecting viewer** that handles more than just PDFs.

- **[MuPDF](https://github.com/ArtifexSoftware/mupdf)**  
  **The open-source software framework for viewing, converting, and manipulating PDF, XPS, and eBook documents** . **Viewers for Linux, Windows, BSD, and Android** — main `mupdf-gl` viewer has table of contents sidebar, full Unicode search, annotation editing, and redaction . **Command-line tools** via `mutool`: `draw` (render to images), `convert` (format conversion), `show` (inspect internal objects), `extract` (pull images/fonts), `clean` (fix broken files), `create`, `merge`, and `poster` . **Library in portable C**, with **JavaScript/TypeScript (WASM)**, **Java (JNI)**, and **Python (PyMuPDF)** bindings . **WebViewer is commercial-license-only** . **Best for developers** needing a PDF rendering library or command-line toolkit, and for mobile/embedded applications.

- **[Sioyek](https://github.com/ahrm/sioyek)**  
  **The PDF viewer optimized for research papers and technical documents** — designed for reading research papers, textbooks, and technical documents . **Enables jumping between references, figures, and bibliographies even in documents without embedded hyperlinks** . **Deep LaTeX integration** for synchronized navigation between source code and rendered PDF . **Highly customizable** with programmable keybindings and external script extensibility for translation or text recognition . **Best for academics and researchers** reading dense technical literature.

- **[Zathura](https://github.com/pwmt/zathura)**  
  **The minimalist keyboard-driven PDF viewer** — zlib licensed, based on the poppler rendering library and GTK+ toolkit . **"A highly customizable and functional PDF viewer"** with a **minimalistic and space-saving interface** focused on keyboard interaction . **vi-like keybindings** for navigation . **Best for Linux users** who live in the terminal and want a no-nonsense, keyboard-first viewer.

- **[qpdfview](https://github.com/tsdgeos/qpdfview)**  
  **The simple tabbed document viewer** — GPL-2.0+ licensed, uses Poppler for PDF rendering and Qt for the interface . **Outline, properties, and thumbnail panes**; scale, rotate, and fit; fullscreen and presentation views; continuous and multi-page layouts . **Persistent per-file settings** and configurable keyboard shortcuts . **DjVu and PostScript support via plugins** . **Partial annotation and form support** (PDF only, Poppler 0.20.1+) . **Best for Qt/KDE users** wanting a straightforward tabbed viewer with SyncTeX support.

- **[Evince](https://github.com/GNOME/evince)**  
  **The default document viewer for GNOME** — GPL-2.0+ licensed . **Multi-page document viewer for PDF, PostScript, and Encapsulated PostScript** . **Search, copy text, hypertext navigation, table-of-contents bookmarks, and form editing** when supported by the format . **DVI and DjVu support via additional backends** . **Best for GNOME desktop users** wanting a clean, integrated viewing experience.

### Additional Strong Open-Source Options

- **LibreOffice Draw** — Open-source drawing program that can open and edit foreign PDF files as graphical documents, though text is often broken into individual snippets rather than continuous text . Best for light PDF edits, not heavy viewing.
- **Xournal++** — Handwritten note-taking and PDF annotation with pen input, pressure sensitivity, shape drawing, LaTeX integration, and PDF/PNG export. Best for tablet users annotating documents.
- **Skim** — macOS PDF viewer with annotation, highlights, bookmarks, split view, and AppleScript support. Best for Mac users wanting a free alternative to Preview.
- **Stirling PDF** — Self-hosted web app for merging, splitting, compressing, signing, OCR, and converting PDFs. Not a viewer per se, but a self-hosted PDF utility suite.

**Frameworks for building custom systems**: Combine **PDF.js** for browser-native rendering without plugins, **SumatraPDF** for the fastest Windows viewing experience, **Okular** for cross-platform feature-rich viewing with annotations, **MuPDF** for embedding rendering into custom applications or using command-line tools, and **Sioyek** for research paper navigation — to build a PDF viewing stack tailored to your platform, annotation needs, and integration requirements.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- PDF viewers differ significantly in platform support, feature scope, and resource footprint. **SumatraPDF is Windows-only** — no Mac or Linux version . **PDF.js powers Firefox's built-in viewer** and is the standard for browser-based PDF rendering, but Mozilla requests that embedded copies be re-skinned rather than used unmodified . **Okular stores annotations separately from the original PDF by default**, keeping source files intact unless you explicitly save annotations into the PDF . **MuPDF's WebViewer is commercial-license-only** despite the library being open source . **Adobe Acrobat's subscription costs $12.99–$19.99/month** and is known for resource-heavy background processes . **LibreOffice Draw's PDF editing is limited** — text is often broken into individual snippets rather than continuous paragraphs .
- Self-hosted open-source solutions require proper file handling, font embedding verification, and awareness that rendering fidelity varies across engines (Poppler, MuPDF, PDFium, PDF.js).

---

**Made for users wanting fast, private PDF viewing and developers embedding PDF rendering into applications.**
Let's make PDF viewing more open, lightweight, and browser-native.
