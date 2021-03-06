# Alterar permissões de arquivos no linux

### Comando `ls`

* **Função**: listagem de arquivos e diretórios

* **Sintaxe**: `$ ls`

* **Exemplo**: `$ ls`

* **Flags**

  * `-l`

    * **Função**: listagem, no formato longa, com informações mais detalhadas sobre arquivos e diretórios

    * **Sintaxe**: `$ ls -l`

    * **Exemplo**

      ![](./assets/exemplo-ls-flag-l.png)

      * Informações exibidas na listagem

        String de permissão | Proprietário | Grupo | Tamanho do arquivo | Mês/Data/hora de criação | Nome do diretório/arquivo
        :-----------------: | :-----: | :---: | :----------------: | :----------------------: | :-----------------------:
        tipo do arquivo
        permissão de leitura (`r` = *read*)
        permissão de escrita (`w` = *write*)
        permissão de execução (`x` = *execution*)

      * String de permissão

        * 1º caractere = tipo do arquivo (`d` = diretório / `-` = arquivo comum / `l` = link)

        * 2º ao 4º caractere = permissões (`rwx`) para o usuário/Proprietário

          > **OBS**: `-` (traço) representa que aquele grupo/usuário não possui essa permissão

        * 5º ao 7º caractere = permissões (`rwx`) para um grupo de vários usuários

          > **OBS**: é possível compartilhar arquivos entre os usuários do mesmo grupo por meio da rede

        * 8º ao 10º caractere = permissões (`rwx`) para os outros usuários

### Comando `chmod`

* **Função**: alterar as permissões de um arquivo

* **Sintaxe**: `$ chmod <alvo da alteração>=<permissões (rwx)>`

* **Exemplo**

  * `$ chmod u=rwx script.sh`

    * `u` (*user*) = alterar a permissão de usuário

    * `rwx` = adicionar as permissões de leitura, escrita e execução

  * `$ chmod u=x script.sh`

    * `u` = alterar a permissão de usuário

    * `x` = adicionar apenas a permissão de execução

  * `$ chmod g=rw script.sh`

    * `g` (*group*) = alterar a permissão de grupo

    * `rw` = adicionar as permissões de leitura e escrita

  * `$ chmod o=rw script.sh`

    * `o` (*others*) = alterar a permissão de outros usuários

    * `rw` = adicionar as permissões de leitura e escrita
