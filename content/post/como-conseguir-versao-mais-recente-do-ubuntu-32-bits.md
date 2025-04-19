---
title: 'Como conseguir a versão mais recente do Ubuntu em 32 bits'
date: 2018-11-19T12:29:00.004-02:00
draft: false
url: /2018/11/como-conseguir-versao-mais-recente-do-ubuntu-32-bits.html
categories: 
- Tutoriais
tags:
- Ubuntu
- Arquiteturas
- 32-bits
socialshare: true
---

As versões mais recentes do Ubuntu, 18.04 (LTS) e 18.10 não possuem imagens ISO 32 bits, que são para computadores mais antigos. Mas, como fazer para "rodar" ~~as últimas versões do~~ o Ubuntu em 32 bits? 
Confira nas dicas a seguir. 

<!--more-->

<b><i><font color="red">
_Matéria atualizada em 10/01/2022_

NOTA: Com as dicas apresentadas nesta matéria só é possível ter o Ubuntu em 32 bits até a versão 18.04 LTS, que terá suporte até meados de 2023.</font></i></b>

## Entendendo o problema

  
A partir da versão 18.04, a Canonical, desenvolvedora do Ubuntu, deixou de fornecer imagens de seus lançamentos em 32 bits. Isto dificultou a vida de quem possui computadores mais antigos e desejam testar o sistema, ou mesmo para quem utiliza em máquinas virtuais, que por algum motivo não aceitam versões 64 bits.  
  
## Solução 1

A dica para resolver este problema é simples, porém, um pouco trabalhosa devido ao tempo e quantidade de downloads.  
Baixe a versão LTS 16.04, que foi a última a ser lançada em ISO de 32 bits, e instale. Após a instalação, o próprio sistema alertará a opção de atualizar para a próxima versão LTS, que é a 18.04. Faça a atualização. Simples assim e você já possuirá a versão LTS mais recente em seu computador de 32 bits.  

Para baixar o Ubuntu 16.04, entre em [http://releases.ubuntu.com/16.04/](http://releases.ubuntu.com/16.04/) e escolha a opção _32-bit PC (i386) desktop image._

## Solução 2
  
Outra solução é a que foi sugerida no comentário da matéria. O [Xubuntu](https://cdimage.ubuntu.com/xubuntu/releases/18.04/release/), [Lubuntu](https://cdimage.ubuntu.com/lubuntu/releases/18.04/release/) e [Ubuntu Mate](https://cdimage.ubuntu.com/ubuntu-mate/releases/18.04/release/), na versão 18.04 LTS _( escolha 32-bit PC (i386))_, ainda possuem imagens para sistemas 32 bits. Baixe e instale uma destas versões.
Após a instalação, instale o Gnome, e assim, estará com uma versão recente e em 32 bits do Ubuntu padrão.

Para instalar o Gnome, execute o comando abaixo no terminal e aguarde a conclusão.

`sudo apt install ubuntu-gnome-desktop`

## Considerações finais

1. Não entrei no mérito dos requisitos de hardware para suportar as versões mais recentes do Ubuntu. Mas quem pretende utilizá-las deve saber que o desempenho poderá não ser satisfatório em computadores com até 2Gb de RAM _(que é o caso de boa parte dos que necessitam utilizar um sistema 32 bits)._  
1. Para a dica acima, considerei que você possui conhecimento em instalação e atualização de sistemas Linux.  
3. Se deseja ter estas versões (18.04 e 18.10) as futuras versões em 32 bits para alguma futura utilização, sem que seja preciso esta trabalheira toda, é possível fazer um backup do sistema utilizando o Remaster-GTK. _([Veja aqui como fazer](https://info.wsouza.com.br/2018/07/backup-com-remaster-gtk.html))_.  
4. Não se sabe exatamente até quando haverá suporte para as versões 32 bits, pois o Ubuntu Mate, por exemplo, não suportará mais esta arquitetura a partir da versão 18.10. Acredito que o 18.04, por ser LTS, vai manter o suporte durante todo seu ciclo.
