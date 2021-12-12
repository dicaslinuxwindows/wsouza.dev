---
title: 'Como conseguir a versão mais recente do Ubuntu em 32 bits'
date: 2018-11-19T12:29:00.004-02:00
draft: false
url: /2018/11/como-conseguir-versao-mais-recente-do-ubuntu-32-bits.html
tags: 
- Linux
- Ubuntu
- Tutoriais
---

![Como conseguir a versão mais recente do Ubuntu em 32 bits - Dicas Linux e Windows](https://3.bp.blogspot.com/-yMpE7mq2Tfg/XImv9mEmdiI/AAAAAAAAKz8/ll1CTOjYOJQJZW9e5IflLmb-lgi2HbiUgCLcBGAs/s200/32BITS.png "Como conseguir a versão mais recente do Ubuntu em 32 bits - Dicas Linux e Windows")

As versões mais recentes do Ubuntu, 18.04 (LTS) e 18.10 não possuem imagens ISO 32 bits, que são para computadores mais antigos. Mas, como fazer para "rodar" as últimas versões do Ubuntu em 32 bits?  
Confira na dica a seguir.

  
  
  
  
  

### Entendendo o problema

  
A partir da versão 18.04, a Canonical, desenvolvedora do Ubuntu, deixou de fornecer imagens de seus lançamentos em 32 bits. Isto dificultou a vida de quem possui computadores mais antigos e desejam testar o sistema, ou mesmo para quem utiliza em máquinas virtuais, que por algum motivo não aceitam versões 64 bits.  
  

### Como resolvê-lo?

  
_**Atualizado em 08/07/2020:**_  
  
Outra solução é a que foi sugerida no comentário da matéria. O [Xubuntu](http://mirror.aarnet.edu.au/pub/xubuntu/releases/18.04/release/xubuntu-18.04.4-desktop-i386.iso), [Lubuntu](http://cdimage.ubuntu.com/lubuntu/releases/18.04/release/lubuntu-18.04.4-desktop-i386.iso) e [Ubuntu Mate](http://cdimage.ubuntu.com/ubuntu-mate/releases/18.04/release/ubuntu-mate-18.04.4-desktop-i386.iso), na versão 18.04 LTS, ainda possuem imagens para sistemas 32 bits. Baixe e instale uma destas versões, depois instale o Gnome, e assim, estará com uma versão recente e em 32 bits do Ubuntu padrão.  
  
A dica para resolver este problema é simples, porém, um pouco trabalhosa devido ao tempo e quantidade de downloads.  
Baixe a versão LTS 16.04, que foi a última a ser lançada em ISO de 32 bits, e instale. Após a instalação, o próprio sistema alertará a opção de atualizar para a próxima versão LTS, que é a 18.04. Faça a atualização. Simples assim e você já possuirá a versão LTS mais recente em seu computador de 32 bits.  
Se deseja a versão mais recente não LTS, que é a 18.10, faça da seguinte forma:  
Após a atualização para a 18.04, faça uma nova atualização do sistema. _(lembre-se de trocar os repositórios em /etc/apt/sources.list)_.  
  

### Considerações finais

  
1 - Para baixar o Ubuntu 16.04, entre em [http://releases.ubuntu.com/16.04/](http://releases.ubuntu.com/16.04/) e escolha a opção _32-bit PC (i386) desktop image_.  
2 - Não entrei no mérito dos requisitos de hardware para suportar as versões mais recentes do Ubuntu. Mas quem pretende utilizá-las deve saber que o desempenho poderá não ser satisfatório em computadores com até 2Gb de RAM _(que é o caso de boa parte dos que necessitam utilizar um sistema 32 bits)._  
3 - Para a dica acima, considerei que você possui conhecimento em instalação e atualização de sistemas Linux.  
4 - Se deseja ter estas versões (18.04 e 18.10) as futuras versões em 32 bits para alguma futura utilização, sem que seja preciso esta trabalheira toda, é possível fazer um backup do sistema utilizando o Remaster-GTK. _([Veja aqui como fazer](https://info.wsouza.com.br/2018/07/backup-com-remaster-gtk.html))_.  
5 - Não se sabe exatamente até quando haverá suporte para as versões 32 bits, pois o Ubuntu Mate, por exemplo, não suportará mais esta arquitetura a partir da versão 18.10. Acredito que o 18.04, por ser LTS, vai manter o suporte durante todo seu ciclo.