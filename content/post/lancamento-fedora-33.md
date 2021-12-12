---
title: 'Lançamento Fedora 33'
date: 2020-10-28T14:56:00.011-03:00
draft: false
url: /2020/10/lancamento-fedora-33.html
tags: 
- Linux
- Fedora
---

![Lançamento Fedora 33 - Dicas Linux e Windows](https://1.bp.blogspot.com/-p8CfnXzNuRg/X5mwSIIy0yI/AAAAAAAAQt4/zWg1PhA8Fts5JPikZ9JO16XUW0ndNk4cgCNcBGAsYHQ/s16000/Fedora33.png "Lançamento Fedora 33 - Dicas Linux e Windows")

No dia 27 de outubro de 2020 foi lançada a versão 33 do Fedora, que traz diversas novidades. Veja a seguir mais detalhes sobre este lançamento e como baixar, instalar e atualizar.

  
  
  
  
  
  

> _"Hoje, estou animado para compartilhar os resultados do trabalho árduo de milhares de colaboradores para o Projeto Fedora: nosso último lançamento, Fedora 33, está aqui! Este é um grande lançamento com muita mudança, mas acredito que todo esse trabalho também o tornará confortável, cumprindo nosso objetivo de trazer-lhe o mais recente software estável, poderoso e robusto de código livre e de código aberto em muitas ofertas fáceis de usar..."_

O anúncio acima foi publicado na [Fedora Magazine](https://fedoramagazine.org/announcing-fedora-33/) e anuncia o lançamento do Fedora 33.  
  
Conforme publicado na matéria [Fedora 33 Beta](https://info.wsouza.com.br/2020/10/fedora-33-beta.html), sabíamos que ainda neste mês seria lançado oficialmente o Fedora 33. A princípio seria no dia 21/10/2020, porém, acabou saindo no dia 27/10/2020.  
  

### Notas de lançamento

  
Conforme adiantado na matéria que foi tratado da versão beta, o Fedora 33 viria com a nova versão do GNOME e com o sistema de arquivos BTRFS ativado como padrão.  
O GNOME chegou na versão [3.38](https://info.wsouza.com.br/2020/09/gnome-338-e-lancado.html).1, que possui diversas melhorias. Destaco a possibilidade de alternar a posição dos ícones na grade de aplicativos e a tela de boas vindas.  
O sistema de arquivos BRTFS chega em substuição ao sistema EXT4. Dentre algumas coisas interessantes do BRTFS estão:  

*   Copy-on-Write - Otimiza o uso do disco, pois diminui a entrada/saída de dados;
*   Snapshots - Funciona como um backup, pois cria imagens do sistema de arquivos, permitindo a sua restauração para uma versão anterior;
*   Compressão de dados - Compacta todo sistema de arquivos, resultando em economia de espaço;

Desde que você esteja fazendo uma instalação limpa (do zero), o BTRFS será instalado como padrão, caso contrário, permanecerá o mesmo sistema de arquivos que já estava instalado anteriormente.  
  
Além da confirmação destas duas situações, temos:  

*   Kernel 5.8
*   Libre Office 7.0.2.2
*   Firefox 82
*   Bash 5.0.17
*   Novo papel de parede

  

### Download e instalação

  
Os links abaixo são do Fedora Workstation, que é a versão padrão e vem com ambiente GNOME. _Live_ é o modo de download onde a imagem baixada ser executada diretamente de um pendrive ou DVD, sem a necessidade de instalação. Ainda assim é possível instalar após o teste. _Netinstall_ é o modo de download onde a imagem baixada é um pouco menor, podendo caber num CD, ou pendrive. Tudo o que for necessário para a instalação será baixado no momento da mesma, portanto, você precisa estar conectado à internet. _Torrent_ é a maneira mais rápida de baixar a imagem Live.  
  

Fedora 33 Wokstation X86\_64

[ Live](https://download.fedoraproject.org/pub/fedora/linux/releases/33/Workstation/x86_64/iso/Fedora-Workstation-Live-x86_64-33-1.2.iso)

[ Netinstall](https://download.fedoraproject.org/pub/fedora/linux/releases/33/Server/x86_64/iso/Fedora-Server-netinst-x86_64-33-1.2.iso)

[ Torrent](https://torrent.fedoraproject.org/torrents/Fedora-Workstation-Live-x86_64-33.torrent)

[Mais...](https://alt.fedoraproject.org/)

  

#### Fedora Spins

  
Fedora Spins são o equivalente aos Flavours do Ubuntu, ou seja, são os "sabores" do Fedora. Nada mais são do que o Fedora Workstation com outras intefaces que não o GNOME. Os links abaixo levam até a página de download de cada Spin.  
  
[ Fedora 33 KDE PLASMA](https://spins.fedoraproject.org/kde/download/index.html)  
[ Fedora 33 XFCE](https://spins.fedoraproject.org/pt_BR/xfce/)  
[ Fedora 33 LXQT](https://spins.fedoraproject.org/pt_BR/lxqt/)  
[ Fedora 33 MATE-COMPIZ](https://spins.fedoraproject.org/pt_BR/mate-compiz/)  
[ Fedora 33 CINNAMON](https://spins.fedoraproject.org/pt_BR/cinnamon/)  
[ Fedora 33 LXDE](https://spins.fedoraproject.org/pt_BR/lxde/)  
[ Fedora 33 SOAS](https://spins.fedoraproject.org/pt_BR/soas/)  
  

### Atualizando a partir do Fedora 32

  
A sequência abaixo mostra como atualizar, por linha de comando e sem a necessidade de formatação.  
  
1 - Execute o comando abaixo.  
  

  

 sudo dnf upgrade --refresh

  
2 - Reinicie o computador. Após reiniciar, instale o plugin de atualização.  
  

  

 sudo dnf install dnf-plugin-system-upgrade

  
3 - Baixe os pacotes atualizados. Este processo pode demorar bastante, dependendo da velocidade da conexão com a internet.  
  

  

 sudo dnf system-upgrade download --refresh --releasever=33

  
4 - O comando abaixo vai reiniciar o computador novamente. Após este processo o sistema ficará na tela de atualização e este processo poderá demorar. Seja paciente e aguarde.  
  

  

 sudo dnf system-upgrade reboot

  
Ao reiniciar, o Fedora 33 já estará instalado.  
  
**Fonte:** [https://docs.fedoraproject.org/en-US/quick-docs/dnf-system-upgrade/](https://docs.fedoraproject.org/en-US/quick-docs/dnf-system-upgrade/)  
  

### Screenshots

  

[![Lançamento Fedora 33 - Dicas Linux e Windows](https://1.bp.blogspot.com/-oucTH9vspG4/X5mVZWe2h4I/AAAAAAAAQtM/XnUfzwNbhaIqoDq6880GLla5n7kDt2sRQCNcBGAsYHQ/s600/01.png "Lançamento Fedora 33 - Dicas Linux e Windows")](https://1.bp.blogspot.com/-oucTH9vspG4/X5mVZWe2h4I/AAAAAAAAQtM/XnUfzwNbhaIqoDq6880GLla5n7kDt2sRQCNcBGAsYHQ/s1366/01.png)

[![Lançamento Fedora 33 - Dicas Linux e Windows](https://1.bp.blogspot.com/-moM2NhlTMOI/X5mVZIuYqFI/AAAAAAAAQtE/05o6-MvtXvIWtgh6k7MPJ3BwAjNFo_9XgCNcBGAsYHQ/s600/02.png "Lançamento Fedora 33 - Dicas Linux e Windows")](https://1.bp.blogspot.com/-moM2NhlTMOI/X5mVZIuYqFI/AAAAAAAAQtE/05o6-MvtXvIWtgh6k7MPJ3BwAjNFo_9XgCNcBGAsYHQ/s1366/02.png)

[![Lançamento Fedora 33 - Dicas Linux e Windows](https://1.bp.blogspot.com/-wpqnOqkkHnw/X5mVZT7gUNI/AAAAAAAAQtI/KhIbLN_xK00lKTK5fGgbeh96DrLeEqedQCNcBGAsYHQ/s600/03.png "Lançamento Fedora 33 - Dicas Linux e Windows")](https://1.bp.blogspot.com/-wpqnOqkkHnw/X5mVZT7gUNI/AAAAAAAAQtI/KhIbLN_xK00lKTK5fGgbeh96DrLeEqedQCNcBGAsYHQ/s1366/03.png)

[![Lançamento Fedora 33 - Dicas Linux e Windows](https://1.bp.blogspot.com/--vWTrJa8djc/X5mVaIMHbBI/AAAAAAAAQtQ/uwDWiZsXSRU7MBd0AnemxvIT5rpNbenzwCNcBGAsYHQ/s600/04.png "Lançamento Fedora 33 - Dicas Linux e Windows")](https://1.bp.blogspot.com/--vWTrJa8djc/X5mVaIMHbBI/AAAAAAAAQtQ/uwDWiZsXSRU7MBd0AnemxvIT5rpNbenzwCNcBGAsYHQ/s1366/04.png)

[![Lançamento Fedora 33 - Dicas Linux e Windows](https://1.bp.blogspot.com/-mq487Sx53ZA/X5mVabvmIqI/AAAAAAAAQtU/XqWx7vf8E3I6g6sVGVEAR4G18DbR6xQXgCNcBGAsYHQ/s600/05.png "Lançamento Fedora 33 - Dicas Linux e Windows")](https://1.bp.blogspot.com/-mq487Sx53ZA/X5mVabvmIqI/AAAAAAAAQtU/XqWx7vf8E3I6g6sVGVEAR4G18DbR6xQXgCNcBGAsYHQ/s1366/05.png)

[![Lançamento Fedora 33 - Dicas Linux e Windows](https://1.bp.blogspot.com/-_8uAL-uonT8/X5mVaaoIFPI/AAAAAAAAQtY/xxPqZZHn8pYeo_BOtQA9npK0ctV8HobegCNcBGAsYHQ/s600/07.png "Lançamento Fedora 33 - Dicas Linux e Windows")](https://1.bp.blogspot.com/-_8uAL-uonT8/X5mVaaoIFPI/AAAAAAAAQtY/xxPqZZHn8pYeo_BOtQA9npK0ctV8HobegCNcBGAsYHQ/s1366/07.png)

[![Lançamento Fedora 33 - Dicas Linux e Windows](https://1.bp.blogspot.com/-8Bztu0VmtLU/X5mVawI8RGI/AAAAAAAAQtc/TEWim4__UCsgpeh2s-LVua3lDOgxfC4qwCNcBGAsYHQ/s600/08.png "Lançamento Fedora 33 - Dicas Linux e Windows")](https://1.bp.blogspot.com/-8Bztu0VmtLU/X5mVawI8RGI/AAAAAAAAQtc/TEWim4__UCsgpeh2s-LVua3lDOgxfC4qwCNcBGAsYHQ/s1366/08.png)