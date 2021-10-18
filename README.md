# Comandos Git

## Configurações iniciais do Git

- [x] ```git --version```
- [x] ```git config --global user.name "seu nome aqui"```
- [x] ```git config --global user.email "seu email aqui"```

## Trabalhando com Branchs
```git branch``` --> Exibe as branchs remotas

```git branch -a``` --> Lista todas as branchs 

```git branch teste``` --> Só cria uma nova branch

```git branch -M teste``` --> Substitui\renomeia a branch atual

```git branch -d teste``` --> Exclui uma branch

```git checkout -b nova-branch``` --> Cria uma nova branch e entra nela

```git checkout -b nova-branch origemDaBranch``` --> Cria uma nova branch ligando com a branch remota 

```git checkout master``` --> Volta para a branch atual

```git checkout teste``` --> Entra na branch teste

### Juntando Branchs(merge)
Para juntar os commits de uma branch "teste" na branch "main". Deve-se estar dentro da branch main, que trazerá os dados

```git checkout main``` --> Entra na branch main 

```git merge teste``` --> Junta o commit conforme o histórico

```git rebase teste``` --> Junta o commit colocando-o no topo

## Outros comandos

```git log``` --> Mostra todos os commits --> Argumentos a mais -->  ```--oneline``` + ```--graph``` + ```--all```

```git reset HEAD arquivo``` - desfaz o git add no arquivo

```git revert (HASH do commit)``` - desfaz o commit 

```git stash``` - salva uma alteração para resolver mais tarde

```git stash save mensagem``` - cria uma stash com mennsagem

```git stash list``` --> lista todos os stashs

```git stash pop``` - recupera essa alteração

```git diff (hash..hash)``` - Compara o hash ao outro


### Manipulando arquivos

```cd (nomeDaPasta)``` - Navega/entra nas pastas

```mkdir exemplo/``` --> Cria uma pasta

```touch exemplo.txt``` --> Cria um arquivo de texto

```mv arquivo.txt diretorio/``` / ```mv *.txt diretorio/``` --> Move um arquivo para o diretório ou todos

```mv arquivo.txt``` --> Exclui um arquivo

```mv *.txt``` --> Exclui todos os arquivos com extensão .txt


 ## Enviar repositório existente 
```git remote add origin git@github.com:MatheusMMonteiro/teste.git``` --> VIA SSH<br></br>
```git remote add origin https://github.com/MatheusMMonteiro/teste.git``` --> OU VIA HTTP<br></br>
```git branch -M main``` --> Cria\substitui uma nova branch<br></br>
```git push -u origin main``` --> Sobe as branchs para o repositório

## Criando uma nova chave SSH
Com chaves SSH, você pode conectar-se a GitHub sem inserir seu nome de usuário e token de acesso pessoal em cada visita. É uma forma onde que o cliente e servidor remoto troquem informações de maneira segura e dinâmica.
 - [x] No terminal, digite: ```ssh-keygen```
 - [x] Em seguida dê Enter sem preencher nada até finalizar
 - [X] Depois copie a chave ssh localizada no arquivo id_rsa.pub que foi criado
    - Copie tudo o que houver dentro do arquivo
 - [X] E acesse o seu GitHub, depois vá em Settings --> SSH and GPG Keys --> New SSH Key
 - [X] Adicione o título(geralmente coloco o nome da máquina) e cole a chave ssh em Key
 - [X] Após clique em "Add SSH Key"
 - [ ] Pronto!

## Lançando versões(release)
```git tag -a v0.1.0 -m "Lançando Primeira versão"``` --> Criando release

```git push origin master```

```git push origin v0.1.0``` --> subindo no git
 

