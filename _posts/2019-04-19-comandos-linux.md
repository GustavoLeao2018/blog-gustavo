---
title: Comandos Linux Básicos
layout: post
date: '2019-04-19 18:30:00'
categories: linux, shell, shellscript, script, bash, comandos, commands
---

# Comandos Básicos do Linux

## Mostrando algo na tela
Para mostrar algo na tela, como uma informação, vamos usar o comando `echo`, como abaixo:

```bash
$ echo "Hello, Cruel World!"
```

Este comando é muito util para sabermos o valor que está dentro de uma variável, como as que ja existem no sistema. 

Veja por, exemplo, a variável que  mostra a linguagem do sistema:

```bash
$ echo $LANGUAGE
```

## Lendo do teclado
Podemos, também, ler do teclado e salvar em uma variável o valor digitado, como abaixo:

```bash
$ read nome_da_variavel
$ echo $nome_da_variavel
```

Um atributo, que nada mais é do que um texto que podemos adicionar que segue a regra de `--nome_do_atributo` ou `-atributo_simplificado`.

Por exemplo, caso queremos saber como funciona determinado comando podemos colocar o atributo `--help` ou `-h` , veja:

```bash
$ apt -h
$ apt --help
```

Para o comando read podemos colocar o atributo para colocar um texto antes da variável:

```bash
$ read -p "Digite seu nome: " nome
$ echo "Prazer $nome, seja bem-vindo!"
```

## Diretórios
### Saber qual diretório estamos 
Para sabermos em qual diretório estamos digitamos o seguinte comando:

```bash
$ pwd
```

### Ir para o algum diretório
Para irmos para um determinado caminho podemos colocar o comando `cd` com o `caminho_do_diretorio/separado_por_barra`.

Por exemplo, se estivermos no diretório home do usuário, podemos ir para os documentos:

```bash
$ cd Documentos/
```

Ou podemos voltar uma pasta acima, ou seja, o diretório pai do em que estamos:

```bash
$ cd ..
```

Podemos, também voltar para o anterior, utilizando o como abaixo:

```bash
$ cd -
```

### Listando o conteúdo de um diretório
Assim como podemos ver em qual diretório estamos, podemos ver o conteúdo do mesmo, veja:

```bash
$ ls
```

### Criando um diretório
Criando um diretório é facil, basta apenas digitar:

```bash
$ mkdir nome_do_diretorio
```

## Arquivos
### Criando um arquivo
Para criar um arquivo, podemos executar o comando:

```bash
$ touch README.md
```

### Editando um arquivo
Podemos editar com algum editor em modo texto, como `nano`, `vi` ou `vim`. 

>  Eu recomento como o que mais utilizo, por ser também mais simples e geralmente vir com o sistema o `nano`.

Vamos executar o editor, e como atributo o nome do arquivo:
```bash
$ nano README.md
```

### Lendo um arquivo
Podemos ler o conteúdo do arquivo com o comando:

```bash
$ cat README.md
```

### Inserindo em um arquivo
Podemos, diretamente, inserir algum texto diretamente em um arquivo, no formato:

```bash
$ echo "# Leia-me " >> README.md
```

## Sistema
### Uso de memória e processamento
Para sabermos quanto de memória e processamento estamos usando, para isso utilize:

```bash
$ top
```

### Uso de disco
Para sabermos quanto de disco estamos usando e não estamos usando digite:

```bash
$ df
```

## Remover
Para remover um arquivo ou diretório, basta apenas digitar:

```bash
$ rm -R nome_do_diretorio
```

Ou:
```bash
$ rm nome_do_diretorio
```

E para remover tudo dentro de um diretório, coloque:

```bash
$ rm *
```
