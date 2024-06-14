# AthinAI_Submission
Introducing our PDF-Based Chatbot: revolutionizing document navigation. With advanced NLU and PDF parsing, easily access content via natural conversation. Customizable and accessible across platforms. Say hello to streamlined document exploration!

**Dataset : **
I have created dataset using the document given by Athina, I have analysed whole document and have taken 30 questions from different sections to maintain diversity among the questions and I have also used ChatGPT to generate few questions for different sections of the 

**Evaluation Metrics:**
I have evaluated each query-response pair using my understanding and matching the semantics of the sentence with the expected answer as the dataset was small. Other evaluation metrics are like BLEU Score , ROUGE Score and Perplexity.
I first used RAG - Chain without preserving chat history i.e. Stateless , which is by default. So , to improve accuracy , I have used memory buffer to preserve chat history too for better results.

**Thought Process:**
I have used mistral model and developed chatbot on my local system by downloading mistral LLM and then used concept of RAG(Retreival Augmented Generation) to augment given pdf on it. Then , I used memory chain of LangChain and built a Question - Answering machine using based on given pdf. I have tried to minimize hallucination by setting temperature to 0. And matching similarity using 0.7 as a similarity socre. 
