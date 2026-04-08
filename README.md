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

### 🧠 Conceito Importante
🔹 Estados dos arquivos no Git
- Modified → arquivo alterado
- Staged → pronto para commit
- Committed → salvo no histórico

━━━━━━━━━━━━━━━━━━

## 💻 Comandos Git

### 🔹 Configuração inicial

**Ao criarmos a pasta do projeto seguir esses comandos é essencial**

```bash
git init
```
➡️ Esse comando inicia um repositório local e cria um arquivo chamado **.git**

```bash
git config --global user.name "seu nome"
git config --global user.email "seu melhor email"
```

Esses comandos servem para cadastrar o usuário que está realizando os versionamentos.


━━━━━━━━━━━━━━━━━━

### 👀 De olho no meu código
```bash
git status
```
O git status mostra:
- Em qual branch você está
- Quais arquivos foram modificados

Arquivos em vermelho indicam que foram alterados, mas ainda não foram adicionados.

🌿 Mas o que é uma Branch?

🔸 Explicando de forma simples:

Imagine que seu projeto é uma árvore 🌳

O tronco principal é a branch principal (geralmente main)
Cada nova funcionalidade é um galho (branch)

👉 Isso permite trabalhar em novas funcionalidades sem alterar o código principal

➕ Adicionando alterações
```bash
git add .
```
👉 Esse comando adiciona todas as alterações feitas.

```bash
git add nome-do-arquivo
```
➡️ Adiciona um arquivo específico

👉 Os arquivos saem do estado modified e vão para staged.

📊 Verificando diferenças
```bash
git diff
```
👉 Mostra as linhas que foram alteradas no código.

💾 Salvando alterações
```bash
git commit -m "mensagem"
```
👉 Cria um ponto de salvamento do projeto com uma descrição das mudanças.

📜 Histórico de commits
```bash
git log
```
👉 Mostra todo o histórico de commits realizados.

```bash
git log --oneline
```
➡️ Versão resumida do histórico

🔄 Restaurando arquivos
```bash
git restore
```
Permite desfazer alterações em arquivos.

━━━━━━━━━━━━━━━━━━

## 🌐 Repositórios Remotos

### 🔗 Interagindo com o Repositório Remoto

Aprenda os principais comandos para trabalhar com repositórios remotos no Git:

🔹 Conecta repositório local ao remoto
```bash
git remote add origin <url>
```
👉 Para acessar o URL do seu repositório é só olhar em "CODE" e depois HTTPS

```bash
git remote -v
```
➡️ Lista repositórios conectados

```bash
git push -u origin main
```
➡️ Envia commits para o GitHub

```bash
 git pull
```
Atualiza o repositório local com as alterações do remoto, realizando um *merge* automático.  
> ⚠️ Pode gerar conflitos se houver alterações locais não sincronizadas.

```bash
 git fetch 
```
Baixa as alterações do repositório remoto, mas **não aplica automaticamente** no seu projeto local.

### ✅ Boa prática recomendada

Antes de usar o `git pull`, siga este fluxo:

```bash
git fetch
git diff
git pull
```
━━━━━━━━━━━━━━━━━━

### 📌 Comandos e Conceitos Essenciais do Git

**🌿 Branches (Ramificações)**

- Branches permitem trabalhar em funcionalidades sem afetar o código principal.

```bash
 git branch
```
Lista todas as branches existentes (locais e remotas).  
> ⚠️ Este comando **não envia código** para o repositório remoto.

```bash
 git branch nome-da-branch
```
> Este comando permite você criar uma nova branch

```bash
 git checkout nome-da-branch
```
> Este comando permite você trocar de branch

```bash
 git checkout -b nome-da-branch
```
> Este comando permite você criar e já troca para a nova branch

```bash
 git rm nome-do-arquivo
```
> Este comando permite você remover arquivo do Git

```bash
 git reset
```
> Este comando permite você desfazer alterações (cuidado ⚠️)

 **.gitignore**

Arquivo usado para ignorar arquivos/pastas que não devem ser versionados.

📌 Exemplo:
```bash
node_modules/
.env
__pycache__/
```

➡️ Evita subir arquivos desnecessários ou sensíveis (como senhas)
━━━━━━━━━━━━━━━━━━

**🔀 Merge (Junção de Branches)**

O git merge é utilizado para unir alterações de uma branch em outra, integrando funcionalidades desenvolvidas separadamente ao projeto principal.

```bash
 git merge nome-da-branch
```

➡️ Aplica os commits da branch informada na branch atual

⚠️ É importante estar na branch que receberá as alterações

💡 Pode ocorrer conflito de merge quando duas branches alteram a mesma parte do código, sendo necessário resolver manualmente

---
**🔹 Fluxo básico do Git**
```bash
git status → git add → git commit → git push
```

### 🌐 Conceitos do Mundo Real (GitHub)
**🔹 Pull Request (PR)**

O Pull Request é uma solicitação para que suas alterações sejam analisadas antes de entrar no projeto principal.

📌 Fluxo:

Criar uma branch
Fazer alterações
Enviar (git push)
Abrir um PR no GitHub

➡️ Permite:

- Revisão de código
- Discussão em equipe
- Aprovação antes do merge
🔹 Fork

**O Fork é uma cópia de um repositório para sua conta.**

➡️ Usado para:

Contribuir em projetos open source
Fazer alterações sem afetar o projeto original

📌 Fluxo:

1. Fazer um fork no GitHub
2. Clonar o repositório
3. Criar uma branch
4. Fazer alterações
5. Abrir Pull Request

**⚡ Fluxo Profissional (Resumo)**
```bash
git clone
git checkout -b minha-feature
git add .
git commit -m "feat: minha alteração"
git push
```

➡️ Depois: abrir Pull Request no GitHub

