#Return Policy Assistant

Returns are a tricky business, the goal of this project is to leverage AI to create a chatbot that in theory could be used by a customer service rep to assist them in making decisions. 
In a real-world use case, if calls were recorded they could be encoded speech-to-text into the text being directly fed into the chatbot as a query, and when the result is bad per CS rep, that data can be sent for further training.  

====================================================

Files in Repository:

**For any to work, an up-to-date openai key is required, all files are pulled directly from url**

- Raw Kaggle Start Non Functional.ipynb
      -The work that was started on Kaggle, transferred environments to Google Cloud to test specific integrations with github. 
      
- Raw Customer-Service-Query-AI
      -A working query bot with prompts based on embeddings pulled from return policy articles.
      -The notebook with my thoughts, learnings, notes, exploration, errors, and testing
      -The file is NOT well organized but breaks down crucial points in text cleaning, tokenization, and the core functions in interacting with an LLM and private data set 

- Cleaned Customer-Service-Query-AI
     -A working query bot with prompts based on embeddings pulled from return policy articles.
     -Any excess code, notes, links, and comments were removed and formatting corrected 

====================================================

Steps Completed 

1) Acquired data sets

2) Established coding environment in Google Colab, shifting from Kaggle to experience new tools and prepare for practice with Google Gemini and rest/gain experience with their new co-pilot coming out

3) Connected with OpenAI key - tested connection in a notebook 

4) Working on cleaning text file 

5) Determined effective normalization and cleaning procedures e.g , keeping capitalization, removing html, removing specific symbols.
    
6) Train a chatbot around a set of return policy data
   
7) Have it take the role of Customer Service to advise the policy given a scenario prompt

   
====================================================

**Pivot Point** 

To this point, what has been done has been using embeddings which is depreciated in the most recent openai. 
As well, there are cheaper query alternatives now available and Langchain is now used for similar queries.
My next step is to re-create the customer service query agent with Langchain via openai. 

====================================================

To-Do-List 

1) Recreate what has been done using embeddings with Langchain & openai 4.0 
2) Test a variety of scenarios, and place them on a table (prompt & response)
3) For incorrect or poor responses, improve them to be the desired result or remove
4) Utilize that new table for reinforcement learning/fine-tuning
5) Repeat until satisfied with the results
6) Create an application that includes a feature of 'Was this helpful?' that is stored with the query and response as data to support large-scale reinforcement.
  

