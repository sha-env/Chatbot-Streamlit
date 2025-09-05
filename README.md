# Streamlit Chatbot Demo

This repository provides a Streamlit-based chatbot application with multiple UI options (basic and React). It is a practical starting point for building, customizing, and deploying AI-powered chatbot interfaces using Python. Developers can run it locally or inside Docker for quick experimentation and prototyping.

<hr><br>

## Purpose of This Repository

- Explore conversational AI with Streamlit
- Customize chatbot interfaces with ease
- Deploy prototypes quickly in a local or containerized environment


<hr><br>

## Demonstration

Here’s a simple demo of the chatbot logic in action:

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

- Streamlit-based chatbot UI for fast prototyping
- Multiple application variants: basic, advanced, and React-integrated
- Customizable chatbot logic with simple Python functions
- Optional React tools integration for richer user experience
- Docker support for containerized deployment
- Database utility (database_tools.py) for data storage and interaction
- Clean and modular code structure separating logic and UI

<hr><br>

## Technologies Used

- Python 3.x – main programming language
- Streamlit – for building interactive chatbot UIs
- React (optional) – for advanced and dynamic frontend integration
- SQLite / database_tools.py – lightweight database handling
- Docker – containerized setup and deployment

<hr><br>

## Project Setup

To set up this project on your local machine:

1. **Clone the repository**
   ```bash
   git clone https://github.com/sha-env/streamlit-chatbot-demo.git
   ```
2. **Navigate to the project directory**
   ```bash
   cd streamlit-chatbot-demo
   ```
3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   
<hr><br>

## Steps to Run

1. **Start the Streamlit app**
   ```bash
   streamlit run streamlit_react_app.py
   ```
1. **Open the app in your browser**
   ```bash
   http://localhost:8501
   ```

<hr><br>

## License

This project is licensed under the Apache-2.0 License. See the [LICENSE](LICENSE) file for details.

<hr><br>

<div align="center">
  <a href="https://www.instagram.com/sha.env/">
    <img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=100:00000,20:FFFFFF&section=footer&reversal=false&textBg=false&fontAlignY=50&descAlign=48&descAlignY=59"/>
  </a>
</div>
