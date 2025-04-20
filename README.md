# 🧩 Roteiro de Colaboração - Projeto APAE

Este documento tem como objetivo organizar o fluxo de trabalho em equipe utilizando **Git e GitHub**, para que todos possam contribuir de forma prática, segura e sem conflitos no código.

---

## 📌 Regras Básicas

- Nunca trabalhar diretamente na `main`.
- Cada tarefa (ex: login, cadastro, página inicial) deve ser feita em uma branch separada.
- Sempre criar um **Pull Request (PR)** para juntar a sua branch na `main`.
- Antes de começar, sempre **puxar a versão mais atual da `main`**.

---

## 🚀 Fluxo de Trabalho

### 1. Clonar o repositório (somente na primeira vez)

```bash
git clone https://github.com/seu-usuario/repositorio-apae.git
cd repositorio-apae
```

---

### 2. Atualizar o projeto antes de começar qualquer tarefa

```bash
git checkout main
git pull origin main
```

---

### 3. Criar uma branch com o nome da sua tarefa

```bash
git checkout -b feature/nome-da-tarefa
```

Exemplos:
```bash
git checkout -b feature/login
git checkout -b feature/cadastro
```

---

### 4. Fazer commits conforme for desenvolvendo

```bash
git add .
git commit -m "Mensagem clara do que foi feito"
```

---

### 5. Enviar a branch para o GitHub

```bash
git push origin feature/nome-da-tarefa
```

---

### 6. Criar um Pull Request (PR)

- Vá até o repositório no GitHub.
- Clique em “Pull requests” > “New Pull Request”.
- Compare a sua branch com a `main`.
- Adicione uma descrição clara e envie o PR.

---

### 7. Revisar e Aprovar PRs

- Um colega deve revisar o código antes do merge.
- Se estiver tudo certo, pode fazer o **Merge** no GitHub.

---

### 8. Atualizar sua branch (se necessário)

Se alguém fez merge na `main` antes de você, atualize sua branch:

```bash
git checkout main
git pull origin main

git checkout feature/sua-branch
git merge main
```

Resolva os conflitos (se houver), depois:

```bash
git push origin feature/sua-branch
```

---

## 🌟 Padrões de Branches

- `feature/`: Para novas funcionalidades (ex: `feature/contato`)
- `fix/`: Para correções de bugs (ex: `fix/erro-login`)
- `docs/`: Atualizações de documentação (ex: `docs/readme`)

---

## 📚 Boas práticas

- Commits com mensagens claras e diretas.
- Nunca faça push direto na `main`.
- Sempre revise seu código antes de criar um PR.
- Trabalhe em arquivos diferentes sempre que possível, para evitar conflitos.

---

## 💬 Dúvidas?

Fale com o responsável pelo Git no projeto: **DataGusIT**

---
