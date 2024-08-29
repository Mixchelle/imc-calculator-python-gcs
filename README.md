# 🧮 IMC Calculator with Python on Google Cloud Shell

## 📜 Overview

Welcome to the IMC Calculator project! This Python application calculates the Body Mass Index (BMI) and classifies it into different categories. This project is developed using Google Cloud Shell Editor and Python, and is designed to be a simple and effective tool for health monitoring.

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine or on Google Cloud Shell.

### 🛠️ Prerequisites

- [Google Cloud Shell](https://cloud.google.com/shell/docs)
- [Python](https://www.python.org/downloads/)

### 📂 Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Mixchelle/imc-calculator-python-gcs.git
   cd imc-calculator-python-gcs

2. **🚀 Run the Application**

To run the application, use the following command:

```bash
python imc_calculator.py


💡 **Usage**

The program will ask you to enter your weight (in kg) and height (in meters). After you provide these values, it will calculate your BMI and display both the BMI value and its classification.

🔧 **Development**

The code for this project is written in Python. You can modify it as needed. The main script is located in `imc_calculator.py`.

📝 **Code**

Here is the code used in the project:

```python
def calcular_imc(peso, altura):
    imc = peso / (altura ** 2)
    return imc

def classificar_imc(imc):
    if imc < 18.5:
        return "Abaixo do peso"
    elif 18.5 <= imc < 24.9:
        return "Peso normal"
    elif 25 <= imc < 29.9:
        return "Sobrepeso"
    elif 30 <= imc < 34.9:
        return "Obesidade grau 1"
    elif 35 <= imc < 39.9:
        return "Obesidade grau 2"
    else:
        return "Obesidade grau 3"

def main():
    peso = float(input("Informe o seu peso (em kg): "))
    altura = float(input("Informe a sua altura (em metros): "))
    imc = calcular_imc(peso, altura)
    classificacao = classificar_imc(imc)
    print(f"Seu IMC é: {imc:.2f}")
    print(f"Classificação: {classificacao}")

if __name__ == "__main__":
    main()

🌐 **Links**

- [Google Cloud Shell Editor](https://cloud.google.com/shell/docs)
- [Python Documentation](https://www.python.org/doc/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [GitHub Repository](https://github.com/Mixchelle/imc-calculator-python-gcs)

🤝 **Contributing**

Feel free to fork this repository and submit pull requests with improvements or bug fixes. For any issues, open an issue on GitHub.

📜 **License**

This project is licensed under the MIT License - see the LICENSE file for details.

✨ **Acknowledgments**

- Thanks to Google Cloud Shell for providing a convenient development environment.
- Thanks to the Python Software Foundation for developing a versatile programming language.

💬 **Contact**

For any questions or feedback, you can contact me on [LinkedIn](https://www.linkedin.com/in/mixchelle/) or via email.
