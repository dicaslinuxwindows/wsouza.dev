---
title: 'Java Oracle 11 - Instalando no Debian de maneira rápida e fácil'
date: 2019-03-12T00:53:00.000-03:00
draft: false
url: /2019/03/java-oracle-11-instalando-no-debian-de-maneira-rapida-e-facil.html
tags: 
- Debian
- Linux
- Tutoriais
---

[![Dicas Linux e Windows - Java Oracle 11 - Instalando no Debian de Maneira Rápida e Fácil](https://4.bp.blogspot.com/-srT1ee90kOA/XIh9WLvilaI/AAAAAAAAKzg/INrla_dlj-USFH8QccKxFZt-B9SCTxZXQCLcBGAs/s200/jdk11.png "Dicas Linux e Windows - Java Oracle 11 - Instalando no Debian de Maneira Rápida e Fácil")](https://4.bp.blogspot.com/-srT1ee90kOA/XIh9WLvilaI/AAAAAAAAKzg/INrla_dlj-USFH8QccKxFZt-B9SCTxZXQCLcBGAs/s1600/jdk11.png)Esta dica está desatualizada, veja a nova em [Java Oracle 14 e posteriores no Debian, Ubuntu e Derivados](https://info.wsouza.com.br/2020/03/java-oracle-14-e-posteriores-no-debian-ubuntu-e-derivados.html).

A Oracle lançou recentemente a versão 11 do Java que terá suporte apenas para arquiteturas 64bits e suporte LTS. Veja nesta matéria como instalar facilmente o Java Oracle 11 no Debian.

  
  
  
  
  
  

### O que é Java?

Segundo o site da Oracle: _"O JDK é um ambiente de desenvolvimento para construir aplicativos e componentes usando a linguagem de programação Java. O JDK inclui ferramentas úteis para desenvolver e testar programas escritos na linguagem de programação Java e em execução na plataforma Java."_  
Além de ser uma linguagem de programação, o Java _(Não confunda com JavaScript)_ funciona como uma máquina virtual, onde os programas desenvolvidos na linguagem Java são executados. No "mundo Linux" - e mesmo no "mundo Windows" - vários programas são escritos nesta linguagem, inclusive para a Web, e dependem da Máquina Virtual Java _(JDK)_ para serem executados. Dentre os programas importantes que dependem da JDK para serem executados está o IRPF - Programa Gerador da Declaração de Imposto de Renda Pessoa Física 2019 e anos anteriores.

  

### Download e Instalação

Antes de prosseguir, remova qualquer versa instalada anteriormente.  
Para fazer o download do instalador, acesse o site da Oracle pelo link: [https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html](https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html), aceite a licença e selecione a primeira opção, com a extensão **.deb**, como mostrado na imagem abaixo.  
  

[![Dicas Linux e Windows - Java Oracle 11 - Instalando no Debian de Maneira Rápida e Fácil](https://1.bp.blogspot.com/-PWTVsc1orqk/XIhzUiNsS3I/AAAAAAAAKzM/zOrOoDX-QsI-ePqq-Zl4U8HZaYQcbmw-QCK4BGAYYCw/s640/oracle.png "Dicas Linux e Windows - Java Oracle 11 - Instalando no Debian de Maneira Rápida e Fácil")](http://1.bp.blogspot.com/-PWTVsc1orqk/XIhzUiNsS3I/AAAAAAAAKzM/zOrOoDX-QsI-ePqq-Zl4U8HZaYQcbmw-QCK4BGAYYCw/s1600/oracle.png)

  
Para instalar, abra o terminal (Ctrl +T), copie e cole o comando abaixo:  
  

sudo dpkg -i jdk-11.0.2\_linux-x64\_bin.deb

Pronto, seu Java Oracle está instalado.

  

### Observações finais

1 - Não instalei o plugin de navegador pois o Firefox e o Chromium estão mais aceitando o mesmo.  
2 - Ao testar a versão do Java no terminal, com o comando **java -version**, aparece a mensagem de comando não encontrado. Porém ao executar programas que requerem o JDK estes foram executados normalmente e o JDK está instalado na pasta **/usr/lib/jvm**, como podemos ver abaixo:  
  

[![Dicas Linux e Windows - Java Oracle 11 - Instalando no Debian de Maneira Rápida e Fácil](https://2.bp.blogspot.com/-G5k2gYwjIy4/XIh2GVsCnZI/AAAAAAAAKzU/Z4t6krxfU4wFmWY5Zww5Y5_Cf5hNshNEACK4BGAYYCw/s640/jvm.png "Dicas Linux e Windows - Java Oracle 11 - Instalando no Debian de Maneira Rápida e Fácil")](http://2.bp.blogspot.com/-G5k2gYwjIy4/XIh2GVsCnZI/AAAAAAAAKzU/Z4t6krxfU4wFmWY5Zww5Y5_Cf5hNshNEACK4BGAYYCw/s1600/jvm.png)

  
3 - Testei esta instalação nos seguintes sistemas: Debian Jessie 8.9 64bits. Mas provavelmente funcionará para as versões posteriores e com os derivados do Debian como o Ubuntu. Fica a dica: Teste e comente aqui se o resultado foi satisfatório.