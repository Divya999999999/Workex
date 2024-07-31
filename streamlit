import streamlit as st
#from langchain.llm import OpenAI
from langchain_openai import ChatOpenAI
 

st.title('My First Chatbot')
openai_api_key = st.sidebar.text_input('OpenAI API Key', type='password')

def generate_response(input_text):
    llm = ChatOpenAI(temperature=0.7, openai_api_key=openai_api_key)
    st.info(llm(input_text))
    st.info(llm(input_text))

with st.form('wwww'):
    text = st.text_area('Enter text:', 'What are the three key pieces of advice for learning how to code?')
    submitted = st.form_submit_button('Submit')
    if submitted:
        generate_response(text)
