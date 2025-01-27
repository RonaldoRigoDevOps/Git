# 🚀 Guia Completo para Iniciar um Projeto com Git Bash

## 🛠️ Configuração Inicial do Git

Antes de começar, configure o Git com suas informações pessoais para associar seus commits ao seu nome e email.

1. **Configure seu nome de usuário**:
   ```bash
   git config --global user.name "Seu Nome"
   ```
Substitua "Seu Nome" pelo seu nome completo.

2. **Configure seu email**:
    ```bash
   git config --global user.email "seuemail@exemplo.com"
   ```
Use o mesmo email associado à sua conta do GitHub.

3. **Verifique as configurações**:
    ```bash
    git config --list
    ```
Esse comando mostra todas as configurações globais realizadas.

## 🗂️ Iniciar um Projeto com Git

1. **Crie um diretório para o projeto**:
    ```bash
    mkdir nome-do-projeto
    ```
    Navegue até o diretório criado:
    ```bash
    cd nome-do-projeto
    ```
2. **Inicialize um repositório Git local**:
    ```bash
    git init
    ```
    Esse comando cria uma pasta oculta chamada `.git`, onde o Git armazenará o histórico do projeto.

3. **Adicione arquivos ao projeto (por exemplo, um README.md)**:
    ```bash
    echo "# Nome do Projeto" > README.md
    ```
4. **Adicione os arquivos ao staging area**:
    ```bash
    git add .
    ```
    O ponto (.) adiciona todos os arquivos modificados no diretório atual.
5. **Faça o primeiro commit:**:
    ```bash
    git commit -m "Primeiro commit"
    ```
## 🌐 Criar um Repositório Remoto no GitHub
Agora, precisamos de um repositório remoto para enviar o projeto.
1. **Acesse o GitHub e faça login.**

2. **Crie um novo repositório clicando em New Repository.**
    -   Nomeie o repositório (ex.: nome-do-projeto).
    -   Escolha as configurações (público ou privado).
    -   Não inicialize com nenhum arquivo (sem README.md, .gitignore ou licença).
3. **No Git Bash, conecte o repositório local ao remoto:**
    ```bash
    git remote add origin https://github.com/SEU-USUARIO/nome-do-projeto.git
    ```
    Substitua `SEU-USUARIO` pelo seu nome de usuário no GitHub e `nome-do-projeto` pelo nome do repositório.

## 🚀 Publicar o Projeto no Repositório Remoto
1. **Envie os arquivos para o repositório remoto**:
    ```bash
    git push -u origin main
    ```
    - Se o ramo principal no GitHub for chamado master, substitua main por master.
2. **Confirme que tudo foi enviado corretamente acessando o repositório no GitHub.**

## 🔄 Comandos Adicionais Essenciais
-   **Verificar o status do repositório**:
  
    ```bash
    git status
    ```
-   **Listar os commits do histórico**:
  
    ```bash
    git log
    ```
-   **Fazer alterações e enviar novamente**:
  
    ```bash
    # Faça mudanças nos arquivos
    git add .
    git commit -m "Descrição das mudanças"
    git push
    ```
- **Clonar um repositório existente**:

    ```bash
    git clone https://github.com/SEU-USUARIO/nome-do-repositorio.git
    ```

## 💡 Dicas Finais

1. Use o comando ``git`` help ou ``git <comando> --help`` para obter detalhes sobre qualquer comando.
2. Experimente usar ferramentas como o GitHub Desktop caso prefira algo mais visual, mas mantenha a prática no terminal. 💻
3. Pratique o fluxo de commits e branches para dominar o Git!

## 📖 Resumo dos Comandos

| Comando                         | Descrição                                         |
|---------------------------------|---------------------------------------------------|
| `git config --global user.name` | Configura o nome do usuário                       |
| `git config --global user.email`| Configura o email do usuário                      |
| `git init`                      | Inicializa um repositório Git local               |
| `git add .`                     | Adiciona todos os arquivos ao staging area        |
| `git commit -m "mensagem"`      | Cria um commit com a mensagem especificada        |
| `git remote add origin URL`     | Conecta o repositório local ao repositório remoto |
| `git push -u origin main`       | Envia os arquivos para o repositório remoto       |
| `git status`                    | Mostra o status atual do repositório              |
| `git log`                       | Exibe o histórico de commits                      |
| `git clone URL`                 | Clona um repositório remoto para sua máquina      |