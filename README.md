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
```

### 🔑 Conectando com SSH
```bash
ssh-keygen -t rsa -b 4096 -C "seu-email@exemplo.com"
```
Depois copie a chave pública (geralmente em ~/.ssh/id_rsa.pub) e cole no seu GitHub → Settings → SSH and GPG keys.
Teste a conexão:
```bash
ssh -T git@github.com
```
## 🚀 Subindo um Projeto para o GitHub

| Etapa                            | Comando                                                             |
| -------------------------------- | ------------------------------------------------------------------- |
| 1️⃣ Inicia o Git                 | `git init`                                                          |
| 2️⃣ Adiciona os arquivos         | `git add .`                                                         |
| 3️⃣ Cria o commit                | `git commit -m "primeiro commit"`                                   |
| 4️⃣ Cria o repositório no GitHub | *(feito pelo site do GitHub)*                                       |
| 5️⃣ Conecta o repositório remoto | `git remote add origin git@github.com:usuario/nome-repositorio.git` |
| 6️⃣ Envia os arquivos            | `git push -u origin main` ou `git push -u origin master`            |

## 🔁 Atualizando o Repositório
| Comando                | Descrição                             |
| ---------------------- | ------------------------------------- |
| `git pull origin main` | Baixa as atualizações do GitHub       |
| `git push origin main` | Envia alterações locais para o GitHub |
| `git fetch`            | Busca atualizações sem aplicar        |
| `git merge`            | Une mudanças de diferentes branches   |

## Trabalhando com Branches

| Comando                          | Descrição                         |
| -------------------------------- | --------------------------------- |
| `git branch`                     | Lista as branches existentes      |
| `git branch nome-da-branch`      | Cria uma nova branch              |
| `git checkout nome-da-branch`    | Muda para a branch especificada   |
| `git checkout -b nome-da-branch` | Cria e já muda para a nova branch |
| `git merge nome-da-branch`       | Junta uma branch à atual          |
| `git branch -d nome-da-branch`   | Deleta uma branch local           |

## 🧹 Dicas Úteis

| Dica                                           | Comando                                            |
| ---------------------------------------------- | -------------------------------------------------- |
| Ver os repositórios remotos                    | `git remote -v`                                    |
| Remover repositório remoto                     | `git remote remove origin`                         |
| Desfazer último commit (sem perder alterações) | `git reset --soft HEAD~1`                          |
| Desfazer commit e alterações                   | `git reset --hard HEAD~1`                          |
| Clonar um repositório                          | `git clone git@github.com:usuario/repositorio.git` |
