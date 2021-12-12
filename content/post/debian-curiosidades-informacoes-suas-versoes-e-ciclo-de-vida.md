---
title: 'Debian - Curiosidades, informações, versões e ciclo de vida'
date: 2019-07-03T00:05:00.003-03:00
draft: false
url: /2019/07/debian-curiosidades-informacoes-suas-versoes-e-ciclo-de-vida.html
tags: 
- Debian
- Linux
- Artigos
---

![Debian - Curiosidades, informações, versões e ciclo de vida - Dicas Linux e Windows](https://2.bp.blogspot.com/-olDZe7B03F4/XRudNRxysmI/AAAAAAAALvU/-vK_KAD90Q0YSO-fsQg-a8TtOdZzLL3VQCLcBGAs/s1600/Debian-Logo.png "Debian - Curiosidades, informações, versões e ciclo de vida - Dicas Linux e Windows")

Nesta matéria fiz um resumo de informações e comentei um pouco sobre o Debian, como funciona seu ciclo de desenvolvimento, seu ciclo de vida e mais algumas informações básicas, úteis e necessárias.

  
  
  
  
  
  

### Debian

  

#### O que é

  
O [Debian](https://www.debian.org/) é um sistema operacional composto inteiramente por softwares livres. É mantido pela Fundação Debian e distribuído pelo Projeto Debian. Os sistemas Debian atualmente usam o kernel Linux ou o kernel FreeBSD. Há um trabalho em andamento para disponibilizá-lo com o Kernel Hurd, do projeto GNU. Anteriormente era chamado de Debian GNU/Linux.  
  

#### História e Filosofia

  
O Debian foi iniciado em agosto de 1993 por Ian Murdock, através do [Manifesto Debian](https://pt.wikipedia.org/wiki/Manifesto_Debian), como uma nova distribuição que seria feita abertamente, no espírito do Linux e do projeto GNU. O Debian foi concebido para ser feito cuidadosamente e conscienciosamente, e ser mantido e suportado com cuidado similar. Ele começou como um grupo pequeno, bastante unido, de hackers de Software Livre e cresceu gradualmente para se tornar uma comunidade global e bem organizada de desenvolvedores e usuários.  
O nome Debian vem dos nomes de seus criadores, Ian Murdock, e sua esposa, Debra. Saiba mais sobre a história do Debian [aqui.](https://www.debian.org/doc/manuals/project-history/index.pt.html#contents)  
Uma das grandes diferenças do Debian para outros sistemas Linux é o controle quanto a qualidade dos pacotes para que estes só sejam lançados quando estiverem totalmente prontos, funcionais. Tal política garante estabilidade e, principalmente, confiabilidade ao sistema. Segundo a filosofia adotada pelo Debian, Software Livre refere-se à liberdade e não à custo zero, como muitas pessoas confundem. O projeto Debian é mantido por meio de doações à organização sem fins lucrativos _Software in the Public Interest (SPI)._  
  

#### Pacotes

  
Atualmente o Debian conta com mais de 51.000 pacotes livres. Apesar de ser construído por softwares livres não há nada que impeça a instalação de softwares não-livres, portanto, este número aumenta exponencialmente.  
O Debian possui um conhecido e robusto sistema de gestão de pacotes, o APT. e o formato de pacotes é o ._deb_. Através do APT é possível gerenciar os pacotes relacionados à atualizações de softwares, de partes do sistema e até mesmo a atualização total do sistema de forma relativamente fácil e segura.  
  

#### Hardware e arquiteturas suportadas

  
Geralmente o Debian funciona normalmente em qualquer hardware comum, sendo compatível com a maioria dos computadores pessoais, mesmo os mais antigos. A cada lançamento de uma nova versão o hardware suportado sofre pequenas alterações, podendo ser consultadas na [página da distribuição estável.](https://www.debian.org/releases/stable/) Caso tenha dúvidas se o seu hardware é suportado verifique a [lista de hardware suportado](http://www.tldp.org/HOWTO/Hardware-HOWTO/).  
  

#### Debian, o pai de todos

  
Junto com o Red Hat e Slackware, o Debian é uma mais antigas distribuições Linux. Pode ser considerável o pai de todos, pois há inúmeras distribuições baseadas nele. Algumas destas versões são muito conhecidas, como o Ubuntu, o Linux Mint Debian Edition e o Knoppix _(onde surgiu o sistema live-cd)_. Os usuários brasileiros mais antigos vão lembrar do Kurumin Linux. [Veja as distribuições baseadas no Debian, de acordo com o Debian Wiki.](https://wiki.debian.org/Derivatives/Census)  
  

### Versões

  
O Debian anuncia seu novo lançamento estável de forma regular, porém, qualquer versão só será lançada quando estiver pronta. Portanto, não existem datas estipuladas para os lançamentos. As quatro últimas versões foram lançadas em 2013, 2015, 2017 e 2019.  
Toda versão lançada possui um número e um codinome. Os números são sequenciais e os nomes são derivados dos personagens do filme [Toy Story](https://www.debian.org/doc/manuals/debian-faq/ch-ftparchives#s-sourceforcodenames).  
  

#### Ciclo de desenvolvimento e ciclo de vida

  
Usuários podem contar com 3 anos de suporte total para cada lançamento e, no final de seu  End of Life (EOL) passa a ser Oldstable e recebe mais 2 anos de suporte extra LTS - Long Term Support , ainda recebendo um suporte ELTS por mais um período.  
Normalmente sempre há 3 versões ativas, sendo Unstable _(Instável)_, Testing e Stable _(Estável)_. Veja mais detalhes abaixo:  

*   **Unstable** - É a versão onde ocorre o desenvolvimento do Debian e é utilizada por desenvolvedores, não sendo recomendada para o usuário comum devido à instabilidade dos pacotes. Esta versão sempre receberá o nome de _sid._
*   **Testing** - A distribuição "testing" contém pacotes que ainda não foram aceitos na versão "estável (stable)", mas estão na fila para tanto. A principal vantagem de usar esta distribuição é que ela possui versões mais recentes de software. A partir de momento que uma versão Testing vira Stable, a atual Unstable passa a ser Testing.
*   **Stable** - A distribuição estável (stable) contém a última versão oficialmente lançada do Debian e é a versão recomendada para uso em máquinas de produção. Não é lançada com as últimas versões dos pacotes.
*   **Experimental** - Neste ponto os pacotes estão entrando no Debian. Não é recomendável utilizar pacotes nesta fase.
*   **Debian LTS (Oldstable)** - Após o fim do ciclo de vida da Stable anterior, esta torna-se Oldstable e passa a receber suporte LTS por um período de 2 anos.
*   **Debian ELTS** - A partir do momento que a Stable atual vira Oldstable, a versão que era Oldstable até então passa a receber suporte ELTS, por mais um período.

A imagem abaixo mostra o tempo de suporte LTS e ELTS das últimas versões. Nota-se que o Debian Wheezy, que foi lançada em 2013, deixou de obter suporte ELTS em 01/05/2019.  
  

[![](https://3.bp.blogspot.com/-ymTLg3y2XyY/XRulQoQjroI/AAAAAAAALvg/Q8Fo_nY-E5E73qhRtBUuBeP6-uYKkP33gCLcBGAs/s1600/Debian-LTS.png)](https://3.bp.blogspot.com/-ymTLg3y2XyY/XRulQoQjroI/AAAAAAAALvg/Q8Fo_nY-E5E73qhRtBUuBeP6-uYKkP33gCLcBGAs/s1600/Debian-LTS.png)

  

#### Repositórios/Espelhos

  
Todos os pacotes ficam disponíveis em repositórios que são espalhados em servidores ao redor do mundo (chamados de espelhos). É nestes repositórios que o APT conecta para atualizá-los na distribuição. A lista de repositórios é dividida em seções da seguinte forma, de acordo com o Debian Wiki:  

*   **Main** - Contém todos os pacotes que estão completamente de acordo com o Debian Free Software Guilines.
*   **Contrib -** É um conjunto de programas de código aberto que não podem funcionar sem um elemento não livre. 
*   **Non-Free** - Contém programas os quais não estão (completamente) de acordo com estes princípios do Software Livre, mas que podem, contudo, ser distribuídos sem restrições. Estes pacotes, o qual não é parte oficial do Debian, é um serviço para os usuários que podem precisar de alguns desses programas, entretanto o Debian sempre recomenda dar prioridade aos programas livres. 
*   **Updates -** Esse repositório recebe as atualizações de pacotes, com correções e melhorias. 
*   **Backports - ** O repositório backports oferece “pacotes backports”. O termo refere-se a um pacote de algum software recente, que foi recompilado para uma distribuição mais velha, geralmente para Stable. Quando a distribuição começa a envelhecer, vários projetos de software lançam novas versões que não são integradas na Stable atual (que é modificada apenas para resolver os problemas mais críticos, como problemas de segurança). Como as distribuições Testing e Unstable podem ser mais arriscadas, mantenedores de pacotes oferecem recompilações de software recente para a Stable, que tem a vantagem de limitar instabilidade potencial a um pequeno número de pacotes escolhidos.
*   **Security -** As atualizações de segurança não são hospedadas na rede habitual de espelhos do Debian, mas em security.debian.org (em um pequeno conjunto de máquinas mantidas pelos Administradores de Sistema Debian). Estes arquivos contém as atualizações de segurança (elaboradas pela equipe de segurança do Debian e/ou mantenedores de pacotes) para a distribuição Stable. 
*   **Proposed-Updates** - depois de publicada, a distribuição stable é atualizada em aproximadamente de dois em dois meses. o repositório atualizações-propostas é onde as atualizações esperadas são preparadas (sob a supervisão dos gerentes de versão estável). Os mantenedores de pacotes também têm a oportunidade de corrigir erros importantes que não merecem uma libertação imediata. qualquer um pode usar este repositório para testar estas atualizações antes de sua publicação oficial.

Numa instalação padrão apenas as seções securit, main  e updates vêm habilitadas, sendo necessária habilitar as outras caso necessite.  
  

### Obtendo e instalando o Debian

  
Você pode obter o Debian de diversas maneiras, sendo que uma das mais comuns é através de imagens ISO que podem ser gravadas em CD, DVD ou Pendrive. Esta imagens ISO podem ser baixadas de maneira direta, através de torrents ou por um sistema chamado jigdo. Abaixo, um detalhamento destes tipos de imagens.  

*   NetInst - É uma ISO que possui o instalador em modo gráfico. Após a instalação do sistema básico ele sugere a escolha da interface gráfica, que será baixada da internet e instalada. Geralmente esta ISO possui cerca de 180-250 MB.
*   CD/DVD - Possui o instalador e modo gráfico e e interface gráfica já está no CD/DVD, não necessitando efetuar downloads para concluir a instalação. O tamanho depende da quantidade de pacotes e obviamente, no DVD há mais pacotes do que no CD.
*   Live CD/DVD - O sistema live consiste numa imagem com o sistema compactado que, no momento o boot é descompactado na memória RAM. A grande vantagem este sistema é a possibilidade de ver o sistema funcionando antes da instalação.

Todas as imagens são disponibilizadas para aqueles arquiteturas que a versão em questão suporta. Há imagens para cada interface gráfica, permitindo que o usuário escolha a que desejar.  
Uma boa documentação sobre a instalação está no [Guia de Instalação de Debian GNU/Linux](https://www.debian.org/releases/stable/installmanual), disponível para a versão Stable.  
Há também outras formas de instalar. Veja no exemplo abaixo, utilizando como exemplo o Debian Buster:  
  

**[Atualizando para o Debian Buster](https://info.wsouza.com.br/2019/07/atualizando-para-o-debian-buster.html)**  

  

### Considerações finais

  
Esta matéria não tem, nem de perto, a pretensão de ser uma documentação sobre o Debian. A pretensão da mesma é fornecer algumas informações superficiais para os usuários que não tem muito contato com este sistema. Como sempre posto alguma coisa sobre o Debian, achei necessário fazer um resumo de informações para que estas sirvam de base para as outras matérias do blog. Os links abaixo foram utilizados para gerar este resumo e com certeza aumentarão o conhecimento sobre o sistema, portanto, não hesite em utilizá-los.  
Caso tenha alguma dúvida ou sugestão participe comentando logo abaixo.  
  

### Referências/Fontes

  
[Sobre o Debian](https://www.debian.org/intro/about)  
[Versões](https://www.debian.org/releases/)  
[Ciclo de vida](https://wiki.debian.org/DebianReleases)  
[Debian Long Time Support (LTS)](https://wiki.debian.org/LTS)  
[Debian Extended Long Time Support (ELTS)](https://wiki.debian.org/LTS/Extended)  
[Suporte pago](https://www.debian.org/consultants/)  
[Debian Releases](https://wiki.debian.org/DebianReleases)  
[Documentação do Debian](https://www.debian.org/doc/)  
[Canto dos desenvolvedores](https://www.debian.org/devel/)  
[Manual do Debian](https://www.debian.org/doc/manuals/debian-handbook/)  
[Repositórios](https://wiki.debian.org/configura%C3%A7%C3%A3o%20repositorios%20PT%20BR)  
[Obtendo o Debian](https://www.debian.org/distrib/)  
[Acompanhe as notícias sobre o desenvolvimento do Debian](https://www.debian.org/News/weekly/)  
[Debian Micronews](https://micronews.debian.org/)