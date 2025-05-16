# *Quiz - 10 Regras de Ouro da Segurança no Trabalho* 🛡️

Um jogo educativo interativo sobre segurança no trabalho, desenvolvido para conscientização e treinamento de equipes.

![Preview do Quiz](https://via.placeholder.com/800x400.png?text=Quiz+Segurança+no+Trabalho)

## *Funcionalidades Principais* ✨

- *10 regras de segurança* com 5 perguntas cada
- *Sistema de pontuação* com ranking competitivo
- *Timer* para respostas (30 segundos por pergunta)
- *Progresso salvo* em tempo real (Firebase)
- *Painel de administração* para gerenciamento das regras
- *Interface responsiva* para desktop e mobile
- *Splash screen* animada com barra de progresso
- *Tela de senha* para acesso restrito

## *Tecnologias Utilizadas* 💻

- *Frontend*: HTML5, CSS3, JavaScript (ES6+)
- *Backend*: Firebase Realtime Database
- *Bibliotecas*: Firebase SDK v9

## *Como Executar Localmente* 🚀

1. *Pré-requisitos*:
   - Navegador moderno (Chrome, Firefox, Edge)
   - Conexão com internet (para o Firebase)

2. *Instalação*:
   bash
   # Clone o repositório
   git clone https://github.com/seu-usuario/quiz-seguranca.git
   
   # Acesse a pasta do projeto
   cd quiz-seguranca
   

3. *Execute*:
   - Abra o arquivo index.html no navegador

## *Configuração do Firebase* 🔥

1. Crie um projeto no [Firebase Console](https://console.firebase.google.com/)
2. Ative o *Realtime Database*
3. Substitua as configurações no código:
   javascript
   const firebaseConfig = {
     apiKey: "SUA_API_KEY",
     authDomain: "SEU_PROJETO.firebaseapp.com",
     databaseURL: "https://SEU_PROJETO.firebaseio.com",
     projectId: "SEU_PROJETO",
     storageBucket: "SEU_PROJETO.appspot.com",
     messagingSenderId: "SEU_SENDER_ID",
     appId: "SEU_APP_ID"
   };
   

## *Estrutura do Projeto* 📂


quiz-seguranca/
├── index.html          # Arquivo principal
├── README.md           # Este arquivo
├── assets/             # Pasta para recursos
│   ├── css/            # Estilos adicionais (opcional)
│   └── img/            # Imagens do projeto


## *Credenciais de Acesso* 🔐

- *Senha do Quiz*: 1303
- *Senha de Admin*: admin123

## *Personalização* 🎨

Para alterar as perguntas ou regras:
1. Edite o array rulesData no JavaScript
2. Cada regra deve conter:
   javascript
   {
     id: Number,
     title: String,
     description: String,
     completed: Boolean,
     questions: Array,
     score: Number,
     unlocked: Boolean
   }
   

## *Regras de Banco de Dados* 📝

Configure estas regras no Firebase:
json
{
  "rules": {
    "players": {
      ".read": true,
      ".write": true
    }
  }
}


## *Contribuição* 🤝

Contribuições são bem-vindas! Siga os passos:
1. Faça um fork do projeto
2. Crie uma branch (git checkout -b feature/nova-feature)
3. Commit suas mudanças (git commit -m 'Adiciona nova feature')
4. Push para a branch (git push origin feature/nova-feature)
5. Abra um Pull Request

## *Licença* 📜

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

## *Contato* ✉️

- Desenvolvedor: [John Santos](https://github.com/john3206)
- Email: jlenon.32@outlook.com

---

*Nota*: Este projeto foi desenvolvido para fins educacionais e pode ser adaptado para diferentes contextos de treinamento em segurança no trabalho.
