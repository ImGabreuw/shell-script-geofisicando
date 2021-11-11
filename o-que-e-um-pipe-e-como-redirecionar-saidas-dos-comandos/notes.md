# O que é um Pipe? Como redirecionar saídas dos comandos?

### Barra (`/`) e barra invertida (`\`)

* Barra (`/`): separador de diretórios

  * **Exemplo**: `/home/user`

* Barra invertida (`\`): quebrar linha de um comando muito extenso

  * **Exemplo**

    ```shell
    $ echo "Olá" \
      "Tudo bem?"
    ```

### Pipe (`|`)

* **Função**: direcionar a saída de um comando para a entrada de outro comando

* **Exemplo**: `$ echo "2+1" | bc -l`

  > **OBS**: `bc` é o atalho, via terminal, para a calculadora

  * **Saída**: `3`

### Redirecionamento para arquivos: `>>`, `>` e `<`

* `>>`

  * **Função**: direcionar a saída de um comando para a última linha de um arquivo (caso o arquivo não exista o mesmo será criado)

  * **Exemplo**: `$ echo "Última linha" >> arquivo.txt`

    * `Arquivo.txt` antes do comando

      ```
      Linha 1
      Linha 2
      ```

    * `Arquivo.txt` depois do comando

      ```
      Linha 1
      Linha 2
      Última linha
      ```

* `>`

  * **Função**: direcionar a saída de um comando para um arquivo, substituindo o conteúdo existente (caso o arquivo não exista o mesmo será criado)

  * **Exemplo**: `$ echo "Última linha" >> arquivo.txt`

    * `Arquivo.txt` antes do comando

      ```
      Linha 1
      Linha 2
      ```

    * `Arquivo.txt` depois do comando

      ```
      Última linha
      ```

* `<`

  * **Função**: direcionar um arquivo como entrada de um comando/programa

  * **Exemplo**

    * `arquivo_1.txt`

      ```
      Linha 1
      Linha 2
      ```

    * `$ cat < arquivo_1.txt > arquivo_2.txt`

      * **Saída**

        ```
        Linha 1
        Linha 2
        ```

    * `arquivo_2.txt`

      ```
      Linha 1
      Linha 2
      ```