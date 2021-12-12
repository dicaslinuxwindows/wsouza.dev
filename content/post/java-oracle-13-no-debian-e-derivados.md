---
title: 'Java Oracle 13 no Debian e Derivados'
date: 2020-02-22T23:16:00.002-03:00
draft: false
url: /2020/02/java-oracle-13-no-debian-e-derivados.html
tags: 
- Linux
- Oracle java
- Tutoriais
---

![Java Oracle 13 no Debian e Derivados - Dicas Linux e Windows](https://2.bp.blogspot.com/-_RSTktCfHyg/Xwfp9Itl6UI/AAAAAAAAPXY/oWhD3tuiLQUOuT8MRHd1wRrLtdoPdhCNwCNcBGAsYHQ/s1600/Java_13.png "Java Oracle 13 no Debian e Derivados - Dicas Linux e Windows")

Instalando e configurando a PATH do Oracle Java 13 no Debian e derivados. Se deseja a versão 14, que foi publicada recentemente, veja em [Java Oracle 14 e posteriores no Debian, Ubuntu e Derivados](https://info.wsouza.com.br/2020/03/java-oracle-14-e-posteriores-no-debian-ubuntu-e-derivados.html)

  
  
  
  
  
  

### Java 13

  
O Java Oracle 13 é uma versão máquina virtual do conjunto de ferramentas necessárias para o desenvolvimento de programas com a linguagem de produção Java e execução dos mesmos. Diversos programas que são desenvolvidos para serem executados em multiplataforma são disponibilizados neste formato, portanto, necessitarão do Java para serem executados. Dentre estes programas está o programa de declaração de imposto de renda.  
  

### Download

  
Utilizaremos um pacote .deb, e para baixá-lo acesse: [https://www.oracle.com/java/technologies/javase-jdk13-downloads.html](https://www.oracle.com/java/technologies/javase-jdk13-downloads.html). Após, escolha a versão referente ao pacote Debian, chamada de _Linux Debian Package_, aceite a licença e faça o download sua pasta de usuário _(/home/nome-de-seu-usuario/)_.  
Obs: Desde a versão 12 a Oracle pede login e senha para download destes pacotes, porém, nem sempre este login é pedido. Caso peça, faça um pequeno cadastro e entre com seu login e senha criado.  
  

### Instalação

  
Abra o terminal _(CTRL +ALT +T)_ e digite os comandos abaixo:  
  

cd /home/nome-de-seu-usuario/

  

sudo dpkg -i nome-do-arquivo-baixado.deb

  
O Java foi instalado na pasta "/usr/lib/jvm/jdk-13**.0.2**". (A parte que está em vermelho muda conforme as atualizações)  
  

### Configuração da PATH

  
Para que o Java funcione corretamente, não basta somente a instalação. É necessária uma configuração na PATH, que é variável de ambiente do sistema e serve para indicar onde os executáveis estão instalados. Fonte: [_Wikipedia_](https://en.wikipedia.org/wiki/PATH_(variable))  
A fonte da dica a seguir é o [Viva o Linux](https://www.vivaolinux.com.br/dica/Instalacao-e-configuracao-do-Java-e-do-PATH).  
  
No terminal, digite o seguinte comando:  
  

sudo gedit /etc/profile

_Gedit é o editor gráfico de textos do Gnome. Pode utilizar qualquer editor de textos (Vim, Joe, Pluma, Kedit, Kate, Geany...)_  
  
No início do arquivo que foi aberto, insira o próximo código e salve. (Altere o que está em vermelho para a versão baixada).  
  

export JAVA\_HOME="/usr/lib/jvm/jdk-13**.0.2**"  
export CLASSPATH="$JAVA\_HOME/lib":$CLASSPATH  
export PATH="$JAVA\_HOME/bin":$PATH  
export MANPATH="$JAVA\_HOME/man":$MANPATH

  
A seguir, ainda no terminal, digite os comandos a seguir:  
  

ln -s /usr/lib/jvm/jdk-13**.0.2**/bin/java /usr/local/bin/  
ln -s /usr/lib/jvm/jdk-13**.0.2**/bin/javac /usr/local/bin/

  
Finalizado. Para confirmar que deu certo, no terminal digite _java -version_, e a saída será alguma coisa parecida esta:  
  

java version "13**.0.2**" 2020-01-14  
Java(TM) SE Runtime Environment (build 13**.0.2**+8)