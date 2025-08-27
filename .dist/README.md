# Aprendendo a usar git

## Comandos principais

- **git --version**: exibe a versão do git.

- **git init**: inicia um repositório git na máquina.

- **git add \[file\]**: adiciona os arquivos modificados para **staging area**, que é como se fosse uma "caixa de preparação" no Git. Antes de salvar o histórico no Git (fazer o **commit**), você precisa escolher quais mudanças vão entrar.
    - git add .: Adiciona todos os arquivos modificados.

- **git remote add origin \[link\]**: Cria uma conexão com o repositório git hospedado na Web (normalmente no GitHub ou GitLab). "origin" é o nome que damos a esse repositório remoto.

- **git commit -m "\[mensagem\]"**: Salva as alterações feitas no repositório local.

- **git push origin main**: "Empurrão". Nós mandamos as alterações salvas com o **commit** para o repositório remoto. Neste comando, "origin" é o nome do repositório e main é o nome da **branch**.
    - **git push -u origin main**: Aqui o -u é a abreviação para --set-upstream. Além de enviar o branch, ele configura o branch remoto como "upstream" do branch local. Na prática isso cria um vínculo que permite rodar "git push" e "git pull" sem precisar ficar repetindo origin main toda hora.

- **git branch**: Exibe na tela a branch atual que você está trabalhando.

- **git checkout -b "\[nome da branch\]"**: Este comando cria uma nova branch (indicado por -b), com o nome definido pelo usuário, e por meio do "checkout" já te redireciona para a branch criada.
    - **git checkout "\[nome da branch\]"**: Muda para a branch indicado pelo nome.

- **git merge "\[nome da branch\]"**: Junta a branch especificada na branch principal (main/master)