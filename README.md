# PROJECTS
# Sentiment Analysis Web Application

This project is a simple Sentiment Analysis Web App built with Flask and Scikit-learn. It preprocesses user input, predicts the sentiment (Positive or Negative), and displays the result through an interactive web interface. The application is designed to run seamlessly in a Jupyter Notebook environment.

## Features

- **Sentiment Analysis**: Analyzes user-provided text and determines whether the sentiment is positive or negative.
- **Preprocessing Pipeline**: Includes case normalization, stopword removal, stemming, punctuation removal, and emoji handling.
- **Interactive Interface**: A modern and user-friendly web interface for input and output.
- **Integrated Execution**: The app is designed to run directly from a Jupyter Notebook, eliminating the need for external configuration files.

## Prerequisites

Ensure you have the following installed:

1. **Python**: Version 3.7 or higher.
2. **Jupyter Notebook**: Install via `pip install notebook` if not already installed.
3. **Required Libraries**:
   ```bash
   pip install flask scikit-learn nltk bs4 emoji
   ```

## How to Run the Application

1. **Open the Jupyter Notebook**
   - Copy the provided code into a new cell in your notebook.
   - Execute the cells sequentially to initialize the app.

2. **Access the Web App**
   - The application will start on `http://127.0.0.1:5000`.
   - A browser window should open automatically. If not, use the clickable link provided in the notebook output or manually navigate to the URL.

3. **Analyze Sentiment**
   - Enter text into the provided input box and click the "Analyze Sentiment" button.
   - The app will display whether the sentiment is **Positive 😊** or **Negative 😔**.

## Key Components

1. **HTML Template**:
   - The `HTML_TEMPLATE` variable defines the structure and style of the web interface.
   - Features a gradient background, polished buttons, and dynamic result display.

2. **Preprocessing Function**:
   - Tokenizes and stems text.
   - Removes HTML tags, emojis, punctuation, and stopwords for better accuracy.

3. **Model Training**:
   - A mock dataset is used to train a Multinomial Naive Bayes model.
   - TF-IDF vectorization transforms text data into numerical form.

4. **Flask Routes**:
   - `home`: Renders the main page.
   - `predict`: Processes input text and predicts sentiment.

## Customization

- **Styling**: Update the `HTML_TEMPLATE` variable to modify the app's appearance.
- **Model**: Replace the mock dataset with a larger dataset to improve model accuracy.

## Example

### Input
```
"The food was amazing!"
```

### Output
```
Positive 😊
```

## Future Enhancements

- Expand the training dataset for improved accuracy.
- Implement additional preprocessing steps for diverse text inputs.
- Deploy the application on platforms like Heroku or AWS for wider accessibility.

## License

This project is licensed under the MIT License.

---
**Happy Sentiment Analysis!**

