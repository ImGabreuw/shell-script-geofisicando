# Basename e dirname

### Comando `basename` ou `dirname`

* **Função**: obter o nome do arquivo

* **Sintaxe**: `$ basename <caminho do arquivo>`

* **Exemplo**: `$ ARQUIVO="/home/gabriel/arquivo.txt" && basename $ARQUIVO`

  * **Saída**: `arquivo.txt`

* **Sufixo (extensão)**

  * **Função**: ignorar a extensão do arquivo ao imprimir da tela do terminal

  * **Sintaxe**: `$ basename <caminho do arquivo> <extensão do arquivo>`

  * **Exemplo**: `$ ARQUIVO="/home/gabriel/arquivo.txt" && basename $ARQUIVO .txt`

    * **Saída**: `arquivo`