---
title: 'Como instalar o programa de declaração do imposto de renda 2019 no Linux'
date: 2019-03-11T19:37:00.005-03:00
draft: false
url: /2019/03/como-instalar-o-programa-de-declaracao-do-imposto-de-renda-2019-no-linux.html
tags: 
- Linux
- Tutoriais
- IRPF
---

Se procura a versão 2020, veja em: [Programa de declaração do IRPF 2020 - Instalação no Debian e Derivados](https://info.wsouza.com.br/2020/02/programa-de-declaracao-do-irpf-2020-instalacao-no-debian-e-derivados.html)

  
Chegou o mês de março, passou o carnaval e, como de costume, chegou a hora de declarar o imposto de renda. Se você utiliza algum sistema baseado em Linux, e tem dificuldades para instalar o programa que faz a declaração, leia nesta matéria como fazê-lo.

[![Dicas Linux e Windows - Como instalar o programa de declaração do imposto de renda 2019 no Linux](https://2.bp.blogspot.com/-Bgvir50JhJw/XIbiz7H6sII/AAAAAAAAKyY/c5ndniyHjqQ-rcxV9w4zy52cb5CHuoemwCLcBGAs/s1600/Irfp%25281%2529.png "Dicas Linux e Windows - Como instalar o programa de declaração do imposto de renda 2019 no Linux")](https://2.bp.blogspot.com/-Bgvir50JhJw/XIbiz7H6sII/AAAAAAAAKyY/c5ndniyHjqQ-rcxV9w4zy52cb5CHuoemwCLcBGAs/s1600/Irfp%25281%2529.png)

O programa que será instalado realiza a declaração de imposto de renda de pessoa física, por isto é chamado de IRPF, e seu instalador está disponível no formato _.BIN_.  
Todo procedimento será realizado no Debian, testado na versão Jessie e Stretch.  
Um dos pré requisitos para instalar o IRPF é ter o Java instalado. O Java pertence à uma empresa chamada Oracle, e no Debian os softwares proprietários não vêm incluídos no sistema. Para resolver este problema eu utilizo o OpenJDK, que é uma versão do Java em código aberto e está disponível nos repositórios do Debian. Para instalar, execute os comandos a seguir no terminal:  
  

sudo apt-get update

sudo apt-get install openjdk-8-jdk

  
Mas caso seja necessário utilizar o Java Oracle, veja como fazê-lo na matéria [Java Oracle 11 - Instalando no Debian de maneira rápida e fácil.](https://info.wsouza.com.br/2019/03/java-oracle-11-instalando-no-debian-de-maneira-rapida-e-facil.html)

  

### Download do programa

Após a instalação do OpenJDK, vamos à página de download do IRPF. Faça o download do arquivo de instalação no [neste link](http://receita.economia.gov.br/interface/cidadao/irpf/2019/download/outros-sistemas-operacionais), direto do site da Receita Federal. Note que há a opção para sistemas 32 e 64 bits. Clique na opção referente à arquitetura do seu sistema.  
Para descobrir a arquitetura do seu sistema, abra o terminal e digite: **uname -m**  
  
Escolha a opção desejada e faça o download.  
  

[![Dicas Linux e Windows - Como instalar o programa de declaração do imposto de renda 2019 no Linux](https://1.bp.blogspot.com/-6KN_Bb1cXl4/XIXUWKhcmQI/AAAAAAAAKw0/XmAVQaByRVY5Kdard-N8bQazIlO_DLCtgCLcBGAs/s1600/Captura%2Bde%2Btela%2Bde%2B2019-03-10%2B23-02-33.png "Dicas Linux e Windows - Como instalar o programa de declaração do imposto de renda 2019 no Linux")](https://1.bp.blogspot.com/-6KN_Bb1cXl4/XIXUWKhcmQI/AAAAAAAAKw0/XmAVQaByRVY5Kdard-N8bQazIlO_DLCtgCLcBGAs/s1600/Captura%2Bde%2Btela%2Bde%2B2019-03-10%2B23-02-33.png)

  
Neste exemplo utilizei a versão para arquitetura 64bits. Recomendo que faça o download na pasta /home/seu-nome-de-usuário. O nome do arquivo baixado, neste caso é IRPF2019Linux-x86\_64v1.0.bin.

  

### Instalação

Antes de iniciar a instalação é preciso dar ao arquivo baixado a permissão de execução, isto pode ser feito de duas maneiras: 1 - Clique com o botão direito do mouse e vá em propriedades, depois marque a opção permitir execução ou executável _(os nomes podem variar dependendo da distribuição/interface)._ 2 - Abra o terminal (Ctrl + T) e dê as permissões de execução para o arquivo IRPF2019Linux-x86\_64v1.0.bin, que foi baixado no passo anterior e é o instalador do IRPF. Para fazer isto execute o comando abaixo:  
  

chmod +x IRPF2019Linux-x86\_64v1.0.bin

  
Após, para instalar, há duas opções: 1 - Clique duas vezes no arquivo. 2- Ainda no terminal execute o comando abaixo.  
  

./IRPF2019Linux-x86\_64v1.0.bin

  
A instalação será iniciada, basta avançar até o final pronto, o atalho será criado no menu, e pronto, IRPF2019 instalado com sucesso.  
  

[![Dicas Linux e Windows - Como instalar o programa de declaração do imposto de renda 2019 no Linux](https://4.bp.blogspot.com/-xy0lku_XWgs/XIXWfcFTuII/AAAAAAAAKxc/fqT78FqLw8MORjeFrQc8cmVo-4MWwOZiACPcBGAYYCw/s1600/Captura%2Bde%2Btela%2Bde%2B2019-03-11%2B00-27-57.png "Dicas Linux e Windows - Como instalar o programa de declaração do imposto de renda 2019 no Linux")](https://4.bp.blogspot.com/-xy0lku_XWgs/XIXWfcFTuII/AAAAAAAAKxc/fqT78FqLw8MORjeFrQc8cmVo-4MWwOZiACPcBGAYYCw/s1600/Captura%2Bde%2Btela%2Bde%2B2019-03-11%2B00-27-57.png)

  
  

Abaixo o IRPF2019 instalado.

  
  

[![Dicas Linux e Windows - Como instalar o programa de declaração do imposto de renda 2019 no Linux](https://3.bp.blogspot.com/-AhQEhcOItZY/XIY_KitD0TI/AAAAAAAAKxw/dXM0mhPF04IyMc7iaXg_Pb7VGKJJvCAIQCPcBGAYYCw/s640/Captura%2Bde%2Btela%2Bde%2B2019-03-11%2B00-29-42.png "Dicas Linux e Windows - Como instalar o programa de declaração do imposto de renda 2019 no Linux")](https://3.bp.blogspot.com/-AhQEhcOItZY/XIY_KitD0TI/AAAAAAAAKxw/dXM0mhPF04IyMc7iaXg_Pb7VGKJJvCAIQCPcBGAYYCw/s1600/Captura%2Bde%2Btela%2Bde%2B2019-03-11%2B00-29-42.png)

  

### Observações finais

Caso precise de um ou mais destes programas baixe-os no endereço a seguir: [http://receita.economia.gov.br/orientacao/tributaria/declaracoes-e-demonstrativos/dirpf/entrega-da-declaracao-do-irpf/download-programas-dirpf](http://receita.economia.gov.br/orientacao/tributaria/declaracoes-e-demonstrativos/dirpf/entrega-da-declaracao-do-irpf/download-programas-dirpf). O princípio de instalação é o mesmo para os programas dos anos anteriores.