# Emotion-Cause-Pair-Extraction

Emotion Cause Pair Extraction is a new task proposed by Rui Xia and Zixiang Ding in 2019 (https://arxiv.org/abs/1906.01267) and this task has been implemented in this project.But this is not a exact implementation of the models presented in the paper, the idea of two stage approach mentioned in the paper has been used in the project.

Emotion-Cause data used for the implementation (http://www.site.uottawa.ca/~diana/resources/emotion_stimulus_data/):Diman Ghazi, Diana Inkpen & Stan Szpakowicz (2015). “Detecting Emotion Stimuli in Emotion-Bearing Sentences”. Proceedings of the 16th International Conference on Intelligent Text Processing and Computational Linguistics (CICLing 2015), Cairo, Egypt.

Since there is no English dataset available for Emotion Cause Pair Extraction task, Emotion Cause extraction dataset mentioned above is preprocessed and used.The sentences in the dataset are divided into clauses and preprocessed so as to make it suitable for Emotion-Cause Pair extraction task. If any one of the emotion seed word mentioned in emotion_seeds.pickle file is present in a clause it is  a emotion clause. If "cause" XML tag is present in the clause then it is cause clause. 

Python 3.6.9 used for this project.
Dependencies required: 
sklearn,tensorflow 2.0, numpy, pandas, scipy, gensim, keras and ktrain.
Use "pip install" to install the above dependencies.
This jupyer notebook can be run directly on Google colab and only ktrain is required to be installed on Google colab if incase you want to run the BERT model.
Change the locations of the emotion_data.txt and emotion_seeds.pickle accordingly to run the code.
