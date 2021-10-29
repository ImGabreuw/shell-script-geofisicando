# O que é shell? O que é shell script?

### Shell

> Comando `$ echo $SHELL`: imprime na tela o caminho até o binário do *shell* (Exemplo: `/bin/bash`)

* **Definição**: é um software responsável por validar um comando, transformá-lo em linguagem de máquina e por fim o executar via uma comunicação entre o *sistema operacional* e *shell* (no caso do Linux, o *Kernel*)

* Existem vários tipos de *shell*, um exemplo é o **bash** (utilizado no Ubuntu)

### Shell Script

* É uma linguagem de programação utilizado no *shell*

* Os comandos `ls` / `cd` / `pwd` são algumas instruções dessa linguagem

* Estrutura de um *shell script*

  * Cabeçalho (1º linha do arquivo)

    > Também conhecido de **shebang**
  
    * **Função**: especificar o *shell* responsável por interpretar o *shell script*

    * **Sintaxe**: `#!<tipo do shell>`

    * **Exemplo**

      ```shell
      #!/bin/bash

      ...
      comandos
      ...
      ```

* Cometário: `# comentário no shell script`