# Textual-Brain-Encoding-and-Decoding 
The brain encoding problem aims to automatically generate fMRI brain representations given a stimulus. The brain decoding problem is the inverse problem of reconstructing the stimuli given the fMRI brain representation. In this task we would be constructing an encoder as well as a decoder for textual stimuli. Textual stimuli is processed through the conepts of NLP sentence represetnations. 
<br><br>
We need to build 4 encoder and 4 decoders for each region of brain explained in the bottom of this read.me, for each participant(2). Using sentence representation like BERT CLS, BERT Pooled, and GloVe. So we can say:- <br>
We have used <strong>Ridge regression model</strong> to create encoders and decodes for the given FMRI dataset. <em><strong>3 different sentence representations are used : BERT CLS, BERT Pooled and GloVe</strong></em>. 2 Participants x 4 ROI FMRIs x 3 Sentence representations x 2 (Decoder and Encoder model) = 48
<br>
So, a total of <strong>48 models</strong> were trained. We obtained the above given plots for <strong>2v2 accuracy and
Pearson’s Correlation</strong> computed for each model using the following formulae.  Damn that's a lot of models!!!
<br>
![image](https://github.com/guneeshvats/Textual-Brain-Encoding-and-Decoding/assets/70188630/48ce7c00-ff30-4991-b913-c6dbd992b90d)


![image](https://github.com/guneeshvats/Textual-Brain-Encoding-and-Decoding/assets/70188630/05c82ee1-3817-47d8-9dbf-20462087369e)

<h3>About the Dataset (Avail in the Assignment sheet)</h3>

Dataset consists of 627 sentences and the corresponding fMRI, recorded when the sentences were presented to a subject one by one. fMRI is provided for four different brain ROIS listed below:<br><br>
• <strong>Language:</strong> Related to language processing, understanding, word meaning, and sentence
comprehension. <br>
• <strong>Vision:</strong> Related to the processing of visual objects, object recognition<rb>
• <strong>Task Positive:</strong> Related to attention, salience information. <br>
• <strong>Default Mode Network (DMN):</strong> Linked to the functionality of semantic processing.<br><br>
Dataset contains three files:<br><br>
• <strong>stimuli.txt:</strong> It contains 627 sentences, each in one line.<br>
• <strong>subj1.npy:</strong> Contains fMRI data for Subject 1. Stored as a dictionary, with keys as the
four brain regions and values as the corresponding fMRI for 627 sentences.<br>
• <strong>subj2.npy:</strong> Contains fMRI data for Subject 2. Stored as a dictionary, with keys as the
four brain regions and values as the corresponding fMRI for 627 sentences.

<h3>Files in Repository</h3>
<strong>This is part of my Cognitive Science and AI course</strong>. The information about Problem statements, Links to dataset, stimuli are given in the pdf named 'Assignment' in this repository. 
<br>

The analysis of the results is in the file named <strong>'Report'</strong>
The solution code is in the ipynb file named <strong>'Code'</strong> and it is structured in the following way for both Encoder and Decoder Models: 
<br><br> 
![image](https://github.com/guneeshvats/Textual-Brain-Encoding-and-Decoding/assets/70188630/1fae2726-55f5-4b92-800c-d615b8228154)





