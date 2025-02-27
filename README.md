# Subjectivity Detection Case Study

## Overview

In this case study, you will work on a **subjectivity detection** task, which aims to accurately determine the subjectivity of a given text snippet. Subjectivity refers to the expression of opinions, sentiments, or personal experiences within the text, while objectivity represents factual information without personal biases.

For this case study, the dataset consists of over 1,100 tweets in English, and the sentences are represented as a list of images. Each image corresponds to a single character in the sentence. Your task is to extract the text from the sequence of character images and use it for classification.

The dataset is stored in a **JSON** file, where each entry has the following attributes:

- **sentence_id**: A unique identifier for each sentence.
- **image_paths**: A list of strings representing the paths to the images for each character in the sentence. For spaces, it will be represented as a string with a space `" "`.
- **label**: A binary label for the sentence (0 for OBJ, 1 for SUBJ).

### Example

```json
{
  "sentence_id": "8745d4da-91c9-4538-acee-b0e7b1c413fd",
  "image_paths": [
    "./images/e5b0e1cb52a548e78112a8dff39b9947.png",
    "./images/c7e54e8c43ff4464b6b5d68f085b8595.png",
    "./images/4325830389b1424b8ea6bdeec5008031.png",
    " ",
    "./images/8151b6c60621444f848644fa8bacf644.png",
    "./images/3c4db43560534cc092088b6400845329.png",
    "./images/a6b8c0e9b7bc46d9836f79ab509d45d2.png",
    "./images/83b5ccd8479a456cbe51a3ea14d2a491.png"
  ],
  "label": "SUBJ"
}
