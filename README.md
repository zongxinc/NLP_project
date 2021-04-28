# NLP_project

This project is related to gun violence news frame classification (see [here](https://www.aclweb.org/anthology/K19-1047/) for
background in news frame classification on the gun violence frame dataset). The
gun violence frame data can be found in this [folder](https://drive.google.com/drive/folders/19O_DaW6zwH9tRChXZzUSYiTsIeBsEI_e?usp=sharing). You can find the description
of columns in the annotated data file (GVFC AnnotatedHeadlines.xlsx) in the
two Codebook files. The folder also contains a zip file of lead images for the
articles. The names of lead images for the articles can be found in the column
ImageID of the annotated data file. The annotated data file also contains
textual information about the image, including generated captions of the image
(generated automatically using [Transform-and-Tell](https://github.com/alasdairtran/transform-and-tell) image captioning system),
as well as Google Visual API tags of the image that contains a string of web
entities and pages detected in the image (see [here](https://cloud.google.com/vision/docs/detecting-web) for more details).

## Our task

 Conducting relevance classification. Not all lead images of articles are
relevant to the frames of the articles’ headlines. Column V3Relevance of
the annotated data file contains annotations of whether the lead image of
an article is relevant (1) or not relevant (0) to the frame of the article’s
headline. You would train models to predict relevance of lead images to
their headline frames. The highest accuracy obtained so far for relevance
prediction is 71% using headlines and image captions. You can explore
different models and/or data (images, captions, Google Visual API tags,
whole text, summary of whole text, etc.) for predicting relevance. You can
also explore [text generation models](https://huggingface.co/transformers/v2.0.0/examples.html#language-generation) (GPT-2, etc.) for relevance prediction e.g., what’s the probability that a pre-trained text generation model
generates a particular caption given a headline? Does caption of relevant
images score higher than caption of irrelevant images? (watch [here](https://www.youtube.com/watch?v=G5lmya6eKtc) on
why text generation model may be the future of NLP pre-trained models)

## Result

 Our result in at RelevanceDetector.ipynb, or see the result in pdf format at RelevanceDetector.pdf


## Group Member

Zongxin Cui,
Mahir Patel,
Sooyoun Lee,
Yanjie Chen 
