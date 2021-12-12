---
title: 'Flatpak e Snap no Debian, Fedora e Ubuntu'
date: 2020-12-31T01:07:00.013-03:00
draft: false
url: /2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html
tags: 
- Flatpak
- Debian
- Ubuntu
- Tutoriais
- Fedora
- Snap
---

![Flatpak e Snap no Debian, Fedora e Ubuntu - Dicas Linux e Windows](https://1.bp.blogspot.com/-2rPVAD8KZKI/X-1DOpcczHI/AAAAAAAARbA/gOigtPYtHj0nJI4JfrUlCyMzfnTDBx7egCNcBGAsYHQ/s16000/Snap_Flatpak_Pt1.png "Flatpak e Snap no Debian, Fedora e Ubuntu - Dicas Linux e Windows")

Veja nesta matéria como ativar o suporte e instalar pacotes Snap e Flatpak em distribuições Linux, além de um esboço sobre pacotes de aplicativos nas distribuições Linux.

  
  
  
  
  
  

### Índice

  
Como a matéria é um pouco extensa, fiz um índice para facilitar o acesso aos tópicos.  

1.  [Aplicativos em sistemas Linux](https://info.wsouza.com.br/2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html#aplicativos)
2.  [Flatpak](https://info.wsouza.com.br/2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html#flatpak)
3.  [Snap](https://info.wsouza.com.br/2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html#snap)
4.  [Vantagens e desvantagens do uso de Snap ou Flatpak](https://info.wsouza.com.br/2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html#vantagens)
5.  [Ativar o suporte ao Snap no Debian e Fedora](https://info.wsouza.com.br/2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html#suportesnap)
6.  [Ativar o suporte ao Flatpak no Ubuntu e Debian](https://info.wsouza.com.br/2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html#suporteflatpak)
7.  [Instalando Snap no Debian e Fedora](https://info.wsouza.com.br/2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html#instalasnap)
8.  [Instalando Flatpak no Debian e Ubuntu](https://info.wsouza.com.br/2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html#instalaflatpak)
9.  [Considerações finais](https://info.wsouza.com.br/2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html#consideracoes)
10.  [Referências](https://info.wsouza.com.br/2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html#referencias)

  
[](https://draft.blogger.com/null)

### 1\. Aplicativos em sistemas Linux

  
Há várias formas de instalar aplicativos nos sistemas baseados em Linux. Uma forma que funciona em qualquer distribuição é a instalação por código fonte. Desta forma o código é compilado de acordo com a arquitetura do sistema (32, 64 bits...). Porém, não é uma maneira tão simples de se fazer.  
Outra forma é através de pacotes. O código fonte é colocado num arquivo junto com todos os arquivos necessários para sua instalação, somado à um sistema de checagem das dependências e bibliotecas necessárias e scripts para instalação e remoção. Ao instalar um aplicativo por meio de um pacote, este se utilizará destes scripts e do sistema de checagem para instalar ou atualizar tudo o que for necessário para o funcionamento do aplicativo. Cada família de distribuição Linux possui seu sistema de empacotamento de aplicativos e estes sistemas de empacotamento diferem - e sua instalação também - dependendo da "família" da distribuição. Explico:  

*   Nos sistemas baseados no Debian - que têm entre os mais populares o Ubuntu _(que por sua vez possui seus derivados)_ - o sistema de empacotamento é chamado **Deb**, gerando um arquivo com a extensão _.deb_;
*   Em sistemas como Red Hat, Fedora, OpenSuse, CentOS _(entre outros)_ o sistema de empacotamento é chamado de **Rpm** _(Red Hat Package Manager)_, gerando um arquivo com a extensão _.rpm_.
*   Nem todo pacote .deb de uma distribuição pode ser instalado numa outra, mesmo que as duas suportem o formato .deb. O mesmo acontece com os pacotes .rpm.
*   Tanto os pacotes .deb quanto os .rpm podem ser instalados via terminal ou com um duplo clique _(desde que haja um gerenciador que faça a instalação deles)_. Tanto com um duplo clique, quanto pelo terminal, os pacotes são gerenciados por gerenciadores de pacotes, que buscam as dependências necessárias e instalam o aplicativo;
*   Dentre estes gerenciadores estão o **Apt e Dpkg** no Debian, Ubuntu e derivados dos dois; **Dnf** no Fedora; **Zypper** no OpenSuse; além das lojas como a Gnome Software e similares.

Além destes formatos de empacotamento tradicionais, que são, digamos, presos à determinadas distribuições _(ou à famílias de distribuições)_, temos alguns formatos que podemos dizer que são multiplataforma, e podem ser instalados e executados de maneira diferente. Dentre estes formatos estão o Flatpak e Snap, que serão mostrados a seguir:  
  
[](https://draft.blogger.com/null)

### 2\. Flatpak

  
O formato de empacotamento Flatpak foi desenvolvido como parte do projeto [freedesktop.org](https://www.freedesktop.org/wiki/), com o apoio da Red Hat, e tem o intuito de facilitar a utilização de aplicativos em sistemas linux. O Flatpak é um tipo de contêiner, onde tudo o que é necessário para o funcionamento de um aplicativo está nele. Como as bibliotecas necessárias para o funcionamento do aplicativo estão dentro deste contêiner, no momento em que o aplicativo é executado não é solicitado nenhum privilégio administrativo do usuário _(root)_ e este não é capaz de alterar nenhuma configuração do sistema. Só ocorre solicitação de senha de root quando o suporte é ativado e no momento de instalação do runtime (_que geralmente ocorre ao instalar o primeiro pacote Flatpak)_.  
Os aplicativos empacotados neste formato podem ser obtidos na loja [flathub.org](https://flathub.org/home), e/ou em outras fontes. No Fedora o suporte ao Flatpak já vem ativado e há uma integração com a Gnome Software, que permite utilizar a Flathub como fonte.  
Diversos aplicativos populares são disponibilizados neste formato. Dentre estes estão: Firefox, Chromium, Spotify, Gimp, Inkscape, Libre Office, VLC, entre outros.  
  
[](https://draft.blogger.com/null)

### 3\. Snap

  
Desenvolvido pela Canonical _(desenvolvedora do Ubuntu)_ a ideia é que o formato Snap permita que os aplicativos distribuídos neste formato sejam executados em diversos tipos de dispositivos. O suporte Snap já vem integrado ao Ubuntu, inclusive a Gnome Software no Ubuntu virou Snap Store, onde se encontram os aplicativos neste formato. Atualmente é suportado por diversas distribuições Linux.  
Da mesma forma que acontece com os Flatpaks, tudo o que é necessário para um aplicativo ser executado está incluído num pacote Snap e o aplicativo é executado sem interferir nas configurações do sistema operacional e sem exigir permissões de superusuário. Diferentemente do Flatpak, só é possível obter os aplicativos Snap de apenas uma fonte.  
Diversos aplicativos populares são disponibilizados neste formato. Em alguns casos - quando se está utilizando o Ubuntu - ao solicitar a instalação de um aplicativo, este será instalado no formato Snap, mesmo que este aplicativo exista no repositório tradicional do Ubuntu. Em outros casos, a Canonical removeu o aplicativo tradicional, deixando apenas o Snap _(caso do navegador Chromium no Ubuntu)_. Mais detalhes sobre Snaps em [http://guialinux.uniriotec.br/snap/](http://guialinux.uniriotec.br/snap/)  
  
[](https://draft.blogger.com/null)

### 4\. Vantagens e desvantagens do uso de Snap ou Flatpak

  
Algumas vantagens de utilizar pacotes Snap ou Flatpak, salvo algumas exceções pontuais, são:

*   Maior segurança, pois os aplicativos não podem causar danos ao sistema e geralmente é preciso ter acesso de superusuário;
*   Praticamente tudo o que é preciso para o aplicativo funcionar já está incluído no pacote;
*   Em casos onde o usuário utiliza _(por algum motivo específico)_ um sistema desatualizado e, desta forma, não consegue instalar alguns aplicativos mais recentes. Ou quando determinado aplicativo não está nos repositórios da distribuição preferida do usuário. Nestes dois casos o usuário poderá encontrar uma solução disponível em Snap ou Flatpak.

  
Alguns pontos negativos:

*   Utiliza-se de um grande espaço em disco, pois os arquivos geralmente são grandes mas, se você não tem limitação com espaço no HD ou SSD, isto não é um problema;
*   Pode tornar lenta a inicialização do sistema _(Snap)_;
*   Em alguns casos, fora do Ubuntu, os aplicativos em Snap podem não ter uma aparência muito agradável;

  
[](https://draft.blogger.com/null)

### 5\. Ativar o suporte ao Snap no Debian e Fedora

  
Como o Snap já vem ativado por padrão no Ubuntu, vou mostrar nesta seção como instalar e utilizar no Debian e no Fedora. Estes já possuem o suporte ao Snap nos repositórios, porém, o mesmo não vem instalado por padrão.  
  
Instale o Snapd, que é o mesmo que ativar o suporte ao Snap. No terminal, coloque o comando a seguir:  
  
**5.1. No Debian:**  
  

  

 sudo apt install snapd

  
**5.2. No Fedora:**  
  

  

 sudo dnf install snapd

  
[](https://draft.blogger.com/null)

### 6\. Ativar o suporte ao Flatpak no Debian e Ubuntu

  
Da mesma forma, como o suporte ao Flatpak já vem ativado no Fedora, vou mostrar nesta seção como ativá-lo no Debian e no Ubuntu.  
  
Os passos a seguir funcionam no Debian e Ubuntu. No terminal, coloque o comando a seguir:  
  

  

 sudo apt install flatpak

  
Ative a loja Flathub com o comando abaixo:  
  

  

 flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo

  
  
[](https://draft.blogger.com/null)

### 7\. Instalando Snap no Debian e Fedora

  
Com o suporte ao Snap ativado, vamos na sequência ver quais os procedimentos para instalação e remoção de pacotes Snap no Debian e no Fedora. Tais ações são possíveis tanto via terminal, quando via interface gráfica. Vou mostrar das duas formas:  
  
**7.1. No Debian**  
  
Como exemplo, vou instalar a Snap Store pelo **terminal**:  
  

  

 snap install snap-store

  
Para executar:  
  

  

 snap run snap-store

  
Para remover:  
  

  

 snap remove snap-store

  
**Via Interface Gráfica**  
  
Da maneira como está ativado, há duas maneiras de instalar pacotes Snap no Debian.  
A primeira delas é através da Snap Store _(que já foi instalada no passo anterior)_. Basta abri-la, buscar pelo aplicativo desejado, e instalar o mesmo. A Snap Store lista apenas aplicativos em Snap.  
A segunda maneira é através da própria loja de aplicativos do Gnome, a Gnome Software. Para isto será necessário instalar um plugin para Snap. faça com o comando abaixo:  
  

  

 sudo apt install gnome-software-plugin-snap

  
Após instalar o plugin, abra a Gnome Software (_Programas)_. Neste caso, instalei o Firefox apenas para mostrar que foi uma versão em Snap.  
A animação abaixo mostra o processo.  
  

[![Flatpak e Snap no Debian, Fedora e Ubuntu - Dicas Linux e Windows](https://1.bp.blogspot.com/-Mo2-8MDHtmc/X_EoQuv1GhI/AAAAAAAARd8/rsXz3q23pGsmus7x49mZW76W_rVndDCiwCNcBGAsYHQ/s600/Firefox_SNAP-optimize.gif "Flatpak e Snap no Debian, Fedora e Ubuntu - Dicas Linux e Windows")](https://1.bp.blogspot.com/-Mo2-8MDHtmc/X_EoQuv1GhI/AAAAAAAARd8/rsXz3q23pGsmus7x49mZW76W_rVndDCiwCNcBGAsYHQ/s784/Firefox_SNAP-optimize.gif)

  
**7.2. No Fedora:**  
  
Da mesma forma que fiz no Debian, vou instalar a Snap Store pelo **terminal**. Os comandos de instalação, execução e remoção são exatamente os mesmos que já foram listados no item 7.1.  
  

  

 snap install snap-store

  

  

 snap run snap-store

  

  

 snap remove snap-store

  
**Via Interface Gráfica**  
  
No Fedora - via interface gráfica - podemos utilizar a Snap Store, já instalada acima. Ao contrário do que ocorre no Debian, não há um plugin para a Gnome Software.  
  
[](https://draft.blogger.com/null)

### 8\. Instalando Flatpak no Debian e Ubuntu

  
Agora que o suporte ao Flatpak foi ativado no Debian e no Ubuntu, veremos como instalar e remover pacotes Flatpak nestes dois sistemas, via terminal e via interface gráfica. A fonte dos pacotes será a Flathub, já adicionada no momento em que o suporte foi ativado. Os passos para as duas distribuições são os mesmos e foram testados no Debian Buster e Ubuntu Focal Fossa, ambos com a interface Gnome.  
  
Neste exemplo vou instalar o Inkscape pelo **terminal**. Na instalação via terminal não basta apenas saber o nome do aplicativo, é preciso saber o nome completo. Então, antes do comando de instalação, podemos fazer uma busca com o comando abaixo:  
  

  

 flatpak search inkscape

  
A pesquisa acima terá a saída como a mostrada abaixo:  

[![Flatpak e Snap no Debian, Fedora e Ubuntu - Dicas Linux e Windows](https://1.bp.blogspot.com/-CV5eH2wcyYM/X-5b5tBAB8I/AAAAAAAARcM/XeuDfsg9hkMfnS81Qey1yyVN-rlf4iHEQCNcBGAsYHQ/s16000/001.png "Flatpak e Snap no Debian, Fedora e Ubuntu - Dicas Linux e Windows")](https://1.bp.blogspot.com/-CV5eH2wcyYM/X-5b5tBAB8I/AAAAAAAARcM/XeuDfsg9hkMfnS81Qey1yyVN-rlf4iHEQCNcBGAsYHQ/s726/001.png)

Como podemos ver acima, o nome completo do programa Inkscape é **org.inkscape.Inkscape**.  
  

  

 flatpak install org.inkscape.Inkscape

  
Confirme as eventuais mensagens que podem surgir e pronto, o aplicativo estará instalado.  
  
Para executar:  
  

  

 flatpak run org.inkscape.Inkscape

  
Para remover:  
  

  

 flatpak remove org.inkscape.Inkscape

  
**Via Interface Gráfica**  
  
Da mesma forma que ocorreu com os Snaps, também é possível trabalhar com pacotes Flatpak diretamente na Gnome Software. Basta instalar um plugin para Flatpak, conforme mostrado abaixo.  
  
**Detalhe importante:** No Ubuntu, a Gnome Software não vem instalada por padrão, pois foi substituída pela Ubuntu Software, equivalente à Snap Store. Portanto, ao executar o comando abaixo, a Gnome Software será instalada. Tanto a Gnome Software, quanto a Ubuntu Software tem interfaces quase idênticas, porém, o ícone não é igual e a Gnome Software é chamada de Programas.  
  

  

 sudo apt install gnome-software-plugin-flatpak

  
  
Após instalar o plugin, abra a Gnome Software (_Programas)_. No exemplo instalei o aplicativo Cheese em Flatpak.  
A animação abaixo mostra o processo de instalação.  
  

[![Flatpak e Snap no Debian, Fedora e Ubuntu - Dicas Linux e Windows](https://1.bp.blogspot.com/-RSmWd4ZnkWw/X_En2iuvjWI/AAAAAAAARd0/0RSce99zrTEG6_hFwPj2K9UvDrPd61akgCNcBGAsYHQ/s600/Cheese_FLATPAK-optimize.gif "Flatpak e Snap no Debian, Fedora e Ubuntu - Dicas Linux e Windows")](https://1.bp.blogspot.com/-RSmWd4ZnkWw/X_En2iuvjWI/AAAAAAAARd0/0RSce99zrTEG6_hFwPj2K9UvDrPd61akgCNcBGAsYHQ/s782/Cheese_FLATPAK-optimize.gif)

  
[](https://draft.blogger.com/null)

### 9\. Considerações Finais

  
Minha opinião é que utilizar pacotes em Snap ou Flatpak deve ocorrer apenas em casos pontuais, quando o usuário precisa de um aplicativo numa versão atualizada e a distribuição do usuário não tem este aplicativo no repositório, ou quando não o aplicativo não existe para aquela distribuição. Fora estes dois casos, eu prefiro sempre utilizar a versão disponível nos repositórios tradicionais da distribuição. Mas é apenas a minha opinião de acordo com as minhas necessidades como usuário.  
  
Uma última observação: O objetivo desta matéria foi mostrar o básico de como trabalhar com pacotes nos formatos descritos, mostrando apenas como instalar, executar e remover. Porém, há diversas outras opções que permitem ao usuário diversas ações de manipulação destes pacotes no sistema. Caso o usuário esteja a fim de se aprofundar nos assuntos, deixei alguns links como referência da matéria e há uma quantidade imensa de informações na internet.  
  
[](https://draft.blogger.com/null)

### 10\. Referências

  
[http://guialinux.uniriotec.br/snap/](http://guialinux.uniriotec.br/snap/)[https://docs.flatpak.org/en/latest/index.html](https://docs.flatpak.org/en/latest/index.html)  
[https://snapcraft.io/docs](https://snapcraft.io/docs)  
[https://snapcraft.io/docs/getting-started](https://snapcraft.io/docs/getting-started)  
[https://guiafoca.org/guiaonline/inicianteintermediario/](https://guiafoca.org/guiaonline/inicianteintermediario/)