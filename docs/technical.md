# Technical Details

## How the Search Occurs

OCRmyPDF uses the Tesseract OCR engine to recognize text in scanned PDF files. The process involves several steps:

1. **Preprocessing**: The input PDF is preprocessed to improve the quality of the images. This may include deskewing, cleaning, and other image enhancements.
2. **OCR**: Tesseract is used to perform OCR on the preprocessed images. Tesseract analyzes the images and identifies text regions, recognizing characters and words.
3. **Text Layer Creation**: The recognized text is used to create an OCR text layer, which is added to the PDF. This text layer is positioned accurately below the original image to ensure proper alignment.
4. **PDF/A Conversion**: If requested, the output PDF is converted to PDF/A format, which is suitable for long-term archiving.

## Output Format of the Search Results

The output of OCRmyPDF is a searchable PDF file. The key features of the output format are:

- **Searchable Text**: The OCR text layer allows the PDF to be searched for specific words or phrases. The text is hidden behind the original image, preserving the visual appearance of the document.
- **Copy/Paste Functionality**: The recognized text can be selected and copied from the PDF, enabling easy extraction of text content.
- **PDF/A Compliance**: If PDF/A conversion is enabled, the output PDF will comply with the PDF/A standard, ensuring long-term preservation and compatibility with archival systems.
- **Optimized File Size**: OCRmyPDF optimizes the PDF images, often resulting in smaller file sizes compared to the input file.

## Design Decisions and Why It Works Optimally

OCRmyPDF is designed to work optimally by leveraging several key design decisions:

1. **Use of Tesseract OCR Engine**: Tesseract is a widely used and highly accurate OCR engine that supports multiple languages. By using Tesseract, OCRmyPDF ensures high-quality text recognition.
2. **Image Preprocessing**: Preprocessing steps such as deskewing and cleaning improve the quality of the input images, leading to better OCR results.
3. **Accurate Text Layer Positioning**: The OCR text layer is positioned accurately below the original image, ensuring that the visual appearance of the document is preserved while making the text searchable.
4. **PDF/A Conversion**: PDF/A is a standardized format for long-term archiving. By converting the output PDF to PDF/A, OCRmyPDF ensures that the document remains accessible and compatible with archival systems.
5. **Optimized File Size**: OCRmyPDF optimizes the PDF images, reducing the file size without compromising the quality of the document. This makes it easier to store and share the PDF files.

These design decisions contribute to the overall effectiveness and efficiency of OCRmyPDF, making it a reliable tool for adding OCR text layers to scanned PDF files.
