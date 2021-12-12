---
title: 'Programa de declaração do IRPF 2020 no Debian, Ubuntu e derivados (Arquivo .bin + Java Oracle)'
date: 2020-02-23T00:54:00.007-03:00
draft: false
url: /2020/02/programa-de-declaracao-do-irpf-2020-instalacao-no-debian-e-derivados.html
tags: 
- Linux
- Imposto de Renda
- Tutoriais
- IRPF
---

![Programa de declaração do IRPF 2020 no Linux (Arquivo .bin + Java Oracle) - Dicas Linux e Windows](https://3.bp.blogspot.com/-KoF2hUek1gk/XwfTQWPbUKI/AAAAAAAAPTM/xq97kHuVF14pao1Uvp5lGFZbj2eowyQAACNcBGAsYHQ/s1600/Irpf_Oracle_Java.png "Programa de declaração do IRPF 2020 no Linux (Arquivo .bin + Java Oracle) - Dicas Linux e Windows")

A Receita Federal disponibilizou o download do programa para declaração do imposto de renda para pessoa física - DIRPF 2020. Saiba aqui como instalar no Debian, Ubuntu e derivados utilizando um arquivo _.BIN_ e o Java Oracle.  
Se procura a versão 2021, veja em: [Instalando o programa do IRPF 2021 no Debian e Fedora](https://info.wsouza.com.br/2021/02/instalando-o-programa-do-irpf-no-debian-e-fedora.html)

  
  
  
  

### IRPF 2020

  
O programa é necessário para efetuar as declarações do imposto de renda de pessoa física, que podem ser entregues do dia 01/03/2020 à 30/04/2020 30/06/2020.  
  

### Download

  
O download do DIRPF 2020 pode ser feito no site da RFB, no seguinte endereço: [http://downloadirpf.receita.fazenda.gov.br/irpf/2020/irpf/arquivos/IRPF2020Linux-x86\_64v2.0.bin](http://downloadirpf.receita.fazenda.gov.br/irpf/2020/irpf/arquivos/IRPF2020Linux-x86_64v2.0.bin)  
Escolha a versão equivalente à arquitetura do seu sistema _(32 ou 64 bits)_. Será baixado um arquivo no formato _.bin_, salve na sua pasta de usuário (_/home/nome-de-seu-usuario/)._  
  

### Instalação

  
Para a instalação dê a permissão de execução no arquivo baixado. Para fazer isto abra o terminal _(CTRL +ALT +T)_ e digite os comandos abaixo:  
  

  

  

 cd $HOME/

  

  

  

 chmod +x nome-do-arquivo-baixado.bin

  
Após a permissão permaneça no terminal e digite o comando de instalação:  
  

  

  

 ./nome-do-arquivo-baixado.bin

  
A instalação será iniciada. Caso apareça um aviso de que é necessária a instalação do Java da Oracle, interrompa a instalação do DIRPF 2020 e faça a do Java. Caso tenha dúvidas de como instalar o Java veja em [Java Oracle 14 e posteriores no Debian, Ubuntu e Derivados](https://info.wsouza.com.br/2020/03/java-oracle-14-e-posteriores-no-debian-ubuntu-e-derivados.html). Após instalar o Java, repita o comando anterior e a instalação será iniciada. Apenas avance até o fim e o DIRPF 2020 estará instalado.  
  

### Programas dos anos anteriores

  
Se por algum motivo precisar de algum programa dos anos anteriores, baixe-os [aqui](http://receita.economia.gov.br/orientacao/tributaria/declaracoes-e-demonstrativos/dirpf/entrega-da-declaracao-do-irpf/download-programas-dirpf) e siga o mesmo processo de instalação desta matéria.

  

Caso precise da versão com OpenJDK veja em: [Programa de declaração do IRPF 2020 no Linux com Java OpenJDK](https://info.wsouza.com.br/2020/03/programa-de-declaracao-do-irpf-2020-no-linux-com-java-openjdk.html)