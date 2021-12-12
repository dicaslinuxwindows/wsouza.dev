---
title: 'Lançado o Ubuntu 21.04 Hirsute Hippo'
date: 2021-04-25T23:03:00.003-03:00
draft: false
url: /2021/04/lancado-o-ubuntu-2104-hirsute-hippo.html
tags: 
- Linux
- Ubuntu
- Ubuntu 21.04
---

![//](https://1.bp.blogspot.com/-uIugK_p6nsg/YIYRoicxxQI/AAAAAAAASDA/qslFrua-uhA2g8UWobX9DnYxkgXcl1CrwCNcBGAsYHQ/s0/Ubuntu_21.04_lan%25C3%25A7ado.png)

Conforme programado, o Ubuntu 21.04 Hirsute Hippo foi lançado no dia 22 de abril. Veja a seguir mais detalhes, como baixá-lo e instalá-lo.


### Hirsute Hippo

  
Como citado nas matérias anteriores sobre a versão 21.04, o nome Hirsute Hippo significa "Hipopótamo Peludo".  
Esta será a segunda de 3 versões intermediárias que são lançadas entre cada versão LTS _(a primeira foi a 20.10 e a próxima será a 21.10)._ É uma versão estável e seu suporte terá duração de 9 meses, durando até janeiro de 2022, conforme o [ciclo de vida das versões do Ubuntu](https://info.wsouza.com.br/2019/03/ubuntu-como-funciona-politica-de-seu-ciclo-de-vida.html).  
  

### Novidades

  
Não houve grandes mudanças em relação ao seu antecessor e algumas já foram adiantadas em matérias anteriores. Mas, de qualquer forma, algumas das principais novidades são:  

*   Kernel 5.11 com maior supote e atualizações, incluindo melhorias no sistema de arquivos BTRFS;
*   Wayland por padrão;
*   Firefox 87;
*   LibreOffice 7.1.2-rc2;
*   Thunderbird 78.8.1;
*   GNOME 3.38.4. Ainda não foi nesta versão que o GNOME 40 desembarcou no Ubuntu, mas alguns aplicativos já foram atualizados para a versão 40;
*   BlueZ 5.56;
*   NetworkManager 1.30;
*   Samba 4.13.3
*   A integração do Active Directory foi melhorada.

  

### Download

  
Seguem os links para download das imagens de instalação _(amd64)_ do Ubuntu e de alguns dos seus _"flavours" ou "sabores"_ oficiais. Todas as imagens são da versão Desktop e podem ser utilizadas sem necessidade de instalação. Há também a opção de download em Torrent. Escolha o "sabor" de sua preferência e faça o download.  
  

Ubuntu 21.04 - Hirsute Hippo

[ Live](https://releases.ubuntu.com/hirsute/ubuntu-21.04-desktop-amd64.iso)
[ Torrent](https://releases.ubuntu.com/hirsute/ubuntu-21.04-desktop-amd64.iso.torrent)
[ Mais...](https://ubuntu.com/download)

  

#### Flavours:

  
[ Kubuntu 21.04](https://kubuntu.org/getkubuntu/)  
[ Xubuntu 21.04](https://xubuntu.org/download)  
[ Ubuntu Mate 21.04](https://ubuntu-mate.org/download/)  
[ Lubuntu 21.04](https://lubuntu.me/downloads/)  
[ Ubuntu Kylin 21.04](https://www.ubuntukylin.com/downloads/show.php?id=451&lang=en)  
[ Ubuntu Studio 21.04](https://ubuntustudio.org/download/)  
[ Ubuntu Budgie 21.04](https://ubuntubudgie.org/downloads/)  
  

### Instalação ou atualização

  

#### Atualizar a partir do Ubuntu 20.10 - Groovy Gorilla

  
Se você está utilizando atualmente a versão anterior, o Ubuntu 20.10 você pode atualizar para o Hirsute Hippo através da atualização do sistema, ou pelo terminal, que é o que será mostrado a seguir. Siga os passos abaixo:  
  

*   Para ter certeza que a versão atual está com as atualizações mais recentes instaladas, no terminal, execute os comandos:

  

  

##### sudo apt update

  
  

  

##### sudo apt upgrade

  

*   Após atualizar, execute:

  

  

#####  sudo do-release-upgrade -d

  
O comando anterior vai:  

*   Verificar se há uma nova versão em desenvolvimento;
*   Desativar os repositórios de terceiros (PPAs);
*   Alterar os repositórios de _groovy_ para _hirsute_;
*   Haverá uma solicitação para confirmar a atualização.

1.  Se confirmar a atualização será iniciada. O processo pode ser bem demorado. Preste atenção às solicitações de confirmação de ações, confirme-as e aguarde a finalização. Após finalizado reinicie o sistema e você terá o Ubuntu 21.04 Hirsute Hippo instalado.
2.  Se não confirmar pode ser que seja preciso alterar os repositórios manualmente de _hirsute_ para _groovy_.  
    Neste caso, utilize o editor de texto que preferir _(joe gedit, kate, nano, vim, pluma...)_, e abra o arquivo sources.list com o comando abaixo:

  

#####  sudo _joe_ /etc/apt/sources.list

  

*   No arquivo aberto, faça as alterações solicitadas e salve o arquivo.

  

#### Executando a imagem _ISO_ num pendrive e instalando do zero

  
Primeiramente é necessário gravar num pendrive a imagem ISO baixada anteriormente. Veja como gravar a ISO no pendrive, se você estiver utilizando [Linux](https://info.wsouza.com.br/2020/04/3-maneiras-de-gravar-uma-imagem-iso-num-pendrive-utilizando-linux.html) ou [Windows](https://info.wsouza.com.br/2015/01/criar-um-pendrive-multiboot-linux.html).  
  
O vídeo abaixo mostra o Hirsute Hippo sendo executado via pendrive e sendo instalado numa máquina sem outro sistema operacional instalado.

[![Assista ao vídeo](https://img.youtube.com/vi/T-DW9jioJac/maxresdefault.jpg)](https://www.youtube.com/embed/T-DW9jioJac)
