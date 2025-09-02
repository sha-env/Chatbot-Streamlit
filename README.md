# Chatbot Streamlit

This repository provides a Streamlit-based chatbot application, featuring multiple UI variants (basic and React). It serves as a starting point for building and deploying interactive chatbot interfaces locally or with Docker.

<hr><br>

## Purpose of This Repository

The purpose of this repository is to provide developers with a starting point for building chatbot applications using Streamlit. By offering multiple UI variants, optional React integration, and Docker support, this project aims to make it easier for developers to explore, customize, and deploy interactive chatbot interfaces.

<hr><br>

## Demonstration

Here is a quick demo of what you can achieve with this repository:

```python
# streamlit_app.py

import streamlit as st

# Simple chatbot response function
def chatbot_response(user_input: str) -> str:
    if "hello" in user_input.lower():
        return "Hi there! How can I help you today?"
    elif "bye" in user_input.lower():
        return "Goodbye! Have a great day! 👋"
    else:
        return "I'm just a demo chatbot. Try saying 'hello' or 'bye'."

# Streamlit UI
st.title("Chatbot Demo 🤖")

# Input box
user_input = st.text_input("You:", "")

# Display chatbot response
if user_input:
    response = chatbot_response(user_input)
    st.write(f"**Bot:** {response}")
```

<hr><br>

## Features

- Streamlit-based chatbot UI for quick prototyping
- Multiple application variants (basic, advanced, and React-integrated)
- Simple chatbot logic with customizable responses
- Optional React tools integration for richer user experience
- Docker support for easy containerized deployment
- Database utility (database_tools.py) for data storage and interaction
- Clean code structure with clear separation of logic and UI

<hr><br>

## Technologies Used

- Python 3.x
- Streamlit – for building the chatbot UI
- React (optional) – for enhanced and interactive frontend integration
- SQLite / database_tools – for data handling and storage
- Docker – for containerized deployment

<hr><br>

## Project Setup

To set up this project on your local machine, follow these steps:

1. **Clone the repository**
   ```bash
   git clone https://github.com/sha-env/chatbot-streamlit.git
   ```
2. **Navigate to the project directory**
   ```bash
   cd chatbot-streamlit
   ```
3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   
<hr><br>

## Steps to Run

To run the Python scripts provided in this repository, use the following command:

1. **Run command**
   ```bash
   streamlit run streamlit_react_tools_app.py
   ```
1. **Automatically open at**
   ```bash
   http://localhost:8501
   ```

<hr><br>

## License

This project is licensed under the Apache-2.0 License. See the [LICENSE](LICENSE) file for details.

<hr><br>

<div align="center">
  <a href="https://www.instagram.com/sha.env/">
    <img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=100:00000,20:EEEEEE&section=footer&reversal=false&textBg=false&fontAlignY=50&descAlign=48&descAlignY=59"/>
  </a>
</div>
