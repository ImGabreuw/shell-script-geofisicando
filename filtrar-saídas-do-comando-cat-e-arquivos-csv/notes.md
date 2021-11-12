# Filtrar saídas do comando cat e arquivos csv

### Comando `cut`

* **Função**: cortar caracteres de uma String

* **Flags**

  * `-c`

    * **Função**: especificar o caractere a ser cortado da String

    * **Sintaxe**: `$ <...> | cut -c<posição do caractere, começa em 1>`

    * **Exemplo**

      * `$ echo "Dirack" | cut -c1`

        * **Saída**: `D`

      * `$ echo "Dirack" | cut -c2`

        * **Saída**: `i`

      * `$ echo "Dirack" | cut -c2-3`

        * **Saída**: `ira`

  * `-d`

    * **Função**: especificar um caractere delimitador para cortar a String

    * **Sintaxe**: `$ <...> | cut -d"<caractere>"`

    * **Exemplo**

      ```shell
      $ echo -e "1,2,3\n4,5,6\n7,8,9" >> matriz.csv && `$ cat matriz.csv | cut -d","`
      ```

  * `-f`

    * **Função**: separar colunas de um arquivo csv

    * **Sintaxe**
    
      * `$ <...> | cut -d"," -f<coluna>`

      * `$ <...> | cut -d"," -f<começo do intervalo>-<fim do intervalo>`

    * **Exemplo**

      ```shell
      $ echo -e "1,2,3\n4,5,6\n7,8,9" >> matriz.csv && `$ cat matriz.csv | cut -d","` -f1
      ```

      * **Saída**

        ```
        1
        4
        7
        ```