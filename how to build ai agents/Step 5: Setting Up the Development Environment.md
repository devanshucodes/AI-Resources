# 🛠️ Step 5: Setting Up the Development Environment

## Local Development
Setting up a proper development environment ensures smooth testing and iteration. Follow the steps below to get started:

### Install Dependencies
Ensure you have Python installed (preferably 3.8 or later). Install the required libraries:
```sh
pip install jupyter openai requests langchain llama-index
```

### Setup Jupyter Notebooks
Jupyter notebooks are useful for prototyping and testing models. Install and launch Jupyter:
```sh
pip install notebook
jupyter notebook
```

### Environment Variables
Store API keys and sensitive information securely:
```sh
export OPENAI_API_KEY="your-api-key-here"
```
Alternatively, use a `.env` file and load it in your scripts.

## Version Control
Use Git to track changes and collaborate:
```sh
git init
git add .
git commit -m "Initial setup"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main
```


Happy coding! 🚀
