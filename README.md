# Movie Prediction

This project provides a web application for predicting movie ratings or success using a pre-trained machine learning model. The application is built using Streamlit and allows users to input various movie features to get predictions.

## Features

- Input various movie-related features to predict ratings or success.
- Provides a user-friendly interface for interaction.
- Utilizes a pre-trained model for accurate predictions.

## Prerequisites

- Python 3.7 or higher

## Installation

1. **Clone the repository**

   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```

2. **Create and activate a virtual environment (optional but recommended)**

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows use `env\Scripts\activate`
   ```

3. **Install the required packages**

   Create a `requirements.txt` file with the following content:

   ```txt
   streamlit
   pandas
   numpy
   pickle
   ```

   Then run:

   ```bash
   pip install -r requirements.txt
   ```

4. **Save the pre-trained model**

   Ensure you have the pre-trained model saved in the file `movie_prediction_model.pkl`. If you need to save the model, use the following code:

   ```python
   import pickle

   # Assuming `model` is your trained model
   with open('movie_prediction_model.pkl', 'wb') as file:
       pickle.dump(model, file)
   ```

5. **Run the Streamlit app**

   ```bash
   streamlit run app.py
   ```

## Usage

1. Open the application in your browser (typically at `http://localhost:8501`).
2. Use the sidebar to input movie features.
3. Click on "Predict" to get the prediction.

## Notes

- Customize the `app.py` and model according to your specific features and prediction goals.
- Ensure all feature names in `app.py` match those used in your model training.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
