# **Pesquisa de Relação de Artigos Sem Arquivos na Pasta do Drive**

O programa **Pesquisa de Relação de Artigos Sem Arquivos na Pasta do Drive** é um conjunto de scripts desenvolvidos para manipulação, organização e análise de dados. Este programa foi inicialmente criado para automatizar processos de comparação e gerenciamento de arquivos relacionados ao trabalho realizado na Biblioteca Central da Unicamp.

---

## **Funcionalidades**

### **1. Pesquisa de Relação de Artigos Sem Arquivos na Pasta do Drive**
- Gera uma lista com os nomes dos arquivos presentes em uma pasta específica do Google Drive.
- Compara os nomes dos arquivos com uma lista fornecida pelo usuário (copiada do Google Sheets ou outra fonte).
- Gera um arquivo com os nomes dos artigos que não possuem PDFs correspondentes na pasta do Drive.

### **2. Contagem de Arquivos em uma Pasta do Google Drive**
- Lista os nomes dos arquivos presentes em uma pasta do Google Drive.
- Exibe a quantidade total de arquivos na pasta especificada.

### **3. Interface de Menu Interativo**
- Menus que permitem configurar os caminhos de pastas e arquivos durante a execução.
- Opções para realizar diferentes operações com base na escolha do usuário.

---

## **Como Funciona**

### **Fluxo Principal**
1. O script monta o Google Drive no ambiente Colab para acessar as pastas e arquivos.
2. Exibe um menu inicial com as seguintes opções:
   - **0**: Sair do programa.
   - **1**: Pesquisa de relação de artigos sem arquivos correspondentes.
   - **2**: Contagem de arquivos em uma pasta do Google Drive.
3. Dependendo da escolha, o usuário é direcionado para menus específicos para configurar os caminhos e executar as ações.

### **Menus Secundários**
#### **Menu de Pesquisa de Relação de Artigos**
- Configuração dos caminhos:
  - Pasta do Google Drive contendo os arquivos.
  - Arquivo de saída para os nomes encontrados.
  - Arquivo de saída para os artigos sem arquivos correspondentes.
- Entrada dos nomes dos artigos (copiados e colados pelo usuário).
- Execução da pesquisa e geração dos arquivos de saída.

#### **Menu de Contagem de Arquivos**
- Configuração do caminho da pasta a ser analisada.
- Exibição do número total de arquivos na pasta especificada.

---

## **Estrutura do Código**

### **Funções Principais**
- **`main()`**: Controla o fluxo principal do programa e exibe o menu inicial.
- **`menu_relacao_pdf()`**: Gerencia a configuração e execução da pesquisa de relação de artigos.
- **`menu_n_arquivos()`**: Gerencia a configuração e execução da contagem de arquivos em uma pasta.

### **Funções Auxiliares**
- **`aplica_pdf(lista_nome)`**: Adiciona a extensão ".pdf" aos nomes fornecidos pelo usuário.
- **`pega_dados()`**: Recebe e processa os nomes de artigos fornecidos pelo usuário.
- **`limpa_lista(arquivo_saida)`**: Limpa o conteúdo de um arquivo de saída.
- **`puxa_nomes(pasta_drive, arquivo_saida)`**: Recupera os nomes dos arquivos em uma pasta do Google Drive e os salva em um arquivo.
- **`montegem_caminho()`**: Solicita ao usuário o caminho de uma pasta ou arquivo.
- **`limpar_tela()`**: Limpa a tela do terminal para melhorar a exibição dos menus.

---

## **Requisitos**

- **Python 3.x**
- **Google Colab** (para acesso ao Google Drive)
- Bibliotecas utilizadas:
  - `os`
  - `time`
  - `IPython.display`

---

## **Como Usar**

1. Monte o Google Drive no Google Colab:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
2. Execute o script principal.
3. Siga as instruções do menu para configurar os caminhos e realizar as operações desejadas.

---

## **Contribuições**

Contribuições são bem-vindas! Caso tenha sugestões ou encontre problemas, sinta-se à vontade para abrir issues ou enviar pull requests.
