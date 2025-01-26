```markdown
# 🏦 Detecção de Fraude Bancária

## 📄 Descrição

Este projeto foi desenvolvido como parte de um curso da **Alura**, com o objetivo de detectar fraudes bancárias utilizando técnicas de Machine Learning. O conjunto de dados utilizado é fictício e foi retirado do Kaggle:  
[Fraud Detection Example](https://www.kaggle.com/datasets/gopalmahadevan/fraud-detection-example).  

Durante o desenvolvimento, foram exploradas diversas abordagens de modelagem para identificar transações fraudulentas, considerando métricas de desempenho e técnicas de balanceamento de dados.

---

## 📂 Estrutura do Projeto

```bash
📂 detecção-fraude-bancária
│-- 📂 data               # Conjunto de dados original
│-- 📂 notebooks          # Jupyter Notebooks com análises e modelagens
│-- 📂 models             # Modelos treinados e serializados
│-- 📄 requirements.txt   # Dependências do projeto
📄 README.md           # Documentação do projeto
```

---

## 🛠 Tecnologias Utilizadas

As principais bibliotecas e ferramentas utilizadas neste projeto incluem:

- **Pandas** – Manipulação e análise de dados  
- **Scikit-learn** – Modelagem (Árvore de Decisão, Regressão Logística e Random Forest) e métricas de avaliação (Acurácia, Precisão, Recall, F1, Curva ROC, Matriz de Confusão)  
- **Matplotlib** – Visualização de dados  
- **Numpy** – Operações numéricas  
- **SMOTE** – Balanceamento das classes para lidar com desbalanceamento da variável alvo  
- **ydata_profiling** – Geração de relatórios automáticos para análise exploratória  
- **RandomizedSearchCV** – Busca de hiperparâmetros para otimização do melhor modelo  

---

## ⚙️ Instalação e Uso

### **Pré-requisitos:**

1. Clone o repositório:  
   ```bash
   git clone https://github.com/thiagoaaraujo/aplicacao-deteccao-de-fraude-bancaria.git
   cd aplicacao-deteccao-de-fraude-bancaria
   ```
2. Crie e ative um ambiente virtual:  
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/macOS
   venv\Scripts\activate     # Windows
   ```
3. Instale as dependências:  
   ```bash
   pip install -r requirements.txt
   ```

---

### **Execução:**

Para rodar o notebook principal:  
```bash
jupyter notebook notebooks/Detec_Fraude.ipynb
```

---

## 🔍 Exemplos de Uso

Para realizar novas predições, utilize a função definida no próprio notebook, passando uma lista com as informações da transação:

```python
# Exemplo de uma nova transação
nova_movimentacao = {
    'step': 1,
    'amount': 9839.640000,
    'oldbalanceOrg': 170136.000000,
    'newbalanceOrig': 160296.36,
    'oldbalanceDest': 0.000000,
    'newbalanceDest': 0.000000,
    'type': 'PAYMENT'
}

# Chamando a função de previsão no notebook
resultado = nova_transacao(nova_movimentacao)

print(resultado)
# Saída esperada: [1] = "Fraude" ou [0] = "Transação legítima"
```
---

## 📊 Resultados

Foram comparados três modelos de Machine Learning, e o melhor desempenho foi obtido com **Random Forest**, que foi posteriormente otimizado com **RandomizedSearchCV**.  

### **Principais métricas do melhor modelo:**  
- **Acurácia:** 99%  
- **Precisão:** 99%  
- **Recall:** 99%  
- **F1-score:** 99%  

---

## 🤝 Contribuição

Contribuições são bem-vindas! Siga os passos abaixo para contribuir com o projeto:

1. Faça um **fork** do repositório  
2. Crie uma **branch** com sua funcionalidade (`git checkout -b feature-nova`)  
3. Faça o **commit** das suas alterações (`git commit -m "Adiciona nova feature"`)  
4. Envie para o repositório remoto (`git push origin feature-nova`)  
5. Abra um **Pull Request**  

---

## 📧 Contato

Desenvolvido por [Thiago]([https://www.linkedin.com/in/seuperfil](https://www.linkedin.com/in/thiago-aparecido-de-araujo-1931341b4).  
Entre em contato via e-mail: thiagoaparecidoaraujo23@gmail.com 

---
