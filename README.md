# coding-project-template
This repo is for the practice project which is to be based on Embedded AI libraries. 


Create a sentiment analysis application using Watson NLP library:

NLP sentiment analysis is the practice of using computers to recognize sentiment or emotion expressed in a text. Through NLP, sentiment analysis categorizes words as positive, negative or neutral.

Sentiment analysis is often performed on textual data to help businesses monitor brand and product sentiment in customer feedback, and understanding customer needs. It helps attain the attitude and mood of the wider public which can then help gather insightful information about the context.

For creating the sentiment analysis application, we'll be making use of the Watson Embedded AI Libraries. Since the functions of these libraries are already deployed on the Cloud IDE server, there is no need of importing these libraries to our code. Instead, we need to send a POST request to the relevant model with the required text and the model will send the appropriate response.

A sample code for such an application could be:

import requests

def <function_name>(<input_args>):
    url = '<relevant_url>'
    headers = {<header_dictionary>}
    myobj = {<input_dictionary_to_the_function>}
    response = requests.post(url, json = myobj, headers=header)
    return response.text