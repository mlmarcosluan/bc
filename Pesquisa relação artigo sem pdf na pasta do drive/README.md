# Pesquisa de Relação de Artigos sem Arquivos na Pasta do Drive

Este código cria uma lista de nomes de todos os arquivos em uma pasta específica e compara com uma lista de dados copiada e colada do terminal. Ele salva um arquivo com a relação de nomes de artigos que não possuem o PDF correspondente na pasta do Drive.

## Descrição

Este projeto é baseado nas seguintes etapas:

1. **Criação de uma lista de nomes de arquivos**: O código gera uma lista com os nomes dos arquivos presentes em uma pasta especificada pelo usuário.
2. **Entrada de caminhos de arquivos**: O usuário deve fornecer dois caminhos de arquivos:
    - `nomes.txt`: Lista com os nomes de todos os arquivos na pasta especificada.
    - `nomes_sem_arquivos.txt`: Lista com a relação de artigos que não possuem PDF na pasta especificada.
3. **Inserção de dados**: O usuário deve copiar e colar uma lista de dados do Google Sheets.
4. **Execução do script**: O script compara os dados copiados e colados com os nomes dos arquivos na pasta e salva um arquivo com a relação de artigos que não possuem PDF.

## Funcionalidades

- **puxa_dados**: Função que coleta os nomes dos arquivos dentro de uma pasta especificada.
- **pegar_dados**: Função pega dados do copia e cola do google sheelts e transforma em uma lista de nomes incluindo o .pdf
- **montagem_caminho**: Salva os caminhos dos dois arquivos que serão limpos e encrementado com a pesquisa
- **limpa_lista**: Limpa a lista para depois serem encrementada

## Requisitos

Para executar o código, é necessário estar logado no Google Colab, que contém o Drive com os arquivos compartilhados com você.

## Como Usar

1. **Inicialização**: Ao iniciar o programa, escolha entre:
    - `1`: Continuar
    - `2`: Sair

2. **Menu de Opções**: No menu, selecione quais dados você deseja inserir na pesquisa.

3. **Execução da Pesquisa**: Após inserir todos os dados, escolha a opção `5` para realizar a pesquisa.

4. **Resultados**: Após alguns segundos, os arquivos `nomes.txt` e `nomes_sem_arquivo.txt` serão salvos na pasta especificada no passo 2.

## Exemplo de Uso

```python
# Exemplo de execução

1, Adicionar pasta para pesquisa.
2, Acicionar arquivo de saida da lista de nomes.
3, Adicionar arquivo de saida da relação de nomes sem arquivos.
4, Adicionar nomes do copia e cola do excel.
0, sair.

Pasta do drive para pesquisa:  /content/drive/Shareddrives/BC
Arquivo para salvar nomes.txt /content/drive/MyDrive/nomes.txt
Arquivo para salvar relação de nomes sem arquivos /content/drive/MyDrive/nomes_sem_arquivos.txt
Lista de nomes do excel copiado.