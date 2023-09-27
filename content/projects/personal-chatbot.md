---
title: "Personal Chatbot"
---

This is a project that I thought of when working for Perficient and developing chatbots to automatically answer questions people would have for companies on their website.
This would answer all of the lower level questions that customer service representatives would answer but was easily answerable from the website information but may be somewhat hard to find.
The chatbot would be integrated with an LLM to answer questions.
We would also index the website or whatever information was available into documents and store it into a vector database such as ChromaDB.
We could then query the database with the query to fetch potentially relevant documents, pass it into the LLM along with the original question to get up to date, human-like answers.

For this project I decided to learn SvelteKit as it is enables SSR and quick and easy backend integration with the frontend also allowing for SSR pages for SEO optimization.
After building the basic frontend for this app I integrated it with the Llama2 LLM and fed it my resume to answer any basic questions a recruiter could have.

Feel free to check out the end result:

https://portfolio-chatbot-gi2e6smr4a-uc.a.run.app