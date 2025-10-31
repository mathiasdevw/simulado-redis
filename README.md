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
