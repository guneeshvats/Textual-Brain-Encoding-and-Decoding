# Textual Brain Encoding and Decoding (fMRI Image Analysis and NLP)

This project explores the brain encoding and decoding tasks using fMRI data and textual stimuli. The goal of **brain encoding** is to generate fMRI brain representations given a textual stimulus, while **brain decoding** involves reconstructing the original textual stimuli from fMRI data. We developed both encoders and decoders for textual stimuli using NLP sentence representations.

## Project Overview
For this study, we built **4 encoders** and **4 decoders** for each region of the brain, across **2 participants**. Using advanced sentence representations, such as **BERT CLS**, **BERT Pooled**, and **GloVe**, we trained models to handle fMRI data from different brain regions. Specifically:

- **Ridge Regression Models** were used for both encoding and decoding.
- We utilized **3 sentence representations**: BERT CLS, BERT Pooled, and GloVe.
- This resulted in a total of **48 trained models**:
  - 2 Participants × 4 Brain ROIs × 3 Sentence Representations × 2 (Encoder and Decoder) = 48 Models.

We evaluated our models using **2v2 accuracy** and **Pearson’s Correlation**, both of which are computed using the following formulae.

![2v2 Accuracy Plot](https://github.com/guneeshvats/Textual-Brain-Encoding-and-Decoding/assets/70188630/48ce7c00-ff30-4991-b913-c6dbd992b90d)

![Pearson's Correlation Plot](https://github.com/guneeshvats/Textual-Brain-Encoding-and-Decoding/assets/70188630/05c82ee1-3817-47d8-9dbf-20462087369e)

## Dataset Description
The dataset comprises **627 sentences** and the corresponding fMRI data recorded while these sentences were presented to participants. fMRI data is provided for four specific brain regions (ROIs):

- **Language**: Associated with language processing, comprehension, and word meaning.
- **Vision**: Related to visual object processing and recognition.
- **Task Positive**: Linked to attention and salience information processing.
- **Default Mode Network (DMN)**: Engaged in semantic processing and mind-wandering.

### Dataset Files
The dataset includes the following files:

- **stimuli.txt**: Contains 627 sentences, one per line.
- **subj1.npy**: fMRI data for Subject 1, organized as a dictionary with keys representing the brain regions and values containing fMRI data for each sentence.
- **subj2.npy**: fMRI data for Subject 2, similarly structured as `subj1.npy`.

## Repository Structure
This project was developed as part of a **Cognitive Science and AI course**. The detailed problem statements, dataset information, and stimuli details are provided in the **'Assignment.pdf'** file.

- **Analysis**: The results and analysis are documented in the **'Report'** file.
- **Solution Code**: The implementation, including both encoder and decoder models, is available in the **'Code.ipynb'** file. The code is organized as follows:

![Code Structure](https://github.com/guneeshvats/Textual-Brain-Encoding-and-Decoding/assets/70188630/1fae2726-55f5-4b92-800c-d615b8228154)

We hope this project provides valuable insights into the intersection of fMRI image analysis and natural language processing.
