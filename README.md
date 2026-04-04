# 🚀 Projeto de Estudos - Git e Versionamento

<p align="center">
  <img src="https://img.shields.io/badge/status-em%20desenvolvimento-yellow"/>
  <img src="https://img.shields.io/badge/feito%20com-Git-blue"/>
  <img src="https://img.shields.io/badge/GitHub-repositório-black"/>
</p>

---

## 📌 Sobre o Projeto
Este repositório contém meus estudos sobre Git e versionamento de código, com base no curso da Ada Tech e conteúdos complementares do YouTube.

---

## 🎯 Objetivo
- Aprender versionamento de código  
- Dominar comandos essenciais do Git  
- Praticar o uso do GitHub  
- Construir uma base sólida para Cloud/DevOps  

━━━━━━━━━━━━━━━━━━

## 🛠️ Tecnologias e Conceitos

### 🔹 Versionamento de código
O versionamento de código veio para facilitar a vida de empresas e programadores.  
Ele permite o registro de mudanças nos arquivos, possibilitando a recuperação de versões anteriores e evitando prejuízos em ambientes de trabalho.  

Além disso, torna possível o desenvolvimento de código de forma colaborativa entre diferentes integrantes de uma equipe.

---

### 🔹 Git
O Git é um sistema de versionamento de código que armazena snapshots (fotos) do estado do projeto ao longo do tempo, além de registrar todo o caminho percorrido pelo projeto.  

Ele funciona como um conjunto de ferramentas que realizam o controle de versão com precisão.  
Grande parte das suas operações são locais, o que faz com que muitos comandos sejam extremamente rápidos.

---

### 🔹 GitHub
O GitHub é uma plataforma que permite armazenar repositórios na nuvem, facilitando o compartilhamento de código e o trabalho em equipe.

━━━━━━━━━━━━━━━━━━

## 💻 Comandos Git

### 🔹 Configuração inicial
```bash
git config --global user.name "seu nome"
git config --global user.email "seu melhor email"

Esses comandos servem para cadastrar o usuário que está realizando os versionamentos.

🔹 Como acessar um repositório Git?
🔸 Existem duas formas: remota e local
🌐 Forma remota

Se você estiver utilizando o GitHub:

Acesse seu repositório
Clique em Code
Copie o link HTTPS

Depois:

Crie uma pasta no seu computador
Copie o caminho dessa pasta
Abra o terminal (ou CMD)

Execute:

cd caminho-da-sua-pasta
git clone <link-do-repositório>

➡️ O comando cd entra na pasta
➡️ O git clone baixa o repositório para sua máquina

💻 Forma local
Crie ou abra uma pasta do projeto
Abra essa pasta na sua IDE
Use o terminal e execute:
git init

➡️ Esse comando inicia um repositório local

━━━━━━━━━━━━━━━━━━

👀 De olho no meu código
git status

O git status mostra:

Em qual branch você está
Quais arquivos foram modificados

Arquivos em vermelho indicam que foram alterados, mas ainda não foram adicionados.

🌿 Mas o que é uma Branch?

🔸 Explicando de forma simples:

Imagine que seu projeto é uma árvore 🌳

O tronco principal é a branch principal (geralmente main)
Cada nova funcionalidade é um galho (branch)

👉 Isso permite trabalhar em novas funcionalidades sem alterar o código principal

➕ Adicionando alterações
git add .

Esse comando adiciona todas as alterações feitas.
Os arquivos saem do estado modified e vão para staged.

📊 Verificando diferenças
git diff

Mostra as linhas que foram alteradas no código.

💾 Salvando alterações
git commit -m "mensagem"

Cria um ponto de salvamento do projeto com uma descrição das mudanças.

📜 Histórico
git log

Mostra todo o histórico de commits realizados.

🔄 Restaurando arquivos
git restore

Permite desfazer alterações em arquivos.