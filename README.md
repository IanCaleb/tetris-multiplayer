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
git clone https://github.com/seu-usuario/tetris-multiplayer.git
cd tetris-multiplayer
