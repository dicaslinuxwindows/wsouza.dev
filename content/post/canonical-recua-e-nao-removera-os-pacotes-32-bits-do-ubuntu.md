---
title: 'Canonical recua e não removerá os pacotes 32 bits do Ubuntu'
date: 2019-06-26T22:24:00.002-03:00
draft: false
url: /2019/06/canonical-recua-e-nao-removera-os-pacotes-32-bits-do-ubuntu.html
tags: 
- Linux
- Ubuntu
---

![Canonical recua e não removerá os pacotes 32 bits do Ubuntu - Dicas Linux e Windows](https://1.bp.blogspot.com/-gZexsjHkz9A/XRQQ6KaGNEI/AAAAAAAALtU/aG5dqZPJ8sIKlkCvDxvr0VStA5oJNxfkwCLcBGAs/s200/32BITSV.png "Canonical recua e não removerá os pacotes 32 bits do Ubuntu - Dicas Linux e Windows")

Após pressões a Canonical comunicou que o Ubuntu continuará oferecendo suporte à arquitetura 32 bits nas próximas versões. Leia mais detalhes a seguir.

  
  
  
  
  
  
  

Na semana passada foi anunciado que o Ubuntu não teria suporte para pacotes na arquitetura 32 bits (i386, x86), conforme divulgado em [Fim do Ubuntu 32bits](https://info.wsouza.com.br/2019/06/fim-do-ubuntu-32-bits.html).  
Porém, devido à pressões da comunidade, usuários, desenvolvedores e "parceiros", a empresa [soltou um comunicado oficial](https://blog.ubuntu.com/2019/06/24/statement-on-32-bit-i386-packages-for-ubuntu-19-10-and-20-04-lts) informando que a história não será bem assim.  
Os grandes afetados com a mudança seriam alguns projetos baseados no Ubuntu como o Wine e a Steam, e os desenvolvedores destes projetos abandonariam o Ubuntu. Como estas comunidades contribuem com o desenvolvimento de pacotes, isto não seria viável para a Canonical.  
Mas esta "volta" não será completa . Segundo o que foi divulgado neste comunicado, a empresa vai definir quais são os pacotes necessários e que devem continuar a receber suporte para seja possível a continuidade do uso nos projetos que dependem da arquitetura i386. Também, junto com os parceiros, a Canonical vai reforçar o uso de contêineres _(pacotes snap)_ para que seja possível rodar aplicativos antigos em versões recentes do Ubuntu.  
**Portanto:** As próximas versões do Ubuntu voltarão a ter suporte à arquitetura i386. Tal ação não muda nada em relação à não disponibilização de imagens _ISO_ de instalação para estas arquiteturas.  
  
Leia o comunicado na íntegra:  
  
  

_(Traduzido pelo Google Tradutor)_  
_Declaração sobre pacotes i386 de 32 bits para o Ubuntu 19.10 e 20.04 LTS Canonical em 24 de junho de 2019 Tags: i386, Ubuntu_  
_Graças à enorme quantidade de feedback deste fim de semana dos gamers, do Ubuntu Studio e da comunidade WINE, vamos mudar nosso plano e construir pacotes i386 de 32 bits selecionados para o Ubuntu 19.10 e 20.04 LTS._  
_Vamos colocar em prática um processo de comunidade para determinar quais pacotes de 32 bits são necessários para suportar software legado, e podemos adicionar a essa lista pós-lançamento se perdermos algo que é necessário._  
_As discussões da comunidade podem, às vezes, acontecer de forma inesperada, e essa é uma delas. A questão do suporte ao x86 de 32 bits foi levantada e discutida seriamente em fóruns de desenvolvedores e comunidades do Ubuntu desde 2014. É assim que tomamos decisões._  
_Após o lançamento do Ubuntu 18.04 LTS, tivemos vários tópicos na lista do ubuntu-devel e também consultamos a Valve detalhadamente sobre o assunto. Nenhuma dessas discussões levantou as paixões que vimos aqui, então sentimos que tínhamos consenso suficiente para a mudança no Ubuntu 20.04 LTS. Acreditamos que é razoável esperar que a comunidade participe e encontre o equilíbrio certo entre ativar a próxima onda de recursos e manter a cauda longa. No entanto, neste caso, é relativamente fácil para nós alterar o plano e ativar nativamente no Ubuntu 20.04 LTS os aplicativos para os quais há uma necessidade específica._  
_Também trabalharemos com o WINE, o Ubuntu Studio e as comunidades de jogos para usar a tecnologia de contêineres para abordar o fim da vida útil das bibliotecas de 32 bits; Deve ficar possível rodar aplicativos antigos em versões mais recentes do Ubuntu. O Snaps e o LXD permitem que tenhamos ambientes completos de 32 bits e bibliotecas integradas para resolver esses problemas a longo prazo._  
_Existe um risco real para quem está executando um conjunto de softwares que obtém poucos testes. Os fatos são que a maioria dos pacotes x86 de 32 bits dificilmente são usados. Isso significa menos globos oculares e mais bugs. O software continua a crescer em tamanho no nível mais alto, dificultando muito a criação de novos aplicativos em ambientes de 32 bits. Você já ouviu falar sobre o Specter e o Meltdown - muitas das atenuações desses ataques estão indisponíveis para sistemas de 32 bits._  
_Isso nos levou a parar de criar a mídia de instalação do Ubuntu para o i386 no ano passado e a considerar abandonar a porta completamente em uma data futura. Sempre foi nossa intenção manter a capacidade dos usuários de executar aplicativos de 32 bits no Ubuntu de 64 bits - nossos kernels suportam especificamente isso._