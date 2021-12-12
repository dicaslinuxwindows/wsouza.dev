---
title: 'Máquina Virtual: Instalando e configurando o VMware Player'
date: 2018-07-25T02:15:00.004-03:00
draft: false
url: /2018/07/maquina-virtual-instalando-e-configurando-o-wmware-player.html
tags: 
- Linux
- Máquina Virtual
- Tutoriais
- VMware Player
- Ferramentas Linux
---

Neste post iremos falar sobre máquinas virtuais. Veremos como instalar e configurar uma Máquina Virtual (VM), para posterior instalação de um sistema operacional (SO) e, para isto, utilizaremos o VMware Workstation Player instalado no Debian.

  
  
  

A utilização de uma máquina virtual torna-se muito importante quando, por exemplo, o usuário deseja ou precisa testar algum sistema que por algum motivo não pode ser executado num Live CD/DVD. Ou quando este deseja/precisa instalar o Windows para ter um acesso rápido.  

####   
1 - Introdução

  
O conceito de máquina virtual _(VM)_ é um software que emula as funções de um computador, permitindo que outro (s) SO (s) _(convidado)_ sejam instalados dentro de um SO hospedeiro. Existem várias VMs e a mais conhecida entre os usuários Linux é o [Virtual Box](https://info.wsouza.com.br/2021/01/instalar-o-virtualbox-em-qualquer-distribuicao-linux.html), que possui uma grande quantidade de recursos. A opção pela utilização do VMware Workstation Player foi meramente por estar mais acostumado ao uso. Vale ressaltar que este é um software proprietário e pago, sendo que a versão player é de uso gratuito para usuários domésticos.

  

####   
2 - Instalação

  
Baixe a VM, na versão 12, [neste link](https://my.vmware.com/en/web/vmware/free#desktop_end_user_computing/vmware_workstation_player/12_0).  
Se preferir, baixe a 14 [neste link](https://my.vmware.com/en/web/vmware/free#desktop_end_user_computing/vmware_workstation_player/14_0), porém aqui utilizaremos a 12, mas a idéia é a mesma.  
Baixe na pasta de seu usuário _(/home/nomedeseuusuario)_ e não renomeie o arquivo.  
  
Para instalar vá no terminal _(CTRL+T)_ e digite o comando a seguir, que dará a permissão de execução do arquivo:  
  

 sudo chmod +x vmware/VMware-Player-12.5.9-7535481.x86\_64.bundle

  
Em seguida,ainda no terminal, execute o comando abaixo, que instalará a VM:  
  

 sudo ./VMware-VIX-1.15.8-5528349.x86\_64.bundle

  
A instalação iniciará, aceite os termos e avance até o final para concluir a instalação.  
Após o término, para abrir, procure no menu de aplicações algo parecido com o que está na imagem abaixo.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://3.bp.blogspot.com/-xZa9b2dZtv4/W1fnKuVulqI/AAAAAAAAIu0/0Pn1454DfAoL7D87HV8_8YzsfP97YtJ0QCLcBGAs/s400/10.png "Ferramentas Linux 3 - Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://3.bp.blogspot.com/-xZa9b2dZtv4/W1fnKuVulqI/AAAAAAAAIu0/0Pn1454DfAoL7D87HV8_8YzsfP97YtJ0QCLcBGAs/s1600/10.png)

  
Interface inicial do WMware Wokstation Player 12.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://4.bp.blogspot.com/-lu5r2gB_Eoc/W1fBAw3trII/AAAAAAAAIus/9BAVWPmXn7wD3lV-qIRe1fz3oE75fFbxACPcBGAYYCw/s640/06.png "Ferramentas Linux 3 - Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://4.bp.blogspot.com/-lu5r2gB_Eoc/W1fBAw3trII/AAAAAAAAIus/9BAVWPmXn7wD3lV-qIRe1fz3oE75fFbxACPcBGAYYCw/s1600/06.png)

  

#### 3 - Configuração

  
A partir deste ponto iniciaremos a configuração da VM para receber um SO. Não será abordada a instalação do sistema, isto ficará para uma próxima oportunidade, visto que o objetivo do tópico é apenas de instalação e configuração da VM.  
Crie uma nova máquina virtual na opção Create a New Virtual Machine.  
Ao criar a VM, o primeiro passo é escolher de onde virá o sistema a ser instalado. Você poderá escolher do drive de CD/DVD do sistema hospedeiro, ou poderá escolher uma imagem .ISO . Normalmente escolho uma imagem .ISO pois torna a instalação mais rápida. Se preferir poderá escolhe o sistema em outro momento. Neste caso o sistema escolhido foi o Lubuntu 18.04 LTS.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://4.bp.blogspot.com/-rBVTH7-Cmyk/W1fr0Yw3ycI/AAAAAAAAIvI/EfuhC2n5D38XNladHiZ5YqILKd6kmWOIQCLcBGAs/s640/02.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://4.bp.blogspot.com/-rBVTH7-Cmyk/W1fr0Yw3ycI/AAAAAAAAIvI/EfuhC2n5D38XNladHiZ5YqILKd6kmWOIQCLcBGAs/s1600/02.png)

  
Defina qual o tipo  e verão do sistema que será instalado.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://4.bp.blogspot.com/-DRJY1YFs_Ac/W1fr0ZhO1AI/AAAAAAAAIvE/Hy0gkbKAexwycR37y8-q584xbYiHka6LQCLcBGAs/s640/03.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://4.bp.blogspot.com/-DRJY1YFs_Ac/W1fr0ZhO1AI/AAAAAAAAIvE/Hy0gkbKAexwycR37y8-q584xbYiHka6LQCLcBGAs/s1600/03.png)

  
Nome da VM e o local onde será instalada.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://1.bp.blogspot.com/-Lnxp2vdNnbA/W1fr093oYjI/AAAAAAAAIvM/y-nd40A1s8AHercx1wFgDQ_4dOoimubXwCLcBGAs/s640/04.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://1.bp.blogspot.com/-Lnxp2vdNnbA/W1fr093oYjI/AAAAAAAAIvM/y-nd40A1s8AHercx1wFgDQ_4dOoimubXwCLcBGAs/s1600/04.png)

  
Em _Disk Size_ escolha o tamanho do disco virtual, o tamanho varia de acordo com o sistema convidado e com o que você deseja instalar nele. Escolha o tamanho desejado e deixe as opções marcadas como estão na imagem abaixo.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://3.bp.blogspot.com/-amr_gbPuST0/W1fr1P3kp5I/AAAAAAAAIvQ/jPpTCX6R-14BP2dtUSy62rHgawybc-tXgCLcBGAs/s640/05.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://3.bp.blogspot.com/-amr_gbPuST0/W1fr1P3kp5I/AAAAAAAAIvQ/jPpTCX6R-14BP2dtUSy62rHgawybc-tXgCLcBGAs/s1600/05.png)

  
Na opção _Customize Hardware_ é possível uma configuração mais detalhada da VM, onde podemos definir outras configurações, adicionar outros discos. Veremos a seguir algumas destas opções.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://2.bp.blogspot.com/-6rc5_8Bg0Uo/W1fr1e3hG9I/AAAAAAAAIvU/j0Yl1bgmLjc3rUBjIFRih3eWMflA7IZYwCLcBGAs/s640/06.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://2.bp.blogspot.com/-6rc5_8Bg0Uo/W1fr1e3hG9I/AAAAAAAAIvU/j0Yl1bgmLjc3rUBjIFRih3eWMflA7IZYwCLcBGAs/s1600/06.png)

  
Definir a quantidade de memória RAM que será utilizada pela VM. Detalhe: Não utilize mais que a metade da memória disponível no sistema hospedeiro, pois o funcionamento do mesmo poderá ser prejudicado.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://2.bp.blogspot.com/-D2jmlf9a-k8/W1fr1U_baTI/AAAAAAAAIvY/QCoOXsPUt0Ex9aZrM6aCAzC9NlEG9QlawCLcBGAs/s640/07.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://2.bp.blogspot.com/-D2jmlf9a-k8/W1fr1U_baTI/AAAAAAAAIvY/QCoOXsPUt0Ex9aZrM6aCAzC9NlEG9QlawCLcBGAs/s1600/07.png)

  
Na opção abaixo é possível definir quanto processadores _(núcleos)_ estarão disponíveis para a VM. Se você possui um core i3, por exemplo, pode definir 2 núcleos para a VM. Podemos seguir a mesma métrica que seguimos para a memória RAM, nunca passe da metade de núcleos que o sistema hospedeiro possui.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://3.bp.blogspot.com/-H4kkIqEY9vo/W1fr1uYkBnI/AAAAAAAAIvc/QMPjUyiGQEsx1Z1LVQgPY6XDlSuIc7VHQCLcBGAs/s640/08.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://3.bp.blogspot.com/-H4kkIqEY9vo/W1fr1uYkBnI/AAAAAAAAIvc/QMPjUyiGQEsx1Z1LVQgPY6XDlSuIc7VHQCLcBGAs/s1600/08.png)

  
  
A opção _Network Adapter_ permite a configuração da interface de rede. Normalmente deixo-a em Bridge, pois assim é possível utilizar a mesma faixa de IP do hospedeiro. Opção interessante quando se está testando um servidor web sistema convidado e deseja acessar no sistema hospedeiro. Na opção NAT é criado um IP de faixa diferente do hospedeiro, não possibilitando o acesso do hospedeiro para o convidado.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://4.bp.blogspot.com/-AwAt4uNr3jM/W1fr1xODztI/AAAAAAAAIvk/FACcFBXiz1gRcmGMZIj16YZDcdpmwsKUwCLcBGAs/s640/10.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://4.bp.blogspot.com/-AwAt4uNr3jM/W1fr1xODztI/AAAAAAAAIvk/FACcFBXiz1gRcmGMZIj16YZDcdpmwsKUwCLcBGAs/s1600/10.png)

  
Em _USB Controller_ é possível escolher qual a versão USB _(1, 2, ou 3)_ será compatível com o hospedeiro.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://4.bp.blogspot.com/-bJpAHVB9D8M/W1fr2TSZrQI/AAAAAAAAIvw/PsZatoN9OyYczYRmeEccGfAXV2cuAoIHQCLcBGAs/s640/13.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://4.bp.blogspot.com/-bJpAHVB9D8M/W1fr2TSZrQI/AAAAAAAAIvw/PsZatoN9OyYczYRmeEccGfAXV2cuAoIHQCLcBGAs/s1600/13.png)

  
Na opção _Display_, se tiver uma placa de boa qualidade, deixe as opções padrão. Caso contrário desmarque a opção _Accelerate 3D graphics_.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://2.bp.blogspot.com/-5XiHhU0faig/W1fr2vhB61I/AAAAAAAAIv0/IywCAAacqssNSe6VPpU7MwmjVKK7jYPAgCLcBGAs/s640/14.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://2.bp.blogspot.com/-5XiHhU0faig/W1fr2vhB61I/AAAAAAAAIv0/IywCAAacqssNSe6VPpU7MwmjVKK7jYPAgCLcBGAs/s1600/14.png)

  
Na aba Options é possível configurar opções como pastas compartilhadas entre o hospedeiro e convidado, ativar a tela cheia ao iniciar a VM, entre outras opções.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://1.bp.blogspot.com/-yTe3tPZrCPc/W1fr2nDC6tI/AAAAAAAAIv4/-v5kc1Xvy5kCksRuJTZ2OzEdzxScTWi8ACLcBGAs/s640/15.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://1.bp.blogspot.com/-yTe3tPZrCPc/W1fr2nDC6tI/AAAAAAAAIv4/-v5kc1Xvy5kCksRuJTZ2OzEdzxScTWi8ACLcBGAs/s1600/15.png)

  
Alteradas as configurações, salve a VM. Demarque a opção _Automatic power on this virtual machine after creation_, caso não deseje iniciá-la automaticamente após salvar.  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://2.bp.blogspot.com/-RMuJXqOb1IQ/W1fr3brYwhI/AAAAAAAAIwA/1Ll-Hbh6lgM7WcdXmBRPKP-2e7qQWa-8QCLcBGAs/s640/17.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://2.bp.blogspot.com/-RMuJXqOb1IQ/W1fr3brYwhI/AAAAAAAAIwA/1Ll-Hbh6lgM7WcdXmBRPKP-2e7qQWa-8QCLcBGAs/s1600/17.png)

  
Pronto. A VM está criada e pronta para rodar, basta "dar o Play". Lembrando que, neste caso, na primeira vez que rodar o SO convidado deverá ser instalado. [Veja aqui como instalar e configurar o sistema hospedeiro dentro da VM](https://info.wsouza.com.br/2018/08/maquina-virtual-instalando-e-configurando-o-sistema-no-vmware.html).  
  

[![Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows](https://4.bp.blogspot.com/-yHfvcp46kkM/W1fr3vVRSAI/AAAAAAAAIwE/YucBam6YUFoO_6xjOdtAVgDwGV_iPuL0ACLcBGAs/s640/18.png "Máquina Virtual: Instalando e configurando o VMware Player - Dicas Linux e Windows")](https://4.bp.blogspot.com/-yHfvcp46kkM/W1fr3vVRSAI/AAAAAAAAIwE/YucBam6YUFoO_6xjOdtAVgDwGV_iPuL0ACLcBGAs/s1600/18.png)

  

#### 4 - Considerações finais

  
Utilizar uma VM abre novas possibilidades para conhecer novos SO (s). Quando utilizamos um computador real para instalar um SO sempre ha risco de perder dados pessoais ou perder o acesso aos sistemas que já estavam instalados, o que daria um certo trabalho para recuperar ou instalar tudo novamente. Numa VM não há este risco, pois tudo pode ser deletado e recriado rapidamente.  
Outra vantagem ocorre, por exemplo, quando precisamos utilizar algum software que só roda em Windows e, por algum motivo, não queremos rodá-lo no Wine. Basta abrir a VM com o Windows instalado e rodar o software normalmente, sem sair ou interferir em seu sistema linux.  
  
Para desinstalar:  
  

 sudo vmware-installer -u vmware-player