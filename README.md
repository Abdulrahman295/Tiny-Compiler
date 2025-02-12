# Tiny-Scanner
<div align="center">
  <p align="center">💻 A GUI application for the TINY programming language. It includes a Scanner that processes TINY code to generate a list of tokens, and a Parser that constructs a syntax tree using recursive descent method.</p>
   <p align="center">
      <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
      <img src="https://img.shields.io/badge/PyQt5-41CD52?style=for-the-badge&logo=qt&logoColor=white" alt="PyQt5"/>
      <img src="https://img.shields.io/badge/Graphviz-4ABF53?style=for-the-badge&logo=graphviz&logoColor=white" alt="Graphviz"/>
   </p>
</div>

## ✨ Features
- **Tokenization:**  Efficiently scans TINY language code to convert it into a structured list of tokens, ensuring each token's type and value is correctly identified and preserved.

- **Syntax Tree Generation:**  Utilizes a recursive descent parser to build a detailed syntax tree from the tokenized input, providing a clear and hierarchical representation of the source code.

- **Validation and Error Handling:**  checks the code for syntax errors and inconsistencies, providing informative error messages to assist in debugging and code correction.

- **GUI Support:**  Delivers an interactive graphical user interface that allows users to input code, view tokenization results, and visualize the generated syntax tree, significantly enhancing the user experience.

## ☑️ Prerequisites
Before running the application, ensure you have the following installed:
- [Python 3.7 or higher](https://www.python.org/downloads/)
- [Graphize](https://www.graphviz.org/download/)


## 🗺️ Installation
1. Clone this repo:
```Bash
git clone https://github.com/Abdulrahman295/Tiny-Compiler.git
cd Tiny-Compiler
```
2. Install the required dependencies:
```Bash
pip install -r requirements.txt
```

## 💡 Usage
To start the program, run the following command:
```bash
python app.py
```

### Supported Symbols
The following token types and their corresponding values are supported:
| Token Type    | Example     |
| ------------- | ----------- |
| SEMICOLON     | `;`         |
| IF            | `if`        |
| THEN          | `then`      |
| END           | `end`       |
| REPEAT        | `repeat`    |
| UNTIL         | `until`     |
| IDENTIFIER    | `x`, `abc`  |
| ASSIGN        | `:=`        |
| READ          | `read`      |
| WRITE         | `write`     |
| LESSTHAN      | `<`         |
| EQUAL         | `=`         |
| PLUS          | `+`         |
| MINUS         | `-`         |
| MULT          | `*`         |
| DIV           | `/`         |
| OPENBRACKET   | `(`         |
| CLOSEDBRACKET | `)`         |
| NUMBER        | `12`, `289` |

### Example Input
![image](https://github.com/user-attachments/assets/3f19fcdc-9318-4908-b3ea-23e27b8db9a5)

### Scanner Output
``` text
read , READ
x , IDENTIFIER
; , SEMICOLON
if , IF
0 , NUMBER
< , LESSTHAN
x , IDENTIFIER
then , THEN
fact , IDENTIFIER
:= , ASSIGN
1 , NUMBER
; , SEMICOLON
repeat , REPEAT
fact , IDENTIFIER
:= , ASSIGN
fact , IDENTIFIER
* , MULT
x , IDENTIFIER
; , SEMICOLON
x , IDENTIFIER
:= , ASSIGN
x , IDENTIFIER
- , MINUS
1 , NUMBER
until , UNTIL
x , IDENTIFIER
= , EQUAL
0 , NUMBER
; , SEMICOLON
write , WRITE
fact , IDENTIFIER
end , END
```

### Parser Output
![image](https://github.com/user-attachments/assets/23fb2f47-4c50-4f23-b8b9-30d61784d47e)

## 📰 License
This project is licensed under the MIT License. See the `LICENSE` file for more details.
