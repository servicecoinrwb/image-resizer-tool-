# 🖼️ Image Resizer Tool

A simple, powerful, and private client-side web application to resize images to specific dimensions or aspect ratios. Built entirely with **HTML**, **Tailwind CSS**, and **vanilla JavaScript**, this tool ensures your images are **never uploaded to a server** — all processing happens in your browser.

---

## ✨ Features

- **Dynamic Resizing**: Set custom width and height for precision.
- **Aspect Ratio Locking**: Choose from presets like `1:1`, `3:1`, `4:3`, `16:9`.
- **Drag & Drop or File Picker**: Flexible upload options.
- **Live Canvas Preview**: Instantly see your resized image.
- **Custom Backgrounds**: Use HEX codes or color picker.
- **Transparency Support**: Output transparent PNGs with a single checkbox.
- **Client-Side Privacy**: Nothing is uploaded. Ever.
- **Broad Format Support**: Works with `PNG`, `JPG`, `GIF`, and `WEBP`.
- **Smart Download Naming**: Example: `logo_1500x500.png`.

---

## 🚀 How to Use

### 1. Upload Image
- Click the **upload area** to open a file dialog.
- Or **drag and drop** your image onto the upload box.

### 2. Set Dimensions
- **Aspect Ratio Presets**: Pick one to lock proportions.
- **Custom Size**: Choose \"Custom\" to unlock width & height fields.

### 3. Choose Background
- Select a color via the color picker or type a **HEX** code.
- For **transparent output**, enable the transparency checkbox (saves as `.png`).

### 4. Preview
- A **live canvas preview** shows the resized image in real-time.

### 5. Download
- Hit **Download Image** to save with proper dimensions and format.

---

## 🛠️ How It Works (Technical Details)

- **HTML5 Canvas API** handles all drawing.
- **FileReader API** reads the image into memory as a base64 URL.
- Image is drawn to a `<canvas>` element with the desired dimensions.
- Optional background fill or transparency applied.
- `canvas.toDataURL()` converts it to a downloadable file.
- Final download is triggered with a smart filename based on original + size.

---

## 🧩 Tech Stack

- HTML5 + Canvas API  
- Tailwind CSS  
- Vanilla JavaScript (No Frameworks)  
- 100% Client-Side (No dependencies, no server)

---

## 📸 Example Use Cases

- Resize logos to **1500×500** for Twitter/X or GitHub headers  
- Create perfect **1:1 thumbnails**  
- Add a white or brand-color background to a transparent image  
- Export transparent PNGs for UI assets  

---

## 🔒 Privacy First

This tool **never sends your images anywhere**. Everything stays on your machine. Perfect for designers, developers, and privacy-conscious users.

---

## 📂 License

MIT — Use it freely, modify it, share it. Just don’t sell it as-is.

---

## 🤝 Contribute

Feel free to submit pull requests, report issues, or fork the project. Help improve this simple but mighty resizer!


