# My Portfolio

Este projeto é um site de portfólio pessoal, projetado para ser rápido, responsivo e fácil de gerenciar. Ele é construído utilizando o gerador de sites estáticos Hugo e o tema PaperMod, permitindo que o foco seja totalmente na criação de conteúdo em Markdown.

## 1. Stack Tecnológica

- **Gerador de Site Estático:** Hugo
- **Tema:** PaperMod
- **Linguagem de Conteúdo:** Markdown
- **Configuração:** TOML (`hugo.toml`)
- **Estilização:** CSS e HTML (gerenciados pelo tema e customizações)

## 2. Como Iniciar o Projeto

### Pré-requisitos

- Hugo (versão extended)

### Passos para Execução

1.  **Clonar o repositório:**
    ```bash
    git clone <url-do-repositorio>
    cd my-portfolio
    ```

2.  **Iniciar o servidor de desenvolvimento do Hugo:**
    O comando a seguir iniciará um servidor local, geralmente na porta 1313, com *live reload*, que atualiza o site automaticamente sempre que um arquivo é salvo.
    ```bash
    hugo server
    ```

3.  **Acessar o site:**
    Abra seu navegador e acesse `http://localhost:1313`.

### Outros Scripts

- **`hugo`**: Executa o build do site, gerando todos os arquivos estáticos na pasta `public/`. Este é o comando utilizado para preparar o site para o deploy.

## 3. Fluxos da Aplicação

### 3.1. Adicionando um Novo Projeto

Para adicionar um novo projeto ao portfólio, basta criar um novo arquivo Markdown na pasta `content/projects/`. O Hugo irá automaticamente renderizar o arquivo como uma nova página de projeto.

A estrutura de um arquivo de projeto (`nome-do-projeto.md`) é a seguinte:

```markdown
---
title: "Nome do Projeto"
date: YYYY-MM-DDTHH:MM:SSZ
draft: false
tags: ["Tecnologia1", "Tecnologia2"]
cover:
    image: "link/para/imagem.png"
    alt: "Texto alternativo"
    caption: "Legenda da imagem"
---

## Visão Geral do Projeto

Aqui você descreve o projeto, suas funcionalidades e o que ele representa.

## Tecnologias Utilizadas

- **Backend:** ...
- **Frontend:** ...
```

### 3.2. Atualizando Outras Seções

- **Sobre Mim:** Edite o arquivo `content/about.md`.
- **Experiências:** Adicione ou edite os arquivos em `content/experiences/`.

## 4. Estrutura do Projeto

```
/
├── archetypes/     # Modelos para novos conteúdos
├── content/        # Conteúdo do site em Markdown
│   ├── about.md
│   ├── experiences/
│   └── projects/
├── data/           # Arquivos de dados (ex: JSON, YAML)
├── layouts/        # Templates HTML customizados que sobrescrevem o tema
├── project_docs/   # Documentação detalhada dos projetos
├── static/         # Arquivos estáticos (imagens, CSS, JS)
├── themes/         # Contém os temas do Hugo (neste caso, PaperMod)
├── public/         # Diretório de saída do site gerado (criado pelo comando `hugo`)
└── hugo.toml       # Arquivo de configuração principal do site
```
