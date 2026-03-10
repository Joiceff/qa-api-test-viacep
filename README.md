# QA API Test - ViaCEP

Este projeto contém testes automatizados para a API pública **ViaCEP**, que permite consultar dados de um CEP. O objetivo é garantir o bom funcionamento da API utilizando cenários de testes positivos, alternativos e de exceção.

## Objetivo

Validar a funcionalidade da API ViaCEP utilizando **Newman**, executando os testes via **Postman** e apresentando um **relatório HTML** das execuções.

## API utilizada

**ViaCEP** é uma API pública que fornece os dados de endereço baseado no CEP. Mais detalhes: [ViaCEP API](https://viacep.com.br).

Endpoint utilizado: GET https://viacep.com.br/ws/{cep}/json/

## Ferramentas utilizadas

- **Postman**: Ferramenta para desenvolvimento e execução de testes de API.
- **Newman**: Runner de linha de comando do Postman, utilizado para execução automatizada dos testes.
- **GitHub**: Plataforma para gerenciamento do código fonte e versionamento.

## Como executar os testes

### 1. Clonar o repositório

Clone o repositório para sua máquina local:

```bash
git clone https://github.com/Joiceff/qa-api-test-viacep.git

2. Instalar o Newman

Se ainda não tiver o Newman instalado, execute o comando:
4. Visualizar o relatório

Abra o arquivo newman-report.html gerado na pasta reports em qualquer navegador para visualizar o resultado dos testes.

npm install -g newman
3. Executar os testes com Newman

Execute os testes utilizando o comando abaixo:

newman run collection/viacep-api-tests.postman_collection.json --reporters html --reporter-html-export reports/newman-report.html
