# 🧠 Comandos Essenciais de Terminal e GitHub

Este guia reúne os principais comandos usados no **terminal (Git Bash, Linux ou WSL)** e no **GitHub**, organizados por categoria.  
Perfeito para consultas rápidas no dia a dia de desenvolvimento. 🚀

---

## ⚙️ Comandos Básicos do Terminal

| Comando | Descrição |
|----------|------------|
| `pwd` | Mostra o diretório atual |
| `ls` | Lista os arquivos e pastas |
| `ls -a` | Lista todos os arquivos, incluindo ocultos |
| `cd nome-da-pasta` | Entra em uma pasta |
| `cd ..` | Volta uma pasta |
| `mkdir nome-da-pasta` | Cria uma nova pasta |
| `rmdir nome-da-pasta` | Remove uma pasta vazia |
| `rm nome-do-arquivo` | Remove um arquivo |
| `clear` | Limpa o terminal |
| `touch nome-do-arquivo.ext` | Cria um novo arquivo |
| `code .` | Abre o VS Code na pasta atual |
| `exit` | Fecha o terminal |

---

## 🧩 Iniciando um Repositório Git

| Comando | Descrição |
|----------|------------|
| `git init` | Inicializa um novo repositório Git local |
| `git status` | Mostra o status das alterações |
| `git add .` | Adiciona todas as alterações para o próximo commit |
| `git add nome-do-arquivo` | Adiciona um arquivo específico |
| `git commit -m "mensagem"` | Registra as alterações com uma mensagem |
| `git log` | Mostra o histórico de commits |
| `git diff` | Mostra as diferenças entre arquivos modificados |

---

## 🌍 Conectando ao GitHub

### 🔑 Configuração Inicial (uma vez por máquina)
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@exemplo.com"

