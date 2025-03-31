# Conversor de Moedas 💰

Este projeto é um **Conversor de Moedas** desenvolvido com **HTML, CSS e JavaScript**, que permite converter valores entre **BRL (Real), USD (Dólar) e EUR (Euro)**. Na última etapa, integramos uma API para obter cotações em tempo real.

## 📌 Tecnologias Utilizadas

- **HTML5** → Estruturação da página.
- **CSS3** → Estilização com foco em responsividade e experiência do usuário.
- **JavaScript (ES6+)** → Manipulação de eventos, cálculos e consumo de API.
- **[Exchangerate API](https://www.exchangerate-api.com/)** → Para obter taxas de câmbio atualizadas.

## 🛠️ Funcionalidades

✅ Entrada do valor a ser convertido.
✅ Seleção da moeda de origem e moeda de destino.
✅ Cálculo da conversão em tempo real.
✅ Atualização automática das taxas de câmbio via API.
✅ Interface moderna e responsiva.

## 🚀 Como Executar o Projeto

1. Faça o clone do repositório:
   ```bash
   git clone https://github.com/seu-usuario/conversor-moedas.git
   ```

2. Acesse a pasta do projeto:
   ```bash
   cd conversor-moedas
   ```

3. Abra o arquivo `index.html` no navegador.

## 🔗 Consumo da API

O projeto consome a API **Exchangerate API** para obter cotações em tempo real. Certifique-se de obter uma **chave de API gratuita** no site oficial e substituir `SUA_CHAVE_AQUI` no código:

```javascript
const apiKey = "SUA_CHAVE_AQUI";
const url = `https://v6.exchangerate-api.com/v6/${apiKey}/latest/BRL`;

fetch(url)
  .then(response => response.json())
  .then(data => {
    const taxaUSD = data.conversion_rates.USD;
    const taxaEUR = data.conversion_rates.EUR;
    console.log(`1 BRL = ${taxaUSD} USD`);
    console.log(`1 BRL = ${taxaEUR} EUR`);
  })
  .catch(error => console.error("Erro ao buscar os dados:", error));
```

## 🎥 Vídeos Relacionados

📌 **Criando o Mockup no Canva** → [link do vídeo]  
📌 **Implementando o HTML** → [link do vídeo]  
📌 **Estilizando com CSS** → [link do vídeo]  
📌 **Aplicando JavaScript para Conversão** → [link do vídeo]  
📌 **Integrando API para Obter Cotações em Tempo Real** → [link do vídeo]  

## 📢 Contribuição

Se quiser contribuir para o projeto, sinta-se à vontade para **abrir issues** e **enviar PRs**! 🚀

---

📧 **Contato:** [LinkedIn](https://www.linkedin.com/in/leonardossrocha/)  
⭐ Se gostou do projeto, deixe uma estrela no repositório!