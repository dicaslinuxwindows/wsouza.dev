---
title: 'Novidades sobre a Sis Mirage 3 no Ubuntu Trusty Tahr (14.04) , Linux Mint Rebecca (17.1), Debian Wheezy (7) e Jessie (8)'
date: 2015-01-04T05:05:00.003-02:00
draft: false
url: /2015/01/novidades-sobre-sis-mirage-3-no-ubuntu.html
tags: 
- Debian
- Linux
- Ubuntu
- Sis Mirage 3 Graphics
- Tutoriais
---

  

_Atualizado em 21/02/2016_

  

[![](https://4.bp.blogspot.com/-kn3ABsUN6q8/VKjU_JoftUI/AAAAAAAABHQ/7URh0ud59-M/s1600/sismirage3_mint_ubuntu.png "sis mirage 3 debian, ubuntu e linux mint")](http://4.bp.blogspot.com/-kn3ABsUN6q8/VKjU_JoftUI/AAAAAAAABHQ/7URh0ud59-M/s1600/sismirage3_mint_ubuntu.png)

  

Já escrevi algumas vezes aqui no blog sobre esta placa de vídeo, Sis Mirage 3, [e, num dos posts, cheguei a dizer que quem utiliza Ubuntu e a Sis Mirage 3 ficaria preso à versão 12.04 ou anterior.](http://info.wsouza.com.br/2013/04/sis-mirage3.html) O tempo passou e, pesquisando na net, testando, consegui encontrar uma maneira de pelo menos atingir a resolução 1280 x 800 em alguns notebooks que possuem esta resolução e reproduzir vídeos tranquilamente. Veja a seguir:  

  
**Sis Mirage 3 no Ubuntu 14.04 e Linux Mint 17.1 (Rebecca)**  
  
A solução tanto para o Mint 17.1 (Rebecca) e Ubuntu 14.04 _(testei apenas em x64)_ é a mesma, pois o Mint deriva do Ubuntu. Lembrando que esta dica não funciona no Linux Mint 17.1 Debian Edition. Esta solução eu encontrei no [Viva o Linux](http://www.vivaolinux.com.br/dica/Configurando-SIS-67172-no-Ubuntu-1404) e baseia-se na utilização do driver Sisimedia do Mandriva e tomei a liberdade de fazer pequenas adaptações para facilitar a instalação do driver.  
  
Criei um script que faz todo o procedimento necessário para a instalação do driver e pode ser [baixado aqui](https://www.dropbox.com/s/0jw4h4igr5hapu5/sisi_trusty.sh?dl=0).  
Para instalar via script rode os comandos no terminal e reinicie o computador.

  

**sudo mv sisi\_trusty.sh?dl=0 sisi\_trusty.sh  
sudo bash sisi\_trusty.sh**  
  

Mas quem quiser fazer manualmente pode seguir os passos abaixo.  
  
**Download dos arquivos necessários.**  
  
1 - Driver Sisimedia:  
  
[sisimedia\_drv.la](https://www.dropbox.com/s/xn4ejvd7cp5pxqe/sisimedia_drv.la?dl=0)  
[sisimedia\_drv.so](https://www.dropbox.com/s/zywh84cdmte3s1r/sisimedia_drv.so?dl=0)  
  
2 - Sis Control e o atalho para desktop, responsável por configurar as configurações da placa.  
  
[sisctrl](https://www.dropbox.com/s/hc3b1eeuo1pv2b3/sisctrl?dl=0)  
[SisControl](https://www.dropbox.com/s/wb8plsiivkioz84/SIS%20SisCTRL.desktop?dl=0)  
  
3- Xorg.conf  
  
[xorg.conf](https://www.dropbox.com/s/ux6lbwk6bbpw4ub/xorg.conf?dl=0)  
  
**Instalação.**  
  
1 - Copie e cole os comandos abaixo no terminal:

  

**sudo su  
mv sisctrl /usr/bin/sisctrl  
mv sisimedia\_drv.la /usr/lib/xorg/modules/drivers/sisimedia\_drv.la  
mv sisimedia\_drv.so /usr/lib/xorg/modules/drivers/sisimedia\_drv.so  
mv xorg.conf /etc/X11/xorg.conf**  
  

2 - Copie o atalho SisCTRL.desktop para o local que desejar, é ele que acessa algumas configurações avançadas do driver.  
  
Finalizado, reinicie o computador e a Sis Mirage 3 estará com a resolução correta.  
  
Obs: Nos casos que esta solução não funcionar no Ubuntu 14.04 tente a solução para o Debian Jessie, postada mais abaixo.  
  
**Sis Mirage 3 no Linux Mint 13 (Maya)**  
  
No 1º post que fiz sobre Sis Mirage 3 aqui no blog afirmei que a dica do blog do Hugo Bastos, que funcionava até o Ubuntu 12.04 era também aplicável à versão do Linux Mint equivalente àquela versão do Ubuntu. A versão do Linux Mint era a 13, chamada Maya. Depois de um tempo vi que não era possível utilizar a mesma dica e depois de mais um tempo consegui fazer funcionar no Mint Maya, então adaptei um script que uso faz algum tempo para facilitar a instalação.  
Baixe o script para o Linux Mint Maya  
  
[Baixar o script Sis Mirage 3 no Linux Mint 13 (Maya)](https://www.dropbox.com/s/z7un957r7byh3ac/sis_maya.sh?dl=0)  
  
Para instalar, copie e cole os comandos abaixo no terminal:

  

**sudo mv sis\_maya.sh?dl=0 sis\_maya.sh  
sudo bash sis\_maya.sh**  
  

Aguarde o fim, reinicie o computador, e você já terá a resolução correta do monitor.  
  
**Sis Mirage 3 no Debian Wheezy (7)**  
  
E vamos continuando com as buscas de soluções para, pelo menos, atingir a resolução correta do monitor em notebooks com a Sis Mirage 3.  
Desta vez consegui encontrar uma solução que funcionasse na versão estável do Debian, que nesta data, é o Debian 7, de codinome Wheezy. Após instalado o Wheezy atualizei-o para a versão 8 (Jessie) e o monitor continuou com a resolução correta, porém, quando instalei o Debian Jessie do zero, esta solução não funcionou. Para instalar a solução no Debian Wheezy, abra o terminal e siga os seguintes passos:

  
1 - Instale alguns pacotes necessários para compilar o driver  
  
**sudo su**  
**apt-get update**  
**apt-get install git xorg-dev mesa-common-dev libdrm-dev libtool build-essential xutils-dev automake autoconf autotools-dev libdmx-dev p7zip-full p7zip**  
  
2 - Baixe o fonte do driver a ser compilado  
  
[Baixar xf86-video-sis671-sis-671-fix.tar.gz](https://www.dropbox.com/s/fdnoczya2gq7d1m/xf86-video-sis671-sis-671-fix.tar.gz?dl=0)  
  
3 - Descompacte o arquivo baixado anteriormente  
  
**tar -vzxf xf86-video-sis671-sis-671-fix.tar.gz**  
  
4 - Agora vamos compilar o driver, faça cada um dos comandos abaixo e aguarde  
  
**cd xf86-video-sis671-sis-671-fix  
autoreconf -vi  
./configure --prefix=/usr --disable-static  
make  
make install**  
  
5 - Baixe o Xorg.conf  
  
[Xorg.conf](https://www.dropbox.com/s/32h5h2mqvfqq6h8/xorg.conf?dl=0)  
  
6 - Instale o Xorg.conf  
  
**mv xorg.conf /etc/X11/xorg.conf  
  
**  

Reinicie o computador, e você já terá a resolução correta do monitor.  
  
_Atualização em 21/02/2016, com algumas [dicas](http://disq.us/p/14imkxn) fornecidas por [Matheus Azevedo](https://disqus.com/by/disqus_j5SiXI6COg/)_  
  
**Sis Mirage 3 no Debian 8 (Jessie)** \- _(Funciona também no Ubuntu 14.04.2)_  
  
A última versão estável do Debian é a 8.0, chamada Jessie. Após algumas tentativas, consegui obter êxito quanto ao funcionamento desta placa nesta versão. _Este procedimento funciona no Ubuntu 14.04, para os casos que a solução acima não funcionou_. O procedimento para instalação é praticamente o mesmo dos anteriores, abra o terminal e siga os seguintes passos:

  
1 - Instale alguns pacotes necessários para compilar o driver  
  
**sudo apt-get install git xorg-dev mesa-common-dev libdrm-dev libtool build-essential xutils-dev automake autoconf autotools-dev libdmx-dev p7zip-full p7zip mesa-utils mesa-utils-extra libgl1-mesa-dri-dbg libgl1-mesa-dri libgl1-mesa-swx11 libgl1-mesa-swx11-dbg libgl1-mesa-swx11-dev libglw1-mesa libglu1-mesa libglu1-mesa-dev libx11-dev**  
  
2 - Baixe o fonte do driver a ser compilado  
  
[Baixar sis-mirage3.tar.gz](https://www.dropbox.com/s/4u9lf5li3gbtlgb/sis-mirage3.tar.gz?dl=0)  
  
3 - Descompacte o arquivo baixado anteriormente  
  
**tar -vzxf sis-mirage3.tar.gz**  
  
4 - Agora vamos compilar o driver, faça cada um dos comandos abaixo e aguarde  
  
**sudo su  
cd sis-mirage3  
autoreconf -vi  
./configure --prefix=/usr --disable-static  
make  
make install**  
  
5 - Baixe o Xorg.conf (Fornecido por Matheus Azevedo, nos comentários abaixo)  
  
[Xorg.conf](https://www.dropbox.com/s/32h5h2mqvfqq6h8/xorg.conf?dl=0)  
  
6 - Instale o Xorg.conf  
  
**mv xorg.conf /etc/X11/xorg.conf**  

Reinicie o computador.  
  
E fica a dica, teste e comente aqui no blog se estas soluções funcionaram, assim podemos debater e ajudar outros usuários que passam pelos mesmos problemas.  
  
Obs¹: Não é possível ativar efeitos 3D, pois esta placa não é 3D, logo, Unity, Gnome 3 e Cinnamon não funcionam corretamente.  
Obs²: Para uma melhor experiência utilize o Xfce, Mate, LXDE ou Gnome-Shell Flashback.