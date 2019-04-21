---
layout: post
title: "Instalando o Ruby no Linux Mint/Ubuntu e derivados"
date: 2019-04-19 16:01:49 -03000
categories: install vscode ruby jekyll gem bundler
---
# Instalando o Ruby no Linux Mint/Ubuntu e derivados

O **Ruby** é uma linguagem de programação utilizada para criar programas (e sua versão **Ruby on rails**, que é voltada para desenvolvimento web).

Para instalar ela no linux Mint/Ubuntu e derivados, execute o seguinte passo a passo:

## Instalando o ruby 
Digite o seguinte comando para instalar:

```bash
$ sudo apt-get install ruby-full build-essential zlib1g-dev -y
```

E este para adicionar configurações ao .bashrc:

```bash
$ echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
$ echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
$ echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
$ source ~/.bashrc
```

## Instalando o Jekyll e o Bundler

Estes dois programas são utilizados para criar um blog com **ruby**, **markdown**, **sass**, **css** e **html**.

Execute: 

```bash
$ gem install jekyll bundler
```