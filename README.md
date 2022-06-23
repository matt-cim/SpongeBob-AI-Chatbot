# SpongeBob-AI-Chatbot
## Obtaining data- dialog_parse.ipynb
I wanted to create an AI chatbot that would talk like Spongebob to familiarize myself with machine learning and artificial intelligence concepts and utilize Python's abilities with these two subjects. To start, I went to Wiki Transcripts (https://ideas.fandom.com/wiki/Category:Transcripts) and downloaded transcripts of 14 of my childhood favorite Spongebob episodes into a text file **spongebob dialog.txt**. 

Next, I would parse this text file using **regular expressions** and used **Pandas**, a Python package used for data analysis and associated manipulation of tabular data in data frames, to separate the names of the characters and their actual dialog in the text file. I was then left with a table that had the name of the character on the left side, and their associated dialog on the right side. Finally, this data frame was converted into a csv file that the model would base its training from (see **Spongebob.csv**)

![](transcript_dataframe.png)

## Training the model
After I uploaded my data frame csv file to Kaggle, an online community of data scientists and machine learning practitioners, I would adjust a model derived from the one explained here: https://towardsdatascience.com/make-your-own-rick-sanchez-bot-with-transformers-and-dialogpt-fine-tuning-f85e6d1f4e30. The model utiilized **Pytorch's Transformers library** and **Microsft's dialoGPT** for **natural language processing**. I set the number of training epochs to 6 (# of times the model will cycle through the training set), in order to minimize my perplexity (a measurement of how well a probability distribution or probability model predicts a sample). My perplexity number was 5.28, which is relativley good considering my data set. See below for model training statistics.

![](training_stats.png)

## Results
Below are screenshots of conversations with the Spongebob AI chat bot.

![chat3](https://user-images.githubusercontent.com/100395759/175194886-23deec35-9cd3-4378-9eb3-ba4aea5e5c1b.png) 

![chat4](https://user-images.githubusercontent.com/100395759/175194888-c49364b3-fe1a-4d11-964a-7b3bbcfc11a0.png) 

![chat5](https://user-images.githubusercontent.com/100395759/175194890-07c93656-1db5-4d63-b19c-397da668d5ba.png) 

![chat6](https://user-images.githubusercontent.com/100395759/175194891-70f0147a-f0d8-430e-8d06-847f54214fd6.png) 

![chat7](https://user-images.githubusercontent.com/100395759/175194892-2cfe8880-0f3f-45b3-9a61-be3274a07099.png) 

![chat8](https://user-images.githubusercontent.com/100395759/175194893-e1eeefa2-954a-4a6d-8a11-ccdb5da161cf.png) 

![chat1](https://user-images.githubusercontent.com/100395759/175194894-ea37a855-ad10-4599-b3bc-669cd509165e.png) 

![chat2](https://user-images.githubusercontent.com/100395759/175194895-a7aff808-c9dc-4a0a-8f1d-7b6895c088c2.png) 
