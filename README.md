# Mulheres na política: teste de 12 eixos

Teste político que posiciona quem responde em 12 eixos e compara o resultado só com mulheres da política, brasileiras e de outros países.

O site é um único arquivo, `index.html`, sem servidor e sem dependências para instalar.

## Como publicar no GitHub Pages

1. Suba o `index.html` e este `README.md` num repositório público.
2. Em **Settings → Pages**, escolha a branch `main` e clique em **Save**.
3. O site fica em `seuusuario.github.io/nome-do-repositorio`.

Para atualizar, suba o novo `index.html` por cima do antigo.

## Como colocar as fotos

No começo do `<script>`, dentro do `index.html`, há uma lista chamada `FOTOS_SITE` com o nome de cada política:

```js
"Dilma Rousseff": {url:"", credito:""},
```

Para cada uma:

1. Procure a política no [Wikimedia Commons](https://commons.wikimedia.org) e abra a página da foto escolhida.
2. Clique em **Usar este arquivo na web** (ou "Use this file on the web").
3. Copie o link que começa com `https://upload.wikimedia.org/` e cole em `url`.
4. Na mesma janela, copie o texto de **Atribuição** e cole em `credito`.

Exemplo preenchido (dados fictícios):

```js
"Dilma Rousseff": {url:"https://upload.wikimedia.org/wikipedia/commons/x/xx/Foto.jpg", credito:"Fulana de Tal, CC BY 3.0 BR, via Wikimedia Commons"},
```

Quem ficar sem `url` aparece com as iniciais num círculo colorido. Se um link quebrar, a página volta para as iniciais sozinha. Os créditos aparecem embaixo da foto e na seção "Como este teste foi feito".

Use só fotos com licença livre (CC BY, CC BY-SA, domínio público) e sempre preencha o crédito.

## Metodologia

- As perguntas têm respostas específicas, em vez de concordo/discordo (Saris, Revilla, Krosnick & Shaeffer, 2010).
- Parte das perguntas pede para escolher entre duas afirmações opostas, como na tipologia política do Pew Research Center.
- "Não sei" é uma opção separada e não entra no cálculo (Sturgis, Roberts & Smith, 2014).
- Cada eixo tem quatro perguntas, e o resultado é a média delas (Ansolabehere, Rodden & Snyder, 2008).
- As perguntas tratam de políticas concretas, sem rótulos de esquerda e direita (Treier & Hillygus, 2009; Feldman & Johnston, 2014).

As posições das políticas são estimativas a partir da trajetória pública de cada uma e podem ser revistas. A semelhança é calculada pela distância entre as respostas e a posição de cada política nos 12 eixos.

## Licença

Código sob licença MIT. Perguntas e textos sob CC BY 4.0. As fotos seguem a licença indicada no crédito de cada uma.
