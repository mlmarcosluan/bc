# **BC - Repositório de Scripts para Automação na Biblioteca Central**

O repositório **BC** foi criado para armazenar scripts e ferramentas desenvolvidas para agilizar tarefas realizadas como bolsista BAS na Biblioteca Central da Unicamp. Ele inclui programas para manipulação, organização e análise de dados, com foco principal em Python, mas também está aberto para outras linguagens quando necessário.

---

## **Programas no Repositório**

### **1. Pesquisa de Relação de Artigos Sem Arquivos na Pasta do Drive**
- Um programa que verifica quais artigos listados não possuem arquivos correspondentes em uma pasta do Google Drive.
- Funcionalidades:
  - Geração de lista com os nomes dos arquivos no Drive.
  - Comparação com uma lista fornecida pelo usuário (copiada, por exemplo, de uma planilha do Google Sheets).
  - Geração de relatório com os nomes ausentes.

### **2. Contagem de Arquivos em Pastas do Google Drive**
- Um script simples para listar e contar os arquivos em uma pasta específica no Drive.
- Exibe rapidamente o número total de arquivos na pasta.

### **3. Outros Scripts Futuramente**
- Este repositório será expandido para incluir novas ferramentas que automatizem e facilitem tarefas relacionadas ao trabalho como bolsista BAS.

---

## **Objetivos do Repositório**

- Desenvolver soluções automatizadas para desafios do dia a dia na Biblioteca Central.
- Organizar scripts em um só lugar, facilitando o acesso e a reutilização.
- Documentar e compartilhar ferramentas que possam ser úteis para outros bolsistas ou usuários.

---

## **Como Funciona**

Os programas neste repositório seguem uma estrutura modular, facilitando a configuração e execução. A maior parte dos scripts foi projetada para rodar no Google Colab, utilizando o Google Drive para entrada e saída de arquivos.

### **Passos Gerais**
1. Monte o Google Drive no ambiente Colab para acessar os arquivos necessários:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
2. Configure os caminhos de entrada e saída conforme solicitado pelo programa.
3. Execute as tarefas automatizadas e revise os resultados gerados.

---

## **Requisitos**

- **Python 3.x**
- **Google Colab** ou um ambiente local com acesso ao Google Drive.
- Bibliotecas principais:
  - `os`
  - `time`
  - `IPython.display`

---

