---
title: 'Debian Buster está chegando'
date: 2019-06-25T00:05:00.000-03:00
draft: false
url: /2019/06/debian-buster-esta-chegando.html
tags: 
- Debian
- Linux
- Debian Buster
---

A data de lançamento do Debian 10, codinome Buster, está se aproximando. Veja na matéria a seguir quais são as novidades que virão com ele.

  
  
  

[![Debian Buster está chegando - Dicas Linux e Windows](https://2.bp.blogspot.com/-W6q1uBHLrC0/XRFymgT2FRI/AAAAAAAALs0/ZfkIRuGJG2c1fGnUw7JJO99tgnnG-8LoQCLcBGAs/s1600/Buster.png "Debian Buster está chegando - Dicas Linux e Windows")](https://2.bp.blogspot.com/-W6q1uBHLrC0/XRFymgT2FRI/AAAAAAAALs0/ZfkIRuGJG2c1fGnUw7JJO99tgnnG-8LoQCLcBGAs/s1600/Buster.png)

  

### Debian

Debian é um sistema operacional que contém softwares livres e, atualmente a versão estável é a 9, de codinome Stretch, lançada em 17 de Junho de 2017. Mais informações sobre o Debian em [Debian - Curiosidades, informações, versões e ciclo de vida.](https://info.wsouza.com.br/2019/07/debian-curiosidades-informacoes-suas-versoes-e-ciclo-de-vida.html)  
  

### Buster

O Debian Buster será a próxima versão estável, sendo substituto do Debian Stretch. Ainda não há uma data definida para ser lançada, porém, ao que tudo indica será lançado no mês de julho. Os desenvolvedores do Debian não estipulam datas para os lançamentos, o Debian só é lançado quando está pronto, mesmo que demorem vários anos entre um lançamento e outro. Segundo o [Release-critical bugs stats](https://bugs.debian.org/release-critical/) _(página que divulga detalhes de desenvolvimento)_ na data em que esta matéria foi publicada, o Debian está com 83 bugs que deverão ser resolvidos até o lançamento .  A nível de comparação, a versão anterior foi lançada com 37 bugs.  
  

### O que vem de novidades?

O Debian Buster virá com algumas novidades em relação à versão anterior. Segue uma lista com algumas delas:  

*   Virá com o Gnome 3.30.0, que está com grandes melhorias em relação ao alto consumo de memória RAM.
*   Na interface padrão _(Gnome)_ o servidor gráfico Wayland¹ vem por padrão no lugar servidor gráfico Xorg.
*   O antigo instalador foi substituído pelo instalador Calamares².
*   A senha de root² não será mais definida na instalação, podendo ser definida após a instalação.
*   Assim como ocorre no Ubuntu, o Sudo será instalado por padrão para seu usuário.
*   Além das imagens de instalação normais, haverá uma ISO com a interface LXQT.
*   O gerenciador de pacotes Synaptic⁴ não está disponível na versão Gnome por motivos de incompatibilidade com o Wayland.
*   Suporte ao Secure Boot.
*   A provável versão do Kernel será a 4.19.

### Notas

¹ O Wayland vem causando problemas nos programas quando executados como root. Para fugir destes problemas, no momento do login escolha o servidor gráfico Xorg.  
² Pelos testes que realizei o instalador Calamares está disponível apenas no Live CD/DVD. Quando utiliza-se uma imagem netinst o instalador será o antigo instalador debian.  
³ Se a instalação ocorrer pelo instalador debian aparecerá a opção de digitar a senha de root. Caso não a digite, seu usuário será habilitado como sudo e o su será desativado.  
⁴ É possível instalar o Synaptic e executá-lo normalmente, desde que faça login utilizando o servidor gráfico Xorg.  
  

### Instalação

O vídeo abaixo mostra a instalação do RC1 do Buster pelo Live CD com o instalador Calamares.