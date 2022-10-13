# UTS-RP22-AI-assisted_Multimedia_Summarisation

32933 Research Project 2022 Spring

Kam Kin Kwok 13834724
Sui Lung Hui 14082325
Yan Man Lo   14083897

supervisor: Dr. Wei Liu

## Project description
Multimedia is a form of communication that combines different content forms such as text, audio, images, animations, or video into a single interactive presentation.

Text Summarization is the task of generating a concise summary that captures an abstract of the source text. The generated abstractive summaries involve paraphrasing, potentially containing new phrases and sentences that may not appear in the source text.

We created a method to summarise both texts and visuals as part of this assignment. This is a more realistic scenario because web pages and publications typically contain both of these sorts of data.

## Prerequisites
The project is written in python under Anaconda's jupyter notebook in Windows.

To run the program, you will need to have the following:

1. Pre-trained model for image captioning and text summarization from Huggindface:
https://huggingface.co/nlpconnect/vit-gpt2-image-captioning
https://huggingface.co/google/pegasus-xsum

2. webdriver for chrome:
https://chromedriver.chromium.org/downloads

3. Anaconda environment which could be import from the .yaml file in the repository

4. The jupyter notebook in the repository

5. Update the path in the notebook for the locations of chromedriver and models on your machine.

## Flow
1. Provide a news URL from the guardian. e.g. https://www.theguardian.com/world/2022/sep/11/margrethe-ii-denmark-jubilee-europe-only-reigning-queen
2. Perform web scraping to extract images and text content from the given URL by selenium. Save a local copy of images.
3. Summarize the text by pegasus
4. Image captioning by flax
5. Concatenate the Summarized text with image captions
6. Perform text summarization on the concatenated text


