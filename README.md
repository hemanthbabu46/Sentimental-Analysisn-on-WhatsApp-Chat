Here's a detailed README file for your GitHub repository:

---

# Sentiment Analysis on WhatsApp Chat Data

This repository contains a project focused on performing sentiment analysis on WhatsApp chat data. The primary goal is to extract insights and visualize the sentiments present in the chat using various natural language processing (NLP) techniques. Streamlit has been used to create an interactive web application that displays the results of the analysis.

## Project Overview

The project is divided into several key phases, each aimed at processing and analyzing the chat data:

1. **Data Collection**:
   - The project begins by exporting the chat data from WhatsApp. The exported data is usually in `.txt` format.
   - The chat file is then loaded into the project for further processing.

2. **Data Preprocessing**:
   - **Text Cleaning**: The raw text data contains timestamps, sender names, and various emojis or special characters. These are cleaned to ensure only the necessary text is analyzed.
   - **Tokenization**: The cleaned text is split into individual words (tokens) to allow for further processing.
   - **Stopwords Removal**: Common words that do not contribute to the sentiment (e.g., 'and', 'the', 'is') are removed to focus on the meaningful words.

3. **Sentiment Analysis**:
   - **Sentiment Scoring**: Each message is scored based on its sentiment using a pre-trained sentiment analysis model (like VADER or TextBlob). The score typically ranges from -1 (negative) to +1 (positive), with 0 being neutral.
   - **Categorization**: The sentiment scores are categorized into positive, negative, and neutral sentiments.

4. **Data Visualization**:
   - **Streamlit Integration**: The sentiment analysis results are visualized using Streamlit. Various plots and charts are generated to showcase the distribution of sentiments over time, the most positive/negative days, and more.
   - **Word Clouds**: Word clouds are generated for positive and negative sentiments, highlighting the most frequently used words in each category.

5. **User Interaction**:
   - The Streamlit app allows users to interact with the visualizations. Users can select date ranges, view specific chats, and explore the sentiment trends over time.

## Installation and Setup

To run the project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/hemanthbabu46/Sentimental-Analysisn-on-WhatsApp-Chat.git
   cd Sentimental-Analysisn-on-WhatsApp-Chat
   ```

2. **Install the Required Packages**:
   Make sure you have Python installed. Then, install the necessary dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Streamlit App**:
   Start the Streamlit app by running:
   ```bash
   streamlit run app.py
   ```

   This will launch the web app in your default browser, where you can interact with the sentiment analysis results.

## How to Use

1. **Upload Chat Data**: Once the app is running, upload your WhatsApp chat data in `.txt` format.
2. **View Analysis**: The app will process the data and display the sentiment analysis results through various visualizations.
3. **Explore Insights**: Use the interactive features to explore different time periods, specific chats, and detailed sentiment trends.

## Future Work

Potential improvements and extensions to this project include:

- Enhancing the sentiment analysis model with more sophisticated techniques like transformer-based models (e.g., BERT).
- Adding support for multi-language sentiment analysis to handle chats in different languages.
- Including additional visualizations and metrics, such as sentiment heatmaps or conversation-level analysis.

## Contributing

Contributions are welcome! If you find any bugs or have suggestions for new features, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

This README file provides a comprehensive overview of the project, guiding users through the process of understanding, setting up, and using the sentiment analysis tool.
