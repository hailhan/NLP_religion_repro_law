This repository contains data, code and a video presentation for my individual project, "The 'L' Stands for 'Law': Leveraging NLP Techniques to Examine Linguistic Similarities between Legal Documents". This document will provide a rough outline of the steps taken to complete the project, along with the documents that contain the code and data for each step.
### Data Collection
PDFs containing amicus briefs and Supreme Court opinions were manually downloaded from Proquest's Supreme Court Ruling database. 
### Preprocessing
pdfplumber was used to extract text from the above pdfs. See [file_conversion.ipynb)](file_conversion.ipynb) for the code used to accomplish this. Then regular expressions and other functions were used to clean the text. See [preprocessing.ipynb](preprocessing.ipynb) for the code used to accomplish this, and the cleaned text csv files in the [files folder](files/cleaned_text.csv). 
### Exploratory Data Analysis
Word2Vec was used to vectorize the cleaned text for each corpus, and then explored to determine the dimensions and spread of the vectors in each embedding. See [EDA.ipynb](EDA.ipynb) for the code, and the 'models' folder to access the trained models.
### Principal Component Analysis and K-means Clustering
PCA was conducted on each embedding, followed by several K-means clustering tasks. [PCA_kmeans.ipynb](PCA_kmeans.ipynb) contains the code for the parameter tuning process, as well as the outputs and visualizations for each model. 
### Presentation
The video presentation containing an overview of my project can be found in [here](project_walkthrough.mp4), and the slides (with voiceover recordings!) can be viewed separately [here](project_slides.pptx).