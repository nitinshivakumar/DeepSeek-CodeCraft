# DeepSeek CodeCraft

## Overview
DeepSeek CodeCraft is an AI-powered code generation assistant built on the **DeepSeek R1 1.5B** model. It helps developers generate, refine, and optimize code efficiently. Whether you're working on a new project or debugging existing code, DeepSeek CodeCraft provides intelligent suggestions and autocompletions to enhance your development workflow.

## Features
- **AI-Powered Code Generation**: Generate complete functions, classes, or scripts based on natural language prompts.
- **Code Autocompletion**: Get real-time code suggestions as you type.
- **Multi-Language Support**: Supports multiple programming languages, including Python, JavaScript, Java, C++, and more.
- **Code Optimization**: Suggests improvements for better performance and readability.
- **Bug Detection & Fixing**: Identifies potential errors and provides corrective suggestions.

## Installation

### Prerequisites
- Python 3.8+
- pip
- GPU (recommended for better performance)

### Setup
```sh
# Clone the repository
git clone https://github.com/your-username/DeepSeek-CodeCraft.git
cd DeepSeek-CodeCraft

# Install dependencies
pip install -r requirements.txt

# Download and set up DeepSeek R1 1.5B model (update with actual setup instructions)
python setup_model.py
```

## Usage

### Running the CodeCraft Assistant
```sh
python main.py
```

### Example Usage
```python
from deepseek_codecraft import CodeGenerator

model = CodeGenerator()

prompt = "Write a Python function to check if a number is prime."
generated_code = model.generate_code(prompt)
print(generated_code)
```

### Expected Output
```python
def is_prime(n):
    if n < 2:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True
```

## Configuration
Modify `config.json` to adjust model parameters such as:
- Temperature (controls randomness of output)
- Max tokens
- Programming language preference

## Roadmap
- [ ] Expand multi-language support
- [ ] Add integration with VS Code and JetBrains IDEs
- [ ] Implement more fine-tuning options
- [ ] Introduce a web-based interface

## Contributing
Contributions are welcome! Feel free to fork this repository and submit pull requests.



