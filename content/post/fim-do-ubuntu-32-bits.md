---
title: '[Atualizado] Fim do Ubuntu 32 bits'
date: 2019-06-20T19:41:00.004-03:00
draft: false
url: /2019/06/fim-do-ubuntu-32-bits.html
tags: 
- Linux
- Ubuntu
---

  

![Fim do Ubuntu 32 bits - Dicas Linux e Windows](https://1.bp.blogspot.com/-4YlrSmUIXuc/XRQRvZHlBbI/AAAAAAAALtc/mT_UooJe6lAoe7zxY32v8-HdKYx41R6JwCLcBGAs/s1600/32BITSX.png "Fim do Ubuntu 32 bits - Dicas Linux e Windows")

  

Se você ainda utiliza o Ubuntu 32 bits saiba que a Canonical vai descontinuar o suporte à estas versões. Veja mais detalhes a seguir.  
_Atualizado: Canonical recuou a respeito desta decisão. Leia em [Canonical recua e não removerá os pacotes 32bits do Ubuntu](https://info.wsouza.com.br/2019/06/canonical-recua-e-nao-removera-os-pacotes-32-bits-do-ubuntu.html)_

  
  
  
  

### Ubuntu 32 bits

  
O Ubuntu com arquitetura 32 bits (i386, x86) é geralmente utilizado em dispositivo mais antigos, que possuem ate 2Gb de memória RAM, algo pouco comum atualmente. Porém, por vários motivos ainda há quem utilize o sistema da Canonical com esta arquitetura. Desde a versão 18.04 LTS a empresa não disponibiliza as imagens de instalação _(ISO)_ para esta arquitetura, já sinalizando que o fim poderia estar próximo. A última ISO de 32 bits lançada foi a da versão 16.04 e era necessário alguns passos para obter a versão 18.04, como foi mostrado em [como conseguir a versão mais recente do Ubuntu em 32 bits](https://info.wsouza.com.br/2018/11/como-conseguir-versao-mais-recente-do-ubuntu-32-bits.html).

  

### Fim do suporte. E agora?

  
A notícia sobre o fim do suporte ao 32 bits foi revelada nesta semana, através de conversas em listas de discussão do Ubuntu. Segundo o conteúdo desta lista, há mais de 1 ano já havia a intenção de descontinuar o suporte ao 32 bits e concentrar os esforços no 64 bits, que tem uma quantidade de usuários imensamente maior. Manter suporte às duas arquiteturas estava se tornando inviável, gerando custos adicionais à empresa _(lembre-se que a Canonical é uma empresa, que visa lucro)_, que precisava manter a mesma quantidade de pessoas que são ligados à arquitetura 64 bits.  
A partir da versão 19.10, que será lançada em outubro, já não será construído, empacotado ou distribuído nenhum pacote de 32 bits e não será possível atualizar para esta versão. Portanto, se você está utilizando o 18.04 LTS, 18.10 ou 19.04, na arquitetura 32 bits, será impossível sair desta versão para a 19.10 e para a 20.04, que será lançada em abril de 2020 e será LTS. _(Em caso de dúvidas sobre as versões do Ubuntu, veja [Ubuntu - Como funciona a política de seu ciclo de vida](https://info.wsouza.com.br/2019/03/ubuntu-como-funciona-politica-de-seu-ciclo-de-vida.html))_.  
  
Mas nem tudo é motivo pra desespero. O suporte continuará enquanto durar o ciclo da versão 18.04, que se encerrará em abril de 2023, portanto, se está utilizando alguma versão anterior, atualize para a 18.04.  
Esta decisão da Canonical vai se estender ao Kubuntu, Xubuntu, Lubuntu e provavelmente ao Ubuntu Mate. Também serão afetadas as distribuições derivadas como o Linux Mint, por exemplo. Problemas pontuais poderão surgir com aplicativos de terceiros, que poderão deixar de prestar suporte ao 32 bits.  
Segue na íntegra o conteúdo divulgado nesta semana nas listas de discussão do Ubuntu:  
  

> _i386 architecture will be dropped starting with eoan (Ubuntu 19.10)  
> Steve Langasek steve.langasek at ubuntu.com  
> Tue Jun 18 15:36:45 UTC 2019  
>   
> Messages sorted by: \[ date \] \[ thread \] \[ subject \] \[ author \]  
>   
> Last year, the Ubuntu developer community considered the question of whether  
> to continue carrying forward the i386 architecture in the Ubuntu archive for  
> future releases.\[1\] The discussion at the time was inconclusive, but in  
> light of the strong possibility that we might not include i386 as a release  
> architecture in 20.04 LTS, we took the proactive step to disable upgrades  
> from 18.04 to 18.10 for i386 systems\[2\], to avoid accidentally stranding  
> users on an interim release with 9 months of support instead of letting them  
> continue to run Ubuntu 18.04 LTS with its 5 years of standard support.  
>   
> In February of this year, I also posted to communicate the timeline in which  
> we would take a final decision about i386 support in 20.04 LTS\[3\], namely,  
> that we would decide in the middle of 2019.  
>   
> The middle of 2019 has now arrived. The Ubuntu engineering team has  
> reviewed the facts before us and concluded that we should not continue to  
> carry i386 forward as an architecture. Consequently, i386 will not be  
> included as an architecture for the 19.10 release, and we will shortly begin  
> the process of disabling it for the eoan series across Ubuntu  
> infrastructure.  
>   
> While this means we will not provide 32-bit builds of new upstream versions  
> of libraries, there are a number of ways that 32-bit applications can  
> continue to be made available to users of later Ubuntu releases, as detailed  
> in \[4\]. We will be working to polish the 32-bit support story over the  
> course of the 19.10 development cycle. To follow the evolution of this  
> support, you can participate in the discourse thread at \[5\].  
>   
> \[1\] [https://lists.ubuntu.com/archives/ubuntu-devel/2018-May/040310.html](https://lists.ubuntu.com/archives/ubuntu-devel/2018-May/040310.html)  
> \[2\] [https://launchpad.net/ubuntu/+source/ubuntu-release-upgrader/1:18.10.10](https://launchpad.net/ubuntu/+source/ubuntu-release-upgrader/1:18.10.10)  
> \[3\] [https://lists.ubuntu.com/archives/ubuntu-devel/2019-February/040598.html](https://lists.ubuntu.com/archives/ubuntu-devel/2019-February/040598.html)  
> \[4\] [https://lists.ubuntu.com/archives/ubuntu-devel/2018-May/040348.html](https://lists.ubuntu.com/archives/ubuntu-devel/2018-May/040348.html)  
> \[5\] [https://discourse.ubuntu.com/t/i386-architecture-will-be-dropped-starting-with-eoan-ubuntu-19-10/11263/2](https://discourse.ubuntu.com/t/i386-architecture-will-be-dropped-starting-with-eoan-ubuntu-19-10/11263/2)  
>   
> \--  
> Steve Langasek  
> \-------------- next part --------------  
> A non-text attachment was scrubbed...  
> Name: signature.asc  
> Type: application/pgp-signature  
> Size: 833 bytes  
> Desc: not available  
> URL:  
>   
> Messages sorted by: \[ date \] \[ thread \] \[ subject \] \[ author \]  
>   
> More information about the ubuntu-devel-announce mailing list  
> _