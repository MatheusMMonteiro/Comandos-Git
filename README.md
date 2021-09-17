# Comandos Git

## Configurações iniciais do Git

- [x] ```git --version```
- [x] ```git config --global user.name "seu nome aqui"```
- [x] ```git config --global user.email "seu email aqui"```

## Comandos práticos Git

```cd (nomeDaPasta)``` - Navega/entra nas pastas

```mkdir exemplo/``` --> Cria uma pasta

```touch exemplo.txt``` --> Cria um arquivo de texto

```git init``` --> Cria um repositório/Cotainer

```git status``` --> Verifica a situação do repositório

```git add``` . --> Adiciona os arquivos da pasta no repositório

```git commit``` -m "comentario" --> Sela os arquivos 

```git log``` --> Mostra todos os commits --> Argumentos a mais -->  ```--oneline``` + ```--graph``` + ```--all```

```git branch teste``` --> Só cria uma nova branch

```git branch -M teste``` --> Substitui\renomeia a branch atual

```git checkout -b teste``` --> Cria uma nova branch e entra na branch 

```git checkout teste``` --> Entra na branch teste

```git branch``` --> Exibe todas as branchs

```git branch -d teste``` --> Exclui uma branch

```mv arquivo.txt diretorio/``` / ```mv *.txt diretorio/``` --> Move um arquivo para o diretório ou todos

```mv arquivo.txt``` --> Exclui um arquivo

```mv *.txt``` --> Exclui todos os arquivos com extensão .txt

## Criando uma nova chave SSH
 - [x] No terminal, digite: ```ssh-keygen```
 - [x] Em seguida dê Enter sem preencher nada até finalizar
 - [X] Depois copie a chave ssh localizada no arquivo id_rsa.pub que foi criado
    - Copie tudo o que houver dentro do arquivo
 - [X] E acesse o seu GitHub, depois vá em Settings --> SSH and GPG Keys --> New SSH Key
 - [X] Adicione o título(geralmente coloco o nome da máquina) e cole a chave ssh em Key
 - [X] Após clique em "Add SSH Key"
 - [ ] Pronto!
 
 ## Enviar repositório existente 
```git remote add origin git@github.com:MatheusMMonteiro/teste.git``` --> VIA SSH<br></br>
```git remote add origin https://github.com/MatheusMMonteiro/teste.git``` --> OU VIA HTTP<br></br>
```git branch -M main``` --> Cria\substitui uma nova branch<br></br>
```git push -u origin main``` --> Sobe as branchs para o repositório
 

