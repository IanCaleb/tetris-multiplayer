# 🎮 Tetris Multiplayer — Projeto em HTML, CSS, JS e Node.js

Este é um projeto experimental de **Tetris multiplayer** jogado através de **celulares como controles** conectados a um **monitor principal**.  
Cada jogador escaneia um **QR Code** que o leva a uma página de controle no celular, e seus comandos são enviados em tempo real para o jogo exibido no navegador do computador.

---

## 🧠 Objetivo

Aprender e demonstrar na prática conceitos de:
- Desenvolvimento web completo (**frontend + backend**)
- Comunicação em tempo real com **WebSockets (Socket.IO)**
- Integração entre múltiplos dispositivos
- Lógica de jogos usando **HTML5 Canvas**

---

## ⚙️ Tecnologias utilizadas

| Camada | Tecnologias |
|--------|--------------|
| **Frontend** | HTML5, CSS3, JavaScript |
| **Backend** | Node.js, Express.js |
| **Comunicação em tempo real** | Socket.IO |
| **Extras (futuro)** | QR Code Generator, hospedagem na Vercel/Render |

---

## 🧩 Estrutura do projeto

```
├── public/
│ ├── index.html # Tela principal (monitores do jogo)
│ ├── controller.html # Controle do jogador (celular)
│ ├── js/
│ │ ├── client.js # Lógica do jogo (recebe comandos)
│ │ └── controller.js # Lógica do controle (envia comandos)
│ └── css/
│ ├── style.css
│ └── controller.css
├── server.js # Servidor Express + Socket.IO
├── package.json
└── README.md
```

---

## 🚀 Como rodar o projeto localmente

### 1. Clone o repositório
```bash
git clone https://github.com/IanCaleb/tetris-multiplayer.git
cd tetris-multiplayer

## instale as dependências

npm install

## Executar o servidor

node server.js

# O servidor executa em:

http://localhost:3000
```

## 🚀 Como rodar o projeto localmente

### 4. Acesse as páginas

Após executar o servidor com `node server.js`, você pode abrir as seguintes URLs no navegador:

- **🎮 Monitor principal (jogo):**  
  [http://localhost:3000](http://localhost:3000)

- **📱 Controle (celular):**  
  [http://localhost:3000/controller.html](http://localhost:3000/controller.html)

> 💡 Dica: abra o endereço do controle no seu celular (conectado à mesma rede Wi-Fi) para testar o controle remoto em tempo real.

---

## 📱 Funcionamento

- O servidor **Node.js** utiliza **Socket.IO** para comunicação em tempo real entre navegadores.
- A tela principal exibe o jogo Tetris em dois monitores simulados.
- Cada jogador acessa a página `/controller.html` e envia comandos (⬅️ ➡️ 🔄 ⬇️).
- Os comandos são transmitidos instantaneamente para o jogo via **WebSockets**.

Fluxo de comunicação simplificado:

---

## 🧭 Próximos passos

- [ ] Adicionar geração automática de **QR Codes** que redirecionam para `/controller.html`
- [ ] Implementar a lógica completa do **Tetris em Canvas**
- [ ] Associar cada controle a um jogador específico (Player 1 e Player 2)
- [ ] Adicionar interface aprimorada com **CSS responsivo**
- [ ] Hospedar o projeto online (Render, Vercel, ou outra plataforma)
- [ ] Adicionar placar e status de partida

---

## 🧑‍💻 Autor

**[Seu Nome Aqui]**  
Projeto pessoal de aprendizado sobre **desenvolvimento web e comunicação em tempo real**.  
📅 Início: **Novembro de 2025**

---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).  
Sinta-se livre para usar, modificar e compartilhar.
