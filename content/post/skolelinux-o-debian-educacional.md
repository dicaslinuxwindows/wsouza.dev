---
title: 'Skolelinux, o Debian Educacional'
date: 2019-10-06T22:41:00.001-03:00
draft: false
url: /2019/10/skolelinux-o-debian-educacional.html
tags: 
- Linux
- Educacional
---

Conheça o Skolelinux, a versão do Debian voltada ao ambiente escolar. Mais detalhes na matéria a seguir.

  
  

[![](https://3.bp.blogspot.com/-hyZok5cXOUU/XSJsL-HSrZI/AAAAAAAAL0g/mf5jX31J728vMU1ilkPMyRy3a3xGMlaqgCLcBGAs/s1600/Debian_Edu.png)](https://3.bp.blogspot.com/-hyZok5cXOUU/XSJsL-HSrZI/AAAAAAAAL0g/mf5jX31J728vMU1ilkPMyRy3a3xGMlaqgCLcBGAs/s1600/Debian_Edu.png)

### Skolelinux

  
O Skolelinux _(ou Debian EDU)_ é um ambiente educacional completo e facilmente configurável. Após instalado e configurado disponibiliza um conjunto de aplicativos educacionais que pode ser categorizado por idade, além de um servidor LTSP¹.  
  

### Detalhes, informações e lançamento

  
O Skolelinux é uma versão do Debian com um ambiente educacional instalado e pré-configurado. Possui perfis com aplicativos educacionais voltados para várias faixas de idade. Tais aplicativos, e demais configurações também estão disponíveis no Debian "normal". As interfaces também são as mesmas do Debian e o lançamento de cada versão segue o mesmo calendário, sendo que a versão estável atual é o Debian Buster, lançado em 06/07/2019.  
  

### Download e informações sobre instalação

  
O Skolelinux está disponível 32 e 64 bits, porém, se for utilizado como servidor de rede ou servidor LTSP é recomendável utilizar o 64 bits. Para download das imagens:  
  

Skolelinux amd64

[ Netinst](http://get.debian.org/cdimage/release/current/amd64/iso-cd/debian-edu-10.1.0-amd64-netinst.iso)

[ DVD](http://get.debian.org/cdimage/release/current/amd64/iso-bd/debian-edu-10.0.0-amd64-BD-1.iso)

Skolelinux i386

[ Netinst](http://get.debian.org/cdimage/release/current/i386/iso-cd/debian-edu-10.1.0-i386-netinst.iso)

[ DVD](http://get.debian.org/cdimage/release/current/i386/iso-bd/debian-edu-10.1.0-i386-BD-1.iso)

  
A instalação é praticamente igual ao do Debian, com a adição de alguns perfis que podem torná-la pouco mais demorada. Vejamos:  

*   Se estiver utilizando uma imagem de instalação _netinst_ - aquela onde o ambiente gráfico é escolhido e baixado durante a instalação - num determinado momento aparecerá uma opção onde você poderá escolher os tipos de perfis que deseja. Cada caso se aplica à uma situação:

*   Servidor Principal - Não há interface gráfica e deve haver apenas um servidor na rede;
*   Estação de Trabalho - Para máquinas normais (não servidores) na rede Debian EDU;
*   Estação de Trabalho Itinerante - Para máquinas que hora são utilizadas na rede Debian EDU e hora são utilizadas fora desta rede;
*   Servidor LTSP - Requer duas placas de rede, pois uma é utilizada para a "entrada" de rede e a outra para a "saída" do sistema que será recebido pelos _Thin Clients_, que funcionarão com o perfil Estação de Trabalho _(Ver notas)_;
*   Autônomo - Não interligada à rede Debian EDU e pode conflitar com os outros perfis;
*   Mínimo -  Totalmente integrado à rede Debian EDU, mas sem nenhuma interface gráfica instalada.

*   Se estiver utilizando uma imagem de instalação completa o perfil poderá ser escolhido e instalado diretamente do DVD.

  

### Considerações finais

  
O Skolelinux é ideal para que os administradores de ambientes escolares não tenham grandes preocupações com licenças de software e com configurações constantes e complexas. Quando utilizado como servidor LTSP as vantagens são multiplicadas, pois demanda menos capacidade de hardware nos clientes e a configuração é simplificada, pois ocorre apenas uma vez, e esta é replicada aos _Thin Clients_.  
Para mais informações sobre o Skolelinux acesse: [https://wiki.debian.org/DebianEdu](https://wiki.debian.org/DebianEdu) e [https://www.skolelinux.de/en/](https://www.skolelinux.de/en/)  
  

### Notas

  
¹ Segundo a [Wikipedia](https://pt.wikipedia.org/wiki/LTSP): _"Linux Terminal Server Project (ou somente LTSP) é um projeto baseado em Linux que agrupa várias ferramentas e protocolos, com a finalidade de proporcionar um ambiente de trabalho remoto. Todo o software é corrido no servidor, e os terminais servem apenas de interface entre o utilizador e as aplicações – os poucos ciclos de processamento gastos são para enviar os dados da placa de rede à placa gráfica (...)"_.  
Ou seja: São utilizados terminais com pouca capacidade de processamento e memória _(thin clients)_, que podem rodar um sistema completo, pois todo processo estará num servidor (_que deverá possuir uma boa configuração_). Desta forma minimizam-se os custos, é possível colocar mais máquinas funcionando e facilita a manutenção e configuração, pois tudo será feito apenas uma vez no servidor.