---
title: 'Debian Bullseye entra em congelamento'
date: 2021-01-17T23:20:00.003-03:00
draft: false
url: /2021/01/debian-bullseye-em-congelamento.html
tags: 
- Debian
- Linux
- Debian Bullseye
---

![Debian Bullseye em congelamento - Dicas Linux e Windows](https://1.bp.blogspot.com/-SbhWttE77FY/YATwDEx1s2I/AAAAAAAARio/QqJhOMdH7GApMYaM8L2luokkz0GkezY2wCNcBGAsYHQ/s16000/Bullseye-Freeze.png "Debian Bullseye em congelamento - Dicas Linux e Windows")

O Debian Bullseye entra na fase de congelamento. Veja nesta matéria o que isto significa e quais são as próximas etapas até o lançamento da versão final.

  
  
  
  
  
  
  

Em julho de 2020 fiz uma matéria mostrando como [acompanhar o desenvolvimento do Debian Bullseye](https://info.wsouza.com.br/2020/07/acompanhe-o-desenvolvimento-do-debian-bullseye.html), que naquele momento, fazia aproximadamente 1 ano que estava em desenvolvimento na "fase" testing. De lá pra cá os desenvolvedores continuaram trabalhando, trazendo as versões mais recentes dos aplicativos, corrigindo bugs e agora, em janeiro de 2021, inicia-se o congelamento _(freeze)_.  
  

### Mas, o que é esse congelamento?

  
Segundo o [Guia Foca](https://www.guiafoca.org/guiaonline/avancado/ch07s03.html):  
```
`  
_"Na data programada pela equipe de lançamento da Debian, a distribuição testing é congelada:  
  
nenhum pacote novo da unstable cai na testing e começa a procura de falhas na distribuição testing.  
  
Nenhuma nova característica é implementada nos pacotes (a não ser que seja extremamente necessário)  
  
e os developers se dedicam a correção de erros nos pacotes (...)"_  
`  

```  
O Debian é dividido em stable _(Buster)_, testing _(Bullseye)_, unstable _(Sid)_ e experimental, [_(mais detalhes aqui)_](https://info.wsouza.com.br/2019/07/debian-curiosidades-informacoes-suas-versoes-e-ciclo-de-vida.html). O congelamento do testing é um dos grandes passos para torná-lo stable e por este motivo, a partir do congelamento, os pacotes do unstable não entram mais no testing e a equipe de desenvolvimento concetra as energias para resolver os bugs ao mínimo possível para o lançamento.  
  

### Fases de congelamento e o que falta para o lançamento final.

  
No Debian não há uma data especifica para o lançamento da próxima versão, pois o lançamento só ocorre quando o sistema em níveis aceitáveis aos padrões do Debian. Nas últimas versões os lançamentos têm ocorrido aproximadamente a cada 2 anos.  

*   2011 - Squeeze (6)
*   2013 - Wheezy (7)
*   2015 - Jessie (8)
*   2017 - Stretch (9)
*   2019 - Buster (10)
*   _2021? - Bullseye (11)_

Segundo a [linha do tempo e política de congelamento do Bullseye](https://release.debian.org/bullseye/freeze_policy.html), as fases de congelamento serão: _(Com tradução automática em algumas partes)._  

*   **12/01/2021 - Marco 1 - Transição e congelamento essencial (compilar)**: Transição é quando alguma alteração em um pacote pode causar alterações em outros. [Pacotes essenciais](https://release.debian.org/bullseye/essential-and-build-essential.txt) que estejam nesta situação não serão mais alterados, pois as alterações podem causar bugs que podem demandar muito tempo para serem sanados. Sem grandes mudanças ou interrupções;
*   **12/02/2021 - Marco 2 - Soft Freeze:**
    *   Apenas pequenas correções direcionadas;
    *   Mantenedores focados em pequenas correções direcionadas;
    *   Se houver risco de alguma mudança atrapalhar o processo de lançamento, esta mudança nem entrará em teste;
    *   Se um pacote não entrou em teste até este momento, não entrará mais;
*   **12-03-2021 - Marco 3 - Hard Freeze - para pacotes-chave e pacotes sem autopkgtests:**
    *   Hard freeze para pacotes principais: Como os pacotes principais são isentos de remoções automáticas, erros RC ou regressões nos pacotes principais podem causar atrasos no processo de congelamento. Para diminuir a mudança de novas regressões no teste, todas as mudanças nos pacotes principais precisarão ser desbloqueadas pela equipe de lançamento;
    *   Hard freeze para pacotes não-chave sem autopkgtests: Mudanças em pacotes não-chave que não têm autopkgtests requerem um desbloqueio pela equipe de lançamento.
    *   Soft freeze para pacotes não chave com autopkgtests: Para pacotes não chave com autopkgtests (não triviais), as regras do soft freeze ainda se aplicam, mas o atraso da migração é aumentado para 20 dias. Isso permite que as correções direcionadas ao seu pacote cheguem aos testes (eventualmente), sem a necessidade da equipe de lançamento revisá-las.
*   **TBA - Marco 4 - Congelamento total _(Full Freeze)_**: Só pretendemos iniciar o Full Freeze pouco antes do lançamento real do Bullseye. A data de início do Full Freeze será decidida quando começarmos a planejar uma data de lançamento e será anunciada pelo menos 14 dias antes de entrar em vigor. Durante o Full Freeze, todos os pacotes só podem migrar para teste após revisão manual pela equipe de lançamento. Para pacotes-chave e pacotes sem autopkgtests, as regras permanecem as mesmas. Desde o início do congelamento total, essas regras também se aplicam a outros pacotes.

  

### Alguns pacotes que entraram antes do congelamento

  
Os pacotes listados abaixo são alguns que entraram no Debian Bullseye antes da fase de congelamento, portanto estarão no lançamento final.

*   Kernel 5.10
*   Plasma 5.20
*   XFCE 4.16
*   GNOME 3.38.2
*   LXQT 0.16
*   Cinnamon 4.8

  

### Já posso utilizar o Debian Bullseye?

  
Sim. Você pode tanto baixar uma imagem ISO com as compilações lançadas diariamente _(Daily Builds, apenas Netinstall sem interface gráfica)_, ou ainda uma imagem ISO com as compilações semanais _(Weekly Builds)_, no formato Live, que pode ser [gravado e executado pelo pendrive.](https://info.wsouza.com.br/2020/04/3-maneiras-de-gravar-uma-imagem-iso-num-pendrive-utilizando-linux.html) Os links abaixo são para a arquitetura _amd64_.  
  

Debian Bullseye

[ Daily Build](https://cdimage.debian.org/cdimage/daily-builds/daily/arch-latest/amd64/iso-cd/debian-testing-amd64-netinst.iso)

[ Weekly Build](https://cdimage.debian.org/cdimage/weekly-live-builds/amd64/iso-hybrid/debian-live-testing-amd64-gnome.iso)

[ _Mais..._](https://cdimage.debian.org/cdimage/weekly-live-builds/)

  

### Caso de uso

  
Depois de testar o Bullseye separadamente durante um tempo, há alguns meses deixei o Buster e passei a utilizá-lo como padrão. Não encontrei nenhum problema com os aplicativos que utilizo, muitos deles estão nas versões mais recentes _(ou bem próximos)_. A pouca quantidade de problemas não é uma surpresa, pois os padrões do Debian são bem rígidos, minimizando a chance de um problema sério, mesmo num sistema em testes. Mas sempre há possibilidade de aparecer algum problema sério.  
  

### Considerações finais

  
Nos próximos meses, conforme os marcos listados anteriormente forem cumpridos, o Debian Bullseye vai estar cada vez mais no noticiário, e seu lançamento final estará cada vez mais perto. Este processo será acompanhado e noticiado por aqui.  
  

### Referências

  
[Debian - Curiosidades, informações, suas versões e ciclo de vida](https://info.wsouza.com.br/2019/07/debian-curiosidades-informacoes-suas-versoes-e-ciclo-de-vida.html).  
[Bullseye Freeze Timeline and Policy](https://release.debian.org/bullseye/freeze_policy.html)  
[Guia Foca: O que é sid/testing/frozen/stable?](https://www.guiafoca.org/guiaonline/avancado/ch07s03.html)