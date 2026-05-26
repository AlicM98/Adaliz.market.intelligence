# Adaliz - Plataforma de Inteligência de Mercado

![Adaliz Logo](/public/logo.png)

Plataforma completa de inteligência de mercado para análise competitiva, monitoramento de concorrentes e insights estratégicos.

## Funcionalidades

### Dashboard Analítico
- **Métricas em tempo real** - Acompanhe posição no ranking, market share, pontuação de marca e sentimento do mercado
- **Gráficos interativos** - Visualizações com Recharts incluindo:
  - Gráfico de barras para indicadores de posicionamento
  - Gráfico radar para análise comparativa de mercado
  - Gráfico de área para evolução de market share
  - Gráfico de pizza para distribuição de sentimento
  - Gráfico de barras horizontais para pontuação de concorrentes
  - Gráfico de linhas para tendências de preços

### Monitoramento de Concorrentes
- Tabela detalhada com informações dos concorrentes
- Indicadores de variação (positiva/negativa)
- Filtros e ordenação

### Assistente de IA
- Chatbot integrado com Grok (xAI)
- Respostas sobre funcionalidades da plataforma
- Sugestões de perguntas frequentes
- Interface flutuante acessível em qualquer página

### Autenticação
- Página de login estilizada
- Modo demonstração para testes
- Proteção de rotas do dashboard

## Tecnologias

- **Framework**: Next.js 15 (App Router)
- **Estilização**: Tailwind CSS v4
- **Componentes**: shadcn/ui
- **Gráficos**: Recharts
- **IA**: AI SDK + Grok (xAI)
- **Ícones**: Lucide React
- **Fontes**: Inter + Space Grotesk

## Configuração

### Pré-requisitos
- Node.js 18+
- pnpm (recomendado)

### Variáveis de Ambiente

Crie um arquivo `.env.local` na raiz do projeto:

```env
XAI_API_KEY=sua_api_key_do_xai
```

Para obter a API key do xAI:
1. Acesse [console.x.ai](https://console.x.ai/)
2. Crie uma conta ou faça login
3. Vá em "API Keys" e crie uma nova chave
4. Adicione créditos se necessário

### Instalação

```bash
# Clone o repositório
git clone <url-do-repositorio>

# Instale as dependências
pnpm install

# Execute em modo de desenvolvimento
pnpm dev
```

Acesse [http://localhost:3000](http://localhost:3000) no navegador.

## Estrutura do Projeto

```
├── app/
│   ├── api/
│   │   └── chat/          # API route do chatbot
│   ├── dashboard/         # Página do dashboard
│   ├── login/             # Página de login
│   ├── globals.css        # Estilos globais e tema
│   ├── layout.tsx         # Layout raiz
│   └── page.tsx           # Landing page
├── components/
│   ├── ui/                # Componentes shadcn/ui
│   ├── ai-chatbot.tsx     # Componente do chatbot
│   ├── dashboard-charts.tsx # Gráficos do dashboard
│   └── hero-preview-card.tsx # Card de preview
├── public/
│   └── logo.png           # Logo da Adaliz
└── README.md
```

## Uso

### Login
- Acesse `/login` para a página de autenticação
- Clique em "Acessar Demonstração" para entrar no modo demo

### Dashboard
- Visualize métricas e gráficos de inteligência de mercado
- Clique no botão azul no canto inferior direito para abrir o assistente de IA
- Use o botão "Voltar ao Site" no sidebar para retornar à landing page

### Assistente de IA
- Faça perguntas sobre a plataforma Adaliz
- Clique nas sugestões de perguntas frequentes
- O assistente responde em português

## Licença

Projeto proprietário - Adaliz © 2024
