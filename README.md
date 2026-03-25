# Interactive-Canvas-Art-Generator
Create stunning generative art with your mouse! Features real-time particle effects, color theory algorithms, and high-res PNG export.
I built this using Vanilla JavaScript and the HTML5 Canvas API. It features an interactive particle system, a "constellation" effect (connecting nearby points), dynamic hue-shifting (color theory), and a high-resolution PNG export function.

How to use it:
Double-click the file to open it in your browser.
Move your mouse around to draw, and click the Export Artwork button when you're done!

What makes this code awesome:
Physics & Math: Uses Pythagorean theorem (Math.sqrt(dx * dx + dy * dy)) to calculate the distance between particles and draw lines between them, creating a mesmerizing web effect.
Color Theory: Uses hsl() (Hue, Saturation, Lightness). By constantly incrementing the hue variable on every frame, it smoothly cycles through the entire color spectrum without hard-coding colors.
Performance: Implements a garbage collector by splicing particles out of the array once they shrink too much, preventing browser lag.
Flawless Export: Standard canvas.toDataURL sometimes exports transparent pixels, making the image look weird in image viewers. The export function creates a temporary canvas, paints it solid dark-mode black, overlays your art, and then exports it!
Flawless Export: Standard canvas.toDataURL sometimes exports transparent pixels, making the image look weird in image viewers. The export function creates a temporary canvas, paints it solid dark-mode black, overlays your art, and then exports it!
