# DevOps Lab

## Pré-requisitos para instalação do Docker

Ter um computador

## Instalação do Docker

Em desenvolvimento...

## Introdução ao Git e GitHub

## Git e GitHub na Prática para DevOps

> Um guia prático para aprender Git e GitHub utilizando cenários reais encontrados na rotina de um profissional DevOps.

### Sobre este repositório

Este repositório foi criado para ensinar Git e GitHub de uma forma diferente.

Aqui você não encontrará apenas listas de comandos ou definições teóricas. Cada módulo simula situações reais enfrentadas por equipes de desenvolvimento e operações, permitindo compreender como o Git é utilizado em projetos profissionais.

O objetivo é desenvolver não apenas conhecimento técnico, mas também a forma de pensar exigida no dia a dia de um DevOps.

Ao longo da trilha você aprenderá a:

* Criar e organizar repositórios Git.
* Trabalhar com branches de maneira profissional.
* Resolver conflitos de merge.
* Colaborar utilizando GitHub e Pull Requests.
* Automatizar processos utilizando GitHub Actions.
* Construir uma base sólida para Docker, Terraform, Kubernetes e CI/CD.

---

# Estrutura da Trilha

## 📚 Módulo 1 — Fundamentos do Git

### Objetivos

* Entender o funcionamento do Git.
* Compreender a função da pasta `.git`.
* Aprender o ciclo de vida de um arquivo.
* Utilizar a Staging Area corretamente.
* Criar commits organizados.

### Exemplo Prático

Imagine que sua empresa precisa começar a documentar toda a infraestrutura.

Crie um repositório chamado:

```text
devops-lab
```

Adicione um README contendo:

```markdown
# DevOps Lab
```

Faça seu primeiro commit.

---

### Desafio

Crie três commits separados para:

* adicionar documentação;
* corrigir um erro de escrita;
* adicionar uma seção de tecnologias.

Depois visualize o histórico utilizando:

```bash
git log --oneline
```

Pergunta:

> Por que três commits pequenos são melhores do que um único commit enorme?

---

### Comandos Essenciais

```bash
git init
git status
git add .
git commit -m "mensagem"
git log
git log --oneline
git diff
git restore
```

---

## 🌿 Módulo 2 — Branches e Fluxo de Trabalho

### Objetivos

* Trabalhar com Feature Branch.
* Fazer Merge.
* Resolver conflitos.
* Entender o histórico do Git.

### Exemplo Prático

Sua branch `main` representa produção.

O gerente pede uma documentação sobre Docker.

Crie:

```text
feature/docker-docs
```

Adicione:

```markdown
## Instalação do Docker
```

Realize o commit.

Depois faça o merge.

---

### Desafio

Crie simultaneamente:

```text
feature/docker

feature/nginx

feature/terraform
```

Realize alterações diferentes em cada uma.

Depois integre todas na `main`.

Agora provoque um conflito alterando exatamente a mesma linha em duas branches diferentes.

Resolva o conflito manualmente.

---

### Comandos Essenciais

```bash
git branch
git switch
git checkout
git merge
git branch -d
git log --graph --decorate --all
```

---

## ☁️ Módulo 3 — GitHub e Colaboração

### Objetivos

* Trabalhar com repositórios remotos.
* Publicar alterações.
* Criar Pull Requests.
* Simular Code Reviews.

### Exemplo Prático

Crie um repositório vazio no GitHub.

Conecte ao projeto local.

Envie sua branch principal.

Depois crie:

```text
feature/github-actions
```

Faça um commit.

Realize o push.

Abra uma Pull Request.

---

### Desafio

Simule um fluxo profissional.

1. Crie uma Pull Request.
2. Faça uma revisão.
3. Solicite alterações.
4. Corrija o código.
5. Faça novo push.
6. Observe a Pull Request sendo atualizada automaticamente.

---

### Comandos Essenciais

```bash
git remote add origin
git remote -v
git fetch
git pull
git push
git push -u origin main
git push origin nome-da-branch
```

---

## ⚙️ Módulo 4 — GitHub Actions

### Objetivos

* Criar workflows.
* Entender Runners.
* Automatizar tarefas.
* Introduzir CI.

### Exemplo Prático

Crie:

```text
.github/workflows/ci.yml
```

Adicione um workflow simples que execute:

* echo
* date
* pwd
* ls

Faça um push.

Acompanhe a execução na aba **Actions**.

---

### Desafio

Monte uma pipeline capaz de:

* validar um Dockerfile;
* verificar arquivos YAML;
* executar testes;
* validar Terraform;
* armazenar artefatos.

Pesquise a documentação oficial sempre que necessário.

---

### Comandos Essenciais

Embora o GitHub Actions seja configurado por arquivos YAML, estes comandos fazem parte da rotina:

```bash
git add .
git commit -m "ci: adiciona workflow"
git push
```

---

# Desafios Extras

## 🏆 Desafio 1 — Simule uma Equipe

Crie cinco branches:

```text
feature/login

feature/docker

feature/nginx

feature/docs

feature/terraform
```

Faça commits diferentes em todas.

Depois integre cada uma utilizando Pull Requests.

---

## 🏆 Desafio 2 — Gere Conflitos

Faça duas branches alterarem exatamente a mesma linha.

Resolva o conflito manualmente.

Explique por que ele aconteceu.

---

## 🏆 Desafio 3 — Histórico Limpo

Faça vários commits pequenos.

Depois utilize `git rebase -i` (após estudar o assunto) para organizar o histórico.

---

## 🏆 Desafio 4 — Infraestrutura como Código

Crie este projeto:

```text
infra/

docker/

terraform/

ansible/

.github/workflows/
```

Versione tudo utilizando Git.

Imagine que esse seja o repositório oficial da infraestrutura da empresa.

---

# Comandos Mais Utilizados por um DevOps

## Versionamento

```bash
git status
git add
git commit
git log
git diff
git restore
```

## Branches

```bash
git branch
git switch
git merge
git branch -d
```

## Repositórios Remotos

```bash
git remote -v
git fetch
git pull
git push
git clone
```

## Investigação

```bash
git show
git blame
git reflog
git stash
git tag
```

## Limpeza

```bash
git clean -fd
git reset --soft
git reset --mixed
git reset --hard
```

---

# Próximos Estudos

Após dominar esta trilha, recomenda-se aprofundar os estudos em:

* Docker
* Docker Compose
* Linux
* Bash Script
* Redes
* Terraform
* Ansible
* Kubernetes
* GitHub Actions Avançado
* CI/CD
* Monitoramento
* Cloud Computing (AWS, Azure ou GCP)

Essas tecnologias complementam o uso do Git e fazem parte da rotina de praticamente todo profissional DevOps.
