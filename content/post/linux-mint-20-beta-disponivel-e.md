---
title: 'Linux Mint 20: Beta disponível e polêmica com pacotes Snap'
date: 2020-06-12T23:05:00.000-03:00
draft: false
url: /2020/06/linux-mint-20-beta-disponivel-e.html
tags: 
- Linux
- Linux Mint
---

![](https://2.bp.blogspot.com/-Fr_JhHnX1_w/Xuq7hVJxZfI/AAAAAAAAPIQ/4jdjFOav-tkvg1pYNpdzeq8JLOOq8m5mACNcBGAsYHQ/s1600/Linux_Mint_Beta.png)

A data de lançamento do Linux Mint 20 está se aproximando e o sistema vai tomando forma.  
Confira aqui as últimas novidades e a "polêmica" sobre o uso dos pacotes Snap do Ubuntu.

  
  
  
  
  

### O que sabemos sobre o LM20 até agora.

  
A matéria de 1º de abril "[Linux Mint 20 Ulyana](https://info.wsouza.com.br/2020/04/linux-mint-20-ulyana.html)" abordou sobre o que se sabia a respeito do LM20 até aquele momento, como seu codinome que será Ulyana e que este seria baseado no Ubuntu 20.04 LTS.  
Após mais de dois meses, e com o lançamento do mesmo se aproximando, surge mais algumas informações sobre o que encontraremos no Linux Mint 20 - Ulyana.  

*   Beta disponível _(Veja no final como obter)_;
*   Kernel 5.4. Para efeitos de comparação, o Debian Buster utiliza a versão 4.19, e a versão mais atual é a 5.7;
*   Nova ferramenta de transferência de arquivos pela rede com criptografia chamada Warpinator. Esta ferramenta foi desenvolvida para o Linux Mint, ou seja, não é derivada do Ubuntu;
*   Os usuários que possuem placas de vídeo híbridas _(ex: Nvidia + Intel)_ terão como iniciar aplicativos utilizando a placa que desejar, graças ao suporte aprimorado para o Nvidia Optimus.
*   Melhorias no aplicativo bandeja do sistema;

Os destaques acima somam-se com os destaques que já comentados na matéria anterior, que são:  

*   Melhorias no suporte à vários monitores;
*   Melhorias que tornam o gerenciador de arquivos Nemo mais rápido;
*   Suporte à escala fracionada;
*   Novos temas de cores;
*   Melhorias na taxa de atualização do monitor;

  

### Pacotes Snap no Linux Mint 20

  
O Linux Mint 20, a princípio, não permitirá a instalação dos pacotes Snap do Ubuntu via _apt install snapd_. Tal decisão ocorreu pelo fato dos desenvolvedores do Mint não concordarem com a maneira que a Canonical _(desenvolvedora do Ubuntu)_ está trabalhando com esses pacotes, forçando os usuários a utilizá-los.  
O exemplo utilizado pelos desenvolvedores do Mint foi o Chromium que no Ubuntu é forçado a ser instalado via Snap, pois o pacote _.deb_ encontra-se vazio. Segundo o pessoal do Mint, tal situação ocorre sem que o usuário seja avisado.  
Mas Canonical ainda tenta convencer os desenvolvedores do Mint para que mudem de ideia, então, muita coisa ainda pode acontecer.  
Aos que quiserem utilizar os pacotes Snap no LM20, há uma solução alternativa. Segundo uma dica divulgada no [omg! ubuntu!](https://www.omgubuntu.co.uk/2020/06/enable-snap-apps-linux-mint-20), basta remover o arquivo responsável pelo bloqueio do snapd. O tal arquivo é o _nosnap.pref_.  
Para evitar problemas futuros, podemos apenas renomear este arquivo e, assim podemos reativá-lo caso seja necessário. Para renomeá-lo basta usar os comandos abaixo, renomeando-o para _nosnap.pref.old_.  
  

 sudo su

  

 cd /etc/apt/preferences.d/

  

 mv nosnap.pref nosnap.pref.old

  
Caso precise do arquivo antigo, basta renomeá-lo novamente para _nosnap.pref_. Para instalar o snapd, use os comandos abaixo e o suporte aos aplicativos Snap estará ativo nomamente.  
  

 sudo apt update

  

 sudo apt install snapd

  

### Download da versão Beta

  
Seguem os links para o download da versão beta. Vale lembrar que por se tratar de uma versão de testes ainda podem aparecer sérios bugs, portanto, não utilize como sistema operacional principal.  
  

Linux Mint 20 Beta

[ Cinnamon](https://mirrors.edge.kernel.org/linuxmint/testing/linuxmint-20-cinnamon-64bit-beta.iso)

[ Mate](https://mirrors.edge.kernel.org/linuxmint/testing/linuxmint-20-mate-64bit-beta.iso)

[ XFCE](https://mirrors.edge.kernel.org/linuxmint/testing/linuxmint-20-xfce-64bit-beta.iso)

  
  
Fonte: [Blog do Linux Mint](https://blog.linuxmint.com/?p=3906)