# SpongeBob-AI-Chatbot
## Obtaining data- dialog_parse.ipynb
I wanted to create an AI chatbot that would talk like Spongebob to familiarize myself with machine learning and artificial intelligence concepts and utilize Python's abilities with these two subjects. To start, I went to Wiki Transcripts (https://ideas.fandom.com/wiki/Category:Transcripts) and downloaded transcripts of 14 of my childhood favorite Spongebob episodes into a text file **spongebob dialog.txt**. 

Next, I would parse this text file using **regular expressions** and used **Pandas**, a Python package used for data analysis and associated manipulation of tabular data in data frames, to separate the names of the characters and their actual dialog in the text file. I was then left with a table that had the name of the character on the left side, and their associated dialog on the right side. Finally, this data frame was converted into a csv file that the model would base its training from (see **Spongebob.csv**)

![](transcript_dataframe.png)

## Training the model
