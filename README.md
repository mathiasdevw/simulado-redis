<<<<<<< HEAD
# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
=======
# Simulado Redis Interativo

Um simulado interativo de 30 questões sobre Redis, desenvolvido para ajudar estudantes a se prepararem para exames.

## Funcionalidades

- **30 Questões**: Cobrindo Strings, Lists, Sets e Sorted Sets
- **Modo Multi-página**: Uma questão por vez com navegação
- **Tipos Mistos**: Múltipla escolha e entrada de texto
- **Timer**: 30 segundos por questão
- **Feedback Imediato**: Verificação de resposta com explicações
- **Ranking**: Sistema de pontuação persistente via Supabase
- **PDF Export**: Baixe seus resultados
- **Responsivo**: Funciona em desktop e mobile

## Estrutura do Projeto

```
/
├── index.html              # Página inicial
├── pages/
│   ├── quiz.html           # Página do simulado
│   └── ranking.html        # Página de ranking
├── assets/
│   ├── css/
│   │   └── styles.css      # Estilos globais
│   ├── js/                 # Scripts JavaScript (futuro)
│   └── images/             # Imagens (futuro)
└── README.md               # Este arquivo
```

## Tecnologias

- HTML5
- CSS3
- JavaScript (ES6+)
- Supabase (banco de dados)
- jsPDF (export PDF)

## Como Usar

1. Clone o repositório
2. Abra `index.html` no navegador
3. Clique em "Iniciar Simulado"
4. Digite seu nome
5. Responda as 30 questões
6. Veja seu resultado e envie para o ranking

## Deploy no Vercel

1. Faça push para um repositório Git
2. Conecte ao Vercel
3. Deploy automático

## Configuração Supabase

O projeto usa Supabase para armazenar pontuações. A tabela `scores` tem a seguinte estrutura:

```sql
CREATE TABLE scores (
  id SERIAL PRIMARY KEY,
  name TEXT NOT NULL,
  score INTEGER NOT NULL,
  percentage INTEGER NOT NULL,
  created_at TIMESTAMP DEFAULT NOW()
);
```

## Desenvolvimento

Para contribuir:

1. Fork o projeto
2. Crie uma branch para sua feature
3. Faça commit das mudanças
4. Abra um Pull Request

## Licença

Este projeto é open source e está sob a licença MIT.
>>>>>>> origin/main
