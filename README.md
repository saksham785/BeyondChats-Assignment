# Reddit User Persona Generator 

This project was built as part of the assignment for the **AI/LLM Engineer Internship at BeyondChats**. The task was to take a Reddit user profile, analyze their posts and comments, and generate a detailed **user persona** with key insights like:

- Behavioral traits  
- Interests  
- Goals  
- Needs  
- Motivations  

...with direct citations from the user's own posts or comments.

---

## Why I Chose a Jupyter Notebook (and Not a `.py` Script)

Even though the assignment asked for an executable script, I decided to use a **Colab-compatible Jupyter Notebook** for a few reasons:

- It better reflects how I think through problems step by step  
- It makes the entire pipeline like scraping, summarizing, interpreting more visible and interactive  
- It's easier to experiment and tune models or parameters on the fly  
- It allows for secure credential handling using `getpass()` or `userdata.get()` rather than hardcoding anything

That said, all logic is modularized and can easily be converted into a `.py` script if needed.

---

## What This Project Does

1. Takes a Reddit profile URL (e.g., `https://www.reddit.com/user/kojied/`)
2. Scrapes the user's most recent 100 posts and 100 comments using Reddit's API
3. Uses a lightweight summarization model to condense each entry
4. Analyzes and classifies summaries into:
   - Traits
   - Interests
   - Needs
   - Goals
   - Motivations
5. Outputs a `.txt` file with the final persona, citing sources for each insight

---
