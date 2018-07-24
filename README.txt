Here are programs to evaluate your model:

Monobloc_evaluator needs bounding boxes while Monobloc_evaluator(classifier) needs tags.
Of course, these programs need also valid.json

Monobloc_evaluator is a program which will use our model to predict every image of the validation set.
On every prediction, we will see if our model has right on this question :
"Does the image contain a monobloc chair?" and evaluate it

mAP_master is a folder which contain an algorithm to calculate a mAP score. This algo was made by João Cartucho and is on his github : https://github.com/Cartucho/mAP
I only create a notebook to create .txt files in order to use João algorithm