# SQuAD2.0_project
This is my project in the lecrture Deep learning and its application
I use BERT to complete the task of English reading comprehension 

Fisrt I reproduce BERT model in pytorch,
then initiate few improvement method to deal with the SQuAD problem.

## Environment need
1. pytorch 1.4.0
2. tensorflow 1.x ( used to load the pre-train model)
3. tqdm
4. transformers (use the AdamW Optimizer)

## improvement method introduction
### (1) model 
1. use the multilinear output layer
2. highlight the importance of the start postion prediction in reading comprehension
3. Only predict the existence of the answer model and ensemble with others

### (2) Optimizer
1. RecAdam Optimizer rather than traditional AdamW

### (3) Data
1. Use data augmentation by back translation
