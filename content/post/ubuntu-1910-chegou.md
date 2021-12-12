---
title: 'Ubuntu 19.10 chegou'
date: 2019-10-18T11:31:00.000-03:00
draft: false
url: /2019/10/ubuntu-1910-chegou.html
tags: 
- Linux
- Ubuntu
- Ubuntu 19.10
---

[![Ubuntu 19.10 chegou - Dicas Linux e Windows](https://4.bp.blogspot.com/-xT53CwOc4fY/XaiZWAG3wlI/AAAAAAAAMbM/ouBAGaaGJEcQs29MnFOkDcjiQ1VQ2DaVACNcBGAsYHQ/s200/19.10-ermine-wallpaper.jpg "Ubuntu 19.10 chegou - Dicas Linux e Windows")](https://4.bp.blogspot.com/-xT53CwOc4fY/XaiZWAG3wlI/AAAAAAAAMbM/ouBAGaaGJEcQs29MnFOkDcjiQ1VQ2DaVACNcBGAsYHQ/s1600/19.10-ermine-wallpaper.jpg)

No dia 17 de outubro de 2019 foi lançado o Ubuntu 19.10, chamado de _Eoan Ermine._ Esta é a última versão antes do próximo LTS. Veja aqui o que o _Eoan Ermine_ traz de novidades e como obtê-lo.

  
  
  
  
  

### Sobre o Ubuntu

  
O Ubuntu é um sistema operacional de código aberto, construído a partir do Kernel Linux. É desenvolvido por uma empresa chamada Canonical, é baseado no Debian, uma das mais antigas distribuições Linux e pai de várias distribuições Linux. Sua primeira versão foi lançada em 2004 e agora chega na versão 19.10, que terá suporte até julho de 2020. Saiba mais sobre o Ubuntu, seu suporte e ciclo de vida em: [Ubuntu - Como funciona a política de seu ciclo de vida](https://info.wsouza.com.br/2019/03/ubuntu-como-funciona-politica-de-seu-ciclo-de-vida.html).

  

### Quais são as novidades que virão com o Eoan Ermine?

  
Como citei anteriormente, esta é a última das 3 versões intermediárias lançadas entre uma versão LTS. As versões intermediárias contém os pacotes estáveis mais recentes, que funcionam como um teste para o que será lançado no próximo LTS. Dentre as novidades que chegam com o Ubuntu Eoan Ermine estão:  

*   Kernel 5.3;
*   Gnome 3.34 - o gerenciador padrão do Ubuntu com os pacotes básicos para o funcionamento da interface gráfica. Esta nova versão traz _(entre outras coisas)_ melhorias no Gnome Music, Gnome Fotos, possibilidade de criar pastas no Dash, correção de bugs, melhorias nas configurações do plano de fundo, facilitando a seleção de papéis de parede personalizados;
*   Tema Yaru, que já foi o padrão na versão anterior, agora traz variações clara e escura;
*   O navegador padrão é o Firefox, que chega em sua versão 69;
*   O LibreOffice, suíte de aplicativos de escritório, chega na versão 6.3;
*   Cliente de email Thunderbird na versão 68;
*   Suporte ao sistema de arquivos ZFS _(Em caráter experimental);_
*   Boot mais rápido;
*   Aplicativos 32 bits como Wine e Steam continuam firmes e fortes no sistema, confirmando o que foi anunciado em Junho/2019, quando a [Canonical voltou atrás na decisão que havia tomado em não dar suporte aos aplicativos de 32 bits no Ubuntu](https://info.wsouza.com.br/2019/06/canonical-recua-e-nao-removera-os-pacotes-32-bits-do-ubuntu.html);
*   Inclusão dos drivers proprietários da NVIDIA na ISO de instalação. Tal inclusão é muito interessante pois a GPU será reconhecida já no momento da inicialização do sistema pelo modo _Live_.

  

  

### Como obter o Ubuntu Eoan Ermine?

  
Há duas formas de obtê-lo: Por meio de atualização ou instalando do zero _(instalação limpa)_.  
  
Para obter através de atualização aguarde a mensagem do atualizador do sistema ou siga os 3 próximos passos:  
  
Atualize os repositórios:  
  

 sudo apt update

  
Atualize os pacotes da versão atual:  
  

 sudo apt full-upgrade

  
Se não deu erro na saída após utilizar o comando anterior, atualize a versão do sistema:  
  

 sudo do-release-upgrade -c -d

  
Detalhe: Após iniciada a atualização não é possível interrompê-la. Caso interrompida, o sistema irá quebrar e não será possível utilizá-lo.  
  
A maneira mais recomendável utilizar a instalação limpa, pois praticamente não há chances de quebrar o sistema. O problema da instalação limpa é que você irá perder os aplicativos instalados e suas configurações pessoais _(caso a pasta pessoal não esteja numa partição separada)_. Para fazer uma instalação limpa, baixe uma imagem ISO _(ver links para download abaixo)_, grave num CD/DVD ou pendrive e instale.  
Não recomendo instalar esta versão no computador que você utiliza diariamente, pois seu suporte irá durar apenas 9 meses, portanto, teste numa máquina virtual. Veja como fazer isto em: [Máquina Virtual: Instalando e configurando o VMware Player](https://info.wsouza.com.br/2018/07/maquina-virtual-instalando-e-configurando-o-wmware-player.html) e em [Máquina Virtual: Instalando e configurando o sistema no VMware](https://info.wsouza.com.br/2018/08/maquina-virtual-instalando-e-configurando-o-sistema-no-vmware.html).  
Também é possível testar pelo CD/DVD ou pendrive, sem necessidade de instalação.

  

### Download

  
Baixe a imagem ISO da interface que mais lhe agradar:  
  

[ Ubuntu](https://ubuntu.com/download/desktop/thank-you/?version=19.10&architecture=amd64)

[ Xubuntu](http://cdimage.ubuntu.com/xubuntu/releases/19.10/release/xubuntu-19.10-desktop-amd64.iso)

[ Kubuntu](http://cdimage.ubuntu.com/kubuntu/releases/19.10/release/kubuntu-19.10-desktop-amd64.iso)

[ Ubuntu Mate](http://cdimage.ubuntu.com/ubuntu-mate/releases/19.10/release/ubuntu-mate-19.10-desktop-amd64.iso)

[ Lubuntu](http://cdimage.ubuntu.com/lubuntu/releases/19.10/release/lubuntu-19.10-desktop-amd64.iso)