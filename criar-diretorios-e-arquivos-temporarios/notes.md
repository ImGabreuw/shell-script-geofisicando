# Criar diretórios e arquivos temporários

### Comando `mktemp`

* **Função**: gerar arquivos temporários

  > **OBS**: por padrão, os arquivos temporários são criados no diretório `/tmp`

* **Sintaxe**: `$ mktemp`

* **Exemplo**: `$ mktemp`

  * **Saída**: `/tmp/tmp.BWG6KksEw4` 

    > `BWG6KksEw4`: é a extensão alfa numérica de arquivos temporários

* **Opções**

  * Criar um arquivo temporário em um determinado diretório

    * **Sintaxe**: `$ mktemp ./tmp.XXXX`

      > `XXXX`: é um *placeholder*, ou seja, apenas para representar a extensão alfa numérica desse tipo de arquivo

    * **Exemplo**: `$ mktemp ./tmp.XXXX`

      * **Saída**: `./tmp.V066`

### Comando `mkdir`

* **Função**: gerar diretórios

* **Sintaxe**: `$ mkdir <nome do diretório>`

* **Exemplo**: `$ mkdir teste`

* **Flags**

  * `-p`

    * **Função**: gerar múltiplos diretórios, ou seja, gerar 1 diretório dentro do outro

    * **Sintaxe**: `$ mkdir -p ./teste/teste2/teste3`