# Unique Words Model

This repository contains a Python script for training a language model using unique words from a given text corpus. The trained model can be used to generate text or perform various natural language processing (NLP) tasks.

## Table of Contents

- [Introduction](#introduction)
- [Usage in Google Colab](#usage-in-google-colab)
- [Example](#example)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The **Unique Words Model** script is designed to train a language model using unique words present in a text corpus. It uses recurrent neural networks (RNNs) to learn the patterns and relationships between words, allowing it to generate coherent text or perform other NLP tasks.

## Usage in Google Colab

To use the **Unique Words Model** script in Google Colab, follow these steps:

1. Open Google Colab in your web browser.

2. Click on `File` > `New Notebook` to create a new notebook.

3. In a code cell, run the following command to clone the repository:
   ```python
   !git clone https://github.com/Coderdivine/UniqueWordsModel.git
   ```

4. Change into the project directory:
   ```python
   %cd UniqueWordsModel
   ```

5. Install the required dependencies:
   ```python
   !pip install -r requirements.txt
   ```

6. Upload your input text corpus file to Google Colab by clicking on the folder icon in the left sidebar, selecting the file, and choosing "Upload".

7. In a code cell, run the following command to train the language model:
   ```python
   !python train_model.py --input <path_to_input_file> --output <path_to_output_model>
   ```

   Replace `<path_to_input_file>` with the path to your uploaded input file and `<path_to_output_model>` with the desired path to save the trained model.

8. Once the training process completes, you can use the trained model for various NLP tasks, such as text generation, by running the following command in a code cell:
   ```python
   !python generate_text.py --model <path_to_trained_model> --length <desired_text_length>
   ```

   Replace `<path_to_trained_model>` with the path to your trained model file and `<desired_text_length>` with the desired length of the generated text.

## Example

To train a language model using unique words from a text corpus file named `corpus.txt` and save the trained model as `unique_words_model.pth`, you can use the following command:

```python
!python train_model.py --input corpus.txt --output unique_words_model.pth
```

After training, to generate text using the trained model, you can run the following command:

```python
!python generate_text.py --model unique_words_model.pth --length 100
```

This will generate text with a length of 100 characters using the trained model.

## Contributing

Contributions to this repository are always welcome. If you find any issues or want to add new features, please submit a pull request with your changes. Make sure to follow the existing code style and provide appropriate documentation for the modifications.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code for both commercial and non-commercial purposes.
