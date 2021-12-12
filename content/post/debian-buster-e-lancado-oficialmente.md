---
title: 'Debian Buster é lançado oficialmente'
date: 2019-07-06T23:13:00.002-03:00
draft: false
url: /2019/07/debian-buster-e-lancado-oficialmente.html
tags: 
- Debian
- Linux
- Debian Buster
---

[![Debian Buster é lançado oficialmente - Dicas Linux e Windows](https://1.bp.blogspot.com/-zYN54Qok9BY/XSFTWcSsEPI/AAAAAAAALzQ/RZTornaz-ecWuhI1lnR8KUh7AH0M5D5ywCLcBGAs/s200/blog-banner.png "Debian Buster é lançado oficialmente - Dicas Linux e Windows")](https://1.bp.blogspot.com/-zYN54Qok9BY/XSFTWcSsEPI/AAAAAAAALzQ/RZTornaz-ecWuhI1lnR8KUh7AH0M5D5ywCLcBGAs/s1600/blog-banner.png)

O Debian Buster enfim está entre nós em sua versão final.  
Saiba aqui os detalhes do lançamento.

  
  
  
  
  
  
  

### Debian

  
Debian é um sistema operacional que contém softwares livres. Até o dia 06/07/2019 a versão estável era a versão 9, chamada Stretch  e lançada em 2017. Após dois anos é lançada a versão 10, de codinome Buster (_cachorro do  Andy, do filme Toy Story)_, que passa a ser a versão estável.  
Para entender como funciona, e para mais informações sobre o Debian leia: [Debian - Curiosidades, informações, versões e ciclo de vida](https://info.wsouza.com.br/2019/07/debian-curiosidades-informacoes-suas-versoes-e-ciclo-de-vida.html)  
  

### Novidades e notas de lançamento

  
Conforme adiantado em matérias anteriores, O Debian Buster vem com algumas diferença em relação à seu antecessor. Algumas diferenças são naturais, relativas à atualizações de pacotes. Já outras são um pouco mais, digamos, radicais se comparado com a maneira que o Debian é trabalhado. Veja alguns exemplos:  

*   Uma das atualizações que considero "mais radicais" é a não habilitação do usuário root _(su)_ por padrão e habilitação do sudo na instalação. O Ubuntu, por exemplo, faz isto há bastante tempo. 
*   A preferência pelo servidor gráfico Wayland no lugar o Xorg também é uma destas mudanças que considero um pouco mais radicais, pois o Wayland ainda tem algumas incompatibilidades.

Dentre as novidades há também aquelas que continuam seguindo o padrão Debian. Um exemplo é o Kernel adotado. O Kernel 5 foi lançado em abril e, por exemplo, já foi adotado no Ubuntu 19.04. O Debian Buster é lançado com a versão 4.19 _(4.19.0-5)_, mas é certo que futuramente será atualizado para o 5.  
A troca do instalador padrão pelo instalador Calamares é algo que considero como mais um ponto positivo, pois trata-se de um instalador prático, intuitivo e moderno. Vale destacar que o Calamares será o instalador padrão quando a instalação ocorrer pelo modo Live _(quando estiver utilizando um Live CD//DVD)_. Quando a instalação ocorrer via um CD//DVD Netinst o instalador utilizado será o antigo instalador gráfico padrão,podendo ainda ser utilizado o instalador no modo texto.  
Outras novidades que chegam com o Buster:  

*   Novas versões para os softwares mais populares como Firefox, Chromium, GIMP, OpenJDK, Apache, LibreOfiice,
*   Além das imagens com as interfaces tradicionais, foi adicionada uma imagem com a interface LXQT, que é basicamente um LXDE construido com as bibliotecas QT. _(Veja [aqui](https://www.youtube.com/watch?v=koNy5wCBS2M) a instalação e visual da interface LXQT)_
*   Um total de 59.000 pacotes disponíveis, frente aos 51.000 da versão anterior.
*   Versões das interfaces gráficas: Cinnamon 3.8, GNOME 3.30, KDE Plasma 5.14, LXDE 0.99.2, LXQt 0.14, MATE 1.20, Xfce 4.12.
*   O suporte à Inicialização Segura está incluído nesta versão para as arquiteturas amd64, i386 e arm64
*   [AppArmor](https://debian-handbook.info/browse/pt-BR/stable/sect.apparmor.html), uma camada de segurança do sistema, vem ativada por padrão
*   Firewall NFtables em substituição ao iptables
*   Novo tema e novo papel de parede

  

#### Notas de Lançamento

  

*   No GNOME o servidor gráfico padrão é o Wayland em vez do Xorg. O Wayland tem um design mais simples e moderno, que tem vantagens para a segurança. O servidor de gráfico Xorg ainda é instalado por padrão e o gerenciador de exibição _(GDM, MDM LIGHTDM...)_ permite que os usuários escolham o Xorg como o servidor de exibição para a sessão.
*   Arquiteturas suportadas:  
    *   PC de 64 bits -Intel EM64T / x86-64 (amd64);
    *   PC de 32 bits / Intel IA-32 (i386);
    *   Motorola little-endian de 64 bits;
    *   IBM PowerPC (ppc64el);
    *   IBM S / 390 de 64 bits (s390x), para ARM, armel e armhf para hardware de 32 bits mais antigo e mais recente, além de arm64 para a arquitetura "AArch64" de 64 bits e para MIPS, mips (big-endian) e arquiteturas mipsel (little-endian) para hardware de 32 bits e arquitetura mips64el para hardware little-endian de 64 bits.
*   O Debian Stretch vai receber suporte da equipe de segurança durante 1 ano e depois se tornará LTS.
*   Se você quer experimentar o Buster sem instalá-lo, você pode usar uma das imagens Live que carregam e executam o sistema operacional completo em um estado somente leitura através da memória do seu computador. Tais imagens podem ser obtidas nos links logo abaixo.
*   [Leia aqui](https://www.debian.org/News/2019/20190706) as todas as notas de lançamento _(em inglês)_

  

### Download

  
Para obter o Debian Buster faça o download da imagem Live que mais lhe agrade nos links abaixo _(em 64 bits):_  
  

amd64

[ Gnome](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-10.5.0-amd64-gnome.iso)

[ Plasma](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-10.5.0-amd64-kde.iso)

[ XFCE](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-10.5.0-amd64-xfce.iso)

[ Mate](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-10.5.0-amd64-mate.iso)

[ LXDE](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-10.5.0-amd64-lxde.iso)

[ LXQT](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-10.5.0-amd64-lxqt.iso)

[ Cinnamon](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-10.5.0-amd64-cinnamon.iso)

[ Netinst](https://cdimage.debian.org/debian-cd/current/amd64/iso-cd/debian-10.5.0-amd64-netinst.iso)

i386

[ Gnome](https://cdimage.debian.org/debian-cd/current-live/i386/iso-hybrid/debian-live-10.5.0-i386-gnome.iso)

[ Plasma](https://cdimage.debian.org/debian-cd/current-live/i386/iso-hybrid/debian-live-10.5.0-i386-kde.iso)

[ XFCE](https://cdimage.debian.org/debian-cd/current-live/i386/iso-hybrid/debian-live-10.5.0-i386-xfce.iso)

[ Mate](https://cdimage.debian.org/debian-cd/current-live/i386/iso-hybrid/debian-live-10.5.0-i386-mate.iso)

[ LXDE](https://cdimage.debian.org/debian-cd/current-live/i386/iso-hybrid/debian-live-10.5.0-i386-lxde.iso)

[ LXQT](https://cdimage.debian.org/debian-cd/current-live/i386/iso-hybrid/debian-live-10.5.0-i386-lxqt.iso)

[ Cinnamon](https://cdimage.debian.org/debian-cd/current-live/i386/iso-hybrid/debian-live-10.5.0-i386-cinnamon.iso)

[ Netinst](https://cdimage.debian.org/debian-cd/current/i386/iso-cd/debian-10.5.0-i386-netinst.iso)

amd64 _(Torrent)_

[ Gnome](https://cdimage.debian.org/debian-cd/current-live/amd64/bt-hybrid/debian-live-10.5.0-amd64-gnome.iso.torrent)

[ Plasma](https://cdimage.debian.org/debian-cd/current-live/amd64/bt-hybrid/debian-live-10.5.0-amd64-kde.iso.torrent)

[ XFCE](https://cdimage.debian.org/debian-cd/current-live/amd64/bt-hybrid/debian-live-10.5.0-amd64-xfce.iso.torrent)

[ Mate](https://cdimage.debian.org/debian-cd/current-live/amd64/bt-hybrid/debian-live-10.5.0-amd64-mate.iso.torrent)

[ LXDE](https://cdimage.debian.org/debian-cd/current-live/amd64/bt-hybrid/debian-live-10.5.0-amd64-lxde.iso.torrent)

[ LXQT](https://cdimage.debian.org/debian-cd/current-live/amd64/bt-hybrid/debian-live-10.5.0-amd64-lxqt.iso.torrent)

[ Cinnamon](https://cdimage.debian.org/debian-cd/current-live/amd64/bt-hybrid/debian-live-10.5.0-amd64-cinnamon.iso.torrent)

[ Netinst](https://cdimage.debian.org/debian-cd/current-live/amd64/bt-hybrid/debian-live-10.5.0-amd64-standard.iso.torrent)

i386 _(Torrent)_

[ Gnome](https://cdimage.debian.org/debian-cd/current-live/i386/bt-hybrid/debian-live-10.5.0-i386-gnome.iso.torrent)

[ Plasma](https://cdimage.debian.org/debian-cd/current-live/i386/bt-hybrid/debian-live-10.5.0-i386-kde.iso.torrent)

[ XFCE](https://cdimage.debian.org/debian-cd/current-live/i386/bt-hybrid/debian-live-10.5.0-i386-xfce.iso.torrent)

[ Mate](https://cdimage.debian.org/debian-cd/current-live/i386/bt-hybrid/debian-live-10.5.0-i386-mate.iso.torrent)

[ LXDE](https://cdimage.debian.org/debian-cd/current-live/i386/bt-hybrid/debian-live-10.5.0-i386-lxde.iso.torrent)

[ LXQT](https://cdimage.debian.org/debian-cd/current-live/i386/bt-hybrid/debian-live-10.5.0-i386-lxqt.iso.torrent)

[ Cinnamon](https://cdimage.debian.org/debian-cd/current-live/i386/bt-hybrid/debian-live-10.5.0-i386-cinnamon.iso.torrent)

[ Netinst](https://cdimage.debian.org/debian-cd/current-live/i386/bt-hybrid/debian-live-10.5.0-i386-standard.iso.torrent)

  
Mais informações em [www.debian.org/distrib/](https://www.debian.org/distrib/).  
  

### Instalação

  
Veja algumas maneiras de instalar o Debian Buster em seu dispositivo:  

*   [Atualizando para o Debian Buster](https://info.wsouza.com.br/2019/07/atualizando-para-o-debian-buster.html)
*   [Instalação do zero (limpa)](https://info.wsouza.com.br/2019/07/debian-buster-instalacao-limpa.html)