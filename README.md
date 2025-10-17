# Captcha Solver Web App
A simple, single-page responsive web application designed to display captcha images and validate user input. Built with HTML, Tailwind CSS for styling, and JavaScript for client-side logic.

## Features
-   **Responsive Design**: Adapts gracefully to various screen sizes using Tailwind CSS.
-   **Captcha Display**: Shows a captcha image, either from a local file or a dynamically provided URL.
-   **User Input Validation**: Allows users to enter the captcha text and provides feedback on their submission.
-   **Default Image**: Defaults to `sample.png` if no specific image URL is provided.

## Usage
To use this application, simply open `index.html` in your web browser.

### Loading Custom Captcha Images
You can load an image from a URL by passing it as a query parameter named `url`.

**Example:**
`index.html?url=https://example.com/path/to/your/captcha.png`

If the `url` parameter is omitted, the application will display the `sample.png` image located in the same directory.

### Solving the Captcha
For the default `sample.png` image, the correct solution is `ADQR3`. Enter this text (case-insensitive) into the input field and click 'Verify Captcha' to see a success message.

For external URLs, the application currently only verifies that input is provided, as a full image-to-text OCR solution is beyond the scope of a client-side only implementation. You are expected to manually solve and input the text for such images.

## Project Structure
-   `index.html`: The main single-page application.
-   `sample.png`: The default captcha image.
-   `README.md`: This file.
-   `LICENSE`: The MIT License text.

## Technologies Used
-   **HTML5**: Structure of the web page.
-   **Tailwind CSS**: Utility-first CSS framework for styling and responsiveness.
-   **JavaScript**: Client-side logic for image loading and input validation.

## License
This project is open source and available under the MIT License.