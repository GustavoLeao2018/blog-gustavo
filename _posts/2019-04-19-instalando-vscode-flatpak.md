---
layout: post
title: "Instalando o Visual Studio Code no Linux com o Flatpak"
date: 2019-04-19 15:48:49 -03000
categories: install vscode visual studio code
---

# Instalando o Visual Studio Code no Linux com o Flatpak

Com essa nova ferramenta chamada flatpak, que instala o programa e suas dependências diretamente, e caso excluidas não irão alterar outros programas que as utilizam, podemos instalar várias ferramentas com apenas um comando, que é o seguinte:

```bash
$ sudo flatpak install repositório nome do pacote
```

Substituiremos, portantanto o repositório   que é o `flathub`, e o pacote para `com.visualstudio.code`, ficando:

```bash
$ sudo flatpak install flathub  com.visualstudio.code
```

## O que é visual studio code?

Visual studio code, ou VSCode, é um editor multiplataforma, utilizado na criação de programas e sites.

A interface gráfica do programa tende a ser assim:
![Tela de exemplo Visual Studio Code](/assets/tela-vscode.png)


A principal diferença, e seu maior forte,  que por ser um editor, e não uma IDE, possui muitas extenções, temas, pacotes e configurações para se adequar a quais quer linguagem.

