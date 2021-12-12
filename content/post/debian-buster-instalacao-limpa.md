---
title: 'Debian Buster - Instalação limpa com Dual Boot'
date: 2019-07-20T20:31:00.002-03:00
draft: false
url: /2019/07/debian-buster-instalacao-limpa.html
tags: 
- Debian
- Linux
- Debian Buster
- Tutoriais
---

Neste tutorial mostro o passo a passo, com o máximo de detalhes possíveis, de como fazer uma instalação limpa do Debian Buster.

  
  
  

### Debian Buster

  
O Buster é a 10º versão do sistema operacional Debian e foi lançado no dia 06/07/2019, mais detalhes sobre seu lançamento em [Debian Buster é lançado oficialmente.](https://info.wsouza.com.br/2019/07/debian-buster-e-lancado-oficialmente.html)  
  

### Download

  
Utilizarei como exemplo um Live CD com a versão padrão, que vem com a interface Gnome e pode ser baixado num dos links abaixo:  
  

64 Bits _(amd64)_

[ ISO](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-10.0.0-amd64-gnome.isoo)

[ Torrent](https://cdimage.debian.org/debian-cd/current-live/i386/bt-hybrid/debian-live-10.0.0-i386-gnome.iso.torrent)

[Mais...](https://cdimage.debian.org/debian-cd/current-live/amd64/)

32 Bits _(i386)_

[ ISO](https://cdimage.debian.org/debian-cd/current-live/i386/iso-hybrid/debian-live-10.0.0-i386-gnome.iso)

[ Torrent](https://cdimage.debian.org/debian-cd/current-live/i386/bt-hybrid/debian-live-10.0.0-i386-gnome.iso.torrent)

[Mais...](https://cdimage.debian.org/debian-cd/current-live/i386/)

  

### Instalação

  
Após o download grave a ISO num CD/DVD ou Pendrive Bootável _(Utilizando o Yumi, Unetbootin, Universal USB Installer, Criador de Discos de Inicialização do Ubuntu...)_ .  
  
Agora vamos à instalação propriamente dita. Ao iniciar o instalador a primeira opção que aparece é a opção para iniciar no modo live, onde você pode testar, conhecer o sistema antes de instalar. Caso acesse esta opção o sistema iniciará no idioma inglês e você poderá utilizar o novo instalador Calamares para efetuar a instalação. Caso deseje iniciar em português, escolha as opções iguais as mostradas na segunda e terceira imagem.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://3.bp.blogspot.com/-xfzwuXX4uJs/XSvHBQb5dVI/AAAAAAAAL1M/XnXFKFZXh3sM0pS8FcZ0NPpoZYjGeUoqgCLcBGAs/s640/01.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-xfzwuXX4uJs/XSvHBQb5dVI/AAAAAAAAL1M/XnXFKFZXh3sM0pS8FcZ0NPpoZYjGeUoqgCLcBGAs/s1600/01.png)

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-ym3cObrpjIA/XSvHBcLbp0I/AAAAAAAAL1Q/3J27NGyxjaYoEXfNhVv4EujdECCmTbe2QCLcBGAs/s640/02.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-ym3cObrpjIA/XSvHBcLbp0I/AAAAAAAAL1Q/3J27NGyxjaYoEXfNhVv4EujdECCmTbe2QCLcBGAs/s1600/02.png)

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-hTYVv-icsao/XSvHBcJj9YI/AAAAAAAAL1I/fwyMBNLCpBAWDLv-_1D7XQqbamTweMbGQCLcBGAs/s640/03.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-hTYVv-icsao/XSvHBcJj9YI/AAAAAAAAL1I/fwyMBNLCpBAWDLv-_1D7XQqbamTweMbGQCLcBGAs/s1600/03.png)

  
Por opção, decidi não entrar no sistema em modo live e preferi instalar direto pela tela inicial. Para isto escolhi a opção "Graphical Debian Installer", que é o velho instalador Debian em modo gráfico, como podemos ver na imagem abaixo.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://2.bp.blogspot.com/-qFXEJpanyGk/XSvHB6gzqwI/AAAAAAAAL1U/Iz85gkrXfhY9rWqjI2aGHLr8pDw5w5LkwCLcBGAs/s640/04.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://2.bp.blogspot.com/-qFXEJpanyGk/XSvHB6gzqwI/AAAAAAAAL1U/Iz85gkrXfhY9rWqjI2aGHLr8pDw5w5LkwCLcBGAs/s1600/04.png)

  
Na tela a seguir é onde podemos definir o idioma do instalador e o idioma que o sistema será configurado.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://3.bp.blogspot.com/-S2VBNVhkiFk/XSvHCIjoHAI/AAAAAAAAL1Y/Y9fOsHPmawIZ-sYb4WPhUHBSeLdV0GQBQCLcBGAs/s640/07.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-S2VBNVhkiFk/XSvHCIjoHAI/AAAAAAAAL1Y/Y9fOsHPmawIZ-sYb4WPhUHBSeLdV0GQBQCLcBGAs/s1600/07.png)

  
Abaixo definimos a variável _locale_ referente à localidade padrão do sistema. Esta variável configura detalhes sobre a região escolhida, como o tipo de moeda, fuso horário...  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://1.bp.blogspot.com/-W6sPakTwh0Y/XSvHCb5x4FI/AAAAAAAAL1c/SNCpG_l001A26RzuHV8395GCmQHMvBn1QCLcBGAs/s640/08.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://1.bp.blogspot.com/-W6sPakTwh0Y/XSvHCb5x4FI/AAAAAAAAL1c/SNCpG_l001A26RzuHV8395GCmQHMvBn1QCLcBGAs/s1600/08.png)

  
Abaixo é onde podemos definir o idioma e configuração padrão do teclado.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://2.bp.blogspot.com/-ggsn2qlMfpQ/XSvHCnQdkDI/AAAAAAAAL1g/3MG5ILldX2QYRFWjK3LlGW9_CzCO3rdCACLcBGAs/s640/09.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://2.bp.blogspot.com/-ggsn2qlMfpQ/XSvHCnQdkDI/AAAAAAAAL1g/3MG5ILldX2QYRFWjK3LlGW9_CzCO3rdCACLcBGAs/s1600/09.png)

  
Defina um nome para a sua máquina. O nome pode ser qualquer um e este nome é o que aparece no terminal após o _@_.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://1.bp.blogspot.com/-kbSSm4lAOLQ/XSvHCy3m-jI/AAAAAAAAL1k/xgGoRP74EmQIr97PToGNzKKKAwwn2R2LQCLcBGAs/s640/13.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://1.bp.blogspot.com/-kbSSm4lAOLQ/XSvHCy3m-jI/AAAAAAAAL1k/xgGoRP74EmQIr97PToGNzKKKAwwn2R2LQCLcBGAs/s1600/13.png)

  
Se sua máquina faz parte de um domínio de rede coloque o nome do domínio, caso contrário, deixe em branco, omo vemos na tela abaixo.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://1.bp.blogspot.com/-OIMVlqbgC90/XSvHDQvyZmI/AAAAAAAAL1o/X9kGxmZIm_E6W1svmaXhjZUAAbDCYMDdwCLcBGAs/s640/14.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://1.bp.blogspot.com/-OIMVlqbgC90/XSvHDQvyZmI/AAAAAAAAL1o/X9kGxmZIm_E6W1svmaXhjZUAAbDCYMDdwCLcBGAs/s1600/14.png)

  
A próxima opção deve ser analisada com muita atenção. Nela é que definiremos a senha do super usuário _root_, porém, esta senha não precisa ser criada, o root será desabilitado e seu usuário _(que será criado no próximo passo)_ terá o **sudo** habilitado para ele. Um problema em não definir a senha de root é que você poderá encontrar dificuldades quando acessar pelo modo de recuperação, pois o root estará desativado. Portanto, sugiro que defina uma senha de root neste passo.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-DUq_y5dLt1Y/XSvHDtXy5MI/AAAAAAAAL1s/-d7kO2oFttMjxBs7NGyhQyZE3pQHFQS0QCLcBGAs/s640/15.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-DUq_y5dLt1Y/XSvHDtXy5MI/AAAAAAAAL1s/-d7kO2oFttMjxBs7NGyhQyZE3pQHFQS0QCLcBGAs/s1600/15.png)

  
Nas próximas 3 telas definiremos o nome completo, nome de usuário _(login)_ e senha para a conta padrão.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://2.bp.blogspot.com/-DqSsIkwOkzA/XSvHD4cSZ1I/AAAAAAAAL1w/bE1LS4rS0GMxwYU8KAvNAiFCGjvLLnUfACLcBGAs/s640/16.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://2.bp.blogspot.com/-DqSsIkwOkzA/XSvHD4cSZ1I/AAAAAAAAL1w/bE1LS4rS0GMxwYU8KAvNAiFCGjvLLnUfACLcBGAs/s1600/16.png)

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://2.bp.blogspot.com/-EXmfp-mT6aY/XSvHEGTbaII/AAAAAAAAL10/K785seauSTUWXqyX0XG8555if6w-JyQKACLcBGAs/s640/17.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://2.bp.blogspot.com/-EXmfp-mT6aY/XSvHEGTbaII/AAAAAAAAL10/K785seauSTUWXqyX0XG8555if6w-JyQKACLcBGAs/s1600/17.png)

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://1.bp.blogspot.com/-Oeqq3J8Q7g0/XSvHEcuff2I/AAAAAAAAL14/diQQn3ZNnfgJRn866qWxNMWC9C4NDw33QCLcBGAs/s640/18.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://1.bp.blogspot.com/-Oeqq3J8Q7g0/XSvHEcuff2I/AAAAAAAAL14/diQQn3ZNnfgJRn866qWxNMWC9C4NDw33QCLcBGAs/s1600/18.png)

  
Escolha o estado onde você está localizado para configurar corretamente o relógio do sistema.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://3.bp.blogspot.com/-G1THjvOTuiM/XSvHE5aGJ0I/AAAAAAAAL18/PEjpeol0M-Y_1tdd_1mfHrvXiEP7wX3YgCLcBGAs/s640/20.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-G1THjvOTuiM/XSvHE5aGJ0I/AAAAAAAAL18/PEjpeol0M-Y_1tdd_1mfHrvXiEP7wX3YgCLcBGAs/s1600/20.png)

  
O próximo passo é o particionamento do disco e este passo é um dos mais importantes e seguem algumas considerações:  

1.  Se você estiver instalando num computador novo, ou deseja substituir o sistema que está instalado nele e não precisa salvar nenhum dado, escolha a opção _"Assistido - usar o disco inteiro";_
2.  Caso tenha um sistema operacional instalado e deseje mantê-lo. Ou caso  deseje separar a pasta de arquivos pessoais _/home_ do restante do sistema, escolha a opção _"Manual"_ e é esta opção que será utilizada como exemplo.
3.  Citei apenas as 2 opções que mais utilizo.

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-AB5T0Huw-mQ/XSvHF4mT0CI/AAAAAAAAL2E/9BjiVoQpJJYiz3PcivFQoDpGu3aUtzUxgCLcBGAs/s640/24.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-AB5T0Huw-mQ/XSvHF4mT0CI/AAAAAAAAL2E/9BjiVoQpJJYiz3PcivFQoDpGu3aUtzUxgCLcBGAs/s1600/24.png)

  
Como o disco principal (sda) já está vazio, o instalador pede para criar uma nova tabela de partições nele. Escolha sim e confirme.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://1.bp.blogspot.com/-TN2o0dg5TH0/XSvHGeZWq_I/AAAAAAAAL2I/EVbfB837OVMqaliKMFvZxt1_v1CInN8CwCLcBGAs/s640/25.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://1.bp.blogspot.com/-TN2o0dg5TH0/XSvHGeZWq_I/AAAAAAAAL2I/EVbfB837OVMqaliKMFvZxt1_v1CInN8CwCLcBGAs/s1600/25.png)

  
Na tela abaixo aparecem 3 discos, sendo que o sdc _(de 64.3 Gb)_ possui 2 partições. Neste disco há o Windows 7 instalado, ótimo para mostrarmos uma instalação em Dual Boot. O disco sdd (2.1 Gb) é uma partição utilizada para troca de arquivos, conhecida como swap. Como ela já está formatada não é preciso mexer nela. Vamos instalar o Buster no primeiro disco, chamado de sda _(21.5 Gb)_ e vamos separar os arquivos do usuário /home, no disco sdb _(16.1 GB)._ Nos próximos passos comentarei mais a respeito desta separação e para mais detalhes sobre as partições veja as notas no final da matéria.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://3.bp.blogspot.com/-QHbe8Od5R9U/XSvHGhJ6efI/AAAAAAAAL2M/InRcdrnljCwBFdRgh7Apg5bNDeQkC5ZAwCLcBGAs/s640/26.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-QHbe8Od5R9U/XSvHGhJ6efI/AAAAAAAAL2M/InRcdrnljCwBFdRgh7Apg5bNDeQkC5ZAwCLcBGAs/s1600/26.png)

  
Como citei acima, o disco sda estava vazio, criamos a tabela de partições e agora vamos criar uma nova partição nele.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://2.bp.blogspot.com/-7QrnbVOKWDo/XSvHGkELC4I/AAAAAAAAL2Q/5nMj4xnUZag82LxmEliSGrKNubMYmpzVQCLcBGAs/s640/27.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://2.bp.blogspot.com/-7QrnbVOKWDo/XSvHGkELC4I/AAAAAAAAL2Q/5nMj4xnUZag82LxmEliSGrKNubMYmpzVQCLcBGAs/s1600/27.png)

  
Neste caso escolhi o tamanho máximo porque tenho mais de 1 disco. Mas se tiver um único disco, um disco vazio, ou um disco maior, como sugestão pode deixar uns 30% para o sistema, 20% para a /home e 48% para outros dados ou instalação de um outro sistema operacional e 2% para a partição swap.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://3.bp.blogspot.com/-A9QzxyB2AhI/XSvHG4cNU2I/AAAAAAAAL2U/4TWdU7tNt-ccbXwbgkCdPkNguh0nX9TfgCLcBGAs/s640/28.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-A9QzxyB2AhI/XSvHG4cNU2I/AAAAAAAAL2U/4TWdU7tNt-ccbXwbgkCdPkNguh0nX9TfgCLcBGAs/s1600/28.png)

  
No sistema MBR partições primárias devem ser utilizadas para o sistema instalado e há um limite de 4 _(ou 3 caso haja uma estendida)_. Partições lógicas são criadas dentro de uma partição estendida. Há um limite maior da quantidade de partições lógicas, o que pode aumentar a quantidade de partições no disco. Partições lógicas podem ser utilizadas para arquivos.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-vrSu85x1hn8/XSvHHA2Zh5I/AAAAAAAAL2Y/LS34Mx48pTQckG1lCYV6Y8EfNIw3qCcAwCLcBGAs/s640/29.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-vrSu85x1hn8/XSvHHA2Zh5I/AAAAAAAAL2Y/LS34Mx48pTQckG1lCYV6Y8EfNIw3qCcAwCLcBGAs/s1600/29.png)

  
Escolhida a partição /sda chegou a hora de formatá-la e definir o ponto de montagem. Deixe como está na imagem abaixo e a partição estará formatada. Para modificar uma opção basta clicar em cima do nome_._ Após, escolha a opção _Finalizar a configuração da partição._  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://3.bp.blogspot.com/-PKQKz6_t6nE/XSvHHrNDfQI/AAAAAAAAL2c/3I-HT5bSEBso63vYPDTRS7OOJrXLKnN1ACLcBGAs/s640/30.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-PKQKz6_t6nE/XSvHHrNDfQI/AAAAAAAAL2c/3I-HT5bSEBso63vYPDTRS7OOJrXLKnN1ACLcBGAs/s1600/30.png)

  
O instalador voltará para a tela de escolha dos discos. Vamos agora escolher a partição onde ficarão salvos os arquivos do usuário, a partição /home que é a /sdb.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://3.bp.blogspot.com/-RZPOTMgr2Hs/XSvHInZRwXI/AAAAAAAAL2k/kvxcUH6FyTgxFBdfcZv8DejJz-pQ7vtxgCLcBGAs/s640/32.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-RZPOTMgr2Hs/XSvHInZRwXI/AAAAAAAAL2k/kvxcUH6FyTgxFBdfcZv8DejJz-pQ7vtxgCLcBGAs/s1600/32.png)

  
Da maneira que está definido na imagem abaixo a partição não será formatada, pois já estava formatada anteriormente. Se deseja formatá-la mude a opção selecionada para sim e finalize a configuração da partição na opção correspondente.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://3.bp.blogspot.com/-g1On2fSxmnE/XSvHIwTyjiI/AAAAAAAAL2o/SngJdcdtFEE3Jpaz9J4YNcCSj2XKN804gCLcBGAs/s640/33.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-g1On2fSxmnE/XSvHIwTyjiI/AAAAAAAAL2o/SngJdcdtFEE3Jpaz9J4YNcCSj2XKN804gCLcBGAs/s1600/33.png)

  
O sdc é onde está instalado o Windows, portanto não vou mexer nele. Já a unidade sdd formatei como como swap, da mesma maneira que fiz alterações nas partições anteriores.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://2.bp.blogspot.com/-Jmx0cco0_O0/XSvHJY44acI/AAAAAAAAL2s/Rss8kX2M-Pgl43rkQK_3q_ItNxznAzauQCLcBGAs/s640/34.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://2.bp.blogspot.com/-Jmx0cco0_O0/XSvHJY44acI/AAAAAAAAL2s/Rss8kX2M-Pgl43rkQK_3q_ItNxznAzauQCLcBGAs/s1600/34.png)

  
Após realizadas as alterações escolha a opção _"Finalizar o particionamento e escrever as mudanças no disco"_ e confirme-as.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://1.bp.blogspot.com/-l1Sz2DVA0FY/XSvHKHOI-lI/AAAAAAAAL2w/xEIlH-c0D1Q6ogYincFyVlTlZrGc2oB8wCLcBGAs/s640/35.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://1.bp.blogspot.com/-l1Sz2DVA0FY/XSvHKHOI-lI/AAAAAAAAL2w/xEIlH-c0D1Q6ogYincFyVlTlZrGc2oB8wCLcBGAs/s1600/35.png)

  
A partir deste ponto é que a instalação efetivamente se inicia. É um processo que pode demorar alguns minutos, mas nada demais.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-HEOJCRmFSPk/XSvHKlRzy1I/AAAAAAAAL20/zIw3lWL7vlgxstkNzkv3EXkUlfBADwuwgCLcBGAs/s640/36.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-HEOJCRmFSPk/XSvHKlRzy1I/AAAAAAAAL20/zIw3lWL7vlgxstkNzkv3EXkUlfBADwuwgCLcBGAs/s1600/36.png)

  
  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://3.bp.blogspot.com/-_owN2eJJAhg/XSvHLCjBm-I/AAAAAAAAL24/nH8xlRHz5_Ih7jSgNCn6vz1UpaoJrIidQCLcBGAs/s640/42.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-_owN2eJJAhg/XSvHLCjBm-I/AAAAAAAAL24/nH8xlRHz5_Ih7jSgNCn6vz1UpaoJrIidQCLcBGAs/s1600/42.png)

  
Na opção abaixo, escolhendo "Sim", o instalador pode baixar as versões mais recentes dos softwares que estão sendo instaladas. Caso queira uma instalação mais rápida, escolha "Não". Os pacotes podem ser atualizados depois que o sistema estiver instalado.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-D7lgL79PHUk/XSvHLo8OgUI/AAAAAAAAL28/uYeTHgpokugO1pI1mmpRhj7pIfjTkiW4ACLcBGAs/s640/44.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-D7lgL79PHUk/XSvHLo8OgUI/AAAAAAAAL28/uYeTHgpokugO1pI1mmpRhj7pIfjTkiW4ACLcBGAs/s1600/44.png)

  
Configuração do gestor de pacotes do Debian, o apt.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-dFc2R1gdsqo/XSvHMCgr2SI/AAAAAAAAL3A/x52Rmx1hnXkWiRDuaRi7VkhEdEKBTLlvQCLcBGAs/s640/45.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-dFc2R1gdsqo/XSvHMCgr2SI/AAAAAAAAL3A/x52Rmx1hnXkWiRDuaRi7VkhEdEKBTLlvQCLcBGAs/s1600/45.png)

  
A partir de agora inicia-se a instalação do GRUB2, que é o carregador de inicialização do Debian. Este ponto é muito importante e se o instalador for interrompido antes dele você não conseguirá inicializar o sistema.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://1.bp.blogspot.com/-IGHvM7IJ2GM/XSvHNEeYIGI/AAAAAAAAL3I/B16SlIyAxign-51Q4qp-wdUACKpJpLmNwCLcBGAs/s640/47.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://1.bp.blogspot.com/-IGHvM7IJ2GM/XSvHNEeYIGI/AAAAAAAAL3I/B16SlIyAxign-51Q4qp-wdUACKpJpLmNwCLcBGAs/s1600/47.png)

  
O instalador do GRUB detectou que há um outro sistema operacional instalado no computador. Apesar dele detectar como Windows Vista na realidade é o Windows 7 que tenho instalado aqui. Recomendo que aceite a sugestão do instalador e instale o GRUB no registro mestre de inicialização.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-CDeXIflyjik/XSvHNleqXFI/AAAAAAAAL3M/PJ30f22gdD4BM9uK7JsEIWU85xvjGoNjQCLcBGAs/s640/48.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-CDeXIflyjik/XSvHNleqXFI/AAAAAAAAL3M/PJ30f22gdD4BM9uK7JsEIWU85xvjGoNjQCLcBGAs/s1600/48.png)

  
Independente se você tem um ou mais discos, se você escolheu instalar no registro mestre de inicialização, escolha o disco onde está instalado o Debian Buster que, neste caso, é o sda. Após, clique em continuar.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://3.bp.blogspot.com/-HiN4sv4SxB4/XSvHN4AyGhI/AAAAAAAAL3Q/bukc0WdnwN4s5zoPVxIzJeiyv2lEp4qGwCLcBGAs/s640/49.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://3.bp.blogspot.com/-HiN4sv4SxB4/XSvHN4AyGhI/AAAAAAAAL3Q/bukc0WdnwN4s5zoPVxIzJeiyv2lEp4qGwCLcBGAs/s1600/49.png)

  
O GRUB está sendo instalado...  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://2.bp.blogspot.com/-Mp3RlRBc6L0/XSvHOI4FUxI/AAAAAAAAL3U/-4pzuTFRZ3QlN_97xuNqtR8ml4Uqp53PwCLcBGAs/s640/50.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://2.bp.blogspot.com/-Mp3RlRBc6L0/XSvHOI4FUxI/AAAAAAAAL3U/-4pzuTFRZ3QlN_97xuNqtR8ml4Uqp53PwCLcBGAs/s1600/50.png)

  
GRUB instalado e a instalação do sistema está chegando ao fim.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-0ITAqq_COfw/XSvHOUs0WZI/AAAAAAAAL3Y/-A0an2xcx8k9hl0ChbISGcTU4kMFEFEKgCLcBGAs/s640/51.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-0ITAqq_COfw/XSvHOUs0WZI/AAAAAAAAL3Y/-A0an2xcx8k9hl0ChbISGcTU4kMFEFEKgCLcBGAs/s1600/51.png)

  
Pronto. O Debian Buster foi instalado com sucesso. Escolha a opção continuar e remova a mídia de instalação pois o computador irá reinicializar.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-50Fe5xHETI0/XSvHOt-RS4I/AAAAAAAAL3c/iX_iwPYLj6cx-7Z-6FMws7JgnbF4kRVegCLcBGAs/s640/52.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-50Fe5xHETI0/XSvHOt-RS4I/AAAAAAAAL3c/iX_iwPYLj6cx-7Z-6FMws7JgnbF4kRVegCLcBGAs/s1600/52.png)

  
A primeira tela que aparece é a do GRUB2 mostrando os dois sistemas que estão instalados. Aqui você pode escolher em qual sistema iniciar.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-TPnUbxuppOk/XSvHO9BuP7I/AAAAAAAAL3g/Xv4ZXVj3AT0l8zveMVP6JM4WDvaWCwcTgCLcBGAs/s640/53.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-TPnUbxuppOk/XSvHO9BuP7I/AAAAAAAAL3g/Xv4ZXVj3AT0l8zveMVP6JM4WDvaWCwcTgCLcBGAs/s1600/53.png)

  
A tela que aparece na sequência é do gerenciador de sessão, neste caso o GDM. É a partir dele que é possível selecionar os usuários e as opções para iniciar o sistema.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-o18_8aIrB_I/XSvHPONzpAI/AAAAAAAAL3k/ihU6aIzjcCQmo7FWQFF9YZIcC1GonSXzQCLcBGAs/s640/54.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-o18_8aIrB_I/XSvHPONzpAI/AAAAAAAAL3k/ihU6aIzjcCQmo7FWQFF9YZIcC1GonSXzQCLcBGAs/s1600/54.png)

  
Nas matérias anteriores comentei que o Wayland causa alguns problemas e que o usuário poderia escolher iniciar pelo Xorg. A imagem abaixo mostra exatamente a escolha desta opção. A opção GNOME é a opção padrão com o Wayland.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://4.bp.blogspot.com/-GC8S0Xnq_e4/XSvHPVRucDI/AAAAAAAAL3o/RSDoJ0pRZm0ZmrXget_EKO6WxsVHn36zgCLcBGAs/s640/55.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://4.bp.blogspot.com/-GC8S0Xnq_e4/XSvHPVRucDI/AAAAAAAAL3o/RSDoJ0pRZm0ZmrXget_EKO6WxsVHn36zgCLcBGAs/s1600/55.png)

  
Após o login, enfim  temos o Debian Buster rodando normalmente.  
  

[![Debian Buster - Instalação limpa - Dicas Linux e Windows](https://2.bp.blogspot.com/-9-2f2uWozCM/XSvHPikOukI/AAAAAAAAL3s/45_bSODW-nkbPEWdKvrYomwdEWwvf1GwQCLcBGAs/s640/56.png "Debian Buster - Instalação limpa - Dicas Linux e Windows")](https://2.bp.blogspot.com/-9-2f2uWozCM/XSvHPikOukI/AAAAAAAAL3s/45_bSODW-nkbPEWdKvrYomwdEWwvf1GwQCLcBGAs/s1600/56.png)

  

### Notas

*   Utilizei uma configuração modesta de máquina virtual,pois o propósito era apenas de mostrar a instalação. Por este motivo a arquitetura de sistema utilizada como exemplo foi a de 32 bits
*   Um detalhe importante que não mencionei: Neste caso, como estou utilizando uma máquina virtual, utilizei o disco _sda_ vazio e coloquei um disco _sdc_ que já tinha o Windows 7 instalado. Portanto: O Windows 7 não está no mesmo disco e o _sdc_ não é uma partição. Caso você possua apenas um disco e deseje separar os arquivos de usuário e um sistema operacional já instalado sugiro que primeiro faça numa máquina virtual para depois testar em seu dispositivo de uso diário, sob o risco de perder os dados nele contidos. A diferença está na configuração da máquina virtual para receber o sistema. Para particionar um disco veja [GParted, Particionador Gráfico](https://info.wsouza.com.br/2018/07/gparted-particionador-grafico.html).
*   Se você deseja testar a instalação numa máquina virtual, [siga este exemplo](https://info.wsouza.com.br/2018/08/maquina-virtual-instalando-e-configurando-o-sistema-no-vmware.html).