# Sentiment Analysis Flask App

## Project Overview

This project is a simple web application built using Flask, which takes user input from an HTML form and performs sentiment analysis on the provided text. The app measures whether the inputted phrase is positive, negative, or neutral using the `TextBlob` library and displays the result back to the user.

## Features

- **User Input:** Users can input a phrase through a web interface.
- **Sentiment Analysis:** The app processes the input text using `TextBlob` and determines the sentiment polarity.
  - **Polarity:** A value between -1.0 and 1.0, where:
    - Negative: less than 0
    - Neutral: 0
    - Positive: greater than 0
- **REST API:** The project includes a RESTful API that can be accessed using tools like Postman to send input data and receive sentiment results in JSON format.
  
## Technology Stack

- **Backend:** Flask (Python)
- **Frontend:** HTML, CSS
- **Sentiment Analysis:** TextBlob
- **Database:** MySQL
- **API Testing:** Postman

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ChathuminiBandara/TextBlob_Flask.git
   ```
2. Navigate to the project directory:
   ```bash
   cd TextBlob_Flask
   ```
3. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Flask app:
   ```bash
   python app.py
   ```
5. Open the app in your browser at `http://127.0.0.1:5000`.

## API Usage

To test the API:
1. Use Postman to send a `POST` request to the following endpoint:
   ```
   POST http://127.0.0.1:5000/sentiment
   ```
2. In the request body, use the following JSON format:
   ```json
   {
     "phrase": "Your input text here"
   }
   ```

## Future Improvements

- Add authentication for API access.
- Implement more advanced NLP features such as entity recognition and language translation.
- Expand database functionality for storing and tracking sentiment analysis results.

\
