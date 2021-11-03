# Criar arquivos em branco e arquivos ocultos

### Comando `touch`

* **Função**: criar arquivos em branco ou ocultos

  > Arquivos ocultos são arquivos iniciados com `.` (Exemplo: `.oculto.txt`)

* **Sintaxe**

  * Criar arquivo em branco: `$ touch <nome do arquivo>`

  * Criar arquivo oculto: `$ touch .<nome do arquivo>`

* **Exemplo**

  * `$ touch .oculto.txt`

  * `$ touch arquivo.txt`

### OBS

* Abrir o gerenciador de arquivo via terminal
  
  * **Sintaxe**: `$ nautilus <diretório> &`

    > A opção `&` tem a função de não travar o terminal enquanto esse comando estiver em execução

  * **Exemplo**: `$ nautilus . &`

* Atalho `CTRL + H`

  * **Função**: habilitar/desabilitar a exibição de arquivos ocultos