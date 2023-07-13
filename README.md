# Handwritten Digits Generation using GAN

This project aims to generate realistic handwritten digit images using a Generative Adversarial Network (GAN). The GAN architecture consists of a generator and a discriminator that compete against each other to generate high-quality digit images.

## Dataset
The project utilizes the MNIST dataset, which is a widely-used benchmark dataset for handwritten digit recognition. The MNIST dataset contains a large number of grayscale images of handwritten digits from 0 to 9. Each image is a 28x28-pixel square.

## Dependencies
The following dependencies are required to run the project:
- Python (3.7+)
- TensorFlow (2.0+)
- Keras (2.2.0+)
- NumPy
- Matplotlib

## Project Structure
The project includes the following files:
- `generator.py`: Defines the generator model that generates digit images.
- `discriminator.py`: Defines the discriminator model that distinguishes real and generated images.
- `gan.py`: Combines the generator and discriminator into a GAN model and handles the training process.
- `train.py`: Trains the GAN using the MNIST dataset and saves the trained models.
- `generate_digits.py`: Loads the trained models and generates handwritten digit images.
- `utils.py`: Contains utility functions for data preprocessing and visualization.
- `README.md`: Instructions and information about the project.

## Usage
To train the GAN:
1. Ensure that the MNIST dataset is downloaded or available in the `data/` directory.
2. Run the `train.py` script. Adjust the hyperparameters and training configurations as needed.
3. The script will train the GAN on the MNIST dataset and save the trained models.

To generate digit images:
1. Ensure that the trained generator and discriminator models are available in the `models/` directory.
2. Run the `generate_digits.py` script.
3. The script will load the trained models and generate handwritten digit images, saving them in the `generated_digits/` directory.

## Results
The GAN model, after adequate training, should be able to generate realistic handwritten digit images that resemble the ones in the MNIST dataset. The quality and diversity of the generated images will depend on the training duration and the hyperparameters chosen.

## Acknowledgments
The project is inspired by the original GAN paper by Ian Goodfellow et al. (2014) and adapts the concepts to the specific task of generating handwritten digits using the MNIST dataset.



