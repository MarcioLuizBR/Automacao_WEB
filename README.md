# Projeto Automação Web - Busca de Preços

## Objetivo
Este projeto tem como objetivo treinar automações web utilizando o Selenium para realizar buscas de preços de produtos em sites como Google Shopping e Buscapé. O propósito é identificar produtos que estejam abaixo de um preço limite definido, enviar essas informações por e-mail e atualizá-las em uma planilha.

## Como Funciona
Imaginando um cenário no qual você trabalha na área de compras de uma empresa, o projeto simula a busca e comparação de preços de insumos/produtos de fornecedores. A cada busca, os preços promocionais dos produtos são monitorados para ajudar na tomada de decisão.

- Se o valor dos produtos for abaixo de um preço limite, o sistema lista os produtos mais baratos e atualiza as informações em uma planilha.
- Posteriormente, um e-mail é enviado com a lista de produtos abaixo do preço máximo de compra.

## Funcionalidades

- Procurar cada produto no Google Shopping e Buscapé, obtendo os resultados que estejam dentro da faixa de preço definida e que correspondam ao produto correto.
- Evitar resultados incorretos com base nos parâmetros pré-definidos, como preço mínimo e termos a serem evitados.
- Enviar um e-mail com uma tabela que contém os itens encontrados, preços e links de compra.

## Tecnologias Utilizadas

- **Python**
- **Selenium**: Para automação das buscas web.
- **Pandas**: Para manipulação de dados e planilhas.
- **Smtplib**: Para envio de e-mails com as informações dos produtos.

## Entrada de Dados

O projeto utiliza uma planilha contendo:
- Nome dos produtos
- Preço máximo permitido
- Preço mínimo para evitar erros
- Termos a serem evitados nas buscas

## Execução

1. Realizar a busca dos produtos no Google Shopping e Buscapé.
2. Filtrar os resultados que estejam dentro da faixa de preço e correspondam ao produto.
3. Atualizar a planilha com os resultados encontrados.
4. Enviar um e-mail para o responsável (no caso de testes, será enviado para seu próprio e-mail).

## API (opcional)
Como alternativa, é possível utilizar APIs dos fornecedores ao invés da automação com Selenium.

## Testes
Use um e-mail próprio para testar se o envio de notificações está funcionando corretamente.

## Observações

- Certifique-se de que os sites utilizados suportem automação ou APIs.
- Ajuste o tempo de espera entre as requisições para evitar bloqueios devido a acessos frequentes.
