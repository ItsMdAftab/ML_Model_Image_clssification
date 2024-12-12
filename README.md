

# Image Classification Web App

This repository contains the code for an interactive image classification web application built using Streamlit. The app allows users to upload images and classify them using either the MobileNetV2 model trained on ImageNet or a custom model trained on CIFAR-10.

## Features

- **User-Friendly Interface:** A simple and interactive web interface powered by Streamlit.
- **Model Options:** 
  - **MobileNetV2:** Utilizes the MobileNetV2 model pre-trained on the ImageNet dataset for general image classification.
  - **CIFAR-10 Model:** Classifies images using a custom model trained on the CIFAR-10 dataset, which includes 10 different classes.
- **Real-Time Classification:** Provides immediate classification results along with confidence scores.
- **Image Upload:** Users can upload images in JPEG or PNG format.

## Installation

### Prerequisites

- Python 3.7 or higher
- TensorFlow
- Streamlit
- NumPy
- Pillow (PIL)

### Setup

1. **Clone the repository:**

    ```sh
    git clone https://github.com/yourusername/image-classification-app.git
    cd image-classification-app
    ```

2. **Create a virtual environment:**

    ```sh
    python -m venv myenv
    ```

3. **Activate the virtual environment:**

    - On Windows:

        ```sh
        myenv\Scripts\activate
        ```

    - On macOS/Linux:

        ```sh
        source myenv/bin/activate
        ```

4. **Install the required packages:**

    ```sh
    pip install tensorflow streamlit numpy pillow
    ```

## Usage

1. **Run the Streamlit app:**

    ```sh
    streamlit run app.py
    ```

2. **Navigate to the web interface:**

    Open your web browser and go to `http://localhost:8501`.

3. **Upload an image:**

    - Click on "Choose an image..." and upload a JPEG or PNG image.

4. **Choose the model:**

    - Use the sidebar to select either "CIFAR-10" or "MobileNetV2 (ImageNet)".

5. **View the results:**

    - The app will display the uploaded image and provide classification results with confidence scores.

## Code Overview

### MobileNetV2 Classification

- **Function:** `mobilenetv2_imagenet()`
- **Description:** 
  - Allows users to upload and display an image.
  - Preprocesses the image for the MobileNetV2 model.
  - Uses the MobileNetV2 model to classify the image.
  - Displays the top prediction with the label and confidence score.

### CIFAR-10 Classification

- **Function:** `cifar10_classification()`
- **Description:** 
  - Allows users to upload and display an image.
  - Preprocesses the image for the CIFAR-10 model.
  - Uses the custom CIFAR-10 model to classify the image.
  - Displays the predicted class and confidence score.

### Main Function

- **Function:** `main()`
- **Description:** 
  - Provides navigation options in the sidebar.
  - Calls the appropriate classification function based on user selection.

## Future Improvements

- Add support for more image classification models.
- Enhance the user interface for a better experience.
- Implement more advanced image preprocessing techniques.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please read the [CONTRIBUTING](CONTRIBUTING.md) guidelines for more information.

## Acknowledgments

- Special thanks to the open-source community for their invaluable resources and tools.
- Inspired by advancements in AI and machine learning for image classification.

---

