---
title: 'Instalando o programa do IRPF 2021 no Debian e Fedora'
date: 2021-02-28T19:25:00.006-03:00
draft: false
url: /2021/02/instalando-o-programa-do-irpf-no-debian-e-fedora.html
tags: 
- Debian
- Linux
- Oracle java
- Ubuntu
- Tutoriais
- Fedora
- IRPF
- OpenJDK
---

![Instalando o programa do IRPF no Debian e Fedora - Dicas Linux e Windows](https://1.bp.blogspot.com/-88UIhEs61oA/YDwWR6Dc2wI/AAAAAAAARws/L37oamMEOk8Mity9TYFH0TknvO3yWdwywCNcBGAsYHQ/s16000/IRPF2021.png "Instalando o programa do IRPF no Debian e Fedora - Dicas Linux e Windows")

Nesta semana foi disponibilizado o DIRPF, que é o programa gerador da declaração de imposto de renda de pessoa física. Veja nesta matéria como instalar no Debian _(e seus derivados)_ e Fedora.

  
  
  
  
  
  

### DIRPF 2021

  
O DIRPF é o programa que gera a declaração do imposto de renda para pessoa física. Há versões para sistemas operacionais Linux, Windows, MacOS e uma versão Multiplataforma. Nesta matéria será mostrado como instalar/executar a versão para Linux e a Multiplataforma. Há uma novidade neste ano, pois a versão para Linux já vem com o Java embutido, não sendo necessário a instalação da plataforma.  
  

### Linux 64 Bits

  
Vou mostrar todo o processo pelo terminal, mas se quiser baixar os arquivos via navegador, acesse o site da [Receita Federal.](https://www.gov.br/receitafederal/pt-br/centrais-de-conteudo/download/pgd/dirpf)  
  

#### Download

  

  

  

 wget https://downloadirpf.receita.fazenda.gov.br/irpf/2021/irpf/arquivos/IRPF2021Linux-x86\_64v1.1.bin

  

#### Instalação

  
Como citei no início, esta versão não é preciso ter alguma versão do Java instalada, pois ele já vem com o Java embutido. Desta forma, a instalação fica bem mais simples do que era nos anos anteriores. A dica a seguir funciona para o Debian e seus derivados, Fedora, entre outras distribuições.  
  
1º passo: Dê permissão de execução ao arquivo baixado anteriormente, que é o instalador do programa.  
  

  

  

 chmod +x IRPF2021Linux-x86\_64v1.1.bin

  
2º passo: Execute o instalador, com o comando abaixo e vá avançando até finalizar.  
  

  

  

 ./IRPF2021Linux-x86\_64v1.1.bin

  
3º Passo: Se não ocorreu nenhum erro, o programa está instalado e haverá um atalho no menu.  
  

### Multiplataforma _(zip)_

  
A versão multiplataforma é um arquivo zip, que é descompactado e tem um executável no formato .jar que já é o próprio DIRPF 2021. Sendo assim, não precisa ser instalado. Porém, neste caso é preciso ter uma versão do Java JDK instalada no sistema. Esta versão pode ser tanto o OpenJDK (que é uma versão opensource) ou pode ser o Oracle Java (que é uma versão proprietária). Abaixo vou mostrar como baixar e executar o DIRPF nesta versão multiplataforma.  
  

#### Download

  

  

  

 wget https://downloadirpf.receita.fazenda.gov.br/irpf/2021/irpf/arquivos/IRPF2021-1.1.zip

  

#### Execução

  
1º passo: Instale o Java.  

*   Se optar pelo Oracle Java _(no Debian e derivados)_, veja como instalar na matéria [Java Oracle 14 e posteriores no Debian, Ubuntu e Derivados](https://info.wsouza.com.br/2020/03/java-oracle-14-e-posteriores-no-debian-ubuntu-e-derivados.html);
*   Se optar pelo OpenJDK, siga os passos abaixo, de acordo com a distribuição utilizada.

  
No Debian e derivados:  
  

  

  

 sudo apt install openjdk-11-jdk

  
No Fedora:  
  

  

  

 sudo dnf install java-11-openjdk

  
2º passo: Descompacte o arquivo zip, baixado acima:  
  

  

  

 unzip IRPF2021-1.1.zip

  
3º passo: Acesse a pasta descompactada:  
  

  

  

 cd IRPF2021

  
4º passo: Execute o arquivo do DIRPF 2021:  
  

  

  

 java -jar irpf.jar

  

### Considerações finais

  
Se, por algum motivo precisar do DIRPF 2020, veja nas matérias [Programa de declaração do IRPF 2020 no Debian, Ubuntu e derivados (Arquivo .bin + Java Oracle)](https://info.wsouza.com.br/2020/02/programa-de-declaracao-do-irpf-2020-instalacao-no-debian-e-derivados.html) e [Programa de declaração do IRPF 2020 no Linux com Java OpenJDK](https://info.wsouza.com.br/2020/03/programa-de-declaracao-do-irpf-2020-no-linux-com-java-openjdk.html).