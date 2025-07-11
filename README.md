# 🗺️ Mapa Inteligência

Sistema de inteligência para mapeamento e análise de dados criminais, empresariais e financeiros.

## 🚀 Deploy Rápido

### Opção 1: Deploy Automatizado (Recomendado)

```bash
# Windows
deploy.bat

# Linux/Mac
./deploy.sh
```

### Opção 2: Deploy Manual

1. **Backend (Railway)**
   ```bash
   cd server
   npm install
   npm run build
   # Deploy no Railway
   ```

2. **Frontend (Vercel)**
   ```bash
   npm install
   npm run build
   # Deploy no Vercel
   ```

📖 **Guia completo**: [DEPLOY.md](./DEPLOY.md)

## 🛠️ Tecnologias

### Frontend
- **React 18** + **TypeScript**
- **Vite** - Build tool
- **Tailwind CSS** - Styling
- **Zustand** - State management
- **React Router** - Navigation
- **Leaflet** - Maps
- **Recharts** - Charts

### Backend
- **Node.js** + **Express**
- **TypeScript**
- **SQLite** - Database
- **JWT** - Authentication
- **Multer** - File uploads
- **CORS** - Cross-origin requests

## 📁 Estrutura do Projeto

```
mapa-inteligencia/
├── src/                    # Frontend React
│   ├── components/         # Componentes React
│   ├── store/             # Zustand stores
│   ├── types/             # TypeScript types
│   └── utils/             # Utilitários
├── server/                # Backend Node.js
│   ├── src/
│   │   ├── routes/        # API routes
│   │   ├── database.ts    # Database setup
│   │   └── server.ts      # Express server
│   └── uploads/           # Uploaded files
├── public/                # Static files
└── dist/                  # Build output
```

## 🚀 Desenvolvimento Local

### Pré-requisitos
- Node.js 18+
- npm ou yarn

### Instalação

```bash
# Clone o repositório
git clone <seu-repo>
cd mapa-inteligencia

# Instale dependências do frontend
npm install

# Instale dependências do backend
cd server
npm install
cd ..

# Inicie o desenvolvimento
npm start
```

### Scripts Disponíveis

```bash
# Desenvolvimento
npm run dev          # Frontend apenas
npm start           # Frontend + Backend

# Build
npm run build       # Frontend
cd server && npm run build  # Backend

# Deploy
npm run deploy:frontend
npm run deploy:backend
```

## 🌐 URLs de Desenvolvimento

- **Frontend**: http://localhost:3000
- **Backend**: http://localhost:3001
- **API Health**: http://localhost:3001/api/health

## 📊 Funcionalidades

### Módulos Disponíveis
- 👤 **CPF** - Cadastro de pessoas
- 🏢 **CNPJ** - Cadastro de empresas
- 🏠 **Imóveis** - Cadastro de propriedades
- 🚗 **Veículos** - Cadastro de veículos
- 📱 **Telefones** - Cadastro de números
- 🌐 **Redes Sociais** - Cadastro de perfis
- 💰 **Financeiro** - Transações financeiras
- 🏭 **Empresarial** - Dados empresariais
- 📍 **Mapa** - Visualização geográfica
- 🧠 **Board** - Visualização de conexões

### Recursos
- ✅ Upload de arquivos Excel
- ✅ Visualização em mapa
- ✅ Gráficos e relatórios
- ✅ Sistema de autenticação
- ✅ Busca e filtros
- ✅ Exportação de dados
- ✅ Interface responsiva

## 🔧 Configuração

### Variáveis de Ambiente

Crie um arquivo `.env` na raiz:

```env
# Frontend
REACT_APP_API_URL=http://localhost:3001

# Backend
NODE_ENV=development
PORT=3001
FRONTEND_URL=http://localhost:3000
JWT_SECRET=sua-chave-secreta
```

### Banco de Dados

O projeto usa SQLite por padrão. Para migrar para PostgreSQL:

1. Instale PostgreSQL
2. Configure `DATABASE_URL` no `.env`
3. Atualize `server/src/database.ts`

## 🐳 Docker

### Desenvolvimento Local

```bash
docker-compose up --build
```

### Produção

```bash
# Frontend
docker build -t mapa-inteligencia-frontend .

# Backend
docker build -t mapa-inteligencia-backend ./server
```

## 📈 Monitoramento

### Logs
- **Frontend**: Console do navegador
- **Backend**: Terminal ou logs do Railway

### Métricas
- **Vercel**: Analytics automático
- **Railway**: Métricas de performance

## 🔒 Segurança

- ✅ CORS configurado
- ✅ JWT para autenticação
- ✅ Validação de entrada
- ✅ Sanitização de dados
- ✅ Headers de segurança

## 🤝 Contribuição

1. Fork o projeto
2. Crie uma branch (`git checkout -b feature/nova-funcionalidade`)
3. Commit suas mudanças (`git commit -am 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🆘 Suporte

- 📖 **Documentação**: [DEPLOY.md](./DEPLOY.md)
- 🐛 **Issues**: Abra uma issue no GitHub
- 💬 **Discussões**: Use as discussões do GitHub

---

**🎯 Desenvolvido com ❤️ para análise de inteligência**
