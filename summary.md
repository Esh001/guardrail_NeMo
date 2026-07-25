# NeMo Guardrails Classroom — Project Summary

## What is this project?
This is a simple teaching app built with Streamlit. It helps you learn how to make AI chatbots safe using **NeMo Guardrails**. 

You will build an "Enterprise IT Assistant" chatbot that only answers questions about networking and computers. You will run through 7 lessons (experiments), where each lesson adds a new safety rule to stop the AI from doing bad things.

## The 7 Lessons
| Lesson | What it teaches |
|---|---|
| **1. Baseline** | See how an unprotected AI acts. It will answer any bad question. |
| **2. Topic Guard** | Teach the AI to only talk about IT topics. |
| **3. Jailbreak Shield** | Stop people from tricking the AI into breaking its own rules. |
| **4. Sensitive Topic Block** | Stop the AI from talking about hacking or stealing data. |
| **5. Dialog Rails** | Create exact, pre-written answers for greetings and goodbyes. |
| **6. Custom Actions** | Write Python code to detect and hide personal information (like emails or credit cards). |
| **7. Output Rail** | A final safety net that checks the AI's answer *before* showing it to the user. |

## The Files
* `app.py`: The main app that shows the screens and chat box.
* `colang_defs.py`: Contains the simple rules (written in Colang) that tell the AI what to do.
* `actions.py`: Python code for checking things like personal information.
* `rail_configs.py`: Connects the rules to the AI.
* `requirements.txt`: The list of Python tools needed to run the app.

## How to use the App
1. When you open the app, look at the **left sidebar**.
2. Put your **Groq API Key** in the boxes. (Your key is safe, it stays on your computer).
3. The app will unlock. You can click on the different tabs to try out the 7 lessons!

## How to Run the App
Open your terminal and type these two commands:
```bash
pip install -r requirements.txt
streamlit run app.py
```
