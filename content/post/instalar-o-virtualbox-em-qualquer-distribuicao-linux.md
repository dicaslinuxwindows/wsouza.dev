---
title: 'Instalando o VirtualBox em qualquer distribuição Linux'
date: 2021-01-25T23:13:00.008-03:00
draft: false
url: /2021/01/instalar-o-virtualbox-em-qualquer-distribuicao-linux.html
tags: 
- Linux
- VirtualBox
- Máquina Virtual
- Tutoriais
---

![Instalando o VirtualBox em qualquer distribuição Linux - Dicas Linux e Windows](https://1.bp.blogspot.com/--09lJ3LkXgE/YA93oXVBAVI/AAAAAAAARmo/9K1YfOF6ybIimoPzMaAy2iRQMbZWK22CACNcBGAsYHQ/s16000/Virtualbox_Linux.png "Instalando o VirtualBox em qualquer distribuição Linux - Dicas Linux e Windows")

Se você têm encontrado dificuldades para instalar o VirtualBox em sua distribuição linux, veja aqui como instalá-lo sem se preocupar com as dependências de bibliotecas recentes.

  
  
  
  
  
  

### VirtualBox

  
VirtualBox _(VB)_ é um software gratuito _(e de código aberto)_ de virtualização, muitas vezes chamado de máquina virtual. Como citei na [matéria que fiz em 2018, quando falei do "concorrente do VB", o VMware](https://info.wsouza.com.br/2018/07/maquina-virtual-instalando-e-configurando-o-wmware-player.html), o conceito de de máquina virtual é:  

> _"O conceito de máquina virtual (VM) é um software que emula as funções de um computador, permitindo que outro (s) SO (s) (convidado) sejam instalados dentro de um SO hospedeiro..."_

  
O VB está presente nos repositórios de diversas distribuições Linux, mas pode ser executado em outras em que não está no repositório oficial, além de Windows, Macintosh e Solaris. Dentre os sistemas operacionais que podem ser instalados utilizando o VB _(sistemas convidados)_ estão: Windows (NT 4.0, 2000, XP, Server 2003, Vista, Windows 7, Windows 8, Windows 10 ), DOS / Windows 3.x, Linux (2.4, 2.6, 3.x, 4.x e 5.x), Solaris e OpenSolaris, OS / 2 e OpenBSD.  
  

### Entendendo o problema

  
Recentemente atualizei meu S.O. do Debian Buster para o Debian Bullseye. Não lembro ao certo se meu VB parou de funcionar, ou se desinstalei por algum motivo. Fato é, que ao tentar instalar o VB novamente não consegui, pois acusava erro de dependências. O VB não está nos repositórios oficiais do Debian. No site do VB existe um pacote para Debian Buster e, mesmo utilizando o Bullseye, tentei utilizá-lo - pois é o mais recente disponível por lá - e não deu certo.  
A solução encontrada está na mesma página de download, um pouco mais abaixo. Trata-se da opção _All distributions_ _(Veja na imagem abaixo)_, que funciona em todas as distribuições e não depende de bibliotecas mais recentes. Esta versão do VB foi construída num sistema equivalente ao Red Hat Enterprise Linux 6.x _(que atualmente está na versão 6 ELS +, com suporte extendido)_.  

[![Instalando o VirtualBox em qualquer distribuição Linux - Dicas Linux e Windows](https://1.bp.blogspot.com/-csecsHTxx9g/YA9ovYqD_GI/AAAAAAAARmU/V5T66hytQ-EiZBQ8W1G1w3vYi9nTbs-DgCNcBGAsYHQ/w400-h281/VB01.png "Instalando o VirtualBox em qualquer distribuição Linux - Dicas Linux e Windows")](https://1.bp.blogspot.com/-csecsHTxx9g/YA9ovYqD_GI/AAAAAAAARmU/V5T66hytQ-EiZBQ8W1G1w3vYi9nTbs-DgCNcBGAsYHQ/s612/VB01.png)

### Download e instalação

  

#### Pela interface gráfica:

  
Acesse: [https://www.virtualbox.org/wiki/Linux\_Downloads](https://www.virtualbox.org/wiki/Linux_Downloads), clique com o botão direito e depois em _"Salvar link como"_ e será salvo um arquivo com a extensão _**.run**_. Após, acesse a pasta onde baixou, clique com o botão direito, depois Propriedades, Permissões e marque a opção Permitir a execução como um programa _(ou algo equivalente)_.  
  

#### Pelo terminal:

  
O link abaixo é para a versão 6.1.18, que pode ser atualizado a qualquer momento.  
  

  

  

 wget https://download.virtualbox.org/virtualbox/6.1.18/VirtualBox-6.1.18-142142-Linux\_amd64.run

  
Após, dê a permissão de execução.  
  

  

  

 chmode +x VirtualBox-6.1.18-142142-Linux\_amd64.run

  

#### Instalação

  
Faça a instalação pelo terminal, independente se baixou pela interface gráfica, ou pelo terminal. Desta forma a chance de acontecer erros é bem menor.  
  

  

  

 sudo ./VirtualBox-6.1.18-142142-Linux\_amd64.run

  

### Pós-instalação

  
Para utilizar todo o potencial do VB, após a instalação baixe VirtualBox Extension Pack, disponível em [https://www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads). Após instalar algum sistema operacional convidado em seu VB - e se este for baseado no Debian - execute os comandos mostrados abaixo no terminal e depois, com o sistema convidado aberto, vá ao menu do VB _Dispositivos_ e escolha a opção _Inserir imagem de Cd para os Adicionais para Convidado_.  
  

  

  

 sudo apt update

  

  

  

 sudo apt install -y build-essential module-assistant

  

  

  

 sudo m-a prepare