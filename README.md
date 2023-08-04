# ASL-detector
This project focuses on the development of a sign language recognition and sentence generation system to help deaf and mute people participate and express themselves in online meetings and conference. Though sign language recognition systems already exists, they are not capable of generating complete sentences. For eg: "I am going home" sentence use sign language can be broken down into 3 words - "I" , "go", "home". But the framing of complete sentence is not yet resolved. The objective is to recognize the hand sign and also filling in the extra details such as prepositions to give prediction on what the sentence could be. 

Sign detection is performed using 2 different methods.
i) One way is to perform image analysis using detection model. YOLOv5 is used in this technique.
ii) A better way is through action sequence detection using an LSTM model from media pipe data.

Now that we have the signs detected, we can process the words to form complete sentences.
Again a comparative approach is followed here:
i) Using a GPT-2 model trained to correct senteces given wrong / incomplete sentences using grammar.
ii) T5 model trained on the same dataset. But T5 is small and performed better given the computational constraints.
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
