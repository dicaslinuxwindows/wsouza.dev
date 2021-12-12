---
title: 'Ubuntu Groovy Gorilla Lançado'
date: 2020-10-22T23:58:00.005-03:00
draft: false
url: /2020/10/ubuntu-groovy-gorilla-lancado.html
tags: 
- Linux
- Ubuntu
- Ubuntu 20.10
---

![](https://1.bp.blogspot.com/-0-StLx5vmSY/X5JJsftGbrI/AAAAAAAAQi8/zX63iV3snoY8az6d5-KLiTyQVBkwnLS4ACNcBGAsYHQ/s0/Groovy_Gorilla_Lan%25C3%25A7ado.png)

Os desenvolvedores do Ubuntu anunciam o lançamento do Ubuntu 20.10 Groovy Gorilla. Veja a seguir como baixar e instalar.

  
  
  
  
  
  
  

### Groovy Gorilla

  
Conforme programado o Ubuntu Groovy Gorilla é lançado no dia 22 de outubro. O nome Groovy é um adjetivo que lembra moda, e Gorilla significa Gorila mesmo.  
O Groovy Gorilla é a primeira das 3 versões intermediárias que são lançadas entre cada versão LTS _(as outras duas serão a 21.04 e 21.10)._É uma versão estável e seu suporte terá duração de 9 meses, acanbando em julho de 2021, conforme o ciclo de vida das versões do Ubuntu. Saiba mais detalhes sobre o Ubuntu, suporte de suas versões e ciclo de vida na matéria: [Ubuntu - Como funciona a política de seu ciclo de vida](https://info.wsouza.com.br/2019/03/ubuntu-como-funciona-politica-de-seu-ciclo-de-vida.html).  
  

### Novidades

  
Não houve grandes mudanças em relação ao seu antecessor e algumas já foram adiantadas em matérias anteriores. Mas, de qualquer forma, algumas das principais novidades são:  

*   Kernel 5.8 com maior supote e atualizações;
*   Active directory ativado na instalação. O active directory é uma ferramenta da Microsoft que gerencia os usuários de rede;
*   Novo papel de parede
*   Firefox 81
*   LibreOffice 7.0.2
*   Thunderbird 78.3.2
*   [Gnome 3.38](https://info.wsouza.com.br/2020/09/gnome-338-e-lancado.html)
*   nftables como padrão de firewall
*   Botão de reiniciar. Antes o botão reiciciar na interface só era possível ser adicionado por meio de extensões

  
Mais novidades nas notas de lançamento. _(traduzidas automaticamente de [https://discourse.ubuntu.com/t/groovy-gorilla-release-notes/15533](https://discourse.ubuntu.com/t/groovy-gorilla-release-notes/15533))_  
```
`  
Notas de lançamento do Groovy Gorilla  
Introdução  
Estas notas de lançamento para o Ubuntu 20.10 (Groovy Gorilla) fornecem uma visão geral do lançamento e documentam os problemas conhecidos com o Ubuntu e seus sabores.  
  
Vida útil do suporte  
Ubuntu 20.10 terá suporte por 9 meses até julho de 2021. Se você precisar de suporte de longo prazo, é recomendável usar Ubuntu 20.04 LTS 290 em vez de.  
  
Novos recursos em 20.10  
Pacotes atualizados  
Kernel Linux :pinguim:  
Ubuntu 20.10 inclui o kernel Linux 5.8 . Isso inclui várias atualizações e suporte adicionado desde o kernel Linux 5.4 lançado no Ubuntu 20.04 LTS. Alguns exemplos notáveis ​​incluem:  
  
Limites da fila de tempo de antena para melhor qualidade de conexão WiFi  
Btrfs RAID1 com 3 e 4 cópias e mais alternativas de checksum  
Suporte a USB 4 (protocolo Thunderbolt 3) adicionado  
X86 Ativar suporte de paginação de 5 níveis por padrão  
Suporte gráfico Intel Gen11 (Ice Lake) e Gen12 (Tiger Lake)  
Suporte inicial para AMD Family 19h (Zen 3)  
Rastreamento de pressão térmica para sistemas para melhor colocação de tarefas no núcleo da CPU  
Reparação online XFS  
Pareamento OverlayFS com VirtIO-FS  
Fila de notificação geral para notificação de chave / chaveiro, alterações de montagem, etc.  
Active State Power Management (ASPM) para maior economia de energia de dispositivos PCIe-para-PCI  
Suporte inicial para POWER10  
Atualizações do conjunto de ferramentas : hammer_and_wrench:  
Ubuntu 20.10 vem com conjunto de ferramentas de última geração, incluindo novas versões upstream de glibc 2.32, :café:OpenJDK 11, rustc 1.41, GCC 10, LLVM 11, :serpente:Python 3.8.6, :gema:ruby 2.7.0, php 7.4.9, : dromedary_camel:perl 5.30 , golang 1,13.  
  
Melhorias de segurança : lock:  
nftables é agora o back-end padrão do firewall.  
  
Ubuntu Desktop  
Ubuntu 20.10 é o primeiro lançamento do Ubuntu a apresentar imagens de desktop para o Raspberry Pi 4 182.  
  
GNOMO : pegadas:  
Ubuntu 20.10 inclui a versão mais recente do GNOME, versão 3.38, com uma visão geral das atividades aprimorada, melhorias na experiência do usuário, melhor desempenho e muito mais.  
  
Aplicativos atualizados  
Firefox :fogo:: fox_face:versão 81  
LibreOffice : livros:versão 7.0.2  
Thunderbird : cloud_with_lightning::pássaro:versão 78.3.2  
Subsistemas atualizados  
BlueZ 5.55  
NetworkManager 1.26.2  
Ubuntu Server  
Mudanças dignas de nota  
squid: o auxiliar de autenticação básica NIS foi removido ( LP: # 1895694 14)  
adcli e realmd: muitas correções upstream foram aplicadas a esses pacotes, melhorando a compatibilidade com as alterações atuais do Active Directory  
samba 4.12 10 mudou para GnuTLS para a maioria de suas operações criptográficas e isso tem uma grande melhoria de desempenho na criptografia SMB3  
QEMU foi atualizado para a versão 5.0. Veja as mudanças anteriores 7 para uma visão geral das muitas melhorias.  
Um novo recurso digno de nota é o virtiofs 3que permite melhor compartilhamento de sistemas de arquivos host com o convidado em comparação com os antigos 9p fs 1 abordagem baseada.  
Libvirt foi atualizado para a versão 6.6. Veja os Changelogs upstream 7pelas muitas melhorias e correções desde a versão 6.0 que estavam no Focal .  
Libvirt 6.6 também suporta os novos virtiofs que foram mencionados na seção QEMU acima.  
O pacote de transição mail-stack-delivery de Dovecot foi preterido no focal e abandonado inteiramente no groovy. (LP: # 1771524 , # 1876564 )  
O próprio Dovecot é atualizado de 2.3.7 para 2.3.11 do focal. Isso adiciona suporte SSL / STARTTLS para conexões doveadm com proxy, lote de transações IMAP, relatórios de eventos aprimorados e várias outras correções. O suporte ao socketmap Postfix foi eliminado. Veja https://dovecot.org/doc/NEWS 5 para obter a lista completa de alterações.  
liburing 3suporte foi adicionado. Este é um novo mecanismo de E / S assíncrona no kernel do Linux. Por enquanto, temos qemu e samba usando este suporte.  
O Samba adicionou suporte de uring na versão 4.12.0 na forma de um módulo VFS. Faz parte do pacote samba-vfs-modules.  
Qemu adicionou suporte para uring na versão 5.0 2, ele pode ser usado com o driver file-posix como aio = io_uring.  
Groovy apresenta o telégrafo 16 pacote 3, parte de uma pilha de registro, monitoramento e alerta (LMA) bem conhecida. Junto com prometheus 2, prometheus alert-manager 2e grafana 1, este trio forma a base de uma solução de monitoramento e alerta forte e confiável que pode ser implantada em sistemas Ubuntu.  
Grafana: painel de métricas rico em recursos e editor de gráficos, disponível como um piscar de olhos em https://snapcraft.io/grafana 4  
Prometheus e gerenciador de alertas: sistema de monitoramento e banco de dados de séries temporais, disponíveis em um piscar de olhos em https://snapcraft.io/prometheus 1 e como um pacote deb em Groovy  
Telegraf: agente de coleta e envio de métricas e eventos de bancos de dados, sistemas e sensores IoT. Disponível como um pacote deb em Groovy.  
Pilha aberta  
Ubuntu 20.10 inclui a versão mais recente do OpenStack, Victoria, incluindo os  
seguintes componentes:  
  
• Identidade OpenStack - Keystone  
  
• OpenStack Imaging - Glance  
  
• Armazenamento em bloco OpenStack - Cinder  
  
• OpenStack Compute - Nova  
  
• Rede OpenStack - Neutron  
  
• Telemetria OpenStack - Ceilômetro, Aodh, Gnocchi e Panko  
  
• Orquestração OpenStack - Calor  
  
• Painel OpenStack - Horizon  
  
• Armazenamento de objeto OpenStack - Swift  
  
• OpenStack DNS - Designado  
  
• OpenStack Bare-metal - Irônico  
  
• Sistema de arquivos OpenStack - Manila  
  
• Gerenciador de chaves OpenStack - Barbican  
  
• Balanceador de carga OpenStack - Octavia  
  
• Instância OpenStack HA - Masakari  
  
Consulte as notas de lançamento do OpenStack Victoria 10para obter todos os detalhes desta  
versão do OpenStack.  
  
OpenStack Victoria também é fornecido por meio do Ubuntu Cloud Archive 1para OpenStack  
Victoria para usuários do Ubuntu 20.04 LTS.  
  
AVISO: Atualizar uma implementação do OpenStack é um processo não trivial e  
deve-se tomar cuidado para planejar e testar os procedimentos de atualização que serão específicos para  
cada implementação do OpenStack.  
  
Certifique-se de ler o OpenStack Charm Release Notes para obter mais informações sobre  
como implantar o Ubuntu OpenStack usando Juju.  
  
Plataformas  
Imagens de nuvem :nuvem:  
Para melhorar o tempo de inicialização, as imagens com kernels KVM e específicos da nuvem inicializam sem um initramfs por padrão. As imagens em nuvem com o kernel genérico continuarão a inicializar com um initramfs por padrão.  
Uma melhoria adicional no tempo de inicialização vem com otimizações de pré-propagação instantânea. Essas mudanças irão melhorar muito a velocidade da primeira inicialização nas nuvens. Os usuários podem encontrar informações adicionais de tempo de snap debug seedinge verificando os seed-completioncomandos para ver quanto tempo demorou a propagação instantânea na primeira inicialização. Agradecemos o feedback dos usuários.  
Raspberry Pi :morango:  
Nova imagem da área de trabalho! Observe que isso só foi criado para a arquitetura arm64 e é compatível apenas com modelos Pi4 com pelo menos 4 Gb de RAM. A imagem ainda pode inicializar em modelos menores ou anteriores, mas essas plataformas não são compatíveis.  
Suporte ao Módulo 4 de computação. As imagens do servidor e da área de trabalho são totalmente suportadas na nova plataforma CM4. No entanto, para a imagem da área de trabalho, observe que apenas modelos com 4 Gb de RAM ou mais são suportados e, além disso, o tamanho da imagem excede 8 Gb e, portanto, o eMMC de 16 Gb é o menor modelo suportado (ou modelos Lite com armazenamento de cartão SD equivalente).  
Com a remoção do U-Boot do processo de inicialização padrão, USB e inicialização de rede agora estão ativados em todos os modelos Pi através do mesmo procedimento do Raspbian 11. O U-Boot permanecerá como uma opção neste ciclo (ainda está instalado na partição de inicialização e ainda pode ser selecionado com config.txtopções), mas é considerado obsoleto.  
Os atualizadores do Ubuntu 20.04 LTS não serão removidos implicitamente do U-Boot. No entanto, você pode alternar para uma sequência sem U-Boot de forma bastante simples. Os modos de inicialização Groovy 13 post tem detalhes sobre como mover entre as duas opções.  
s390x  
Aprimoramentos específicos do IBM Z e LinuxONE / s390x desde 20.04 (parcialmente não limitado ao s390x):  
  
Log FCP link Capacidade EDIF introduzida ( LP: # 1830732 e LP: # 1884773 ) e erros FCP relacionados a EDIF (FSF_SECURITY_ERRORS) adicionados ( LP: # 1830733 ).  
  
SCSI IPL normal ( LP: # 1884737 1) e IPL para suporte a dispositivo NVMe adicionado ( LP: # 1886792 ), incl. suporte do instalador ( LP: # 1884769 ).  
  
Pilha de criptografia atualizada: libica 3.7.0 ( LP: # 1878650 ), suporte a openssl RNG ( LP: # 1799928 ), openssl-ibmca 2.1.1 ( LP: # 1884763 ) openCryptoki 3.14 incl. Dilithium assinatura em tokens openCryptoki EP11 ( LP: # 1886777 ), melhorias na ferramenta de gerenciamento de chaves ( LP: # 1884751 e LP: # 1884755 ), assim como melhorias na ferramenta de conversão de PIN ( LP: # 1854944 e LP: # 1893216 )  
  
Aprimoramentos do suporte à compressão assistida por hardware, especialmente DEFLATE ( LP: # 1884514 ) e exploração de NXU.  
  
Outras atualizações de pacotes relacionados ao s390x: s390-tools 2.14 ( LP: # 1884721 ), smc-tools 1.3.0 ( LP: # 1884508 ), libdfp 1.0.15 ( LP: # 1887900 ), perftest 4.0-29 ( LP: # 1888377 ), agente de cerca de marcapasso para LPARs ( LP: # 1889070 ) e OpenBlas 0.3.10 com otimizações ( LP: # 1884519 e LP: # 1893653 ).  
  
Atualizações da pilha de virtualização KVM e modificações específicas do s390x: amostragem e registro kvm_stat ( LP: # 1884784 ), IPL CCW transparente de DASD ( LP: # 1887935 e LP: # 1887936 ), tratamento de caminho de canal transparente para vfio-ccw ( LP: # 1887930 e LP: # 1887931 ).  
  
Aprimoramentos adicionais específicos do s390x: aprimoramentos de vetor em gcc ( LP: # 1888653 ) e em binutils ( LP: # 1889742 e LP: # 1888654 ), alinhamento de topologia de CPU ( LP: # 1884782 1), Aprimoramentos de desempenho OSA Express no driver qeth ( LP: # 1853294 ) e failover SMC-R ( LP: # 1853151 ), bem como suporte de tolerância SMC-D v2 ( LP: # 1887942 1)  
  
Problemas Conhecidos  
Como era de se esperar, com qualquer lançamento, existem alguns bugs conhecidos significativos que os usuários podem encontrar com este lançamento do Ubuntu. Os que conhecemos neste momento (e algumas das soluções alternativas), estão documentados aqui para que você não precise perder tempo relatando esses bugs novamente:  
  
Geral  
LP: # 1899615 15 - Não é mais possível realizar um teste de memória da RAM do sistema a partir da imagem ISO quando inicializado via EFI - o BIOS está OK.  
LP: # 1891952 1 - Depois de escolher “Habilitar rede” na opção de menu de recuperação do Ubuntu grub, a resolução de nome de domínio não funcionará, iniciar o systemd resolvido corrige o problema.  
LP: # 1899632 3 - Não é mais possível usar “Easy Install” com VMWare Player.  
Kernel Linux  
Os drivers gráficos NVIDIA 455 mais recentes não foram incluídos no lançamento inicial do groovy. Eles estarão disponíveis como uma atualização de versão estável (SRU) logo após o lançamento. Os drivers NVIDIA 455 são necessários para suporte da GeForce RTX 3080, RTX 3090 e MX450.  
Ubuntu Desktop  
LP: # 1900722 34 - Reinstalar o Ubuntu falha.  
LP: # 1897224 24 - Snap gráficos quebrados nas sessões do GNOME Wayland  
LP: # 1901043 2 - Nenhum som no Try / Install Ubuntu (ubiquity-dm) quando o “Modo de gráficos seguros” é selecionado (nomodeset)  
Ubuntu Server  
Nada ainda.  
  
Plataformas  
Imagens de nuvem : cloud_with_lightning_and_rain:  
No Google Compute Engine (GCE), o pacote google-guest-agent introduziu uma regressão (LP: # 1901033) para o serviço google-startup-script. Usuários fazendo uso de scripts de inicialização 1no GCE pode ver os scripts executados antes da propagação do cloud-init e snapd serem concluídos até que a regressão seja resolvida. Sem esperar por cloud-final e snapd.seeded, os scripts de inicialização podem não ser apresentados com um sistema consistente que tenha espelhos de arquivo configurados, snap google-cloud-sdk do GCE instalado, usuários nos grupos adequados ou outras personalizações pertencentes a esses serviços . Como uma cloud-init status --waitsolução alternativa, os usuários podem adicionar ao início de seu script de inicialização (como o cloud-init espera que a propagação instantânea seja concluída).  
Raspberry Pi  
LP: # 1899962 3- Na imagem da área de trabalho, o dispositivo de saída de áudio incorreto é selecionado em cada inicialização. Uma solução alternativa está disponível no relatório de bug.  
  
LP: # 1899953 3- A saída de áudio está “estalada”. Uma solução alternativa (tsched = 0) é detalhada no relatório de bug.  
  
LP: # 1900904 - Portas ethernet auxiliares (por exemplo, conexão USB) não serão configuradas automaticamente. Uma solução alternativa está presente no relatório de bug.  
  
No Pi4, recomendamos que você instale o pacote rpi-eeprom com sudo apt install rpi-eeprompara manter sua EEPROM de inicialização atualizada. Isso também é necessário se você deseja experimentar USB ou inicialização via rede nesta plataforma. Isso deve ser incluído na imagem em versões futuras.  
  
Na placa IO da Pi Foundation para o Módulo de computação 4, as portas USB são roteadas para o controlador DWC2 USB2 (que é conectado à porta USB-C no Pi 4). Isso não está no modo host por padrão, o que significa que os teclados (e outros dispositivos) não funcionarão. Adicione a seguinte linha ao config.txtpara habilitar as portas USB na placa IO:  
  
dtoverlay=dwc2,dr_mode=host  
Uma instância comentada desta linha pode ser encontrada config.txtpor padrão.  
  
ppc64el  
LP: # 1878041 - No caso de sistemas multipath com grandes quantidades de caminhos, o instalador pode atingir o tempo limite.  
s390X  
LP: # 1900900 - Se estiver fazendo uma instalação no armazenamento em disco de vários caminhos zFCP / SCSI usado anteriormente, o instalador pode falhar ao remover uma configuração anterior. A solução alternativa é limpar a configuração manualmente em um shell do instalador. A correção será incluída em futuras atualizações do instalador.  
  
Mais Informações  
Reportando bugs  
Seus comentários, relatórios de bugs, patches e sugestões ajudarão a corrigir bugs e melhorar a qualidade de lançamentos futuros. Por favor Reportar Erros usando as ferramentas fornecidas 33. Se você quiser ajudar com bugs, o Bug Squad 19 está sempre procurando por ajuda.  
  
Participe do Ubuntu  
Se você gostaria de ajudar a moldar o Ubuntu, dê uma olhada na lista de maneiras pelas quais você pode participar em:  
  
https://community.ubuntu.com/contribute 78  
  
`  

```  

### Download

  
Seguem os links para download das imagens de instalação _(amd64)_ do Ubuntu e de alguns dos seus _"flavours" ou "sabores"_ oficiais. Todas as imagens são da versão Desktop e podem ser utilizadas sem necessidade de instalação. Há também a opção de download em Torrent. Escolha o "sabor" de sua preferência e faça o download.  
  

Ubuntu 20.10

[ Live](https://releases.ubuntu.com/20.10/ubuntu-20.10-desktop-amd64.iso)

[ Torrent](https://releases.ubuntu.com/20.10/ubuntu-20.10-desktop-amd64.iso.torrent)

[Mais...](https://ubuntu.com/download)

  

#### Flavours:

  
[ Kubuntu 20.10](https://kubuntu.org/getkubuntu/)  
[ Xubuntu 20.10](https://xubuntu.org/download)  
[ Ubuntu Mate 20.10](https://ubuntu-mate.org/download/)  
[ Lubuntu 20.10](https://lubuntu.me/downloads/)  
[ Ubuntu Kylin 20.10](https://www.ubuntukylin.com/downloads/show.php?id=451&lang=en)  
[ Ubuntu Studio 20.10](https://ubuntustudio.org/download/)  
[ Ubuntu Budgie 20.10](https://ubuntubudgie.org/downloads/)  
  

### Instalação ou atualização

  

#### Atualizar a partir do Ubuntu 20.04

  
Se você está utilizando atualmente o Ubuntu 20.04 _(Focal Fossa)_ você pode atualizar é possível atualizar para o Groovy Gorilla. A atualização pode ser feita pelo modo gráfico, mas aqui vou mostrar como fazê-la pelo terminal. Siga os passos abaixo:  
  

*   Primeiramente tenha certeza que o a versão atual está com as últimas atualizações. No terminal, execute os comandos:

  

  

 sudo apt update

  
  

  

 sudo apt upgrade

  

*   Após atualizar, execute:

  

  

 sudo do-release-upgrade -d

  
O comando anterior vai:  

*   Verificar se há uma nova versão em desenvolvimento
*   Desativar os repositórios de terceiros (PPAs)
*   Alterar os repositórios de focal para groovy
*   Haverá uma solicitação para confirmar a atualização

1.  Se confirmar a atualização será iniciada. O processo pode ser bem demorado. Preste atenção às solicitações de confirmação de ações, confirme-as e aguarde a finalização. Após finalizado reinicie o sistema e você terá o Ubuntu Groovy Gorilla instalado.
2.  Se não confirmar pode ser que seja preciso alterar os repositórios manualmente de **groovy para focal**.  
    Neste caso, utilize o editor de texto que preferir _(joe gedit, kate, nano, vi, pluma...)_, e abra o arquivo sources.list com o comando abaixo:

  

 sudo _joe_ /etc/apt/sources.list

  

*   No arquivo aberto, faça as alterações solicitadas e salve o arquivo.

  

#### Executando a imagem _ISO_ num pendrive e instalando do zero

  
Primeiramente é necessário gravar num pendrive a imagem .iso baixada anteriormente. Para gravar a ISO no pendrive veja como gravar um pendrive em sistemas [Linux](https://info.wsouza.com.br/2020/04/3-maneiras-de-gravar-uma-imagem-iso-num-pendrive-utilizando-linux.html) e no [Windows](https://info.wsouza.com.br/2015/01/criar-um-pendrive-multiboot-linux.html).  
O vídeo abaixo mostra a execução do Groovy Gorilla num pendrive e posterior instalação do zero (limpa).