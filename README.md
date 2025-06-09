# Firebase Login App 🔐

Uma aplicação React Native simples e elegante que implementa autenticação Firebase com Email/Password, construída com Expo.

##  Funcionalidades

- 🔑 **Autenticação Firebase** - Login e registro seguro com email/senha
- 🔄 **Alternância entre telas** - Navegação fluida entre login e cadastro
- 👤 **Sessão autenticada** - Tela personalizada para usuários logados
- 🚪 **Logout** - Funcionalidade completa de saída
- 📱 **Design responsivo** - Interface otimizada para dispositivos móveis
- ⚡ **Gerenciamento de estado** - Controle eficiente do estado de autenticação

## 🛠️ Stack Tecnológica

- **React Native** - Framework para desenvolvimento mobile
- **Expo** - Plataforma de desenvolvimento e deployment
- **Firebase Authentication** - Serviço de autenticação do Google
- **JavaScript/JSX** - Linguagem de programação

## 🚀 Começando

### 📋 Pré-requisitos

Certifique-se de ter instalado:

- [Node.js](https://nodejs.org/) (versão 14 ou superior)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)
- Uma conta no [Firebase](https://firebase.google.com/)

### 📦 Instalação

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/your-username/firebaseLogin.git
   cd firebaseLogin
   ```

2. **Instale as dependências:**
   ```bash
   npm install
   ```

3. **Configure o Firebase** (veja seção abaixo)

4. **Inicie o projeto:**
   ```bash
   npx expo start
   ```

5. **Execute no dispositivo:**
   - Use o aplicativo Expo Go para escanear o QR code
   - Ou use um emulador Android/iOS

## 🔥 Configuração do Firebase

### 1. Criar Projeto Firebase

1. Acesse o [Console do Firebase](https://console.firebase.google.com)
2. Clique em "Criar projeto"
3. Siga as instruções para configurar seu projeto

### 2. Configurar Autenticação

1. No console do Firebase, vá para **Authentication**
2. Clique na aba **Sign-in method**
3. Habilite **Email/Password**
4. Salve as configurações

### 3. Obter Credenciais

1. Vá para **Configurações do projeto** (ícone de engrenagem)
2. Selecione **Configurações gerais**
3. Na seção "Seus aplicativos", clique em **Web**
4. Copie as credenciais do Firebase

### 4. Configurar no App

Substitua a configuração no arquivo `App.js`:

```javascript
const firebaseConfig = {
  apiKey: "sua-api-key",
  authDomain: "seu-projeto.firebaseapp.com",
  projectId: "seu-project-id",
  storageBucket: "seu-projeto.appspot.com",
  messagingSenderId: "seu-sender-id",
  appId: "seu-app-id"
};
```

## 📁 Estrutura do Projeto

```
firebaseLogin/
├── 📄 App.js               # Lógica principal com autenticação Firebase
├── 📄 index.js             # Ponto de entrada da aplicação
├── 📄 app.json             # Configurações do Expo
├── 📄 metro.config.js      # Configuração do Metro bundler
├── 📄 package.json         # Dependências e scripts
├── 📄 README.md            # Documentação do projeto
└── 📁 assets/              # Ícones, imagens e recursos
    ├── 🖼️ icon.png         # Ícone do app
    └── 🖼️ splash.png       # Tela de splash
```

## 🎯 Como Usar

1. **Primeira execução:** Crie uma conta usando email e senha
2. **Login:** Use suas credenciais para acessar o app
3. **Logout:** Use o botão de logout para sair da sessão
4. **Alternar:** Mude entre as telas de login e cadastro conforme necessário

## 🔧 Comandos Úteis

```bash
# Instalar dependências
npm install

# Iniciar o servidor de desenvolvimento
npx expo start

# Iniciar com cache limpo
npx expo start --clear

# Construir para produção
npx expo build:android
npx expo build:ios
