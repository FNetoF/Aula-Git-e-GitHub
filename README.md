<div style="display: inline_block"><br/>
    <img alt="Imgem" src="https://user-images.githubusercontent.com/60360540/186227538-7f8d75c9-88db-4486-b3dd-b2c375918767.png" width="250px" />
    <img align="right" alt="Imagem" src="https://user-images.githubusercontent.com/60360540/186230759-32dc5c33-e211-4922-a6a2-5c6b1cbf3781.png" width="250px" />
</div><br/>


# Sobre o projeto 
<p>
    Preparando aula de Git e GitHub para a matéria de Desenvolvimento de Aplicações para Web II. (Aula prevista para o dia 25/ago/2022).
</p><br>

<div style="display: inline_block"><br/>
    <img align="center" alt="GIT" src="https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white" />
    <img align="center" alt="GitHub" src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white" />
    <img align="center" alt="Markdown" src="https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white" />
</div><br/>

---
## Instalação do Git no Linux
### Siga estas etapas (dentro de um terminal):
1. download do git:
    ```shell
    $ sudo apt-get install git-all
    ```

---
## Gerar chave SSH

1. Criar uma chave SSH:

    ```shell
    $ ssh-keygen -t ed25519 -C "your_email@example.com"
    ```

#### Colocar chave SSH no GitHub

1. Entrar na pasta SSH:

    ```shell
    $ cd ~/.ssh/
    ```

2. Mostra a chave no terminal (copie essa chave):

    ```shell
    $ cat id_rsa.pub
    ```

3. No Site do GitHub:

    ```shell
    Perfil > settings > (no menu) SSH and GPG Keys > New SSH Key > Coloque o título e a chave ssh.
    ```

---

## Envie seu projeto para o GitHub

1. Criar a pasta do projeto:

    ```shell
    $ mkdir projeto
    ```

2. Entrando na pasta do projeto:

    ```shell
    $ cd projeto
    ```

3. Iniciar o Git na pasta:

    ```shell
    $ git init
    ```

4. Configurando o usuário:
* Inseri o usuário
* Inseri o email

    ```shell
    $ git config user.name "usuário"
    $ git config user.email "email@email.com"
    ```

5. Adicionando arquivos:

    ```shell
    $ git add .
    ```

6. Status do projeto:

    ```shell
    $ git status
    ```

7. Cria a branch principal:

    ```shell
    $ git branch "main"
    ```

8. Entra na branch principal:

    ```shell
    $ git checkout main
    ```

9. Entra na branch principal:

    ```shell
    $ git remote add origin <Link_do_projeto>
    ```

10. Checkpoint do seu projeto:

    ```shell
    $ git commit -m "Commit inicial"
    ```
11. Envia o branch principal:

    ```shell
    $ git push origin main
    ```

---
## Estilizando o terminal para produtividade

#### ZSH

1. Download zsh:
    <ul type="square">
        <li><a href="https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH">ZSH</a></li>
    </ul>

    ```shell
    $ sudo apt install zsh
    ```

2. Download Oh My ZSH:
    <ul type="square">
        <li><a href="https://github.com/ohmyzsh/ohmyzsh">Oh My ZSH</a></li>
    </ul>

    ```shell
    $ sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    ```

3. Editar o arquivo:

    ```shell
    $ gedit .zshrc
    ```

4. Coloque o nome do tema na variável de ambiente:

    ```shell
    $ ZSH_THEME="robbyrussell"
    ```

5. Temas do Oh My ZSH:
    <ul type="square">
        <li><a href="https://github.com/ohmyzsh/ohmyzsh/wiki/Themes">Oh My ZSH</a></li>
    </ul><br>

#### ZInit

1. Download ZInit:
    <ul type="square">
        <li><a href="https://github.com/zdharma-continuum/zinit#install">ZInit</a></li>
    </ul>

    ```shell
    $ sudo apt install zsh
    ```

2. Download Oh My ZSH:

    ```shell
    $ bash -c "$(curl --fail --show-error --silent --location https://raw.githubusercontent.com/zdharma-continuum/zinit/HEAD/scripts/install.sh)"
    ```

3. Editar o arquivo:

    ```shell
    $ gedit .zshrc
    ```

4. Coloque os puglins na última linha do arquivo:
* 1º. Plugin que deixa em evidência no terminal.
* 2º. Plugin de sugestões.
* 3º. autocomplete (npm, yarn) .

    ```shell
    zinit light zdharma/fast-syntax-highlighting
    zinit light zsh-users/zsh-autosuggestions
    zinit light zsh-users/zsh-completions
    ```

---
## Autor

| [<img src="https://user-images.githubusercontent.com/60360540/186234612-f71248a4-79ba-4e59-b162-0b948d9a97dc.jpeg" width=115><br><sub>@felipe-fe</sub>](https://www.linkedin.com/in/felipe-fe/) |
| :---: |