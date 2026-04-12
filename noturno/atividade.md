# Atividade Prática

## Orientações

- Execute os comandos com atenção.
- Leia o resultado de cada comando antes de continuar.

## Tarefa I

Crie uma pasta chamada "oficina-linux" na sua pasta pessoal, com três subpastas:
- "anotações"
- "scripts"
- "testes"

1. Entre na pasta "oficina-linux"
2. Liste o conteúdo dela
3. Descubra em que diretório você está

Comandos:
- mkdir
- cd
- ls
- pwd

Responda:
- O que `mkdir` faz?
- O que a opção `-p` faz?
- O que as chaves `{}` fazem no mkdir?
- O que `pwd` mostra?

## Tarefa II

Dentro da pasta `anotações`, crie os arquivos:
- `aula.txt`
- `duvidas.txt`
- `comandos.txt`

1. Escreva uma frase dentro de aula.txt
2. Mostre o conteúdo do arquivo no terminal
3. Copie `aula.txt` para a pasta `testes`
4. renomeia a copia para copia aula 1

Comandos:
- echo
- cat
- cp
- mv

Responda:
- Qual é a diferença entre `touch`, `echo`, `cp`, e `mv`?
- O que `>` faz?
- O que aconteceu com o arquivo copiado?

## Tarefa III

Acesse a pasta `scripts` e:
1. Liste o conteúdo da pasta `anotações` usando caminho relativo
2. Mostre o conteúdo de `aula1.txt` usando caminho relativo
3. Mostre o mesmo conteúdo usando caminho absoluto

Comandos:
- cd
- ls
- cat

Responda:
- Qual é a diferença entre caminho absoluto e relativo?
- O que `..` significa?
- Por que `/home/...` e `home/...` não são a mesma coisa?

## Tarefa IV

Crie um arquivo chamado `saudacao.sh` dentro da pasta `scripts`.

Conteúdo do script:
```bash
#!/bin/bash
echo "olá!"
echo "usuário atual: $(whoami)"
echo "diretório atual: $(pwd)"
echo "data e hora: $(date)"
```

1. Salve o arquivo
2. Tente executá-lo
3. Observe o que acontece
4. Dê permissão de execução
5. Execute novamente

Comandos:
- chmod +x

Responda:
- O que é um script?
- Para que serve a linha `#!/bin/bash`?
- Por que o script não executa sem permissão adequada?
- O que `chmod +x` faz?

## Tarefa V

1. Descubra qual é seu usuário atual
2. Veja os grupos dos quais você faz parte
3. Liste as permissões do script criado
4. Crie um arquivo chamado `segredo.txt`
5. Dê permissão do arquivo apenas para o dono

Comandos:
- whoami
- id
- groups
- ls -l
- touch
- chmod 600
- ls -l

Responda:
- O que significa `600`?
- Quem pode ler ou alterar esse arquivo agora?
- Qual é a diferença entre permissões de leitura, escrita e execução?

## Tarefa VI

Tente listar o conteúdo do diretório `/root` sem `sudo` e depois com `sudo`.

Comandos:
- ls
- sudo ls

Responda:
- O que aconteceu sem `sudo`?
- O que mudou com `sudo`?
- O `sudo` te transforma em root permanentemente?

## Tarefa VII

1. Inicie um processo simples com `sleep`
2. Encontre esse processo
3. Encerre o processo

Comandos:
- sleep 300
- ps aux | grep sleep
- kill

Responda:
- O que é um processo?
- Qual é a diferença entre programa e processo?
- O que o comando `kill` faz?

## Tarefa VIII

1. Atualize a lista de pacotes
2. Pesquise o pacote `tree`
3. Instale o `tree`
4. Use o `tree` para mostrar a estrutura da pasta `oficina-linux`

Comandos:
- sudo apt update
- apt search tree
- sudo apt install tree
- tree

Responda:
- O que é um gerenciador de pacotes?
- O que é um pacote?
- O que `apt update` faz?
- O que `tree` mostrou sobre sua estrutura de diretórios?