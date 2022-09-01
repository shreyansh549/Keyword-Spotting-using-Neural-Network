ABSTRACT:

Spoken Keyword Spotting is the task of identifying predefined words (called as keywords) from speech. Rapid developments and research in the areas of voice-based interaction with machines has tremendously influenced the heavy adaptation of these technologies into everyday life.

With the development of devices such as Google Home, Amazon Alexa and Smartphones, speech is increasingly becoming a more natural way to interact with devices. 
However, always-on speech recognition is generally not preferred due to its energy inefficiency and network congestion that arises due to continuous audio stream from millions of devices to the cloud. Processing such a large amount of audio stream will require more time and adds to the latency and can have privacy issues.

Keyword Spotting (KWS) provides an efficient solution to all the above issues. Modern day voice-based devices first detect predefined keyword(s) — such as ”OK Google”, ”Alexa” — from the speech locally on the device. On successfully detecting such words, a full scale speech recognition is triggered on the cloud (or on the device).
 Since the KWS system is always-on, it is highly preferred to have low memory footprint and computation complexity, but with high accuracy and low latency. We explore using a hybrid system consisting of a Convolutional Neural Network and a Support Vector Machine for KWS task.
 
 
 
 OBJECTIVES AND GOALS:


To provide a suitable solution for the KWS setting, we look at a hybrid system — consisting of a Convolutional Neural Network (CNN) and a Support Vector Machine (SVM). We train the CNN model to be a feature extractor that embeds the input into a suitable representation that properly captures the relevant information. We consider the output of the 256 dimensional penultimate dense layer (marked with arrow on figure below) as an embedding of the input feature. We train the OCSVM with these embedding as input. The performance of OCSVM is highly dependent on its hyperparameters values. To obtain the best performing OCSVM, we tune the hyperparameters using scikit-optimize library.



CONCLUSION :



A small footprint reconfigurable CNN-OCSVM based KWS system is proposed in this work. The raw performance numbers shows that this model outperforms many of the models in the literature. However, a direct comparison is not meaningful be cause of the differences in the datasets and the actual keywords. To prove this claim a lot of further work is necessary, such as performance analysis under noise and far-field conditions.The model can be experimented for multiple sets of Keywords to test the accuracy and robustness of the model.


 
