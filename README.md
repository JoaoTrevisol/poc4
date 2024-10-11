# POC4 - Fetch

## Funcionamento do JavaScript 🖥️
O código JavaScript é responsável por fazer a requisição à API e manipular o DOM (Document Object Model) para exibir a imagem de gato. Vamos detalhar cada parte:

## 1. ⏳ Função async:
O código permite que múltiplas operações sejam executadas de forma concorrente, sem necessidade de que uma operação espere a finalização da anterior:

![image](https://github.com/user-attachments/assets/4febaec7-6ea3-4893-99ec-3868e770837b)


## 🌐 URL da API:

![image](https://github.com/user-attachments/assets/4c2c0db9-2388-4037-b047-746bdb24a295)

Essa linha define o endpoint da API que será usado para buscar a imagem.


## 🔄 Requisição Assíncrona:

![image](https://github.com/user-attachments/assets/4a0f9a0c-b7d2-431e-9751-3f86425e421c)

O fetch é uma função que permite fazer requisições assíncronas a recursos na web, como APIs nesse exemplo.

## ⚠️ Tratamento de Erros:

![image](https://github.com/user-attachments/assets/21b815f7-65c8-4c8a-9a25-41a518c90399)

Se a resposta não for bem-sucedida (status diferente de 200), um erro é lançado.


## 📦 Processamento da Resposta:

![image](https://github.com/user-attachments/assets/2420483c-c195-4ca3-911b-d307f8260d63)

A resposta JSON é convertida e a URL da imagem é extraída.


## 🖼️ Manipulação do DOM:

![image](https://github.com/user-attachments/assets/d3fa591b-a484-49b9-82d9-d5a425a456e5)

A imagem é adicionada ao elemento especificado, permitindo que ela apareça na página.

## 🔘 Evento de Clique no Botão
Um evento de clique é adicionado ao botão, que chama a função fetchCatImage quando acionado:

![image](https://github.com/user-attachments/assets/9986ae6e-0437-4439-975c-4fe6494c51ec)

Selecionando o Botão:

	document.getElementById('fetchButton')
 
Essa linha seleciona o botão com o ID fetchButton.

Adicionando o Evento:


		.addEventListener('click', () => {
   	 fetchCatImage('catContainer');
     
Quando o botão é clicado, a função fetchCatImage é chamada, passando o ID do contêiner onde a imagem será exibida, e a cada vez que o botão é pressionado, uma imagem nova é exibida. Caso queira reiniciar a sequência de imagens, recarregue a página e aperte o botão novamente.

Conclusão 🎉
Esse código é uma excelente introdução à utilização de APIs e manipulação de DOM com JavaScript. Ao clicar no botão, uma nova imagem de gato aparece, tornando a experiência interativa e divertida. Sinta-se à vontade para explorar e modificar o código!
