# ASL-detector
We try to detect sign language and form gramatically complete sentences by correcting and concatenating single words. Here the problem is tried to be solved using 2 different approaches.
<p></p><br>

**Sign_language_detection** - Object detection method<br>
-> It contains files related to sign language detection using YOLOv5 and complete sentence formation using GPT-2 and compare with T5 <br>
-> It has 2 folders <br>
words - YOLOv5 related files with "Sign language Generation.ipynb" file that trains the model and test it.<br>
grammar_correction - It uses GPT2 and T5 model and fit them with custom dataset for grammar correction.<br>
<p></p><br>

**Action detection** - Sequential data analysis and prediction <br>
-> It uses mediapipe and LSTM trained on action sequences for sign language detection. File - ASL.ipynb<br>
-> action.h5 file contains the trained model weights.
