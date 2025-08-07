# QR-code-generator
QR Code Generator
A simple and clean QR Code Generator built with HTML, CSS, and vanilla JavaScript. This application allows users to instantly convert any text or URL into a downloadable QR code by using a free public API.

<img width="1919" height="809" alt="image" src="https://github.com/user-attachments/assets/c1cf66e5-5aed-4889-83f2-6a4b6ca197c4" />

Features
Instant Generation: Creates a QR code in real-time as soon as the "Generate" button is clicked.

Text & URL Support: Can generate a QR code for any string of text or a valid URL.

Dynamic UI: The interface shows a loading state and only displays the QR code once it has been successfully generated.

Input Validation: Prevents unnecessary API calls if the input is empty or unchanged.

Clean Interface: A simple and intuitive user interface.

How It Works
This project does not generate the QR code in the browser. Instead, it uses a clever and efficient approach:

The user enters text or a URL into the input field.

When the "Generate" button is clicked, the JavaScript constructs a specific URL for the goqr.me API.

This URL, which contains the user's data, is set as the src of an <img> tag.

The goqr.me server receives this request, generates the QR code image on its end, and sends it back to be displayed on the page.

This method is lightweight and reliable, as it offloads the complex image generation process to a dedicated external service.

Technologies Used
This project was built using foundational web technologies:

HTML5: For the structure of the application.

CSS3: For all styling and layout.

Vanilla JavaScript: For handling user input, making the API request, and updating the UI.

How to Use
Simply open the index.html file in any modern web browser to start using the QR Code Generator.
