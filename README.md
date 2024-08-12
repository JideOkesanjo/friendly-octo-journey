# Project: Automated Web Content Summarization using GPT-4 and BART

This project involves interacting with a large language model (GPT-4) to retrieve a relevant website, extracting and processing the content from that website, and then summarizing the content using the `facebook/bart-large-cnn` summarizer model from Hugging Face.

## Step 1: Interacting with GPT-4 Model using the `llm` Python Library

The first step in this project involves interacting with the GPT-4 model using the `llm` Python library. The goal here is to generate a prompt that asks for the best website containing information about the former footballer Diego Maradona. The response from the model is expected to include a URL to the relevant website.

## Step 2: Extracting the Website URL using Regular Expressions

The next step is to extract the website URL from the response provided by the GPT-4 model. This is accomplished using Python's `re` module for regular expression matching. The extracted URL is then used in the following steps for accessing and parsing the webpage content.

## Step 3: Accessing, Parsing, and Preprocessing the Webpage

In this step, the extracted URL is used to access the webpage. The content of the webpage is parsed using the `BeautifulSoup` library, specifically focusing on text within `<p>` tags which typically contain the main body of the article. The text is then preprocessed to make it suitable for summarization. This preprocessing may involve cleaning up HTML tags, removing special characters, and normalizing whitespace.

## Step 4: Summarizing the Text using the BART Model

The final step of the project involves summarizing the preprocessed text using the `facebook/bart-large-cnn` model available through the Hugging Face Transformers library. The summarizer is applied to the cleaned text, and the resulting summary is displayed. This provides a concise version of the original article, capturing the key points.

## Conclusion

This project demonstrates the process of using a large language model to automate the retrieval of relevant web content, followed by web scraping, preprocessing, and summarization. The approach leverages state-of-the-art natural language processing tools to extract meaningful insights from web-based information, making it applicable to a wide range of use cases where summarization of long-form content is required.

