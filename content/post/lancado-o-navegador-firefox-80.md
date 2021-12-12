---
title: 'Lançado o navegador Firefox 80'
date: 2020-08-25T23:09:00.001-03:00
draft: false
url: /2020/08/lancado-o-navegador-firefox-80.html
tags: 
- Dicas
- Firefox
---

![Lançado o navegador Firefox 80 - Dicas Linux e Windows](https://1.bp.blogspot.com/-PLlzYvAUUX4/X0WuYKZE4YI/AAAAAAAAPw8/QJZt1Ho9nns_vCwLGl4H-UXtegvussRNACNcBGAsYHQ/s1600/Firefox_80.png "Lançado o navegador Firefox 80 - Dicas Linux e Windows")

Foi anunciado o lançamento da versão 80 do navegador Firefox. Confira a seguir quais foram as novidades lançadas nesta versão.

  
  
  
  
  
  
  

O Mozilla Firefox ainda é o segundo navegador mais utilizado no mundo, porém, esta vice liderança está ameaçada pelo Microsoft Edge _(e pode ser que já tenha sido perdida)_. Paralelamente aos acontecimentos, a fundação Mozilla continua trabalhando nas atualizações com correções e melhorias, e chega agora na versão 80.  
  

### Novidades

  

*   No Windows 10, o Firefox agora pode ser definido como o visualizador de PDF padrão do sistema;
*   No Linux agora é possível habilitar a aceleração de GPU para Firefox no X11, algo que já era possível no Wayland. Para ativar: Na barra de endereços digite **about:config**, depois pesquise por **vaapi** e aparacerão as opções **media.ffmpeg.vaapi-drm-display.enabled** e **media.ffmpeg.vaapi.enabled**. Dê um duplo clique em cima de cada um deles e os valores serão alterados de falso para verdadeiro, ativando a aceleração por GPU. As aletarções terão efeito após reiniciar o navegador.

  

### Bugs e correções de segurança

  
Nesta versão, vários bugs foram corrigidos:  

*   Redução de travamentos quando se utiliza leitores de tela;
*   Correções nas Ferramentas para Desenvolvedores do Firefox, permitindo que os usuários de leitores de tela se beneficiassem de algumas das ferramentas que antes eram inacessíveis;
*   Ainda no campo de leitores de tela, os elementos SVG title e desc (rótulos e descrições) agora estão corretamente expostos a produtos de tecnologia assistiva;
*   Redução no número de animações, como carregamentos de guia, para diminuir o movimento para usuários com enxaqueca e epilepsia;
*   A nova lista de bloqueio de complementos foi habilitada para melhorar o desempenho e a escalabilidade.

  
Segue abaixo a lista de correções de segurança:  
  
```
`  
Vulnerabilidades de segurança corrigidas no Firefox 80  
Anunciado  
25 de agosto de 2020  
Impacto  
Alto  
Produtos  
Raposa de fogo  
Fixo em  
Firefox 80  
#CVE-2020-15663: Ataque de downgrade no Mozilla Maintenance Service pode ter resultado em escalada de privilégio  
Repórter  
Xiaoyin Liu  
Impacto  
Alto  
Descrição  
Se o Firefox estiver instalado em um diretório gravável pelo usuário, o Mozilla Maintenance Service executará o updater.exe a partir do local de instalação com privilégios administrativos. Embora o Mozilla Maintenance Service garanta que o updater.exe seja assinado pela Mozilla, a versão pode ter sido revertida para uma versão anterior, o que teria permitido a exploração de um bug mais antigo e a execução arbitrária de código com privilégios de sistema.  
Observação: esse problema afetou apenas os sistemas operacionais Windows. Outros sistemas operacionais não são afetados.  
  
Referências  
Bug 1643199  
#CVE-2020-15664: prompt induzido pelo invasor para instalação de extensão  
Repórter  
Kaizer Soze  
Impacto  
Alto  
Descrição  
Ao manter uma referência à eval()função de uma janela sobre: ​​em branco, uma página da web mal-intencionada poderia ter obtido acesso ao objeto InstallTrigger, o que permitiria que ela solicitasse ao usuário a instalação de uma extensão. Combinado com a confusão do usuário, isso pode resultar na instalação de uma extensão não intencional ou maliciosa.  
  
Referências  
Bug 1658214  
#CVE-2020-12401: Ataque temporizado na geração de assinatura ECDSA  
Repórter  
Sohaib ul Hassan, Iaroslav Gridin, Ignacio M. Delgado-Lozano, Cesar Pereida García, Jesús-Javier Chi-Domínguez, Alejandro Cabrera Aldaya e Billy Bob Brumley, Grupo de Segurança de Rede e Informação (NISEC), Universidade de Tampere, Finlândia  
Impacto  
moderado  
Descrição  
Durante a geração da assinatura ECDSA, o preenchimento aplicado no nonce projetado para garantir a multiplicação escalar em tempo constante foi removido, resultando em execução em tempo variável dependente de dados secretos.  
  
Referências  
Bug 1631573  
#CVE-2020-6829: P-384 e P-521 vulneráveis ​​a um ataque de canal lateral eletromagnético na geração de assinatura  
Repórter  
Sohaib ul Hassan, Iaroslav Gridin, Ignacio M. Delgado-Lozano, Cesar Pereida García, Jesús-Javier Chi-Domínguez, Alejandro Cabrera Aldaya e Billy Bob Brumley, Grupo de Segurança de Rede e Informação (NISEC), Universidade de Tampere, Finlândia  
Impacto  
moderado  
Descrição  
Ao executar a multiplicação de ponto escalar EC, o algoritmo de multiplicação de ponto wNAF foi usado; que vazou informações parciais sobre o nonce usado durante a geração da assinatura. Dado um traço eletromagnético de algumas gerações de assinatura, a chave privada poderia ter sido computada.  
  
Referências  
Bug 1631583  
#CVE-2020-12400: P-384 e P-521 vulneráveis ​​a um ataque de canal lateral na inversão modular  
Repórter  
Sohaib ul Hassan, Iaroslav Gridin, Ignacio M. Delgado-Lozano, Cesar Pereida García, Jesús-Javier Chi-Domínguez, Alejandro Cabrera Aldaya e Billy Bob Brumley, Grupo de Segurança de Rede e Informação (NISEC), Universidade de Tampere, Finlândia  
Impacto  
moderado  
Descrição  
Ao converter as coordenadas projetivas em afins, a inversão modular não foi realizada em tempo constante, resultando em um possível ataque de canal lateral baseado em tempo.  
  
Referências  
Bug 1623116  
#CVE-2020-15665: Barra de endereço não redefinida ao escolher permanecer em uma página após a caixa de diálogo beforeunload ser exibida  
Repórter  
Luan Herrera  
Impacto  
moderado  
Descrição  
O Firefox não redefiniu a barra de endereço depois que a caixa de diálogo beforeunload foi mostrada se o usuário escolheu permanecer na página. Isso pode ter resultado na exibição de um URL incorreto quando usado em conjunto com outros comportamentos inesperados do navegador.  
  
Referências  
Bug 1651636  
#CVE-2020-15666: a propriedade da mensagem MediaError vaza o status de resposta de origem cruzada  
Repórter  
Gunes Acar  
Impacto  
baixo  
Descrição  
Ao tentar carregar um não-vídeo em um contexto de áudio / vídeo, o código de status exato (200, 302, 404, 500, 412, 403, etc.) foi divulgado por meio da Mensagem MediaError. Esse nível de vazamento de informações é inconsistente com a divulgação padronizada de erro / sucesso e pode levar à inferência do status de login para serviços ou descoberta de dispositivo em uma rede local, entre outros ataques.  
  
Referências  
Bug 1450853  
#CVE-2020-15667: estouro de heap ao processar um arquivo de atualização  
Repórter  
crixer  
Impacto  
baixo  
Descrição  
Ao processar um arquivo de atualização MAR, após a validação da assinatura, um comprimento de nome inválido pode resultar em um estouro de heap, levando à corrupção da memória e à execução de código potencialmente arbitrário. No Firefox, conforme lançado pela Mozilla, esse problema só pode ser explorado com a chave de assinatura controlada pelo Mozilla.  
  
Referências  
Bug 1653371  
#CVE-2020-15668: Data Race ao ler as informações do certificado  
Repórter  
Tyson Smith  
Impacto  
baixo  
Descrição  
Faltava um bloqueio ao acessar uma estrutura de dados e importar as informações do certificado para o banco de dados confiável.  
  
Referências  
Bug 1651520  
#CVE-2020-15670: Erros de segurança de memória corrigidos no Firefox 80 e Firefox ESR 78.2  
Repórter  
Desenvolvedores Mozilla  
Impacto  
Alto  
Descrição  
Os desenvolvedores da Mozilla, Jason Kratzer, Christian Holler, Byron Campen e Tyson Smith relataram bugs de segurança de memória presentes no Firefox 79 e Firefox ESR 78.1. Alguns desses bugs mostraram evidências de corrupção de memória e presumimos que, com esforço suficiente, alguns deles poderiam ter sido explorados para executar código arbitrário.  
`  

```  

### Download e atualização

  
No Ubuntu, Linux Mint e Fedora já é possível baixar o Firefox 80 diretamente pela atualização do próprio sistema, via repositório. No Debian não tem essa possibilidade, pois a mesma conta com o Firefox-ESR em seu repositório, e este está na versão 68.  
Usuários do Windows, ou usuários Linux que que desejam instalar o pacote no formato [Flatpak](https://info.wsouza.com.br/2020/12/flatpak-e-snap-no-debian-fedora-e-ubuntu.html), podem baixar nos links abaixo:  
  

[ Windows](https://www.mozilla.org/firefox/download/thanks/)

[ Flatpak](https://flathub.org/apps/details/org.mozilla.firefox)

  

### Referências

  
[OMG! Ubuntu](https://www.omgubuntu.co.uk/2020/08/firefox-80-release-linux-gpu-acceleration/) e [Notas de lançamento do Firefox 80](https://www.mozilla.org/en-US/firefox/80.0/releasenotes/)