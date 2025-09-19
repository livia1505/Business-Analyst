# MCQ Generator with Astra DB and Langflow

## Introduction
This project demonstrates how transcript data can be transformed into meaningful multiple-choice questions (MCQs).  
The solution uses **DataStax Astra DB** for vector storage and retrieval, combined with **Langflow** and **Groq AI** for workflow orchestration and question generation.

## How It Works
1. **User Input** – The user provides a topic (e.g., *Workflow Design*, *Planner Agent*, *Happy Path*).  
2. **Vector Retrieval** – Relevant transcript passages are fetched from Astra DB using similarity search.  
3. **Prompt Construction** – The topic and retrieved content are combined into a structured prompt.  
4. **LLM Generation** – Groq AI generates MCQs strictly from the transcript data.  
5. **Output** – The generated MCQs are displayed to the user.

## Repository Contents
- **`mcq_generator_workflow.json`** – Exported Langflow workflow for direct import.  
- **`README.md`** – Documentation for understanding and running the project.  

## Setup Instructions
1. Import `mcq_generator_workflow.json` into your Langflow instance.  
2. Configure the Astra DB connection and ensure your transcript embeddings are loaded into the vector collection.  
3. Add your Groq API key to enable LLM calls.  

4. Run the flow and enter a topic to generate MCQs.

5. **SAMPLE**
Question 9
What is the benefit of using Python code to extract parameters?
A) It creates a large amount of data 
B) It simplifies the data and makes it easier to work with 
C) It designs a complex workflow 
D) It ignores the data
Correct answer: B) It simplifies the data and makes it easier to work with

Question 10
What is the preferred approach to handling data for the user?
A) Providing a large amount of data and asking for explanation 
B) Writing Python code to extract specific parameters 
C) Creating a complex workflow 
D) Ignoring the data
Correct answer: B) Writing Python code to extract specific parameters
