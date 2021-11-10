# Remover arquivos e diretórios

### Comando `rm`

* **IMPORTANTE**: esse comando exclui os arquivos/diretórios permanentemente (não fica na lixeira)

* **Função**: remover arquivos

* **Sintaxe**: `$ rm <arquivo>`

* **Flags**

  * `-R` ou `-r`

    * **Função**: remover diretórios **com conteúdo**

    * **Sintaxe**: `$ rm -r <diretório>`

    * **Exemplo**: `$ rm -r teste/`

  * `-i`

    * **Função**: exibir uma mensagem para confirmar a remoção de um arquivo/diretório

    * **Sintaxe**: `$ rm -i <diretório>`

    * **Exemplo**: `$ rm -i teste/*`

      > `*`: selecionar todo o conteúdo dentro do diretório `teste/`

      * `$ y` (*yes*): para confirmar

      * `$ n` (*no*): para cancelar

### Comando `rmdir`

* **Função**: remover diretórios **vazios**

* **Sintaxe**: `$ rmdir <diretório>`

* **Exemplo**: `$ rmdir teste/`