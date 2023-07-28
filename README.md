# URL Shortener Web Application

This repository contains the code for a URL Shortener web application implemented using Django on the backend and HTML, CSS (via Tailwind CSS), and JavaScript (using jQuery) on the frontend. The application allows users to input a long URL and get a shortened URL in return. Additionally, users can copy the shortened URL to their clipboard with the click of a button.

## Demo Video

[![URL Shortener Demo Video](https://example.com/demo-thumbnail.png)](https://example.com/demo-video-link)

[Watch the Demo Video](https://example.com/demo-video-link)

## How It Works

1. **Home Page**: Upon accessing the web application, users are presented with a simple and user-friendly UI for the URL Shortener.

2. **Input**: Users can enter their long URL into the input field provided on the page.

3. **Shorten**: Clicking the "Shorten" button triggers an AJAX call to the Django backend. The entered long URL is sent to the server for processing.

4. **Backend Processing**: The Django backend processes the received long URL and generates a shortened version of the URL.

5. **Response**: The backend responds to the AJAX call with the shortened URL.

6. **Display**: The shortened URL is displayed on the page within a designated section.

7. **Copy URL**: Users can copy the shortened URL to their clipboard by clicking the "Copy URL" button.

8. **Feedback**: After copying the URL, a pop-up alert appears, providing feedback that the shortened URL has been copied successfully.

## Technologies Used

- Django: The backend is built using the Django web framework, which handles URL processing and generation of shortened URLs.

- HTML & CSS (Tailwind CSS): The user interface is designed using HTML and styled using Tailwind CSS, a utility-first CSS framework.

- JavaScript (jQuery): Client-side interactions and AJAX calls are handled using JavaScript with the help of the jQuery library.

## How to Run the Application

1. Clone the repository to your local machine:

   ```
   git clone [https://github.com/your_username/your_project.git](https://github.com/omg12347/Url_Shortner)
   ```

2. Install the required dependencies. It's recommended to use a virtual environment:

   ```
   cd your_project
   python -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt
   ```

3. Run the Django development server:

   ```
   python manage.py runserver
   ```

4. Access the application in your web browser by visiting: `http://localhost:8000/`

5. Enter a long URL in the input field and click the "Shorten" button to get the shortened URL.

6. Click the "Copy URL" button to copy the shortened URL to your clipboard.

## Project Structure

```
|-- url_shortener/
|   |-- templates/
|   |   |-- base.html
|   |   |-- index.html
|   |-- static/
|   |   |-- css/
|   |   |   |-- tailwind.min.css
|   |   |-- js/
|   |   |   |-- jquery-3.1.1.min.js
|   |   |   |-- script.js
|   |-- urls.py
|   |-- views.py
|-- manage.py
|-- requirements.txt
|-- README.md
```

- `url_shortener`: This directory contains the Django application files.
  - `templates`: Contains the HTML templates for rendering the frontend.
  - `static`: Holds static files like CSS and JavaScript.
  - `urls.py`: URL configuration for the Django application.
  - `views.py`: Defines the views and backend logic for the URL Shortener.
  
- `manage.py`: Django management script for various administrative tasks.

- `requirements.txt`: Lists the required Python packages and their versions.

## Acknowledgments

This project is a basic implementation of a URL Shortener web application. The UI design and frontend development utilize the Tailwind CSS framework for a visually appealing and responsive design. The Django backend handles the URL shortening logic and AJAX communication with the frontend. This project can serve as a starting point for a more comprehensive and feature-rich URL Shortener application.

For a more detailed overview of the application and its functionality, please refer to the demo video linked above.
