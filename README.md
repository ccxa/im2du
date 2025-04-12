# 🖼️ im2du - Image to Data URL (Base64) CLI Tool

`im2du` is a tiny, fast CLI utility that converts an image file to a base64 Data URL — perfect for embedding images in HTML/CSS without external hosting.  
It can also copy the result directly to your clipboard with a simple flag.

---

## ⚙️ Features

- Converts `.jpg`, `.png`, `.svg`, `.webp`, etc. to base64 Data URLs
- Automatically detects MIME type
- Copies result to clipboard via `xclip` or `wl-copy`
- Output to a file or print location of result
- Small, dependency-light, and super fast

---

## 🚀 Installation

### From .deb package (Debian/Ubuntu):

```bash
sudo apt install ./im2du_package.deb
```

> You can also use `dpkg -i` but `apt` installs dependencies automatically.

### From source (manually):

```bash
chmod +x im2du
sudo cp im2du /usr/local/bin/
```

---

## 🖥️ Usage

```bash
im2du <image-file> [--copy] [--out <output-file>]
```

### Examples:

Convert image and save output to `./image.png.dataurl.txt`:
```bash
im2du image.png
```

Convert and copy result to clipboard:
```bash
im2du logo.jpg --copy
```

Convert and specify output file:
```bash
im2du icon.svg --out ./dataurl.txt
```

---

## 📦 Dependencies

For clipboard copy functionality, one of the following must be installed:

- [`xclip`](https://github.com/astrand/xclip) (X11)
- [`wl-clipboard`](https://github.com/bugaevc/wl-clipboard) (Wayland)

Install them with:

```bash
sudo apt install xclip wl-clipboard
```

---

## 💡 Why?

Embedding images in emails, single-file HTML/CSS files, or config UIs often requires base64 Data URLs.  
`im2du` simplifies the process into a single command — no online tools, no dragging, no copy-paste.

---

## 🪪 License

MIT License – do whatever you want, just don’t sue me 😄

---

## 👨‍💻 Author

**Arostami** ([@ccxa](https://github.com/ccxa))  
📫 74ne1.pub@gmail.com  
💬 Contributions welcome! PRs and issues are open.
