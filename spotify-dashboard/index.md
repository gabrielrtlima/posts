---
title: "Spotify Dashboard"
date: "2023-05-18"
slug: "spotify-dashboard"
tag: ["typescript", "javascript", "spotify", "tailwindcss"]
category: ["Projetos"]
---

<img src="https://i.imgur.com/L87UsJ4.png" width=650>

## Meu dashboard do spotify! 😅

Decidi fazer esse projeto para aprender um pouco sobre novas tecnologias e com o objetivo de não acompanhar nenhum tutorial/video.

## O que é o dashboard?

Em palavras bem simples e com a autoestima bem elevada, é um mini-spotify. Em apenas uma tela eu tentei reunir algumas das principais funcionalidades da aplicação.

## O que foi usado no projeto

- **TypeScript**
- **JavaScript**
- **Node**
- **Express**
- **React**
- **Tailwindcss**
- **Vite**
- **Spotify API**
- **Render** (deploy)
- **Vercel** (deploy)

## App

<img src="https://i.imgur.com/z1H7jCu.png" width=650>
<video width=650 controls>
  <source src="https://i.imgur.com/cEF4hP2.mp4" type="video/mp4">
</video>

**Caso você tente acessar, o backend está rodando no render. Quando o app fica um tempo ocioso, automaticamente o render desliga o servidor por ser a versão grátis, então pode ser que quando você clique para entrar no aplicativo demore um tempo um pouco alto (2-3 minutos)**

## Funcionalidades

- O aplicativo mostra os Top Artistas mais escutados.
- O aplicativo mostra os Top Músicas mais escutados.
  - Ao clicar na música ela passa a ser tocada.
- O aplicativo mostra as Músicas recentes.
  - Ao clicar na música ela passa a ser tocada.
- O aplicativo mostra a fila de músicas.
- O aplicativo mostra suas playlists.
- O aplicativo permite pausar/passar/voltar a música.
- Barra de tempo da música atual.

## Desenvolvimento

Com o objetivo de não ter um tutorial específico para fazer o app e sim buscando documentação, bibliotecas e tutoriais soltos pela internet sobre erros específicos o desenvolvimento foi um pouco demorado, a intenção era de simular um aplicação de mercado real (onde não temos tutorial pronto pra fazer o que queremos), de fato aprendi muita coisa que não tinha tido contato antes, um exemplo foi o **tailwind**. Tive a oportunidade de usar e também experimentar coisas novas no css para mim que sempre fiz tudo utilizando o flexbox, desta vez utilizei um pouco do grid.

Alguns erros em específico com a API, depois de "terminar" deu pra perceber que não necessariamente é preciso de um backend para rodar a aplicação, mas na documentação da API do spotify foi exemplificado com o node, então utilizei, mesmo configurando com cors tive erro, um dos problemas que foi resolvido com uma gambiarra, *~~passei o token como parametro na url de redirect~~*.  

Para poder atualizar sempre o player e a fila, o useEffect está fazendo a requisição para a API a cada segundo, o que eu não acho que seja o ideal, se abrir o network por algum tempo facilmente vai chegar em 1000 requisições.  

Não implementei o refresh token, então depois de 1 hora a página de dashboard ficará em branco e tem que voltar para página inicial e logar novamente.  

Se você abrir o dashboard sem tá escutando alguma música no spotify, o player fica bugado (não fiz todas as verificações).  

Provavelmente no github vai está uma lista de erros que pode ser resolvido, caso alguem tenha interesse; o repositório é público!

**Todos os erros são simples de serem resolvidos, decidi publicar o projeto mesmo assim devido a falta de paciência que tenho para continuar com projeto pessoal, esse projeto foi feito em 1 dia.**

## Links

[Link do projeto no github](https://github.com/gabrielrtlima/spotify-dashboard)  
[Link da aplicação](https://grtl-spotify.vercel.app/)
