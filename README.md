<h1> Return Policy Assistant</h1>

Returns are a tricky business, the goal of this project is to leverage AI to create a chatbot that in theory could be used by a customer service rep to assist them in making decisions. 
In a real-world use case, if calls were recorded they could be encoded speech-to-text into the text being directly fed into the chatbot as a query, and when the result is bad per CS rep, that data can be sent for further training.  

====================================================

<h4> Files in Repository:</h4>

**For any to work, an up-to-date openai key is required, all files are pulled directly from url**

- <h5>Raw Kaggle Start Non Functional.ipynb</h5>
  
     - The work that was started on Kaggle, transferred environments to Google Cloud to test specific integrations with github. 
      
- <h5>Raw Customer-Service-Query-AI</h5>
  
     - A working query bot with prompts based on embeddings pulled from return policy articles.

     - The notebook with my thoughts, learnings, notes, exploration, errors, and testing

     - The file is NOT well organized but breaks down crucial points in text cleaning, tokenization, and the core functions in interacting with an LLM and private data set 

- <h5>Cleaned Customer-Service-Query-AI</h5>
  
     - A working query bot with prompts based on embeddings pulled from return policy articles.

     - Importing openai key in secret location (top) of code should be only requirement for this code to load in any IDE 

     - Any excess code, notes, links, and comments were removed and formatting corrected
  
- <h5> Customer_Service_Langchain_openai_4_0 _(Work in progress)_</h5> 

     - Unlike the previous files, this will be worked on quickly to deployment using existing tests and examples predominately
  
     - Re-making the query bot using the most up-to-date libraries, this will be the one I focus on building out applications to support & fine-tune
  
     - Strong development consideration: I used most of my tokens in initial training, If this is a purpose-driven bot, I should think about the development of the text I'm feeding it to be more efficient. I can scrape and train, but with written text, I can be more token efficient & have room for tokens in embedding limitations for the fine-tuning process using prompt - solutions from 'gaps' in answers in the inevitable feedback loop when testing. 

====================================================

<h4>Steps Completed </h4>

1) Acquired data sets

2) Established coding environment in Google Colab, shifting from Kaggle to experience new tools and prepare for practice with Google Gemini and rest/gain experience with their new co-pilot coming out

3) Connected with OpenAI key - tested connection in a notebook 

4) Working on cleaning text file 

5) Determined effective normalization and cleaning procedures e.g , keeping capitalization, removing html, removing specific symbols.
    
6) Train a chatbot around a set of return policy data
   
7) Have it take the role of Customer Service to advise the policy given a scenario prompt

   
====================================================

<h4>**Pivot Point** </h4>

To this point, what has been done has been using embeddings which is depreciated in the most recent openai. 
As well, there are cheaper query alternatives now available and Langchain is now used for similar queries.
My next step will to do a project that involve langchain & work on an extension to quickly gather and tokenize data while browsing (chrome extension)
  

