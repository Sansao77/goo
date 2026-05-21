# Curso 4

## Ferramentas de trabalho: Linux e SQL

### Modulo 1:

#### Compare os sistemas operacionais

##### Sistemas operacionais comuns

É útil conhecer os seguintes sistemas operacionais no setor de segurança: Windows, macOS®, Linux, ChromeOS, Android e iOS.

###### Windows e macOS

O Windows e o macOS são sistemas operacionais comuns. O sistema operacional Windows foi lançado em 1985, e o macOS foi lançado em 1984. Ambos os sistemas operacionais são usados em computadores pessoais e corporativos.

O Windows é um software operacional de código fechado, o que significa que o código fonte não é compartilhado livremente com o público. O macOS é parcialmente de código aberto. Ele tem alguns componentes de código aberto, como o kernel do macOS. O macOS também tem alguns componentes de software proprietário.

###### Linux

A primeira versão do Linux foi lançada em 1991, e outras versões importantes foram lançadas no início da década de 1990. O Linux é um sistema operacional totalmente de código aberto, o que significa que qualquer pessoa pode acessar o Linux e seu código-fonte. A natureza de código aberto do Linux permite que os desenvolvedores da comunidade Linux colaborem entre si.

O Linux é particularmente importante para o setor de segurança. Há algumas distribuições que foram projetadas especificamente para a segurança. Mais adiante neste curso, você aprenderá sobre o Linux e sua importância para o setor de segurança.

###### ChromeOS

O ChromeOS foi lançado em 2011. Ele é parcialmente de código aberto e é derivado do Chromium OS, que é totalmente de código aberto. O ChromeOS é frequentemente usado no Campo da educação.

###### Android e iOS

O Android e o iOS são sistemas operacionais móveis. Diferentemente dos outros sistemas operacionais mencionados, os sistemas operacionais móveis são normalmente usados em dispositivos móveis, como telefones, tablets e relógios. O Android foi introduzido para uso público em 2008, e o iOS foi introduzido em 2007. O Android é de código aberto, e o iOS é parcialmente de código aberto.

##### Sistemas operacionais e vulnerabilidades

Problemas de segurança são inevitáveis em todos os sistemas operacionais. Uma parte importante da proteção de um sistema operacional é manter o sistema e todos os seus componentes atualizados.

###### Sistemas operacionais legados

Um sistema operacional legado é um sistema operacional desatualizado, mas que ainda está sendo usado. Algumas organizações continuam a usar sistemas operacionais legados porque o software do qual dependem não é compatível com os sistemas operacionais mais recentes. Isso pode ser mais comum em setores que usam muitos equipamentos que requerem software incorporado - software que é colocado dentro de componentes do equipamento.

Os sistemas operacionais legados podem ser vulneráveis a problemas de segurança porque não são mais suportados ou atualizados. Isso significa que os sistemas operacionais legados podem ser vulneráveis a novas ameaças.
Outras vulnerabilidades

Mesmo quando os sistemas operacionais são mantidos atualizados, eles ainda podem se tornar vulneráveis a ataques. Abaixo estão vários recursos que incluem informações sobre sistemas operacionais e suas vulnerabilidades.

- [Centro de Resposta de Segurança da Microsoft (MSRC)](https://msrc.microsoft.com/update-guide/vulnerability): Lista de vulnerabilidades conhecidas que afetam os produtos e serviços da Microsoft
- [Atualizações de segurança da Apple](https://support.apple.com/en-us/100100): Lista de atualizações de segurança e informações sobre os sistemas operacionais da Apple®, incluindo macOS e iOS, e outros produtos
- [Relatório de Vulnerabilidades e Exposições Comuns (CVE) para Ubuntu](https://ubuntu.com/security/cves): Uma lista de vulnerabilidades conhecidas que afetam o Ubuntu, que é uma distribuição específica do Linux
- [Boletim de Segurança na Nuvem do Google](https://cloud.google.com/support/bulletins): Uma lista de vulnerabilidades conhecidas que afetam os produtos e serviços do Google Nuvem

Manter um sistema operacional atualizado é uma maneira chave de ajudar o sistema a permanecer seguro. Como pode ser difícil manter todos os sistemas atualizados o tempo todo, é importante que os analistas de segurança conheçam os sistemas operacionais legados e os riscos que eles podem criar.

#### Solicitações ao sistema operacional

##### Inicializando o computador

Quando você inicializa ou liga o computador, um microchip BIOS ou UEFI é ativado. O **Basic Input/Output System (BIOS)** é um microchip que contém instruções de carga para o computador e é predominante em sistemas mais antigos. A **UEFI (Unified Extensible Firmware Interface)** é um microchip que contém instruções de carga para o computador e substitui o BIOS em sistemas mais modernos.

Os chips BIOS e UEFI executam a mesma função para inicializar o computador. O BIOS era o chip padrão até 2007, quando os chips UEFI começaram a ser mais usados. Atualmente, a maioria dos computadores novos inclui um chip UEFI. A UEFI oferece recursos de segurança aprimorados.

Os microchips BIOS ou UEFI contêm uma variedade de instruções de carga para o computador seguir. Por exemplo, uma das instruções de carga é verificar a integridade do hardware do computador.

A última instrução do BIOS ou da UEFI ativa o carregador de inicialização. O **carregador de inicialização** é um software que inicializa o sistema operacional. Após a inicialização do sistema operacional, o computador estará pronto para uso.

##### Integridade de uma tarefa

AS discutido anteriormente, os sistemas operacionais nos ajudam a usar os computadores com mais eficiência. Depois que o computador tiver passado pelo processo de inicialização, a conclusão de uma tarefa em um computador é um processo de quatro partes.

[Mostra um processo que passa do usuário para o aplicativo, para os sistemas operacionais e, finalmente, para o hardware.](./public/img/CS_R-060_User-Application-Operating-System-Hardware.png)

###### Usuário

A primeira parte do processamento é o usuário. O usuário inicia o processamento quando tem algo que deseja realizar no computador. Neste momento, você é um usuário! Você iniciou o processo de acesso a esta leitura.

###### Aplicativo

O aplicativo é o software com o qual os usuários interagem para concluir uma tarefa. Por exemplo, se quiser calcular algo, você usaria o aplicativo da calculadora. Se quiser escrever um relatório, usará um aplicativo de processamento de texto. Essa é a segunda parte do processamento.

###### Sistema operacional

O sistema operacional recebe a solicitação do usuário do aplicativo. O trabalho do sistema operacional é interpretar a solicitação e direcionar seu Fluxo. Para concluir a tarefa, o sistema operacional a envia para os componentes aplicáveis do hardware.

###### Hardware

O hardware é onde todo o processamento é feito para concluir as tarefas iniciadas pelo usuário. Por exemplo, quando um usuário deseja calcular um número, a CPU calcula a resposta. Como outro exemplo, quando um usuário deseja salvar um arquivo, outro componente do hardware, o disco rígido, processa essa tarefa.

Depois que o hardware faz o trabalho, ele envia a saída de volta ao aplicativo por meio do sistema operacional para que ele possa exibir os resultados para o usuário.

##### O sistema operacional em ação nos bastidores

Considere mais uma vez como um computador é semelhante a um carro. Há processos que não podem ser observados diretamente ao operar um carro, mas eles o sentem avançar quando pressionam o pedal do acelerador. O mesmo acontece com um computador. Dentro de um computador, ocorre um trabalho importante que não é observado diretamente. Esse trabalho envolve o sistema operacional.

Você pode explorar isso por meio de outra analogia. O processamento do uso de um sistema operacional também é semelhante a fazer um pedido em um restaurante. Em um restaurante, você faz um pedido e recebe a comida, mas não vê o que está acontecendo na cozinha quando os cozinheiros preparam a comida.

Pedir comida é semelhante a usar um aplicativo em um computador. Ao fazer o pedido, você faz uma solicitação específica, como "uma sopa pequena, bem quente" Ao usar um aplicativo, você também faz solicitações específicas, como "imprimir três cópias frente e verso deste documento".

Você pode comparar a comida que recebe com o que acontece quando o hardware envia a saída. Você recebe a comida que pediu. Você recebe o documento que deseja imprimir.

Por fim, a cozinha é como o sistema operacional. Você não sabe o que acontece na cozinha, mas ela é fundamental para interpretar a solicitação e garantir que você receba o que pediu. Da mesma forma, embora o trabalho do sistema operacional não seja diretamente transparente para você, ele é essencial para a conclusão de suas tarefas.

##### Um exemplo: Download de um arquivo de um navegador da Internet

Anteriormente, você explorou como os sistemas operacionais, os aplicativos e o hardware trabalham juntos, examinando uma tarefa que envolve um cálculo. Você pode expandir essa compreensão explorando como o sistema operacional conclui outra tarefa, o download de um arquivo de um navegador da Internet:

- Primeiro, o usuário decide que deseja fazer o download de um arquivo que encontrou on-line, então ele clica em um botão de download próximo ao arquivo no aplicativo do navegador da Internet.
- Em seguida, o navegador da Internet comunica essa ação ao sistema operacional.
- O sistema operacional envia a solicitação de download do arquivo para o hardware apropriado para processamento.
- O hardware começa a fazer o download do arquivo e o sistema operacional envia essas informações para o aplicativo do navegador da Internet. Em seguida, o navegador da Internet informa ao usuário quando o arquivo foi baixado.

#### Tecnologia de virtualização

##### O que é uma máquina virtual?

Uma **máquina virtual (VM)** é uma versão virtual de um computador físico. As máquinas virtuais são um exemplo de virtualização. A virtualização é o processamento do uso de software para criar representações virtuais de várias máquinas físicas. O termo "virtual" refere-se a máquinas que não existem fisicamente, mas que operam como se existissem porque seu software simula o hardware físico. Os sistemas virtuais não usam hardware físico dedicado. Em vez disso, eles usam versões definidas por software do hardware físico. Isso significa que uma única máquina virtual tem uma CPU virtual, um armazenamento virtual e outro hardware virtual. Os sistemas virtuais são apenas códigos.

[Um computador cinza escuro com setas para computadores cinza claro que têm "VM" na tela e são cercados por linhas pontilhadas.](./public/img/VMs_image.jpeg)

É possível executar várias máquinas virtuais usando o hardware físico de um único computador. Isso envolve a divisão dos recursos do computador host para serem compartilhados entre todos os componentes físicos e virtuais. Por exemplo, a **RAM (Random Access Memory, memória de acesso aleatório)** é um componente de hardware usado para memória de curto prazo. Se um computador tiver 16 GB de RAM, ele poderá hospedar três máquinas virtuais, de modo que o computador físico e as máquinas virtuais tenham 4 GB de RAM cada. Além disso, cada uma dessas máquinas virtuais teria seu próprio sistema operacional e funcionaria de forma semelhante a um computador comum.

##### Benefícios das máquinas virtuais

Os profissionais de segurança geralmente usam a virtualização e as máquinas virtuais. A virtualização pode aumentar a segurança de muitas tarefas e também pode aumentar a eficiência.

###### Segurança

Um dos benefícios é que a virtualização pode fornecer um ambiente isolado, ou um Sandbox, na máquina hospedeira física. Quando um computador tem várias máquinas virtuais, essas máquinas virtuais são "convidadas" do computador. Especificamente, elas são isoladas do computador host e de outras máquinas virtuais convidadas. Isso proporciona uma camada de segurança, pois as máquinas virtuais podem ser mantidas separadas dos outros sistemas. Por exemplo, se uma máquina virtual individual for infectada por malware, ela poderá ser tratada com mais segurança porque está isolada das outras máquinas. Um profissional de segurança também pode colocar intencionalmente um malware em uma máquina virtual para examiná-lo em um ambiente mais seguro.

Observação: embora o uso de máquinas virtuais seja útil na investigação de máquinas potencialmente infectadas ou na execução de malware em um ambiente restrito, ainda há alguns riscos. Por exemplo, um programa mal-intencionado pode escapar da virtualização e acessar a máquina host. É por isso que você nunca deve confiar totalmente nos sistemas de virtualização.

###### Eficiência

O uso de máquinas virtuais também pode ser uma maneira eficiente e conveniente de realizar tarefas de segurança. Você pode abrir várias máquinas virtuais de uma só vez e alternar facilmente entre elas. Isso lhe permite simplificar as tarefas de segurança, como testar e explorar vários aplicativos.

É possível comparar a eficiência de uma máquina virtual com a de um ônibus urbano. Um único ônibus urbano tem muito espaço e é uma forma eficiente de transportar muitas pessoas simultaneamente. Se os ônibus urbanos não existissem, todos no ônibus teriam que dirigir seus próprios carros. Isso usa mais gasolina, carros e outros recursos do que andar de ônibus urbano.

Da mesma forma que muitas pessoas podem andar em um único ônibus, muitas máquinas virtuais podem ser hospedadas na mesma máquina física. Dessa forma, não são necessárias máquinas físicas separadas para executar determinadas tarefas.

##### Gerenciamento de máquinas virtuais

As máquinas virtuais podem ser gerenciadas com um software chamado **hipervisor**. Os hipervisores ajudam os usuários a gerenciar várias máquinas virtuais e a conectar o hardware virtual e o físico. Os hipervisores também ajudam a alocar os recursos compartilhados da máquina hospedeira física para uma ou mais máquinas virtuais.

Um hipervisor que é útil para você conhecer é a **máquina virtual baseada em kernel (KVM)**. O KVM é um hipervisor de código aberto compatível com a maioria das principais distribuições do Linux. Ele é incorporado ao kernel do Linux, o que significa que pode ser usado para criar máquinas virtuais em qualquer máquina que esteja executando um sistema operacional Linux sem a necessidade de software adicional.

##### Outras formas de virtualização

Além das máquinas virtuais, há outras formas de virtualização. Algumas dessas tecnologias de virtualização não usam sistemas operacionais. Por exemplo, vários servidores virtuais podem ser criados a partir de um único servidor físico. Também é possível criar redes virtuais para usar com mais eficiência o hardware de uma rede física.

#### A linha de comando em uso

##### CLI vs. GUI

Uma interface gráfica de usuário (GUI) é uma interface de usuário que usa ícones na tela para gerenciar diferentes tarefas no computador. Uma interface de linha de comando (CLI) é uma interface de usuário baseada em texto que usa comandos para interagir com o computador. 

###### Exibição

Uma diferença notável entre essas duas interfaces é como elas aparecem na tela. Uma GUI tem gráficos e ícones, como os ícones da área de trabalho ou da barra de tarefas para iniciar programas. Em contrapartida, uma CLI tem apenas texto. Seu aspecto é semelhante ao de linhas de código. 

[Comparação lado a lado de uma interface gráfica de usuário com ícones e uma interface de linha de comando com código.](./public/img/GUI_CLI.png)

###### Função

Essas duas interfaces também diferem em sua Função. Uma GUI é uma interface que só permite fazer uma solicitação de cada vez. No entanto, uma CLI permite que você faça várias solicitações ao mesmo tempo.


##### Vantagens de uma CLI na segurança cibernética  

A escolha entre usar uma GUI ou uma CLI é parcialmente baseada na preferência pessoal, mas os analistas de segurança devem poder usar ambas as interfaces. O uso de uma CLI pode oferecer algumas vantagens.

###### Eficiência

Alguns preferem a CLI porque ela pode ser usada mais rapidamente quando se sabe como gerenciar essa interface. Para um novo usuário, uma GUI pode ser mais eficiente porque é mais fácil para os iniciantes navegarem. 

Como a CLI pode aceitar várias solicitações ao mesmo tempo, ela é mais poderosa quando você precisa executar várias tarefas com eficiência. Por exemplo, se tivesse que criar vários arquivos novos em seu sistema, poderia realizar essa tarefa rapidamente em uma CLI. Se estivesse usando uma GUI, isso poderia levar muito mais tempo, pois seria necessário repetir as mesmas etapas para cada novo arquivo.

###### Arquivo Histórico

Para os analistas de segurança, usar a CLI do Linux é útil porque ela registra um arquivo de histórico de todos os comandos e ações na CLI. Se estiver usando uma GUI, suas ações não serão necessariamente salvas em um arquivo de histórico.

Por exemplo, você pode estar em uma situação em que está respondendo a um incidente usando um manual. As instruções do playbook exigem que você execute uma série de comandos diferentes. Se você usasse uma CLI, poderia voltar ao histórico e garantir que todos os comandos fossem usados corretamente. Isso poderia ser útil se houvesse problemas ao usar o playbook e você tivesse que revisar as etapas executadas na linha de comando.

Além disso, se suspeitar que um atacante comprometeu seu sistema, você poderá rastrear as ações dele usando o arquivo de histórico.

### Modulo 3: 

#### Explicação da arquitetura do Linux

##### Usuário

O **usuário** é a pessoa que interage com um computador. Ele inicia e gerencia as tarefas do computador. O Linux é um sistema multiusuário, o que significa que vários usuários podem usar os mesmos recursos ao mesmo tempo.

##### Aplicativos

Um **aplicativo** é um programa que executa uma tarefa específica. Há muitos aplicativos diferentes em seu computador. Alguns aplicativos normalmente vêm pré-instalados em seu computador, como calculadoras ou calendários. Outros aplicativos podem ter de ser instalados, como alguns navegadores da Web ou clientes de e-mail. No Linux, você geralmente usa um **gerenciador de pacotes** para instalar aplicativos. Um gerenciador de pacotes é uma ferramenta que ajuda os usuários a instalar, gerenciar e remover pacotes ou aplicativos. Um pacote é um software que pode ser combinado com outros pacotes para formar um aplicativo.

##### Shell

O **shell** é o interpretador de linha de comando. Tudo o que é inserido no shell é baseado em texto. O shell permite que os usuários deem comandos ao kernel e recebam respostas dele. Você pode pensar no shell como um tradutor entre você e o computador. O shell traduz os comandos que você digita para que o computador possa executar as tarefas que você deseja.

##### Padrão de hierarquia do sistema de arquivos (FHS)

O **FHS (Filesystem Hierarchy Standard, padrão de hierarquia do sistema de arquivos)** é o componente do sistema operacional Linux que organiza os dados. Ele especifica o local onde os dados são armazenados no sistema operacional.

Um diretório é um arquivo que organiza onde outros arquivos são armazenados. Às vezes, os diretórios são chamados de "pastas" e podem conter arquivos ou outros diretórios. O FHS define como os diretórios, o conteúdo dos diretórios e outros armazenamentos são organizados para que o sistema operacional saiba onde encontrar dados específicos.

##### Kernel

O **kernel** é o componente do sistema operacional Linux que gerencia os processos e a memória. Ele se comunica com os aplicativos para encaminhar comandos. O kernel do Linux é exclusivo do sistema operacional Linux e é essencial para a alocação de recursos no sistema. O kernel controla todas as principais funções do hardware, o que pode ajudar a agilizar as tarefas com mais eficiência.

##### Hardware

O **hardware** são os componentes físicos de um computador. Talvez você esteja familiarizado com alguns componentes de hardware, como discos rígidos ou CPUs. O hardware é classificado como periférico ou interno.

###### Dispositivos periféricos

Os **dispositivos periféricos** são componentes de hardware que são conectados e controlados pelo sistema do computador. Eles não são componentes principais necessários para executar o sistema do computador. Os dispositivos periféricos podem ser adicionados ou removidos livremente. Exemplos de dispositivos periféricos incluem monitores, impressoras, o teclado e o mouse.

###### Hardware interno

O **hardware interno** é o componente necessário para o funcionamento do computador. O hardware interno inclui uma placa de circuito principal e todos os componentes conectados a ela. Essa placa de circuito principal também é chamada de placa-mãe. O hardware interno inclui o seguinte:

- A CPU (Central Processing Unit, unidade central de processamento) é o processador principal de um computador, usado para executar tarefas gerais de computação em um computador. A CPU executa as instruções fornecidas pelos programas, o que permite que esses programas sejam executados.
- A RAM (Random Access Memory, memória de acesso aleatório ) é um componente de hardware usado para memória de curto prazo. É nela que os dados são armazenados temporariamente enquanto você executa tarefas no computador. Por exemplo, se estiver escrevendo um relatório no computador, os dados necessários para isso serão armazenados na RAM. Depois de terminar de escrever o relatório e fechar o programa, esses dados são excluídos da RAM. As informações na RAM não podem ser acessadas depois que o computador é desligado. A CPU utiliza os dados da RAM para executar programas.
- O disco rígido é um componente de hardware usado para memória de longo prazo. É onde os programas e arquivos são armazenados para que o computador possa acessá-los posteriormente. As informações no disco rígido podem ser acessadas mesmo depois de o computador ter sido desligado e ligado novamente. Um computador pode ter vários discos rígidos.

#### Mais distribuições Linux

##### KALI LINUX ™

O KALI LINUX ™ é uma distribuição de código aberto do Linux que é amplamente usada no setor de segurança. Isso ocorre porque o KALI LINUX ™, que é baseado no Debian, é pré-instalado com muitas ferramentas úteis para testes de penetração e forense digital. Um teste de penetração é um ataque simulado que ajuda a identificar vulnerabilidades em sistemas, redes, sites, aplicativos e processos. A perícia digital é a prática de coletar e analisar dados para determinar o que aconteceu após um ataque. Essas são atividades importantes no setor de segurança.

No entanto, o KALI LINUX ™ não é a única distribuição Linux usada na segurança cibernética.

##### Ubuntu

O Ubuntu é uma distribuição de código aberto e fácil de usar que é amplamente utilizada no setor de segurança e em outros setores. Ele tem uma interface de Linha de Comando (CLI) e uma interface gráfica do usuário (GUI). O Ubuntu também é derivado do Debian e inclui aplicativos comuns por padrão. Os usuários também podem baixar muitos outros aplicativos de um gerenciador de pacotes, incluindo ferramentas voltadas para a segurança. Devido ao seu amplo uso, o Ubuntu tem um número especialmente grande de recursos da comunidade para dar suporte aos usuários.

O Ubuntu também é amplamente usado para computação em nuvem. À medida que as organizações migram para servidores em nuvem, o trabalho de segurança cibernética pode envolver mais regularmente derivados do Ubuntu.

##### Parrot

O Parrot é uma distribuição de código aberto que é comumente usada para segurança. Semelhante ao KALI LINUX ™, o Parrot vem com ferramentas pré-instaladas relacionadas a testes de penetração e forense digital. Como o KALI LINUX ™ e o Ubuntu, ele é baseado no Debian.

O Parrot também é considerado uma distribuição Linux fácil de usar. Isso se deve ao fato de ele ter uma GUI que muitos consideram fácil de navegar. Isso se soma ao CLI do Parrot.

##### Red Hat® Enterprise Linux®

O Red Hat Enterprise Linux é uma distribuição do Linux baseada em assinatura, criada para uso corporativo. O Red Hat não é gratuito, o que é uma grande diferença em relação às distribuições mencionadas anteriormente. Como foi criado e tem suporte para uso corporativo, a Red Hat também oferece uma equipe de suporte dedicada para que os clientes entrem em contato para resolver problemas.

##### AlmaLinux

O AlmaLinux é uma distribuição Linux voltada para a comunidade que foi criada como um substituto estável para o CentOS. O CentOS era uma distribuição de código aberto intimamente relacionada à Red Hat, e sua última versão estável, o CentOS 8, foi lançada em dezembro de 2021. O CentOS usou o código-fonte publicado pela Red Hat para fornecer uma plataforma semelhante. O AlmaLinux foi projetado para ser um substituto imediato do CentOS 8. Isso garante que os aplicativos e as configurações que funcionavam no CentOS continuarão a funcionar no AlmaLinux. 

#### Gerenciadores de pacotes para instalar aplicativos

##### Introdução aos gerenciadores de pacotes

Um pacote é um software que pode ser combinado com outros pacotes para formar um aplicativo. Alguns pacotes podem ser grandes o suficiente para formar aplicativos por conta própria.

Os pacotes contêm os arquivos necessários para que um aplicativo seja instalado. Esses arquivos incluem Dependências, que são arquivos suplementares usados para executar um aplicativo.

Os gerenciadores de pacotes podem ajudar a resolver problemas com Dependências e realizar outras tarefas de gerenciamento. Um gerenciador de pacotes é uma ferramenta que ajuda os usuários a instalar, gerenciar e remover pacotes ou aplicativos. O Linux usa vários gerenciadores de pacotes.

**Observação**: é importante usar a versão mais recente de um pacote sempre que possível. A versão mais recente tem as correções de erros e os patches de segurança mais atualizados. Isso ajuda a manter seu sistema mais seguro.

##### Tipos de gerenciadores de pacotes

Muitas distribuições Linux comumente usadas são derivadas da mesma distribuição principal. Por exemplo, o KALI LINUX ™, o Ubuntu e o Parrot são todos provenientes do Debian. O CentOS vem do Red Hat.

Esse conhecimento é útil ao instalar aplicativos porque determinados gerenciadores de pacotes funcionam com certas distribuições. Por exemplo, o Red Hat Package Manager (RPM) pode ser usado para distribuições Linux derivadas da Red Hat, e gerenciadores de pacotes como o dpkg podem ser usados para distribuições Linux derivadas do Debian.

Gerenciadores de pacotes diferentes normalmente usam extensões de arquivo diferentes. Por exemplo, o Gerenciador de Pacotes Red Hat (RPM) tem arquivos que usam a extensão de arquivo .rpm, como Package-Version-Release_Architecture.rpm. Os gerenciadores de pacotes para distribuições Linux derivadas do Debian, como o dpkg, têm arquivos que usam a extensão de arquivo .deb, como Package_Version-Release_Architecture.deb.

##### Ferramentas de gerenciamento de pacotes

Além dos gerenciadores de pacotes, como o RPM e o dpkg, há também ferramentas de gerenciamento de pacotes que permitem trabalhar facilmente com pacotes por meio do shell. Às vezes, as ferramentas de gerenciamento de pacotes são utilizadas em vez dos gerenciadores de pacotes porque permitem que os usuários executem tarefas básicas com mais facilidade, como a instalação de um novo pacote. Duas ferramentas notáveis são a Advanced Package Tool (APT) e o Yellowdog Updater Modified (YUM).

###### Ferramenta de Pacotes Avançados (APT)

O APT é uma ferramenta usada com distribuições derivadas do Debian. Ele é executado a partir da interface de Linha de Comando (CLI) para gerenciar, pesquisar e instalar pacotes.

###### Yellowdog Updater Modified (YUM)

O YUM é uma ferramenta usada nas distribuições derivadas do Red Hat. É executada a partir da interface de Linha de Comando (CLI) para gerenciar, pesquisar e instalar pacotes. O YUM trabalha com arquivos .rpm.

#### Diferentes tipos de shells

##### Comunicação por meio de um shell

Como você explorou anteriormente, o shell é o interpretador de linha de comando. Você pode pensar em um shell como um tradutor entre você e o sistema do computador. Os shells permitem que você dê comandos ao computador e receba respostas dele. Quando você insere um comando em um shell, ele executa vários processos internos para interpretar o comando, enviá-lo ao kernel e retornar os resultados.

##### Tipos de shells

Os vários tipos diferentes de shells do Linux incluem os seguintes:

- Bourne-Again Shell (bash)
- C++ Shell (csh)
- Korn Shell (ksh)
- Shell em C aprimorado (tcsh)
- Z Shell (zsh)

Todos os shells do Linux usam comandos comuns do Linux, mas podem diferir em outros recursos. Por exemplo, o ksh e o bash usam o cifrão ($) para indicar onde os usuários digitam seus comandos. Outros shells, como o zsh, usam o sinal de porcentagem (%) para essa finalidade.

##### Bash

O Bash é o shell padrão na maioria das distribuições Linux. É considerado um shell fácil de usar. Você pode usar o Bash para comandos básicos do Linux, bem como para projetos maiores.

O Bash também é o shell mais popular na profissão de segurança cibernética. Você usará o Bash ao longo deste curso para aprender e praticar os comandos do Linux.