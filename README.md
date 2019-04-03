# FabricJS layer on top of Mozilla's PDFJS to add ANNOTATIONS

![Alt text](./Screenshot.png?raw=true "Screenshot")

# Features

- Supports PDFs with multiple pages

- Free draw tool

- Add text

- Add arrows

- Add rectangles

- Change colors

- Change Brush size

- Change Font size

- Every object can be resize

- Serialize all canvas data into JSON and re-draw

- Delete individual object

- Clear page

- Export PDF with annotations (using jsPDF)

# Usage 

```javascript
var pdf = new PDFAnnotate('pdf-container-id', 'http://url-to.pdf');

pdf.enableSelector(); // Enable moviing tool

pdf.enablePencil(); // Enable pencil tool

pdf.enableAddText(); // Enable add text tool

pdf.enableAddArrow(); // Enable add arrow tool

pdf.enableRectangle(); // Adds a rectangle

pdf.deleteSelectedObject(); // Delete selected object

pdf.clearActivePage(); // Clear current page

pdf.savePdf(); // Save PDF with name sample.pdf

pdf.serializePdf(); // returns JSON string with canvas data

pdf.setColor(color); // Set color for tools (Example: pdf.setColor(red) , pdf.setColor('#fff'), pdf.setColor('rgba(255,0,0,0.5)'))

pdf.setBorderColor(color); // Set border color for rectangle tool (Example: pdf.setBorderColor(red) , pdf.setBorderColor('#fff'))

pdf.setBrushSize(width); // Set brush size for pencil tool (Example: pdf.setBrushSize(5))

pdf.setFontSize(font_size); // Set font size for text tool (Example: pdf.setFontSize(18))

pdf.setBorderSize(font_size); // Set border size of rectangles (Example: pdf.setBorderSize(2))
```
