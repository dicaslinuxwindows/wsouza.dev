---
title: 'Programa de declaração do IRPF 2020 no Linux com Java OpenJDK'
date: 2020-03-02T22:56:00.007-03:00
draft: false
url: /2020/03/programa-de-declaracao-do-irpf-2020-no-linux-com-java-openjdk.html
tags: 
- Linux
- Imposto de Renda
- Tutoriais
- IRPF
- OpenJDK
---

![Programa de declaração do IRPF 2020 no Linux com Java OpenJDK  - Dicas Linux e Windows](https://2.bp.blogspot.com/-C3gRh412i9U/XwfNT1tf8hI/AAAAAAAAPTA/go1lewH3w_EjEeg6Ct2xm21L36QyfKb-gCNcBGAsYHQ/s1600/Irpf_Open_JDK.png "Programa de declaração do IRPF 2020 no Linux com Java OpenJDK  - Dicas Linux e Windows")

Se você precisa utilizar o DIRPF 2020 no Linux mas não pode instalar o Java Oracle ou tem problemas com a versão disponível no formato _.BIN_, veja aqui como utilizá-lo na versão multiplataforma e com o OpenJDK.  
Se procura a versão 2021, veja em: [Instalando o programa do IRPF 2021 no Debian e Fedora](https://info.wsouza.com.br/2021/02/instalando-o-programa-do-irpf-no-debian-e-fedora.html)

  
  
  
  

### Antes de tudo: O que é, e para que serve o Java?

  
Java _(neste caso Java Runtime Environment, ou JRE)_ é o ambiente de execução para programas criados com a linguagem de programação Java. É uma máquina virtual que permite a execução do código fonte, como se fosse um processador virtual. Foi desenvolvido pela Sun Microsystems e atualmente pertence à Oracle, portanto, é uma tecnologia proprietária.  
Vários sistemas baseados em Linux utilizam a versão não proprietária, chamada de OpenJDK _(Open JRE)_. O OpenJDK é o resultado dos esforços da Comunidade Java para a evolução atemporal da linguagem. Serve como incubadora de novas ideias que normalmente são implementadas no JDK comercial da Oracle para serem rentabilizadas posteriormente.  
Fonte: [Wikipedia](https://pt.wikipedia.org/wiki/OpenJDK)  
  

### DIRPF 2020

  
O DIRPF, nas versões para sistemas operacionais específicos, funciona apenas com o Java Oracle. Muitos usuários encontram dificuldades na instalação do DIRPF em sistemas Linux devido à não disponibilidade do Java Oracle nos repositórios de algumas distribuições, principalmente nas distribuições onde há a predominância de software livre.  
Para contornar este problema a saída é utilizar a versão **multiplataforma** do DIRPF, pois ela funciona com o OpenJDK. Veremos a seguir como fazer isto.  
  

### Testando o Java

  
Antes de qualquer coisa tenha certeza que há uma versão do OpenJDK instalada. No terminal digite:  
  

 java -version

  
Se o OpenJDK estiver instalado, a saída deverá ser alguma coisa parecida com a abaixo:  
  

OpenJDK version "11.0.6" 2020-01-14  
OpenJDK Runtime Environment (build 11.0.6+10-post-Ubuntu-1ubuntu118.04.1)  
OpenJDK 64-Bit Server VM (build 11.0.6+10-post-Ubuntu-1ubuntu118.04.1, mixed mode, sharing)

  
Se não aparecer nada, é porque o OpenJDK não está instalado. Para instalar, acesse a central de software de sua distribuição e procure por **openjdk** ou **default-jre**. Você também pode instalar via terminal utilizando um dos comandos abaixo, de acordo com a sua distribuição.  
  
_**Debian e derivados**_  
  

 sudo apt install default-jre

  
_**openSUSE e derivados**_  
  

 sudo zypper in java-1\_8\_0-openjdk

  
_**Fedora e derivados**_  
  

 sudo dnf install java-1.8.0-openjdk

  
Para ter certeza que tudo deu certo, digite _**java -version**_ no terminal novamente e verifique se a saída do terminal é parecida com a anterior.  
  

### Download e execução do DIRPF

  
Após o Java estar funcionando, vamos ao DIRPF. Para fazer o download da versão multiplataforma do DIRPF, abra o terminal, copie e cole o código abaixo:  
  

 wget http://downloadirpf.receita.fazenda.gov.br/irpf/2020/irpf/arquivos/IRPF2020-1.9.zip

  
Após o download, ainda no terminal,descompacte executando o comando:  
  

 unzip $HOME/IRPF2020-1.9.zip

  
Esta versão não necessita de instalação, basta executar o arquivo com a extensão irpf.jar, que está na pasta que foi criada na descompactação.  
Para executar primeiramente dê as permissões de execução no arquivo **irpf.jar** com o comando:  
  

 chmod +x $HOME/IRPF2020/irpf.jar

  
Depois dê um duplo clique no arquivo, ou execute com o comando:  
  

 java -jar $HOME/IRPF2020/irpf.jar

  
Caso precise da versão com o Java Oracle veja em [Programa de declaração do IRPF 2020 no Linux (Arquivo .bin + Java Oracle)](https://info.wsouza.com.br/2020/02/programa-de-declaracao-do-irpf-2020-instalacao-no-debian-e-derivados.html)