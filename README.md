
![](./images/docpad.jpg)

# LLM Generated Text Detection Project 

**Nicholas Kai**

**Author**: [Nick Kai](mailto:nhknicholas@gmail.com)

## Overview
I created an NLP ML model to detect whether an Essay is AI or Human Generated


## Business Problem

Students are becoming overly reliant on tools like Chat-GPT as they are using it to cheat on tests and writing assignments, however disallowing access to the tools is both a waste of potential benefit to the students,
and a logistical nightmare, so detecting cheating is the best solution.

![img](./images/grey.jpeg)


## Data

Our data come from this [Kaggle dataset](https://www.kaggle.com/competitions/llm-detect-ai-generated-text/data), which includes over 1,000 human written essays, as well as this [Kaggle dataset](https://www.kaggle.com/datasets/radek1/llm-generated-essays/data), which is set of generated essays.

## Methods
To improve computational efficiency, I preprocessed the initial dataset by tokenizing, filtering out stopwords, lemmatizing,.

I then began the modeling process by testing various algorithms varying from Logistic classifiers, Ensemble models, Neural networks, and various Vectorizers, including TF-IDF and Count vectorizer.

I then fine-tuned these models by adjusting various Hyperparameters to improve model accuracy.

Initially I was only working with the original dataset, which was not promising, but after finding the additional 700 generated essays I was able to arrive at over 95% accuracy on multiple models

Then I worked to reduce the dimensions of the data by using LSA and adjusting the number of components.

  
## Results
My best model achieved an accuracy of 99.8% accuracy, but I am currently working on testing it on more unseen data.

</p>

## Conclusions
From this project, we reached the following conclusions Neural Networks tend to be the most efficient and effective way of parsing through large and complex datasets such as these. We also believe that if were able to access more data, we would be able to more effectively train our neural network to achieve an even higher accuracy.


  ![](./images/cheer.jpg)

### Next Steps
- Testing on more unseen data
- Launching a Webapp to both collect more data, and so that individuals can access the model


## For More Information

See the full analysis in the [Jupyter Notebook](./code_LLM.ipynb), review this [presentation](./LLM_presentation.pdf).

For additional info, contact Nick Kai at [nhknicholas@gmail.com](mailto:nhknicholas@gmail.com)

## Repository Structure

```
├── data
│   ├── train.dat
│   ├── train_cleaned.csv
|   code_LLM.ipynb
├── images
├── .gitignore
├── README.md
└── LLM_presentation.pdf
```
