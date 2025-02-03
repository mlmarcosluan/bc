# **BC**

O repositório **BC** é um conjunto de projetos desenvolvidos para manipulação, organização e análise de dados, com foco inicial em automatizar processos de comparação e gerenciamento de arquivos. Foi criado para agilizar o trabalho na bolsa BAS realizada na Biblioteca Central da Unicamp.

---

## **Projetos no Repositório**

### **1. Pesquisa de Relação de Artigos Sem Arquivos na Pasta do Drive**
O projeto inicial deste repositório realiza as seguintes ações:
- Gera uma lista com os nomes dos arquivos em uma pasta específica no Google Drive.
- Compara os nomes dos arquivos com uma lista copiada do Google Sheets.
- Salva um arquivo com a relação de artigos que não possuem PDFs na pasta correspondente.

### **2. Contagem de Arquivos em uma Pasta do Google Drive**
Uma funcionalidade adicional que permite:
- Listar os nomes dos arquivos em uma pasta específica do Google Drive.
- Exibir o número total de arquivos encontrados na pasta.

### **3. Interface de Menu Interativo**
Agora o repositório conta com menus interativos que permitem:
- Configurar os caminhos das pastas e arquivos diretamente durante a execução do script.
- Realizar ações com base em opções selecionadas pelo usuário.

---

## **Objetivo do Repositório**

O objetivo do repositório **BC** é:
- Desenvolver ferramentas automatizadas para análise de dados.
- Facilitar o gerenciamento de arquivos em sistemas locais e na nuvem.
- Criar scripts personalizados para resolver problemas específicos de organização e comparação de dados.

---

## **Requisitos Gerais**

- **Python 3.x**: Todos os projetos utilizam Python como linguagem principal.
- **Google Colab**: Alguns scripts foram projetados para rodar no ambiente do Google Colab com acesso ao Google Drive.

---

## **Como Usar**

1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/bc.git
   ```

2. Execute o script principal no Google Colab ou em um ambiente Python local com acesso ao Google Drive.

---

## **Estrutura do Script Principal**

O script principal possui as seguintes funcionalidades:

### **Função Principal (`main`)**
- Exibe um menu inicial com as seguintes opções:
  - **0**: Sair do programa.
  - **1**: Pesquisa de relação de artigos sem arquivos correspondentes.
  - **2**: Contagem de arquivos em uma pasta do Google Drive.

### **Menus Secundários**
1. **Menu de Pesquisa de Relação de Artigos**:
   - Configuração dos caminhos para a pasta no Drive e arquivos de saída.
   - Opção para colar diretamente uma lista de nomes copiada do Google Sheets.
   - Realização da pesquisa e geração dos arquivos de saída.

2. **Menu de Contagem de Arquivos**:
   - Configuração do caminho da pasta a ser analisada.
   - Exibição do número total de arquivos na pasta.

### **Funções Auxiliares**
- **`limpa_lista(arquivo_saida)`**: Limpa o conteúdo de um arquivo de saída.
- **`puxa_nomes(pasta_drive, arquivo_saida)`**: Recupera os nomes dos arquivos em uma pasta do Drive e os salva em um arquivo.
- **`montegem_caminho()`**: Solicita ao usuário o caminho de uma pasta ou arquivo.
- **`limpar_tela()`**: Limpa a tela do terminal ou ambiente interativo para melhorar a exibição do menu.

---

## **Fluxo de Execução**

1. O script monta o Google Drive para acessar as pastas compartilhadas ou do usuário.
2. O menu inicial é exibido com as opções principais.
3. Dependendo da escolha do usuário, menus adicionais permitem configurar caminhos e realizar as operações desejadas.
4. Arquivos de saída são gerados automaticamente nos locais configurados.

---

## **Estrutura do Repositório**

- **Scripts**:
  - Código principal com funções organizadas.
- **Saída**:
  - Arquivos gerados com os resultados das análises.

---

## **Contribuições**

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests para melhorias no repositório.
