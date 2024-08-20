
# OpenAI API Integration with LangChain

This repository contains a Jupyter Notebook demonstrating how to use the OpenAI API with the LangChain library to perform various tasks, such as generating text responses and performing calculations.

## Getting Started

To run this notebook, you will need to set up a Python environment and create a `.env` file to securely store your API key.

### Prerequisites

Ensure you have the following installed:
- **Python 3.x**
- **Required Python Packages**: You can install the necessary packages using pip:
  ```bash
  pip install openai langchain python-dotenv
  ```

### Setting Up the Environment

#### 1. Create a `.env` File

You will need to create a `.env` file in the root directory of this project to store your OpenAI API key securely. The `.env` file should contain the following line:

```plaintext
OPENAI_API_KEY=your_openai_api_key_here
```

Replace `your_openai_api_key_here` with your actual OpenAI API key.

#### 2. Ensure `.env` is Not Included in Version Control

To avoid accidentally sharing your API key, ensure that the `.env` file is excluded from version control. You can do this by adding the `.env` file to your `.gitignore`:

```plaintext
.env
```

### Running the Notebook

1. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

2. **Open the Notebook:**
   Open the Jupyter Notebook in your web browser, and run the cells sequentially to interact with the OpenAI API.

### How It Works

- The notebook loads environment variables from the `.env` file using the `load_dotenv()` function from the `python-dotenv` package.
- The OpenAI API key is retrieved from the environment variables and used to initialize the LangChain model.
- The notebook includes examples of using the model for generating text responses, performing calculations, and combining multiple chains of logic.

### Security Considerations

- **Do not share your `.env` file** or include it in any public repositories.
- Always use environment variables for storing sensitive information like API keys.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

