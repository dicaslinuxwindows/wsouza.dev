---
title: 'Fedora 33 Beta'
date: 2020-10-07T00:05:00.003-03:00
draft: false
url: /2020/10/fedora-33-beta.html
tags: 
- Linux
- Fedora 33
- Fedora
---

![Fedora 33 Beta - Dicas Linux e Windows](https://1.bp.blogspot.com/-tpCRbqXKdGM/X30vwWI-3oI/AAAAAAAAQOc/CQcSwFz16IgOe_jJkyHzhPf1q8hh5_nFQCNcBGAsYHQ/s16000/Fedora%2B33%2BBeta.png "Fedora 33 Beta - Dicas Linux e Windows")

Na semana passada foi disponibilizada a versão beta do Fedora 33, distribuição Linux desenvolvida pela comunidade do Projeto Fedora. Saiba mais na matéria abaixo.

  
  
  
  
  
  

### Fedora

  
É a primeira vez que falo alguma coisa sobre o Fedora aqui no blog. Como de costume, só falo aqui sobre sistemas e aplicativos que utilizo, e o motivo de nunca ter falado sobre o Fedora era exatamente por nunca tê-lo utilizado. Esta situação mudou há alguns meses, quando resolvi instalar a versão 32 por curiosidade.  
Segue uma breve história do sistema:  
O Fedora é desenvolvido pela comunidade do Projeto Fedora e é um projeto patrocinado pela Red Hat _(hoje adquirida pela IBM)_, que desenvolvia o sistema de mesmo nome. No começo dos anos 2000 o Red Hat passou a se concentrar na versão corporativa do sistema, com suporte pago e etc... A partir daí a Red Hat dá suporte ao projeto Fedora e o Fedora passou a ser, grosseiramente falando, a versão doméstica, desktop, do Red Hat Enterprise.  
Alguns pontos a destacar:

*   O Fedora Workstation _(que é a versão padrão)_ utiliza o GNOME como interface gráfica padrão, mas é claro que podemos instalar outras interfaces. Uma coisa interessante é que o GNOME apresentado pelo Fedora é o GNOME puro, sem modificações, e geralmente é a versão estável mais recente. Quando falo de modificações no GNOME me refiro àquelas como a Canonical faz no Ubuntu, que geralmente facilitam a vida dos usuários;
*   Os pacotes são os _.rpm_, que geralmente são lançadas versões de aplicativos conhecidos para este formato, até mais que para os pacotes _.deb_. Os pacotes _.rpm_ são utilizados por diversas distribuições;
*   Um dos gerenciadores de pacote do Fedora _(equivalente ao Synaptic do Debian e Ubuntu)_ é o DNF Dragora;
*   Também há o suporte para instalação de pacotes Flatpak _(ainda vou falar deles com mais detalhes aqui no blog)_;
*   O _dnf_ é o "equivalente" ao _apt_ dos sistemas baseados no Debian;

  

### Fedora 33 Beta

  
Após uma breve introdução, vamos ao motivo principal desta matéria, que é o lançamento do beta da versão 33. Ainda neste mês será lançada a versão final, provavelmente no dia 20/10/2020. Porém, quem se interessar já pode baixar e instalar a versão beta. Seguem alguns destaques desta versão:  

*   O GNOME e seus aplicativos padrão vem na versão 3.38. Um detalhe é que algumas extensões ainda podem não estar funcionando corretamente no GNOME 3.38, o que pode tornar a experiência um pouco frustante. O GNOME sem algumas extensões _(DashToDock, por exemplo)_ não facilita a vida dos usuários;
*   Kernel 5.8;
*   Firefox 81;
*   Libre Office 7.0.12;
*   O tema padrão é o Adwaita;
*   O sistema de arquivos padrão será o BTRFS, que pode trazer alguns ganhos de performance em comparação ao sistema de arquivos EXT4, que era o padrão na versão anterior;
*   Como citei no início, esta é uma versão pura do GNOME. quem está acostumado ao Ubuntu sentirá a falta de muitos aplicativos, mas nada que um _**sudo dnf install**_ não resolva.

  

#### Download

  
Baixe e instale o Fedora 33 Beta. Note que é uma versão de testes, sujeita à bugs. Se você instalar esta versão, não será necessário um novo download quando a versão final for lançada, pois basta manter esta versão atualizada. Os links abaixo apontam para a versão Workstation e uma instalação de rede, Netinstall.  
  

Fedora 33 Beta

[ Workstation](https://download.fedoraproject.org/pub/fedora/linux/releases/test/33_Beta/Workstation/x86_64/iso/Fedora-Workstation-Live-x86_64-33_Beta-1.3.iso)

[ Netinstall](https://download.fedoraproject.org/pub/fedora/linux/releases/test/33_Beta/Everything/x86_64/iso/Fedora-Everything-netinst-x86_64-33_Beta-1.3.iso)

[Mais...](https://getfedora.org/workstation/download/)

  

#### Fedora 33 em funcionamento

  
O vídeo abaixo mostra o Fedora 33 Beta em funcionamento:  
  

  

### Considerações finais

  
Meu primeiro contato com o "mundo Linux" foi lá em 2004/2005 com o antigo Conectiva Linux, que utilizava pacotes _.rpm_. Este contato durou muito pouco tempo e depois passei a utilizar apenas distribuições baseadas no Debian. Para que está acostumado com os pacotes _.deb_ e comando _apt_, pode ser um pouco estranho no começo, mas nada demais. Confesso que a experiência vem sendo bem interessante e pretendo falar mais vezes por aqui sobre o Fedora.