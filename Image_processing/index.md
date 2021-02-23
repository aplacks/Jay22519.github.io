# Image Processing Module

### Team -

| S. no | Name              | Enrollment no |
| ----- | ----------------- | ------------- |
| 1     | Rishikesh Rachchh | [BT18CSE091]  |
| 2     | Harshal Sable     | [BT18CSEXXX]  |
| 3     | Rishabh Agrawal   | [BT18CSEXXX]  |
| 4     | Ashish Lakra      | [BT18CSE038]  |

#### Our project of Automatic Answer checking is divided into 2 modules ->

##### 1) Converting given input image file into text file

##### 2) Using the text file generated to find how correcrt the given answer is

<b> This page deals with the first module . The crux of it is to use ---. </b>

#### Microsoft Azure Read API
Computer Vision Read API is Azure's latest OCR technology that is optimised to extract printed or handwritten text, digits, currency symbols from text-heavy image files and PDF documents. The Read API supports 7 languages for printed text and only English language for handwritten text. The time for completion of the text extraction process depends on the volume of the text and the number of pages in the document. For this project we will extract handwritten text from image files only because the free tier subscription of the API is limited to process only first two pages of PDF document. 

Input requirements <br>
Supported file formats: JPEG, PNG, BMP, PDF and TIFF <br>
The file size must be less than 50 MB (4 MB for the free tier) and dimensions at least 50 x 50 pixels and at most 10000 x 10000 pixels.


<!-- Document similairty has many aspects . Other than capturing the syntactic similarity we also have to capture the semantic similarity and context and understand that whether
2 given texts (though entirely differnet in words) are same or not .

So we are using the following methods to capture semantic , syntactic and contextual meaning of the texts/documents

#### Words Mover Distance

Word Mover’s Distance targets both semantic and syntactic approach to get similarity between text documents. The WMD distance measures the dissimilarity between two text documents as the
minimum amount of distance that the embedded words of one document need to “travel” to reach the embedded words of another document.[1]

Following the link to the a sample code jupyter notebook to show how WMD works

https://github.com/Jay22519/Automatic-Answer-checker-/blob/main/Language%20Processing/Sample_WMD.ipynb

#### BERT Model

Without any doubt we can say that BERT is magic !!!

“BERT stands for Bidirectional Encoder Representations from Transformers. It is designed to pre-train deep bidirectional representations from unlabeled text by jointly conditioning on both
left and right context. As a result, the pre-trained BERT model can be fine-tuned with just one additional output layer to create state-of-the-art models for a wide range of NLP tasks.”[2]

Now the bi-directionality of the BERT's transformer helps it in learning from context from both sides . That's why it can be used for many tasks such as Question Answering , Predicting
next word , document similairty and many such NLP tasks. We'll use uncased bert model for training our model .
<b>Though we can use the same tokenizer for this task we are finding for better tokenizer which will perform better from scholar point of view </b>

Here is the link for sample jupyter notebook code to show how bert works <b> Yet to add </b>

#### Google's Universal Sentence Encoder (USE)

<b> This is to yet to be updated </b>

#### Further problems to solve

<ol type="1">
  <li>How to overcome document length constraint in BERT</li>
  <li>Find better tokenizer for Bert</li>
  <li>Leveraging the use of WMD</li>
  <li>Add further utility options like spelling correction , keyword finder , length constraint (word limit)</li>
  <li> Solve the problem of negation case </li>
</ol>

[1] ->https://towardsdatascience.com/word-movers-distance-for-text-similarity-7492aeca71b0#:~:text=Word%20Mover's%20Distance%20targets%20both,embedded%20words%20of%20another%20document.
<br>
[2] -> https://www.analyticsvidhya.com/blog/2019/09/demystifying-bert-groundbreaking-nlp-framework/ -->
