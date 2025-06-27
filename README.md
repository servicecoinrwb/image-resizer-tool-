Image Resizer Tool
A simple, powerful, and private client-side web application to resize images to specific dimensions or aspect ratios. This tool is built entirely with HTML, Tailwind CSS, and vanilla JavaScript, meaning your images are never uploaded to a server.

✨ Features
Dynamic Resizing: Manually set a custom width and height for precise control.

Aspect Ratio Locking: Choose from common presets like 1:1 (Square), 3:1 (Banner), 4:3, and 16:9 to automatically maintain proportions.

Intuitive Uploading: Upload images with a standard file picker or by simply dragging and dropping them onto the upload area.

Live Canvas Preview: Instantly see a preview of the final image on the right as you adjust the settings.

Custom Backgrounds: Use the color picker or enter a HEX code to set a solid background color for your image.

Transparency Support: Easily export images with a transparent background by checking a single box (outputs as a PNG file).

Client-Side Privacy: All processing happens in your browser. Images are never sent to a server, ensuring your data remains private.

Broad Format Support: Works with PNG, JPG, GIF, and WEBP image files.

Smart Downloading: The downloaded file is automatically named based on the original filename and the new dimensions (e.g., logo_1500x500.png).

🚀 How to Use
Using the tool is a simple, five-step process:

Upload Image:

Click the "Click to upload an image" area to open a file selection dialog.

Or, drag and drop an image file directly onto the upload area.

Set Dimensions:

For a fixed aspect ratio: Select a preset from the "Aspect Ratio" dropdown. The height will be locked, and you only need to adjust the width.

For custom dimensions: Select "Custom" from the dropdown to unlock and edit both the "Width (px)" and "Height (px)" fields independently.

Choose Background:

For a solid color: Use the color picker or type a HEX code into the text field. The output will be a JPEG file.

For transparency: Check the "Transparent" checkbox. The output will automatically switch to PNG to support transparency.

Preview:

Observe the live preview canvas on the right. It will update in real-time as you change any setting.

Download:

Once you are satisfied with the preview, click the "Download Image" button to save the resized image to your computer.

🛠️ How It Works (Technical Details)
The application leverages the HTML5 Canvas API to perform all image manipulations.

File Reading: When a user uploads a file, the browser's FileReader API reads the image as a Base64 data URL.

Image Object: This data URL is used as the source for a new Image() object.

Canvas Drawing: Once the image object is loaded, it's drawn onto an HTML <canvas> element. The canvas is first set to the user's target dimensions (width and height).

A background fill is applied if a color is selected.

The drawImage() method scales the source image to fit within the canvas while maintaining its original aspect ratio (equivalent to object-fit: contain). The image is centered on the canvas.

Data URL Generation: Finally, the canvas.toDataURL() method converts the contents of the canvas back into a Base64 encoded image string (either image/jpeg or image/png).

Download Trigger: This data URL is assigned to the href attribute of the download button's <a> tag, and the download attribute is set with the new filename. Clicking the link prompts the user to save the generated image.
