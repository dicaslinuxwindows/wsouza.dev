---
title: 'Instalando ou atualizando o Ubuntu 20.04 Focal Fossa'
date: 2020-04-23T12:16:00.000-03:00
draft: false
url: /2020/04/instalando-ou-atualizando-o-ubuntu-20-04-focal-fossa.html
tags: 
- Linux
- Ubuntu
- Ubuntu 20.04
---

![Instalando ou atualizando o Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows](https://2.bp.blogspot.com/-aExmt4axzCk/Xuq7gDoTfsI/AAAAAAAAPH8/l9hR-UFTCQYS4IFQcv-j2xC6yzFxFy21ACNcBGAsYHQ/s1600/Focal_Fossa_Download.png)

Após o [lançamento oficial do Ubuntu 20.04](https://info.wsouza.com.br/2020/04/ubuntu-2004-lts-focal-fossa-e-lancado-oficialmente.html) vamos ver nesta matéria algumas opções para obtê-lo e usufruir de todas as suas funcionalidades. Confira.

  
  
  
  
  
  
  

Há várias formas de obter e utilizar o recém lançado Ubuntu Focal Fossa. Nesta matéria mostrarei algumas destas formas, como:  

*   Atualizar a partir de uma versão anterior, sem perder arquivos e configurações. A dica apresentada nesta matéria ignora a notificação do sistema sobre a nova versão disponível, todo o processo será realizado pelo terminal;
*   Instalar do zero a partir de um Live DVD/USB;
*   Instalar em uma máquina virtual;
*   Executar em modo live.

  

### Atualizar a partir do Ubuntu 18.04 ou 19.10

  
Se você está utilizando atualmente o Ubuntu 18.04 _(Bionic Beaver)_ ou o Ubuntu 19.10 _(Eoan Ermine)_ você pode atualizar diretamente - mantendo os arquivos e configurações - seguindo os passos abaixo:  
  

*   Tenha certeza que o a versão atual está com as últimas atualizações. No terminal, faça:

  

 sudo apt update  
 sudo apt upgrade

  

*   Após atualizar, faça:

  

 sudo do-release-upgrade -d

  
O comando anterior vai:  

*   Verificar se há uma nova versão em desenvolvimento;
*   Desativar os repositórios de terceiros (PPAs);
*   Altera os repositórios de bionic para focal _(Ubuntu 18.04)_ ou de eoan para focal _(Ubuntu 19.10)_;
*   Haverá uma solicitação para confirmar a atualização.

1.  Confirme _(s)_ e a atualização será iniciada. Dependendo da velocidade da sua internet, o processo pode ser bem demorado. Fique atento pois poderão haver solicitações de confirmação de ações, confirme-as e aguarde a finalização. Após finalizado reinicie o sistema e você terá o Ubuntu Focal Fossa instalado.
2.  Caso não confirme _(N)_, pode ser que seja preciso alterar os repositórios manualmente de **focal para bionic** _(se você estava no 18.04)_ ou de **focal para eoan** _(se estava no 19.10)_. Nos testes que realizei não ocorreram problemas quando não confirmei a atualização.  
    Mas, caso ocorram problemas, utilize o editor de texto que preferir _(joe gedit, kate, nano, vi, pluma...)_, e abra o arquivo sources.list com o comando abaixo:

 sudo _joe_ /etc/apt/sources.list

  

*   No arquivo aberto, faça as alterações solicitadas e salve o arquivo.

  

### Download da ISO

  
Seguem os links para download das imagens de instalação _(amd64)_ do Ubuntu e de alguns dos seus _"flavours" ou "sabores"_ oficiais. Todas as imagens são da versão Desktop e podem ser utilizadas sem necessidade de instalação. Há também a opção de download em Torrent. Escolha a de sua preferência, grave num DVD ou Pendrive e desfrute .  
  
  

Ubuntu

[ Live](https://releases.ubuntu.com/focal/ubuntu-20.04-desktop-amd64.iso)

[ Torrent](http://releases.ubuntu.com/focal/ubuntu-20.04-desktop-amd64.iso.torrent)

[Mais...](https://ubuntu.com/download)

Kubuntu

[ Live](http://cdimage.ubuntu.com/kubuntu/releases/focal/release/kubuntu-20.04-desktop-amd64.iso)

[ Torrent](http://cdimage.ubuntu.com/kubuntu/releases/focal/release/kubuntu-20.04-desktop-amd64.iso.torrent)

[Mais...](https://kubuntu.org/getkubuntu/)

Xubuntu

[ Live](http://cdimage.ubuntu.com/xubuntu/releases/focal/release/xubuntu-20.04-desktop-amd64.iso)

[ Torrent](http://cdimage.ubuntu.com/xubuntu/releases/focal/release/xubuntu-20.04-desktop-amd64.iso.torrent)

[Mais...](https://xubuntu.org/download)

Ubuntu Mate

[ Live](http://cdimage.ubuntu.com/ubuntu-mate/releases/focal/release/ubuntu-mate-20.04-desktop-amd64.iso)

[ Torrent](http://cdimage.ubuntu.com/ubuntu-mate/releases/focal/release/ubuntu-mate-20.04-desktop-amd64.iso.torrent)

[Mais...](https://ubuntu-mate.org/download/)

Lubuntu

[ Live](http://cdimage.ubuntu.com/lubuntu/releases/focal/release/lubuntu-20.04-desktop-amd64.iso)

[ Torrent](http://cdimage.ubuntu.com/lubuntu/releases/focal/release/lubuntu-20.04-desktop-amd64.iso.torrent)

[Mais...](https://lubuntu.me/downloads/)

Ubuntu Kylin

[ Live](http://cdimage.ubuntu.com/ubuntukylin/releases/focal/release/ubuntukylin-20.04-desktop-amd64.iso)

[ Torrent](http://cdimage.ubuntu.com/ubuntukylin/releases/focal/release/ubuntukylin-20.04-desktop-amd64.iso.torrent)

[Mais...](https://www.ubuntukylin.com/downloads/show.php?id=451&lang=en)

Ubuntu Studio

[ Live](http://cdimage.ubuntu.com/ubuntustudio/releases/focal/release/ubuntustudio-20.04-dvd-amd64.iso)

[ Torrent](http://cdimage.ubuntu.com/ubuntustudio/releases/focal/release/ubuntustudio-20.04-dvd-amd64.iso.torrent)

[Mais...](https://ubuntustudio.org/download/)

Ubuntu Budgie

[ Live](http://cdimage.ubuntu.com/ubuntu-budgie/releases/20.04/release/ubuntu-budgie-20.04-desktop-amd64.iso)

[ Torrent](http://cdimage.ubuntu.com/ubuntu-budgie/releases/20.04/release/ubuntu-budgie-20.04-desktop-amd64.iso.torrent)

[Mais...](https://ubuntubudgie.org/downloads/)

  
  

### Executar em modo live

  
Essa opção permite utilizar o Ubuntu sem precisar instalar. O sistema é executado pelo Pendrive/DVD e "descarregado" na memória RAM.  

*   Grave a imagem ISO num DVD ou Pendrive _(Veja como gravar o pendrive no [Linux](https://info.wsouza.com.br/2020/04/3-maneiras-de-gravar-uma-imagem-iso-num-pendrive-utilizando-linux.html) ou [Windows](https://info.wsouza.com.br/2015/01/criar-um-pendrive-multiboot-linux.html))_;
*   Mude as configurações de boot do computador para iniciar pelo Pendrive ou pelo DVD. Geralmente apertando a tecla _F2_ logo ao iniciar o computador temos acesso à estas configurações e geralmente a tecla _F10_ salva as configurações.
*   Deixe como está nas duas telas abaixo:

[![Instalando ou atualizando o Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows](https://4.bp.blogspot.com/-u4eCCI1hkmQ/XqJPYnE3JgI/AAAAAAAAOvY/ZGbU9iZk5UAe7DQxGpcManpZTHawdX--QCNcBGAsYHQ/s640/01.png "Instalando ou atualizando o Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-u4eCCI1hkmQ/XqJPYnE3JgI/AAAAAAAAOvY/ZGbU9iZk5UAe7DQxGpcManpZTHawdX--QCNcBGAsYHQ/s1600/01.png)

[![Instalando ou atualizando o Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows](https://4.bp.blogspot.com/-al0MfkYdHV4/XqJPYuvHpRI/AAAAAAAAOvc/l1QOyNe1MkICH-YesirPzy_fEaMkfwAVACNcBGAsYHQ/s640/02.png "Instalando ou atualizando o Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-al0MfkYdHV4/XqJPYuvHpRI/AAAAAAAAOvc/l1QOyNe1MkICH-YesirPzy_fEaMkfwAVACNcBGAsYHQ/s1600/02.png)

*   Após a seleção, aparecerá a tela de carregamento e na sequência o sistema será carregado no modo live.

[![Instalando ou atualizando o Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows](https://4.bp.blogspot.com/--6oAMhozAUg/XqJP6Dn2TEI/AAAAAAAAOvo/Y5MnX3IS_OIeC4we_62U4dHejLaHePwhwCNcBGAsYHQ/s640/03.png "Instalando ou atualizando o Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows")](https://4.bp.blogspot.com/--6oAMhozAUg/XqJP6Dn2TEI/AAAAAAAAOvo/Y5MnX3IS_OIeC4we_62U4dHejLaHePwhwCNcBGAsYHQ/s1600/03.png)

[![Instalando ou atualizando o Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows](https://3.bp.blogspot.com/-k7-9bIHDMdc/XqJP6MltjvI/AAAAAAAAOvs/Nvfuy0ERzFon0WkGuh41On0fe1QG00jJACNcBGAsYHQ/s640/04.png "Instalando ou atualizando o Ubuntu 20.04 Focal Fossa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-k7-9bIHDMdc/XqJP6MltjvI/AAAAAAAAOvs/Nvfuy0ERzFon0WkGuh41On0fe1QG00jJACNcBGAsYHQ/s1600/04.png)

  

### Instalar com um Live DVD/USB

  

*   O vídeo abaixo mostra a instalação normal do Ubuntu num computador que não possui nenhum outro sistema, ou seja, sem dual boot e aproveitando o disco todo com particionamento automático. No vídeo a instalação foi iniciada após entrar no modo live, mas a instalação também pode ser iniciada sem entrar no live. Para isto, basta escolher a opção "Instalar o Ubuntu", mostrada no menu que aparece ao iniciar.

  

  

*   Já no vídeo abaixo, foi utilizada a instalação lado a lado com o Windows 10, ou seja, o Ubuntu e Windows 10 instalados no mesmo disco, em **dual boot**. Neste tipo de instalação, o instalador do Ubuntu cria uma partição a partir do espaço vazio no disco e separa a partição do Windows. Após, ocorre a instalação do Ubuntu.

  

### Instalar em uma Máquina Virtual

  
Se deseja instalar o Focal Fossa, mas nunca fez antes e tem medo de comprometer seus arquivos, tente [instalar o sistema em uma máquina virtual](https://info.wsouza.com.br/2018/08/maquina-virtual-instalando-e-configurando-o-sistema-no-vmware.html).