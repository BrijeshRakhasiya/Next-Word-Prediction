# Next Word Prediction Using LSTM on Hamlet Dataset

## Project Description


This project develops a deep learning model to predict the next word in a given sequence of words using Long Short-Term Memory (LSTM) networks. LSTMs are well-suited for sequence prediction tasks due to their ability to capture long-term dependencies in text.

The project workflow includes:

1. **Data Collection:** Using the text of Shakespeare's *Hamlet* as the dataset, providing rich and complex language for the model to learn.

2. **Data Preprocessing:** Tokenizing the text, converting it into sequences, and padding them to uniform lengths. The data is then split into training and testing sets.

3. **Model Building:** Constructing an LSTM model with:
   - An embedding layer to represent words in dense vectors,
   - Two LSTM layers to capture sequence patterns,
   - A dense output layer with softmax activation to predict the probability distribution of the next word.

4. **Model Training:** Training the model on the prepared sequences with early stopping to prevent overfitting by monitoring validation loss.

5. **Model Evaluation:** Testing the model’s ability to predict the next word accurately on example sentences.

6. **Deployment:** A Streamlit web app allows users to input a sequence of words and receive real-time next word predictions.

## Dataset

- Source: *Hamlet* text file (`hamlet.txt`).
- Preprocessing includes cleaning, tokenization, sequence generation, and padding.

## Technologies Used

- Python 3.11
- TensorFlow / Keras
- NumPy
- Pandas
- nltk
- Streamlit (for deployment)

## Installation

1. Clone the repository:
```
https://github.com/BrijeshRakhasiya/Next-Word-Prediction.git
```
2. Navigate to the project directory:
```
cd next-word-prediction
```
3. Install required packages:
```
pip install -r requirements.txt
```

## Usage

- Run the training script or notebook to preprocess data and train the LSTM model.
- Use the Streamlit app to input text sequences and get next word predictions in real-time:

```
streamlit run app.py
```


## Model Performance

- Achieved approximately 80% accuracy on the validation set.
- The model effectively captures Shakespearean language patterns to predict the next word.

## Contributing

Contributions are welcome! Please fork the repository and submit pull requests with improvements or bug fixes.

## License

This project is licensed under the MIT License.
