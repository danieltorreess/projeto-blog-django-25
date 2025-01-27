CMD
cd "G:\Meu Drive\"
mkdir *NomeDoProjeto*
code *NomeDoProjeto*

Criação do arquivo "README.md" na raiz do Projeto para inserir todos os comandos
cmd, Python ou bibliotecas de modo geral.

# Blog

Este é o blog que foi criado no curso de Python.

# Verificando se existe uma chave SSH no seu computador

CMD Administrador
ls ~/.ssh
cat ~/.ssh/id_rsa.pub
cat ~/.ssh/id_ed25519.pub

# Se não existir

CMD
ssh-keygen -t ed25519 -C "seu-email@example.com"

# Se for RSA
ssh-keygen -t rsa -b 4096 -C "seu-email@example.com" 

# Deixe a senha em branco e apenas pressione Enter

# Adicionar a chave SSH ao agente
Set-Service -Name ssh-agent -StartupType Manual
Start-Service ssh-agent

# Sempre inserir caminho completo
ssh-add C:\Users\Cicero\.ssh\danieltorres_rsa

# Verificando se obteve sucesso
ssh-add -l
ssh -T git@github.com

# Volte para o projeto e inicie o Git no CMD normal
cd "G:\Meu Drive\projeto-blog-django-25"
git init
git remote add origin git@github.com:danieltorreess/projeto-blog-django-25.git
