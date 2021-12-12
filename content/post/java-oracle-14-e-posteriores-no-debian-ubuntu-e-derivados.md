---
title: 'Java Oracle 14 e posteriores no Debian, Ubuntu e Derivados'
date: 2020-03-25T20:35:00.013-03:00
draft: false
url: /2020/03/java-oracle-14-e-posteriores-no-debian-ubuntu-e-derivados.html
tags: 
- Linux
- Oracle java
- Tutoriais
---

![Java Oracle 14 e posteriores no Debian, Ubuntu e Derivados - Dicas Linux e Windows](https://2.bp.blogspot.com/-DbzsS19Ff0M/Xwehb27lHYI/AAAAAAAAPS0/zx0ZpwUuCewFxj-CeBQXvMB6Am9W-JfsACNcBGAsYHQ/s1600/Java_Oracle_14.png "Java Oracle 14 e posteriores no Debian, Ubuntu e Derivados - Dicas Linux e Windows")

A Oracle acabou de lançar a versão 14 15 do Java SE. Veja aqui como baixar, instalar e configurar no Debian, Ubuntu e derivados.  
  
_Atualizado em 06/04/2021_

  
  
  
  
  

### Java Oracle  

  
O Java Oracle _(Java SE)_ é o conjunto de ferramentas necessárias para o desenvolvimento e execução de programas com a linguagem de programação Java. O Java SE _(Java Platform, Standard Edition_) contém o ambiente de execução, chamado de JRE _(Java Runtime Environment)_, e o JDK _(Java Development Kit)_, que é o "modo" utilizado para criar programas na linguagem de programação Java. Diversos programas que são desenvolvidos para serem executados em multiplataforma são produzidos e disponibilizados na linguagem Java - como o programa de declaração do imposto de renda- e necessitarão do Java _(JRE)_ para serem executados.  
Diferentemente da maioria das dicas que encontramos na net, que mostram apenas a instalação do JRE, nesta dica você vou mostrar - de maneira sucinta - como deixar o ambiente completo funcionando no sistema. Esta dica servirá para qualquer atualização futura do Java Oracle _(até segunda ordem)_ bastando apenas trocar o número da versão.  
  

### Download

*   Acesse: [https://www.oracle.com/java/technologies/javase-jdk15-downloads.html](https://www.oracle.com/java/technologies/javase-jdk15-downloads.html);
*   Após, escolha a versão referente ao pacote Debian, chamada de Linux Debian Package. No momento em que escrevo atualizo a matéria o pacote tem o nome de "jdk-**15.0.2**\_linux-x64\_bin.deb", a parte que está em vermelho refere-se ao número da versão, que poderá ser atualizada a qualquer momento, o que causará uma mudança no nome do arquivo;
*   Aceite a licença e faça o download sua pasta de usuário (/home/nome-de-seu-usuario/).

### Instalação

  
Antes de qualquer coisa, desinstale qualquer versão que possa ter sido instalada anteriormente.  
  

  

 sudo apt purge oracle-java\*

  
Após, siga os comandos abaixo para instalação. O asterisco é um curinga, que substitui o número da versão correspondente ao arquivo que você acabou de baixar.  
  

  

 cd $HOME/

 sudo dpkg -i jdk-\*\_linux-x64\_bin.deb

  

### Configuração

  
O Java Oracle está instalado na pasta /usr/lib/jvm/jdk-**15.x.x**. Vamos configurá-lo.  
  

  

 sudo gedit /etc/profile

_Gedit é o editor gráfico de textos do Gnome. Pode utilizar qualquer editor de textos (Vim, Joe, Pluma, Kedit, Kate, Geany...)_  
  
Insira o trecho abaixo no arquivo que foi aberto e salve-o. Caso haja algum trecho parecido, substitua por este. Sempre substitua a parte que está em vermelho pela versão que corresponde à versão que você está instalando.  
  

  

 export JAVA\_HOME="/usr/lib/jvm/jdk-15.x.x"  
 export CLASSPATH="$JAVA\_HOME/lib":$CLASSPATH  
 export PATH="$JAVA\_HOME/bin":$PATH  
 export MANPATH="$JAVA\_HOME/man":$MANPATH

  
Após, digite os comandos a seguir no terminal:  
  

  

 sudo ln -s /usr/lib/jvm/jdk-15.x.x/bin/java /usr/local/bin/

 sudo ln -s /usr/lib/jvm/jdk-15.x.x/bin/javac /usr/local/bin/

  
Por último, digite no terminal o comando abaixo:  
  

  

 java -version

  
E a saída deve ser alguma coisa parecida com a saída mostrada abaixo. Se apareceu algo diferente revise o passo-a-passo e tente novamente.  
  

  

 java version "15" 2020-03-17  
 Java(TM) SE Runtime Environment (build 15+36-1461)  
 Java HotSpot(TM) 64-Bit Server VM (build 15+36-1461, mixed mode, sharing)