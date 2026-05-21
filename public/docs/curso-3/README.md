# Curso 3

## Conectar e Proteger: Redes e segurança de rede

### Modulo 1: Arquitetura de Computadores

#### Componentes, dispositivos e diagramas de rede

##### Dispositivos de rede

Os dispositivos de rede mantêm informações e serviços para os usuários de uma rede. Esses dispositivos se conectam por meio de conexões com e sem fio. Depois de estabelecer uma conexão com a rede, os dispositivos enviam pacotes de dados. Os pacotes de dados fornecem informações sobre a origem e o destino dos dados. É assim que as informações são enviadas e recebidas por meio de diferentes dispositivos em uma rede.

A rede é a infraestrutura geral que permite que os dispositivos se comuniquem entre si. Os dispositivos de rede são veículos especializados, como roteadores e switches, que gerenciam o que está sendo enviado e recebido pela rede. Além disso, dispositivos como computadores e telefones se conectam à rede por meio de dispositivos de rede. 

![demonstracao de rede](./public/img/demonstracao-rede.png)

**Observação**: neste diagrama, um **roteador** se conecta à Internet por meio de um modem, que é fornecido pelo seu provedor de acesso à Internet (ISP). O firewall é um dispositivo de segurança que monitora o tráfego de entrada e saída em sua rede. Em seguida, o roteador direciona o tráfego para os dispositivos em sua rede doméstica, que podem incluir computadores, laptops, smartphones, tablets, impressoras e outros dispositivos. Você pode imaginar aqui que o servidor é um servidor de arquivos. Todos os dispositivos dessa rede podem acessar os arquivos desse servidor. Este diagrama também inclui uma troca de rede, que é um dispositivo opcional que pode ser usado para conectar mais dispositivos à sua rede, fornecendo portas adicionais e conexões Ethernet. Além disso, há dois roteadores conectados ao switch aqui para fins de balanceamento de carga, o que melhorará o desempenho da rede.

##### Dispositivos e computadores desktop

A maioria dos usuários da Internet está familiarizada com dispositivos do dia a dia, como computadores pessoais, laptops, telefones celulares e tablets. Cada dispositivo e computador de mesa tem um endereço MAC e um endereço IP exclusivos, que o identificam na rede. Eles também têm uma interface de rede que envia e recebe pacotes de dados. Esses dispositivos podem se conectar à rede por meio de um fio rígido ou de uma conexão sem fio.

###### Firewalls

Um **firewall** é um dispositivo de Segurança de rede que monitora o tráfego de ou para a sua rede. É como sua primeira linha de defesa. Os firewalls também podem restringir o tráfego específico de entrada e saída da rede. A organização configura as regras de segurança do firewall. Os firewalls geralmente ficam entre a rede interna protegida e controlada e os recursos de rede não confiáveis fora da organização, como a Internet. Lembre-se, porém, de que os firewalls são apenas uma linha de defesa no cenário da segurança cibernética.

###### Servidores

Os **servidores** fornecem informações e serviços para dispositivos como computadores, dispositivos domésticos inteligentes e smartphones na rede. Os dispositivos que se conectam a um servidor são chamados de clientes. O gráfico a seguir descreve esse modelo, que é chamado de modelo cliente-servidor. Nesse modelo, os clientes enviam solicitações ao servidor para obter informações e serviços. O servidor executa as solicitações para os clientes. Exemplos comuns incluem servidores DNS que realizam pesquisas de nomes de domínio para sites da Internet, servidores de arquivos que armazenam e recuperam arquivos de um banco de dados e servidores de correio corporativo que organizam o correio de uma empresa.

![diagrama servidores](./public/img/diagrama-servidores.png)

###### Hubs e switches

Os hubs e os switches direcionam o tráfego em uma rede local. Um **hub** é um dispositivo que fornece um ponto comum de conexão para todos os dispositivos diretamente conectados a ele. Além disso, os hubs repetem todas as informações para todas as portas. Do ponto de vista da segurança, isso torna os hubs vulneráveis a espionagem. Por esse motivo, os hubs não são usados com tanta frequência nas redes modernas; em vez disso, a maioria das organizações usa switches. Os hubs são mais comumente usados para uma configuração de rede LIMIT, como um escritório doméstico.

Os switches são a escolha preferida para a maioria das redes. Um **switch** encaminha pacotes entre dispositivos diretamente conectados a ele. Ele analisa o endereço de destino de cada pacote de dados e o envia para o dispositivo pretendido. Os switches mantêm uma tabela de endereços MAC que faz a correspondência entre os endereços MAC dos dispositivos na rede e os números das portas do switch e encaminha os pacotes de dados recebidos de acordo com o endereço MAC de destino. Os switches fazem parte da camada de enlace de dados no modelo TCP/IP. De modo geral, os switches melhoram o desempenho e a segurança.

###### Roteadores

Os **roteadores** conectam redes e direcionam o tráfego, com base no endereço IP da rede de destino. Os roteadores permitem que dispositivos em redes diferentes se comuniquem entre si. No modelo TCP/IP, os roteadores fazem parte da camada de rede. O endereço IP da rede de destino está contido no cabeçalho IP. O roteador lê as informações do cabeçalho IPS e encaminha o pacote para o próximo roteador no caminho para o destino. Isso continua até que o pacote chegue à rede de destino. Os roteadores também podem incluir um recurso de firewall que permite ou bloqueia o tráfego de entrada com base nas informações da transmissão. Isso impede que o tráfego mal-intencionado entre na rede privada e danifique a rede local.

###### Modems e pontos de acesso sem fio

Os **modems** geralmente conectam sua casa ou escritório a um provedor de acesso à Internet (ISP). Os ISPs fornecem conectividade com a Internet por meio de linhas telefônicas, cabos coaxiais ou cabos de fibra óptica. Os modems recebem transmissões ou sinais digitais da Internet e os convertem em um formato digital compatível com a conexão física fornecida pelo ISP. Normalmente, os modems se conectam a um roteador que recebe as transmissões decodificadas e as envia para a rede local.

**Observação**: as redes corporativas usadas por grandes organizações para conectar seus usuários e dispositivos geralmente usam outras tecnologias de banda larga para lidar com o tráfego de alto volume, em vez de usar um modem.

![diagrama modems](./public/img/diagrama-modems.png)

###### Ponto de acesso sem fio

Um **ponto de acesso sem fio** envia e recebe sinais digitais por ondas de rádio, criando uma rede sem fio. Os dispositivos com adaptadores sem fio se conectam ao ponto de acesso usando Wi-Fi. Wi-Fi refere-se a um conjunto de padrões usados por dispositivos de rede para se comunicar sem fio. Os pontos de acesso sem fio e os dispositivos conectados a eles usam protocolos Wi-Fi para enviar dados por ondas de rádio, onde são enviados a roteadores e interruptores e direcionados ao longo do caminho até o destino final.

##### Uso de diagramas de rede como analista de segurança

Os **Diagramas de rede** permitem que os administradores de rede e a equipe de Segurança de rede imaginem a arquitetura e o design da rede privada de sua organização.

Os Diagramas de rede são mapas que mostram os dispositivos na rede e como eles se conectam. Os Diagramas de rede usam pequenos gráficos representativos para retratar cada dispositivo de rede e linhas pontilhadas para mostrar como cada dispositivo se conecta ao outro. Ao estudar os Diagramas de rede, os analistas de segurança desenvolvem e refinam suas estratégias para proteger as arquiteturas de rede.

![diagrama redes](./public/img/diagrama-redes.png)

#### Computação em nuvem e redes definidas por software

##### Processos de computação em nuvem

As redes tradicionais são chamadas de redes locais, o que significa que todos os dispositivos usados para as operações de rede são mantidos em um local físico de propriedade da empresa, como em um prédio de escritórios, por exemplo. **A computação em nuvem**, no entanto, refere-se à prática de usar servidores, aplicativos e serviços de rede remotos hospedados na Internet em vez de em um local físico de propriedade da empresa.

Um provedor de serviços em nuvem (CSP) é uma empresa que oferece serviços de computação em nuvem. Essas empresas possuem grandes data centers em locais ao redor do mundo que abrigam milhões de servidores. Os data centers fornecem serviços de tecnologia, como armazenamento e computação, em uma escala tão grande que podem vender seus serviços a outras empresas mediante o pagamento de uma taxa. As empresas podem pagar pelo armazenamento e pelos serviços de que precisam e consumi-los por meio da API (Interface de Programação de Aplicação) ou do console da Web do CSP.

Os CSPs oferecem três categorias principais de serviços:

- **Software como serviço (SaaS)** refere-se a conjuntos de software operados pelo CSP que uma empresa pode usar remotamente sem hospedar o software.
- **Infraestrutura como serviço (IaaS)** refere-se ao uso de componentes de computador virtuais oferecidos pelo CSP. Eles incluem contenções virtuais e armazenamento que são configurados remotamente por meio da API ou do console da Web do CSP. Os serviços de computação e armazenamento em nuvem podem ser usados para operar aplicativos existentes e outras cargas de trabalho de tecnologia sem modificações significativas. Os aplicativos existentes podem ser modificados para aproveitar os recursos de disponibilidade, desempenho e segurança que são exclusivos dos serviços do provedor de nuvem.
- **Plataforma como serviço (PaaS)** refere-se a ferramentas que os desenvolvedores de aplicativos podem usar para projetar aplicativos personalizados para sua empresa. Os aplicativos personalizados são projetados e acessados na Nuvem e usados para as necessidades comerciais específicas de uma empresa.

![Diferenças entre IaaS, PaaS e SaaS e como cada um se conecta a um data center físico](./public/img/CSP.png)

##### Ambientes de nuvem híbrida

Quando as organizações usam os serviços de um CSP além de seus computadores, redes de computadores e armazenamento no local, isso é chamado de ambiente de nuvem híbrida. Quando as organizações usam mais de um CSP, isso é chamado de ambiente de várias nuvens. A grande maioria das organizações usa ambientes de nuvem híbrida para reduzir custos e manter o controle sobre os recursos da rede.

##### Redes de computadores definidas por software

Os CSPs oferecem ferramentas de rede de computadores semelhantes aos dispositivos físicos sobre os quais você aprendeu nesta seção do curso. A seguir, você analisará a rede de computadores definida por software na Nuvem. As redes definidas por software (SDNs) são compostas de dispositivos e serviços de rede virtuais. Assim como os CSPs fornecem computadores virtuais, muitas SDNs também fornecem switches virtuais, roteadores, firewalls e muito mais. A maioria dos dispositivos de hardware de rede modernos também oferece suporte à virtualização de rede e à rede definida por software. Isso significa que os switches e roteadores físicos usam software para realizar o roteamento de pacotes. No caso da rede de computadores em nuvem, as ferramentas SDN são hospedadas em servidores localizados no data center do CSP.

##### Benefícios da computação em nuvem e das redes definidas por software 

Três dos principais motivos pelos quais a computação em nuvem é tão atraente para as empresas são a confiabilidade, a redução de custos e o aumento da escalonabilidade. 

###### Confiabilidade

A Confiabilidade na computação em nuvem se baseia na disponibilidade dos serviços e recursos da nuvem, na segurança das conexões e na frequência com que os serviços são efetivamente executados. A computação em nuvem permite que funcionários e clientes acessem os recursos de que precisam de forma consistente e com o mínimo de interrupção. 

###### Custos

Tradicionalmente, as empresas precisavam fornecer sua própria infraestrutura de rede, pelo menos para as conexões de Internet. Isso significava que poderia haver custos iniciais potencialmente significativos para as empresas. No entanto, como os CSPs têm data centers tão grandes, eles podem oferecer dispositivos e serviços de virtualização por uma fração do custo necessário para as empresas instalarem, corrigirem, atualizarem e gerenciarem os componentes e o software por conta própria.

###### Escalonabilidade

Outro desafio que as empresas enfrentam com o computador tradicional é a escalonabilidade. Quando as organizações experimentam um aumento em suas necessidades comerciais, elas podem ser forçadas a comprar mais equipamentos e software para acompanhar o ritmo. Mas e se os negócios diminuírem logo em seguida? Talvez não haja mais negócios que justifiquem o custo incorrido com os componentes atualizados. Os CSPs reduzem esse risco facilitando o consumo de serviços em um modelo de utilidade elástica, conforme necessário. Isso significa que as empresas pagam apenas pelo que precisam, quando precisam.

As mudanças podem ser feitas rapidamente por meio dos CSPs, APIs ou console da Web - muito mais rapidamente do que se os técnicos de rede tivessem que comprar seu próprio hardware e configurá-lo. Por exemplo, se uma empresa precisar se proteger contra uma ameaça à sua rede, os Firewalls de aplicativos da Web (WAF), os Sistemas de detecção de intrusão/proteção (IDS/IPS) ou os Firewalls L3/L4 podem ser configurados rapidamente sempre que necessário, levando a um melhor desempenho e segurança de rede.

#### Saiba mais sobre o modelo TCP/IP

##### O modelo TCP/IP

O **modelo TCP/IP** é uma estrutura usada para visualizar como os dados são organizados e transmitidos em uma rede. Esse modelo ajuda os engenheiros de rede e os analistas de segurança de rede a conceituar os processos na rede e a comunicar onde ocorrem interrupções ou ameaças à segurança.

O modelo TCP/IP tem quatro camadas: a camada de acesso à rede, a camada de Internet, a camada de transporte e a camada do aplicativo. Ao solucionar problemas na rede, os profissionais de segurança podem analisar quais camadas foram afetadas por um ataque com base nos processos envolvidos em um incidente. 
![As quatro camadas do modelo TCP/IP são denominadas camada do aplicativo, camada de transporte, camada da Internet e camada de acesso à rede](./public/img/TCP_IP_camadas.png)

##### Camada de acesso à rede

A **camada de acesso à rede**, às vezes chamada de camada de enlace de dados, lida com a criação de pacotes de dados e sua transmissão em uma rede. Essa camada corresponde ao hardware físico envolvido na transmissão da rede. Hubs, modems, cabos e fiação são todos considerados parte dessa camada. O protocolo de resolução de endereço (ARP) faz parte da camada de acesso à rede. Como os endereços MAC são usados para identificar hosts na mesma rede física, o ARP é necessário para mapear os endereços IP aos endereços MAC para a comunicação na rede local.

##### Camada da Internet

A **camada de Internet**, às vezes chamada de camada de rede, é responsável por garantir a entrega ao host de destino, que possivelmente reside em uma rede diferente. Ela garante que os endereços IP sejam anexados aos pacotes de dados para indicar a localização do remetente e do receptor. A camada de Internet também determina qual protocolo é responsável pela entrega dos pacotes de dados e garante a entrega ao host de destino. Aqui estão alguns dos protocolos comuns que operam na camada de Internet:

- **Protocolo de Internet (IP)**. O IP envia os pacotes de dados para o destino correto e conta com o protocolo TCP/IP (Transmission Control Protocol/User Datagrama IP) para entregá-los ao serviço correspondente. Os pacotes IPS permitem a comunicação entre duas redes de computadores. Eles são roteados da rede de computadores que os envia para a rede receptora. O TCP, em particular, retransmite todos os dados perdidos ou corrompidos.
- **Protocolo de Mensagens de Controle da Internet (ICMP)**. O ICMP compartilha informações sobre erros e atualizações de status de pacotes de dados. Isso é útil para detectar e solucionar problemas de erros de rede. O ICMP relata informações sobre pacotes que foram descartados ou que desapareceram em trânsito, problemas com a conectividade da rede e pacotes redirecionados para outros roteadores.

##### Camada de transporte

A camada de transporte é responsável pela entrega de dados entre dois sistemas ou redes e inclui protocolos para controlar o fluxo de tráfego em uma rede. O TCP e o UDP são os dois protocolos de transporte que ocorrem nessa camada.
Protocolo TCP

O **Protocolo de Controle de Transmissão (TCP)** é um protocolo de comunicação da Internet que permite que dois dispositivos formem uma conexão e transmitam dados. Ele garante que os dados sejam transmitidos de forma confiável para o serviço de destino. O TCP contém o número da porta do serviço de destino pretendido, que contém o cabeçalho TCP de um pacote TCP/IP.
Protocolo de datagrama do usuário 

O **User Datagram Protocol (UDP)** é um protocolo sem conexão que não estabelece uma conexão entre dispositivos antes das transmissões. Ele é usado por aplicativos que não se preocupam com a Confiabilidade da transmissão. Os dados enviados por UDP não são rastreados tão extensivamente quanto os dados enviados por TCP. Como o UDP não estabelece conexões de rede, ele é usado principalmente para aplicativos sensíveis ao desempenho que operam em tempo real, como streaming de vídeo.

##### Camada do aplicativo

A camada de aplicativo no modelo TCP/IP é semelhante às camadas de aplicativo, apresentação e sessão do modelo OSI. A camada do aplicativo é responsável por fazer solicitações de rede ou responder a solicitações. Essa camada define quais serviços e aplicativos da Internet qualquer usuário pode acessar. Os protocolos na camada do aplicativo determinam como os pacotes de dados interagirão com os dispositivos receptores. Alguns protocolos comuns usados nessa camada são:

- Hypertext Transfer Protocol (HTTP)
- Protocolo de transferência de correio simples (SMTP)
- Secure Shell (SSH)
- Protocolo de Transferência de Arquivos (FTP)
- Sistema de Nomes de Domínio (DNS)

Os protocolos da camada de aplicativo dependem das camadas subjacentes para transferir os dados pela rede.

##### Modelo TCP/IP versus modelo OSI

![O modelo TCP/IP ao lado do modelo OSI](./public/img/TCP_IP_OSI.png)

O modelo **OSI** organiza visualmente os protocolos de rede em diferentes camadas. Os profissionais de rede geralmente usam esse modelo para se comunicarem uns com os outros sobre possíveis fontes de problemas ou ameaças à segurança de rede quando elas ocorrem. 

O modelo TCP/IP combina várias camadas do modelo OSI. Há muitas semelhanças entre os dois modelos. Ambos os modelos definem padrões para a rede de computadores e dividem o processamento da comunicação de rede em diferentes camadas. O modelo TCP/IP é uma versão simplificada do modelo OSI.

#### O modelo OSI

##### O modelo TCP/IP vs. o modelo OSI

O **modelo TCP/IP** é uma estrutura usada para visualizar como os dados são organizados e transmitidos em uma rede. Esse modelo ajuda os engenheiros de rede e os analistas de segurança a conceituar os processos na rede e a comunicar onde ocorrem interrupções ou ameaças à segurança.

O modelo TCP/IP tem quatro camadas: a camada de acesso à rede, a camada de Internet, a camada de transporte e a camada do aplicativo. Ao analisar eventos de rede, os profissionais de segurança podem determinar em que camada ou camadas ocorreu um ataque com base nos processos envolvidos no incidente. 

O **modelo OSI** é um conceito padronizado que descreve as sete camadas que os computadores usam para se comunicar e enviar dados pela rede. Os profissionais de segurança de rede e de segurança geralmente usam esse modelo para se comunicarem entre si sobre possíveis fontes de problemas ou ameaças à segurança quando elas ocorrem.

![As sete camadas do modelo OSI rotuladas como aplicativo, apresentação, sessão, transporte, rede, enlace de dados e física](./public/img/OSI_camadas.png)

Algumas organizações dependem muito do modelo TCP/IP, enquanto outras preferem usar o modelo OSI. AS como analista de segurança, é importante estar familiarizado com ambos os modelos. Os modelos TCP/IP e OSI são úteis para entender como as redes de computadores funcionam.

##### Camada 7: camada do aplicativo

A camada do aplicativo inclui os processos que envolvem diretamente o usuário comum. Essa camada inclui todos os protocolos de rede que os aplicativos de software usam para conectar um usuário à Internet. Essa característica é a que identifica a camada do aplicativo: a conexão do usuário à Internet por meio de aplicativos e solicitações.

Um exemplo de um tipo de comunicação que ocorre na camada do aplicativo é o uso de um navegador da Web. O navegador da Internet usa HTTP ou HTTPS para enviar e receber informações do servidor do site. O aplicativo de e-mail usa o protocolo de transferência de correio simples (SMTP) para enviar e receber informações de e-mail. Além disso, os navegadores da Web usam o protocolo DNS (sistema de nomes de domínio) para traduzir os nomes de domínio do site em endereços IP que identificam o servidor da Web que hospeda as informações do site. 

##### Camada 6: camada de apresentação

As funções da camada de apresentação envolvem a tradução de dados e a criptografia para a rede. Essa camada adiciona e substitui dados por formatos que podem ser compreendidos pelos aplicativos (camada 7) nos sistemas de envio e recebimento. Os formatos na extremidade do usuário podem ser diferentes daqueles do sistema receptor. Os processamentos na camada de apresentação exigem o uso de um formato padronizado.

Algumas funções de formatação que ocorrem na camada 6 incluem criptografia, compactação e confirmação de que o conjunto de códigos de caracteres pode ser interpretado no sistema receptor. Um exemplo de criptografia que ocorre nessa camada é o SSL, que criptografa os dados entre os servidores da Web e os navegadores como parte de sites com HTTPS.

##### Camada 5: camada de sessão

Uma sessão descreve quando uma conexão é estabelecida entre dois dispositivos. Uma sessão aberta permite que os dispositivos se comuniquem entre si. Os protocolos da camada de sessão mantêm a sessão aberta enquanto os dados estão sendo transferidos e encerram a sessão quando a transmissão é concluída.

A camada de sessão também é responsável por atividades como autenticação, reconexão e definição de pontos de verificação durante uma transferência de dados. Se uma sessão for interrompida, os pontos de verificação garantem que a transmissão seja retomada no último ponto de verificação da sessão quando a conexão for retomada. As sessões incluem uma solicitação e uma resposta entre aplicativos. As funções na camada de sessão respondem a solicitações de serviço de processos na camada de apresentação (camada 6) e enviam solicitações de serviços para a camada de transporte (camada 4).

##### Camada 4: camada de transporte

A camada de transporte é responsável pela entrega de dados entre dispositivos. Essa camada também lida com a velocidade da transferência de dados, com o Fluxo da transferência e com a divisão dos dados em segmentos menores para facilitar o transporte. Segmentação é o processo de dividir uma grande transmissão de dados em partes menores que podem ser processadas pelo sistema receptor. Esses segmentos precisam ser remontados em seu destino para que possam ser processados na camada de sessão (camada 5). A velocidade e a taxa da transmissão também precisam corresponder à velocidade da conexão do sistema de destino. O TCP e o UDP são protocolos da camada de transporte.

##### Camada 3: camada de rede

A camada de rede supervisiona o recebimento dos frames da camada de enlace de dados (camada 2) e os entrega ao destino pretendido. O destino pretendido pode ser encontrado com base no endereço que reside no frame dos pacotes de dados. Os pacotes de dados permitem a comunicação entre duas redes de computadores. Esses pacotes incluem endereços IP que informam aos roteadores para onde devem ser enviados. Eles são roteados da rede de envio para a rede de recebimento.

##### Camada 2: camada de enlace de dados

A camada de enlace de dados organiza o envio e o recebimento de pacotes de dados em uma única rede. A camada de enlace de dados abriga as trocas de rede locais e as placas de interface de rede (NIC) nos dispositivos locais.

Protocolos como o protocolo de controle de rede (NCP), o controle de link de dados de alto nível (HDLC) e o protocolo de controle de link de dados síncrono (SDLC) são usados na camada de enlace de dados.

##### Camada 1: camada física

Como o nome sugere, a camada física corresponde ao hardware físico envolvido na transmissão da rede. Hubs, modems a cabo e os cabos e a fiação que os conectam são considerados parte da camada física. Para trafegar por um cabo Ethernet ou coaxial, um pacote de dados precisa ser traduzido em um fluxo de 0s e 1s. O fluxo de 0s e 1s é enviado através da fiação e dos cabos físicos, recebido e, em seguida, passado para níveis mais altos do modelo OSI.

#### Componentes da comunicação na camada de rede

##### Operações na camada de rede

As funções da camada de rede organizam o endereçamento e o fornecimento de pacotes de dados pela rede, do dispositivo host ao dispositivo de destino. Isso inclui o direcionamento dos pacotes de um roteador para outro roteador na Internet, até chegar ao endereço IP (Internet Protocol) da rede de destino. O endereço IP de destino está contido no Cabeçalho de cada pacote de dados. Esse endereço será armazenado para fins de roteamento futuro em tabelas de roteamento ao longo do caminho do pacote até seu destino.

Todos os pacotes de dados incluem um endereço IP. Um pacote de dados também é chamado de pacote IP para conexões TCP ou datagrama IP para conexões UDP. Um roteador usa o endereço IP para encaminhar os pacotes de uma rede para outra com base nas informações contidas no Cabeçalho IP de um pacote de dados. As informações do Cabeçalho comunicam mais do que apenas o endereço do destino. Elas também incluem informações como o endereço IP de origem, o tamanho do pacote e qual protocolo será usado para a parte de dados do pacote.

###### Formato de um pacote IPv4

![Um pacote de IPS dividido em duas partes: uma seção à esquerda marcada como "cabeçalho" e uma seção à direita marcada como "dados"](./public/img/pacote_ipv4.png)

A seguir, você pode analisar o formato de um pacote IP versão 4 (IPv4) e ver um gráfico detalhado do Cabeçalho do pacote. Um pacote IPv4 é composto de duas seções, o Cabeçalho e os dados:

- O formato do Cabeçalho IPv4 é determinado pelo protocolo IPv4 e inclui as Informações de roteamento IP que os dispositivos usam para direcionar o pacote. O tamanho do Cabeçalho IPv4 varia de 20 a 60 bytes. Os primeiros 20 bytes são um conjunto fixo de informações que contêm dados como o endereço IP de origem e destino, o comprimento do cabeçalho e o comprimento total do pacote. O último conjunto de bytes pode variar de 0 a 40 e consiste no campo "Options".
- O Comprimento da seção de dados de um pacote IPv4 pode variar muito em tamanho. Entretanto, o tamanho máximo possível de um pacote IPv4 é de 65.535 bytes. Contém a mensagem que está sendo transferida pela Internet, como informações de um site ou texto de e-mail. 

    ![Diagrama de um cabeçalho de pacote IPv4, 13 campos e tamanho de bit](./public/img/cabecalho_pacote_ipv4.png)

Há 13 campos no Cabeçalho de um pacote IPv4:

- **Versão (VER)**: Esse componente de 4 bits informa aos dispositivos receptores qual protocolo o pacote está usando. O pacote usado na ilustração acima é um pacote IPv4.
- **Comprimento do Cabeçalho IP (HLEN ou IHL)**: HLEN é o comprimento do cabeçalho do pacote. Esse valor indica onde termina o Cabeçalho do pacote e começa o segmento de dados.
- **Tipo de serviço (ToS)**: Os roteadores priorizam a entrega de pacotes para manter a qualidade do serviço na rede. O Campo ToS fornece essas informações ao roteador.
- **Comprimento total (Total Comprimento)**: Esse campo comunica o comprimento total de todo o pacote IP, incluindo o "Header" e os dados. O tamanho máximo de um pacote IPv4 é de 65.535 bytes.
- **Identificação**: Os pacotes IPv4 podem ter até 65.535 bytes, mas a maioria das redes de computadores tem um LIMIT menor. Nesses casos, os pacotes são divididos, ou fragmentados, em pacotes IPS menores. O campo "Identification" fornece um identificador exclusivo para todos os fragmentos do pacote IP original, de modo que eles possam ser remontados quando chegarem ao destino.
- **Sinalizadores**: Esse campo fornece ao dispositivo de roteamento mais informações sobre se o pacote original foi fragmentado e se há mais fragmentos em trânsito.
- **Fragmentation Offset (deslocamento de fragmentação)**: O campo "Fragmentation offset" informa aos dispositivos de roteamento a que parte do pacote original o fragmento pertence.
- **Time to Live (TTL)**: o TTL impede que os pacotes de dados sejam encaminhados indefinidamente pelos roteadores. Ele contém um contador que é definido pela fonte. O contador é diminuído em um à medida que passa por cada roteador em seu caminho. Quando o contador TTL chegar a zero, o roteador que estiver segurando o pacote o descartará e retornará uma mensagem de erro ICMP Time Exceeded ao remetente.
- **Protocolo**: O campo "Protocolo" informa ao dispositivo receptor qual protocolo será usado para a parte de dados do pacote.
- **Checksum do Cabeçalho**: O campo "header checksum" contém uma soma de verificação que pode ser usada para detectar corrupção do cabeçalho IPS em trânsito. Os pacotes corrompidos são descartados.
- **Endereço IP de origem**: O endereço IP de origem é o endereço IPv4 do dispositivo de envio.
- **Endereço IP de destino**: O endereço IP de destino é o endereço IPv4 do dispositivo de destino.
- **Options (Opções)**: O campo "Options" permite que opções de segurança sejam aplicadas ao Pacote se o valor HLEN for maior que cinco. O campo "Options" comunica essas opções aos dispositivos de roteamento.

##### Diferença entre IPv4 e IPv6

Em uma parte anterior deste curso, você aprendeu sobre a história do endereço IP. À medida que a Internet crescia, ficou claro que todos os endereços IPv4 acabariam se esgotando; isso é chamado de exaustão de endereços IPv4. Na época, ninguém havia previsto quantos dispositivos de computador precisariam de um endereço IP. O IPv6 foi desenvolvido para mitigar o esgotamento de endereços IPv4 e outras preocupações relacionadas.

Algumas das principais diferenças entre o IPv4 e o IPv6 incluem o comprimento e o formato dos endereços. Os endereços IPv4 são compostos de quatro números decimais separados por pontos, cada número variando de 0 a 255. Juntos, os números abrangem 4 bytes e permitem até 4,3 bilhões de endereços possíveis. Um exemplo de um endereço IPv4 seria: 198.51.100.0. Os endereços IPv6 são formados por oito números hexadecimais separados por dois pontos, sendo que cada número consiste em até quatro dígitos hexadecimais. Juntos, todos os números abrangem 16 bytes e permitem até 340 undecilhões de endereços (340 seguido de 36 zeros). Um exemplo de um endereço IPv6 seria: 2002:0db8:0000:0000:0000:ff21:0023:1234.

**Observação**: para representar um ou mais conjuntos consecutivos de todos os zeros, você pode substituir os zeros por dois pontos duplos "::", de modo que o endereço IPv6 acima seria "2002:0db8::ff21:0023:1234"

Há também algumas diferenças no layout do Cabeçalho de um pacote IPv6. O formato do Cabeçalho do IPv6 é muito mais simples do que o do IPv4. Por exemplo, o Cabeçalho IPv4 inclui os campos "IHL", "Identification" e "Flags", enquanto o IPv6 não inclui. O Cabeçalho IPv6 introduz apenas o campo "Flow Rótulo", no qual o Rótulo de Fluxo identifica um Pacote que requer tratamento especial por outros roteadores IPv6.

![Diagramas lado a lado de um cabeçalho de pacote IPv4 e de um pacote IPv6 simplificado](./public/img/comparacao_cabecalho_ipv4_ipv6.png)

Há algumas diferenças importantes de segurança entre o IPv4 e o IPv6. O IPv6 oferece roteamento mais eficiente e elimina as colisões de endereços privados que podem ocorrer no IPv4 quando dois dispositivos na mesma rede estão tentando usar o mesmo endereço.

### Modulo 2: Operações de Redes

#### Protocolos de rede comuns

##### Visão geral dos protocolos de rede

Um protocolo de rede é um conjunto de regras usadas por dois ou mais dispositivos em uma rede para descrever a ordem de entrega e a estrutura de dados. Os protocolos de rede funcionam como instruções que acompanham as informações do pacote de dados. Essas instruções dizem ao dispositivo receptor o que fazer com os dados. Os protocolos são como uma linguagem comum que permite que dispositivos de todo o mundo se comuniquem e se entendam.

Embora os protocolos de rede desempenhem uma função essencial na comunicação de rede, os analistas de segurança ainda devem entender suas implicações de segurança associadas. Alguns protocolos têm vulnerabilidades que são exploradas por agentes mal-intencionados. Por exemplo, um agente nefasto poderia usar o protocolo do Sistema de Nomes de Domínio (DNS), que resolve endereços da Web para endereços IP, para desviar o Tráfego de um site legítimo para um site malicioso que contenha malware. Você aprenderá mais sobre esse tópico nos próximos Materiais do curso.

##### Três categorias de protocolos de rede

Os protocolos de rede podem ser divididos em três categorias principais: protocolos de comunicação, protocolos de gerenciamento e protocolos de segurança. Há dezenas de protocolos de rede diferentes, mas você não precisa memorizar todos eles para uma função de analista de segurança de nível básico. Entretanto, é importante que você conheça os que estão listados nesta leitura.

###### Protocolos de comunicação

Os protocolos de comunicação regem a troca de informações na transmissão da rede. Eles determinam como os dados são transmitidos entre os dispositivos e o tempo da comunicação. Eles também incluem métodos para recuperar dados perdidos em trânsito. Aqui estão alguns deles.

- **O Protocolo de controle de transmissão/protocolo de Internet(TCP)** é um protocolo de comunicação da Internet que permite que dois dispositivos formem uma conexão e transmitam dados. O TCP usa um processamento de handshake de três vias. Primeiro, o dispositivo envia uma solicitação de sincronização (SYN) a um servidor. Em seguida, o servidor responde com um pacote SYN/ACK para confirmar o recebimento da solicitação do dispositivo. Quando o servidor recebe o pacote ACK final do dispositivo, é estabelecida uma conexão TCP. No modelo TCP/IP, o TCP ocorre na camada de transporte.

- **O UDP (User Datagram Protocol)** é um protocolo sem conexão que não estabelece uma conexão entre dispositivos antes de uma transmissão. Isso o torna menos confiável do que o TCP. Mas isso também significa que ele funciona bem para transmissões que precisam chegar rapidamente ao seu destino. Por exemplo, um dos usos do UDP é o envio de solicitações de DNS para servidores DNS locais. No modelo TCP/IP, o UDP ocorre na camada de transporte.

- **O Protocolo de transferência de hipertexto (HTTP)** é um protocolo da camada do aplicativo que fornece um método de comunicação entre clientes e servidores de sites. O HTTP usa a porta 80. O HTTP é considerado inseguro, por isso está sendo substituído na maioria dos sites por uma versão segura, chamada HTTPS, que usa criptografia de SSL/TLS para comunicação. Entretanto, ainda há muitos sites que usam o protocolo HTTP inseguro. No modelo TCP/IP, o HTTP ocorre na camada do aplicativo.

- **O Sistema de Nomes de Domínio (DNS)** é um protocolo que traduz os nomes de domínio da Internet em endereços IP. Quando um computador cliente deseja acessar o domínio de um site usando seu navegador da Internet, uma consulta é enviada a um servidor DNS dedicado. Em seguida, o servidor DNS procura o endereço IP que corresponde ao domínio do site. O DNS normalmente usa UDP na porta 53. No entanto, se a resposta do DNS a uma solicitação for grande, ele passará a usar o protocolo TCP. No modelo TCP/IP, o DNS ocorre na camada do aplicativo.

###### Protocolos de gerenciamento

A próxima categoria de protocolos de rede são os protocolos de gerenciamento. Os protocolos de gerenciamento são usados para monitorar e gerenciar a atividade em uma rede. Eles incluem protocolos para relatórios de erros e otimização do desempenho na rede.

- **O Protocolo de Gerenciamento de Rede Simples (SNMP)** é um protocolo de rede usado para monitorar e gerenciar dispositivos em uma rede. O SNMP pode redefinir uma senha em um dispositivo de rede ou mudar sua configuração de linha de base. Ele também pode enviar solicitações aos dispositivos de rede para obter um relatório sobre a quantidade de largura de banda da rede que está sendo usada. No modelo TCP/IP, o SNMP ocorre na camada do aplicativo.

- **O Protocolo de controle de transmissão/protocolo de Internet (TCP/IP)** é um protocolo de Internet usado por dispositivos para informar uns aos outros sobre erros de transmissão de dados na rede. O ICMP é usado por um dispositivo receptor para enviar um relatório ao dispositivo remetente sobre a transmissão de dados. O ICMP é comumente usado como uma forma rápida de solucionar problemas de conectividade e latência da rede, emitindo o comando "ping" em um sistema operacional Linux. No modelo TCP/IP, o ICMP ocorre na camada da Internet.

###### Protocolos de segurança

Os protocolos de segurança são protocolos de rede que garantem que os dados sejam enviados e recebidos com segurança em uma rede. Os protocolos de segurança usam algoritmos de criptografia para proteger os dados em trânsito. Abaixo estão alguns protocolos de segurança comuns.

- **O Protocolo de transferência de hipertexto seguro (HTTPS)** é um protocolo de rede que fornece um método seguro de comunicação entre clientes e servidores de sites. O HTTPS é uma versão segura do HTTP que usa criptografia SSL/TLS (Secure Sockets Layer/Segurança da camada de transporte) em todas as transmissões para que agentes mal-intencionados não possam ler as informações contidas. O HTTPS usa a porta 443. No modelo TCP/IP, o HTTPS ocorre na camada do aplicativo.

- **O Protocolo de Transferência de Arquivos (FTP)** é um protocolo seguro usado para transferir arquivos de um dispositivo para outro em uma rede. O SFTP usa o Secure Shell (SSH), normalmente pela porta TCP 22. O SSH usa o Padrão de Criptografia Avançada (AES) e outros tipos de criptografia para garantir que destinatários não intencionais não possam interceptar as transmissões. No modelo TCP/IP, o SFTP ocorre na camada do aplicativo. O SFTP é usado com frequência no armazenamento em Nuvem. Sempre que um usuário faz upload ou download de um arquivo do armazenamento em nuvem, o arquivo é transferido usando o protocolo SFTP.

Observação: os protocolos de criptografia mencionados não ocultam o endereço IP de origem ou de destino do tráfego de rede. Isso significa que um agente mal-intencionado ainda pode saber algumas informações básicas sobre o tráfego de rede se o interceptar.

#### Protocolos de rede adicionais

##### Conversão de endereços de rede

Os dispositivos da rede local de sua casa ou escritório têm um endereço IP privado que usam para se comunicar diretamente uns com os outros. No entanto, para que os dispositivos com endereços IP privados possam se comunicar com a Internet pública, eles precisam ter um único endereço IP público que represente todos os dispositivos da LAN para o público. Para mensagens de saída, o roteador pode substituir um endereço IP de origem privada por seu endereço IP público e realizar a operação inversa para as respostas. Esse processo é conhecido como NAT (Rede Address Translation, conversão de endereços de rede) e geralmente requer que um roteador ou firewall seja configurado especificamente para realizar o NAT. O NAT faz parte da camada 2 (camada de Internet) e da camada 3 (camada de transporte) do modelo TCP/IP.

| Endereços IP privados | Endereços IP públicos |
| --- | --- |
| Atribuídos pelo roteador | Atribuídos pelo ISP e pela IANA |
| Único somente dentro da rede privada | Endereço Único na Internet global |
| Não há custo de uso | Custos de aluguel de um endereço IP público |
| Intervalos de endereços: | Intervalos de endereços atribuíveis: |
| - 10.0.0.0-10.255.255.255 | - 1.0.0.0-9.255.255.255 |
| - 172.16.0.0-172.31.255.255 | - 11.0.0.0-126.255.255.255 |
| - 192.168.0.0-192.168.255.255 | - 128.0.0.0-172.15.255.255 |
| | - 172.32.0.0-192.167.255.255 |
| | - 192.169.0.0-233.255.255.255 |

##### Protocolo de configuração de host dinâmico (DHCP)

O Protocolo de configuração de host dinâmico (DHCP) faz parte da família de gerenciamento de protocolos de rede. O DHCP é um protocolo de camada de aplicativo usado em uma rede para configurar dispositivos. Ele trabalha com o roteador para atribuir um endereço IP exclusivo a cada dispositivo e fornecer os endereços do servidor DNS e do gateway padrão apropriados para cada dispositivo. Os servidores DHCP operam na porta UDP 67, enquanto os clientes DHCP operam na porta UDP 68.

##### Protocolo de resolução de endereço

Até agora, você está familiarizado com os endereços IP e MAC. Você aprendeu que cada dispositivo em uma rede tem um endereço IP público, um endereço IP privado e um endereço MAC que o identificam na rede. O endereço IP de um dispositivo pode mudar com o tempo, mas o endereço MAC é permanente porque é exclusivo da Placa de interface de rede (NIC) do dispositivo. O endereço MAC é usado para se comunicar com dispositivos na mesma rede, mas, às vezes, o endereço MAC é desconhecido. É por isso que o protocolo de resolução de endereço (ARP) é necessário. O ARP é principalmente um protocolo de camada de acesso à rede no modelo TCP/IP usado para conversão de endereços de IP encontrados em pacotes de dados para o endereço MAC do dispositivo de hardware.

Cada dispositivo na rede executa o ARP e mantém o controle dos endereços IP e MAC correspondentes em um cache de ARP. O ARP não tem um número de porta específico, pois é um protocolo da camada 2 e os números de porta estão associados à camada 7 do aplicativo.

##### Telnet

O Telnet é um protocolo da camada do aplicativo usado para se conectar a um sistema remoto. A Telnet envia todas as informações em texto claro. Ele usa linhas de comando para controlar outro dispositivo, semelhante ao SSH (secure shell), mas o Telnet não é tão seguro quanto o SSH. A Telnet pode ser usada para se conectar a dispositivos locais ou remotos e usa a porta TCP 23.

##### Secure Shell

O protocolo Secure Shell (SSH) é usado para criar uma conexão segura com um sistema remoto. Esse protocolo da camada do aplicativo fornece uma alternativa para autenticação segura e comunicação criptografada. O SSH opera pela porta TCP 22 e é um substituto para protocolos menos seguros, como o Telnet.

##### Protocolo Post Office

O Post Office Protocol (POP) é um protocolo da camada do aplicativo (camada 4 do modelo TCP/IP) usado para gerenciar e recuperar e-mails de um servidor de e-mail. O POP3 é a versão mais comumente usada do POP. Muitas organizações têm um servidor de e-mail dedicado na rede que lida com a entrada e saída de e-mails para os usuários da rede. Os dispositivos dos usuários enviarão solicitações ao servidor de e-mail remoto e farão download de mensagens de e-mail localmente. Se você já atualizou seu aplicativo de e-mail e recebeu novos e-mails na sua caixa de entrada, está experimentando o POP e o protocolo de acesso a mensagens da Internet (IMAP) em ação. A autenticação de texto simples não criptografada usa a porta TCP/UDP 110 e os e-mails criptografados usam a Camada de soquetes seguros (SSL) pela porta TCP/UDP 995. Ao usar o POP, o e-mail precisa terminar o download em um dispositivo local antes de poder ser lido. Após o download, o e-mail pode ou não ser excluído do servidor de e-mail, portanto, não garante que um usuário possa sincronizar o mesmo e-mail em vários dispositivos.

##### Protocolo de acesso a mensagens da Internet (IMAP)

O IMAP é usado para e-mails recebidos. Ele baixa os Cabeçalhos dos e-mails e o conteúdo da mensagem. O conteúdo também permanece no servidor de e-mail, o que permite que os usuários acessem seus e-mails de vários dispositivos. O IMAP usa a porta TCP 143 para e-mail não criptografado e a porta TCP 993 sobre o protocolo TLS. O uso do IMAP permite que os usuários leiam parcialmente o e-mail antes de terminar o download. Como o e-mail é mantido no servidor de e-mail, ele permite que o usuário sincronize e-mails em vários dispositivos. 

##### Protocolo de transferência de correio simples (SMTP)

O SMTP (Protocolo de transferência de correio simples (SMTP)) é usado para transmitir e rotear e-mails do remetente para o endereço do destinatário. O SMTP funciona com o software Message Transfer Agent (MTA), que pesquisa nos servidores DNS para resolver endereços de e-mail para endereços IP, a fim de garantir que os e-mails cheguem ao destino pretendido. O SMTP usa a porta TCP/UDP 25 para e-mails não criptografados e a porta TCP/UDP 587 usando TLS para e-mails criptografados. A porta TCP 25 é frequentemente usada por Spam de alto volume. O SMTP ajuda a filtrar o spam regulando a quantidade de e-mails que uma fonte pode enviar por vez.

##### Protocolos e números de porta

Lembre-se de que os números das portas são usados pelos dispositivos de rede para determinar o que deve ser feito com as informações contidas em cada pacote de dados quando eles chegam ao destino. Os firewalls podem filtrar o tráfego indesejado com base nos números das portas. Por exemplo, uma organização pode configurar um firewall para permitir apenas o acesso à porta TCP 995 (POP3) por endereços IP pertencentes à organização.

AS Como analista de segurança, você precisará conhecer muitos dos protocolos e números de porta mencionados neste curso. Eles podem ser usados para determinar seu conhecimento técnico em entrevistas, portanto, é uma boa ideia memorizá-los. Você também aprenderá sobre novos protocolos no trabalho em uma posição de segurança.

##### Principais lições

Como analista de segurança cibernética, você encontrará vários protocolos comuns em seu trabalho diário. Os protocolos abordados nesta leitura incluem NAT, DHCP, ARP, Telnet, SSH, POP3, IMAP e SMTP. É igualmente importante entender onde cada protocolo está estruturado no modelo TCP/IP e quais portas eles ocupam.

| Protocolo | Porta |
|-----------|-------|
| DHCP | Porta UDP 67 (servidores) <br>Porta UDP 68 (clientes) |
| ARP | nenhum |
| Telnet | TCP porta 23 |
| SSH | TCP porta 22 |
| POP3 | Porta TCP/UDP 110 (não criptografada) <br>TCP/UDP porta 995 (criptografia, SSL/TLS) |
| IMAP | Porta TCP 143 (não criptografada) <br>TCP porta 993 (criptografia, SSL/TLS) |
| SMTP | TCP/UDP porta 25 (não criptografada) |
| SMTPS | TCP/UDP porta 587 (criptografia, TLS) |

#### A evolução dos protocolos de segurança sem fio

##### Introdução aos protocolos de comunicação sem fio

Atualmente, muitas pessoas se referem à Internet sem fio como **Wi-Fi**. Wi-Fi refere-se a um conjunto de padrões que definem a comunicação para LANs sem fio. Wi-Fi é um termo de marketing encomendado pela WECA (Wireless Ethernet Compatibilidade Alliance). Desde então, a WECA mudou o nome de sua organização para Wi-Fi Alliance.

Os padrões e protocolos Wi-Fi são baseados na família 802.11 de padrões de comunicação da Internet determinados pelo IEEE (Institute of Electrical and Electronics Engineers). Portanto, como analista de segurança, você também poderá ver o Wi-Fi ser chamado de IEEE 802.11.

As comunicações Wi-Fi são protegidas por protocolos de rede de computadores sem fio. Os protocolos de segurança sem fio evoluíram ao longo dos anos, ajudando a identificar e resolver vulnerabilidades com tecnologias sem fio mais avançadas.

Nesta leitura, você aprenderá sobre a evolução dos protocolos de segurança sem fio de WEP para WPA, WPA2 e WPA3. Você também aprenderá como o Protocolo de Aplicativos Sem Fio foi usado para comunicações móveis pela Internet.

##### Privacidade equivalente à de redes

Privacidade equivalente à de redes com fio (WEP) é um protocolo de segurança de rede sem fio projetado para fornecer aos usuários o mesmo nível de privacidade em conexões de rede sem fio que eles têm em conexões de rede com fio. O WEP foi desenvolvido em 1999 e é o mais antigo dos padrões de segurança sem fio.

Atualmente, o WEP está em grande parte fora de uso, mas os analistas de segurança ainda devem entender o WEP caso se deparem com ele. Por exemplo, um roteador de rede pode ter usado o WEP como protocolo de segurança padrão e o administrador da rede nunca o alterou. Ou os dispositivos em uma rede podem ser muito antigos para suportar protocolos de segurança de Wi-Fi mais recentes. No entanto, um agente mal-intencionado poderia quebrar a criptografia WEP, portanto, agora é considerado um protocolo de segurança de alto risco.

##### Wi-Fi Protected Access

O Wi-Fi Protected Access (WPA) foi desenvolvido em 2003 para aprimorar o WEP, resolver os problemas de segurança que ele apresentava e substituí-lo. O WPA sempre foi planejado para ser uma medida de transição, de modo que a compatibilidade com versões anteriores pudesse ser estabelecida com hardware mais antigo.

As falhas do WEP estavam no próprio protocolo e em como a criptografia era usada. O WPA abordou esse ponto fraco usando um protocolo chamado TKIP (Temporal Key Integrity Protocol). O algoritmo de criptografia WPA usa chaves secretas maiores que as do WEP, o que torna mais difícil adivinhar a chave por tentativa e erro.

O WPA também inclui uma verificação de integridade da mensagem que inclui uma tag de autenticação de mensagem em cada transmissão. Se um agente mal-intencionado tentar alterar a transmissão de alguma forma ou reenviá-la em outro momento, a verificação de integridade da mensagem do WPA identificará o ataque e rejeitará a transmissão.

Apesar dos aprimoramentos de segurança do WPA, ele ainda tem vulnerabilidades. Agentes mal-intencionados podem usar um ataque de reinstalação de chave (ou ataque KRACK) para descriptografar transmissões usando o WPA. Os atacantes podem se inserir no processamento do handshake de autenticação do WPA e inserir uma nova chave de criptografia em vez da chave dinâmica atribuída pelo WPA. Se eles definirem a nova chave com todos os zeros, é como se a transmissão não fosse criptografada.

Devido a essa vulnerabilidade significativa, o WPA foi substituído por uma versão atualizada do protocolo chamada WPA2.

##### WPA2 E WPA3

###### WPA2

A segunda versão do Wi-Fi Protected Access, conhecida como WPA2, foi lançada em 2004. O WPA2 aprimora o WPA usando o Padrão de Criptografia Avançada (AES). O WPA2 também aprimora o uso do TKIP pelo WPA. O WPA2 usa o protocolo CCMP (Counter Mode Cifra de bloco encadeada para autenticação de mensagens), que fornece encapsulamento e garante a autenticação e a integridade das mensagens. Devido à força do WPA2, ele é considerado o padrão de segurança para todas as transmissões Wi-Fi atuais. O WPA2, como seu antecessor, é vulnerável a ataques KRACK. Isso levou ao desenvolvimento do WPA3 em 2018.

###### Personalização

O modo pessoal do WPA2 é mais adequado para redes de computadores domésticas por vários motivos. É fácil de implementar e a configuração inicial leva menos tempo para a versão pessoal do que para a versão corporativa. A frase secreta global da versão pessoal do WPA2 precisa ser aplicada a cada computador e ponto de acesso (PA) em uma rede. Isso a torna ideal para redes de computadores domésticas, mas impossível de gerenciar em organizações.

###### Empresarial

O modo WPA2 Enterprise funciona melhor para aplicativos comerciais. Ele fornece a segurança necessária para redes sem fio em ambientes comerciais. A configuração inicial é mais complicada que a do modo pessoal WPA2, mas o modo enterprise oferece controle individualizado e centralizado sobre o acesso Wi-Fi a uma rede de computadores. Isso significa que os administradores de rede podem conceder ou remover o acesso de usuários a uma rede a qualquer momento. Os usuários nunca têm acesso às chaves de criptografia, o que impede que possíveis atacantes recuperem as chaves de rede de computadores individuais.

###### WPA3

O WPA3 é um protocolo Wi-Fi seguro e está crescendo em uso à medida que mais dispositivos compatíveis com o WPA3 são lançados. Estas são as principais diferenças entre o WPA2 e o WPA3:

- O WPA3 aborda a vulnerabilidade do handshake de autenticação para ataques KRACK, que é apresentada no WPA2.
- O WPA3 usa Simultaneous Authentication of Equals (SAE), um acordo de compartilhamento de chave de cifra autenticado por senha. Isso impede que os atacantes baixem os dados das conexões de rede sem fio para seus sistemas e tentem decodificá-los.
- O WPA3 aumentou a criptografia para tornar as senhas mais seguras, usando criptografia de 128 bits, com o modo WPA3-Enterprise oferecendo criptografia opcional de 192 bits.

#### Sub-rede e CIDR

##### Visão geral da sub-rede

A sub-rede é o processo de pegar uma rede grande e dividi-la em vários grupos menores e organizados, chamados sub-redes. Pense nisso da seguinte forma: Se a rede de sua empresa é uma cidade grande, cada sub-rede é um bairro distinto dentro dessa cidade.

A sub-rede divide um intervalo de endereços de rede em sub-redes menores dentro da rede. Essas sub-redes organizadas são definidas pela combinação exclusiva do endereço IP e da máscara de sub-rede atribuída a cada dispositivo, criando efetivamente uma "rede dentro de uma rede" A sub-rede cria uma rede de dispositivos para funcionar como sua própria rede. Isso torna a rede mais eficiente e também pode ser usado para criar zonas de segurança. Se os dispositivos na mesma sub-rede se comunicam entre si, o interruptor altera as transmissões para que permaneçam na mesma sub-rede, melhorando a velocidade e a eficiência das comunicações.

![Duas sub-redes para duas redes conectadas a um roteador.](./public/img/sub_redes.png)

##### Notação de roteamento interdomínio sem classe para sub-rede

O CIDR (Classless Inter-Domain Routing, roteamento entre domínios sem classe) é um método de atribuição de máscaras de sub-rede a endereços IP para criar uma sub-rede. O endereçamento sem classe substitui o endereçamento com classe. O endereçamento classful foi usado na década de 1980 como um sistema de agrupamento de endereços IP em classes (Classe A a Classe E). Cada classe incluía um número limitado de endereços IP, que foram esgotados à medida que o número de dispositivos conectados à Internet ultrapassou o intervalo de classes na década de 1990. O endereçamento CIDR sem classes expandiu o número de endereços IPv4 disponíveis.

O CIDR permite que os profissionais de segurança cibernética segmentem as redes classful em pedaços menores. Os endereços IP CIDR são formatados como os endereços IPv4, mas incluem uma barra ("/") seguida de um número no final do endereço. Esse número extra é chamado de prefixo de rede IP. Por exemplo, um endereço IPv4 normal usa o formato 198.51.100.0, enquanto um endereço IP CIDR incluiria o prefixo de rede IP no final do endereço, 198.51.100.0/24. Esse endereço CIDR abrange todos os endereços IP entre 198.51.100.0 e 198.51.100.255. O sistema de endereçamento CIDR reduz o número de entradas nas tabelas de roteamento e fornece mais endereços IP disponíveis nas redes. Você pode tentar converter CIDR em endereços IPv4 e vice-versa por meio de uma ferramenta de conversão on-line, como o [IPAddressGuide](https://www.ipaddressguide.com/), para praticar e entender melhor esse conceito.

**Observação**: por enquanto, concentre-se em entender o conceito de CIDR como um método de endereçamento flexível usado para a sub-rede moderna. Um mergulho mais profundo na matemática técnica do CIDR é uma habilidade valiosa que você pode desenvolver em treinamentos futuros, se necessário.

##### Benefícios da sub-rede para a segurança

A sub-rede permite que os profissionais e analistas de rede criem uma rede dentro de sua própria rede sem solicitar outro endereço IP de rede ao provedor de acesso à Internet. Esse processo usa a largura de banda da rede com mais eficiência e melhora o desempenho da rede. A sub-rede é um componente da criação de sub-redes isoladas por meio de isolamento físico, configuração de roteamento e firewalls.

#### Redes virtuais e privacidade

##### Protocolos de rede comuns

Os protocolos de rede são usados para direcionar o tráfego para o dispositivo e o serviço corretos, dependendo do tipo de comunicação que está sendo realizada pelos dispositivos na rede. Os protocolos são as regras usadas por todos os dispositivos de rede que fornecem uma base mutuamente acordada sobre como transferir dados em uma rede.

Há três categorias principais de protocolos de rede: protocolos de comunicação, protocolos de gerenciamento e protocolos de segurança.

- Os protocolos de comunicação são usados para estabelecer conexões entre servidores. Os exemplos incluem TCP, UDP e SMTP (Protocolo de Transferência de Correio Simples), que fornece um framework para comunicação por e-mail.
- Os protocolos de gerenciamento são usados para solucionar problemas de rede. Um exemplo é o Protocolo de Mensagens de Controle da Internet (ICMP).
- Os protocolos de segurança fornecem criptografia de dados em trânsito. Os exemplos incluem IPsec e SSL/TLS.

Alguns outros protocolos comumente usados são:

- HyperText Transfer Protocol (HTTP). O HTTP é um protocolo de comunicação da camada do aplicativo. Ele permite que o navegador e o servidor da Web se comuniquem entre si.
- Sistema de Nomes de Domínio (DNS). O DNS é um protocolo da camada do aplicativo que traduz, ou mapeia, nomes de host para endereços IP.
- Protocolo de resolução de endereço (ARP). O ARP é um protocolo de comunicação da camada de rede que mapeia os endereços IP para máquinas físicas ou um endereço MAC reconhecido na rede local.

##### Wi-Fi

Esta seção do curso também apresentou vários protocolos de segurança sem fio, incluindo WEP, WPA, WPA2 e WPA3. O WPA3 criptografa o tráfego com o Padrão de Criptografia Avançada (AES) à medida que ele viaja do seu dispositivo para o ponto de acesso sem fio. O WPA2 e o WPA3 oferecem dois modos: pessoal e empresarial. O modo Personalização é mais adequado para redes domésticas, enquanto o modo Empresarial é geralmente utilizado para redes e aplicativos comerciais.

##### Ferramentas e práticas de segurança de rede

###### Firewalls

Anteriormente, você aprendeu que os firewalls são dispositivos de virtualização de rede (NVAs) ou dispositivos de hardware que inspecionam e podem filtrar o tráfego de rede antes que ele tenha permissão para entrar na rede privada. Os firewalls tradicionais são configurados com regras que informam quais tipos de pacotes de dados são permitidos com base no número da porta e no endereço IP do pacote de dados.

Há duas categorias principais de firewalls.

- Stateless: Uma classe de firewall que opera com base em regras predefinidas e não mantém o controle das informações dos pacotes de dados
- Stateful: Uma classe de firewall que controla as informações que passam por ele e filtra proativamente as ameaças. Ao contrário dos firewalls sem estado, que exigem que as regras sejam configuradas em duas direções, um firewall com estado só exige uma regra em uma direção. Isso ocorre porque ele usa uma "tabela de estado" para rastrear as conexões, de modo que possa corresponder o tráfego de retorno a uma sessão existente

Os firewalls de próxima geração (NGFWs) são a proteção de firewall mais avançada tecnologicamente. Eles excedem a segurança oferecida pelos firewalls com estado porque incluem inspeção profunda de pacotes (um tipo de interceptação de pacotes que examina os pacotes de dados e toma medidas se houver ameaças) e recursos de prevenção de intrusão que detectam ameaças à segurança e notificam os administradores do firewall. Os NGFWs podem inspecionar o Tráfego na camada do aplicativo do modelo TCP/IP e, em geral, são sensíveis ao aplicativo. Ao contrário dos firewalls tradicionais, que bloqueiam o tráfego com base no endereço IP e nas portas, as regras dos NGFWs podem ser configuradas para bloquear ou permitir o tráfego com base no aplicativo. Alguns NGFWs têm recursos adicionais, como Malware Sandboxing, Antivírus de Rede e Filtragem de URL e DNS.

###### Servidores proxy

Um servidor proxy é outra maneira de adicionar segurança à sua rede privada. Os servidores proxy utilizam a conversão de endereços de rede (NAT) para servir como uma barreira entre os clientes da rede e as ameaças externas. Os proxies avançados lidam com consultas de clientes internos quando eles acessam recursos externos à rede. Os proxies reversos funcionam de forma oposta aos proxies diretos; eles lidam com solicitações de sistemas externos para serviços na rede interna. Alguns servidores proxy também podem ser configurados com regras, como um firewall. Por exemplo, você pode criar filtros para bloquear sites identificados como contendo malware.

###### Redes privadas virtuais (VPN)

Uma VPN é um serviço que criptografa os dados em trânsito e disfarça seu endereço IP. As VPNs usam um processamento chamado Encapsulamento. O encapsulamento envolve seus dados não criptografados em um pacote de dados criptografado, o que permite que seus dados sejam enviados pela rede pública e permaneçam anônimos. As empresas e outras organizações usam VPNs para ajudar a proteger as comunicações dos dispositivos dos usuários com os recursos corporativos. Alguns desses recursos incluem servidores ou máquinas virtuais que hospedam aplicativos comerciais. As personalizações também usam VPNs para aumentar a privacidade pessoal. As VPNs protegem a privacidade do usuário ocultando informações pessoais, inclusive endereços IP, de servidores externos. Uma VPN de boa reputação também minimiza seu próprio acesso à atividade do usuário na Internet usando criptografia forte e outras medidas de segurança. As organizações estão usando cada vez mais uma combinação de recursos de VPN e SD-WAN para proteger suas redes. Uma rede de longa distância definida por software (SD-WAN) é um serviço de WAN virtual que permite que as organizações conectem com segurança os usuários a aplicativos em vários locais e em grandes distâncias geográficas.

#### Protocolos VPN: Wireguard e IPSec

##### Acesso remoto e VPNs site a site

Os usuários individuais usam VPNs de acesso remoto para estabelecer uma conexão entre um dispositivo pessoal e um servidor VPN. As VPNs de acesso remoto criptografam os dados enviados ou recebidos por meio de um dispositivo pessoal. A conexão entre o usuário e a VPN de acesso remoto é estabelecida pela Internet.

As empresas usam VPNs site a site principalmente para estender sua rede a outras redes e locais. Isso é particularmente útil para organizações que têm muitos escritórios em todo o mundo. O IPsec é comumente usado em VPNs site a site para criar um túnel criptografado entre a rede principal e a rede remota. Uma desvantagem das VPNs site a site é a complexidade de configuração e gerenciamento em comparação com as VPNs remotas.

##### VPN WireGuard vs. VPN IPsec

O WireGuard e o IPSec são dois protocolos de VPN diferentes usados para criptografar o tráfego em um túnel de rede seguro. A maioria dos provedores de VPN oferece uma variedade de opções de protocolos de VPN, como WireGuard ou IPsec. Em última análise, a escolha entre IPSec e WireGuard depende de muitos fatores, incluindo velocidades de conexão, Compatibilidade com a Infraestrutura de rede existente e necessidades comerciais ou individuais.

###### VPN WireGuard

O WireGuard é um protocolo VPN de alta velocidade, com criptografia avançada, para proteger os usuários quando estiverem acessando a Internet. Ele foi projetado para ser simples de configurar e manter. O WireGuard pode ser usado tanto para conexão site a site quanto para conexões cliente-servidor. O WireGuard é relativamente mais novo que o IPsec e é usado por muitas pessoas devido ao fato de que sua velocidade de download é aprimorada pelo uso de menos linhas de código. O WireGuard também é um código aberto, o que facilita a implantação e a depuração pelos usuários. Esse protocolo é útil para processos que exigem velocidades de download mais rápidas, como streaming de conteúdo de vídeo ou download de arquivos grandes.

###### VPN IPSec

O IPSec é outro protocolo de VPN que pode ser usado para configurar VPNs. A maioria dos provedores de VPN usa o IPSec para criptografar e autenticar pacotes de dados a fim de estabelecer conexões seguras e criptografadas. Como o IPSec é um dos primeiros protocolos de VPN, muitos sistemas operacionais suportam o IPSec dos provedores de VPN.

Embora o IPSec e o WireGuard sejam ambos protocolos VPN, o IPSec é mais antigo e mais complexo que o WireGuard. Alguns clientes podem preferir o IPSec devido ao seu histórico de uso mais longo, testes de segurança extensivos e adoção generalizada. Entretanto, outros podem preferir o WireGuard devido ao seu potencial de melhor desempenho e configuração mais simples.

### Modulo 3: Segurança contra invasores de rede

#### Como as invasões comprometem seu sistema

##### Ataques de interceptação de rede

Os ataques de interceptação de rede funcionam interceptando o tráfego de rede e roubando informações valiosas ou interferindo na transmissão de alguma forma.

Os agentes mal-intencionados podem usar ferramentas de hardware ou software para capturar e inspecionar dados em trânsito. Isso é chamado de **interceptação de pacotes**. Além de ver informações às quais não têm direito, os agentes mal-intencionados também podem interceptar o tráfego de rede e alterá-lo. Esses ataques podem causar danos a uma organização. Esses ataques podem causar danos à rede de uma organização inserindo modificações de código malicioso ou alterando a mensagem e interrompendo as operações da rede. Por exemplo, um invasor pode interceptar uma transferência bancária e alterar a conta que recebe os fundos para uma que o invasor controla.

Mais adiante neste curso, você aprenderá mais sobre interceptação maliciosa de pacotes e outros tipos de ataques de interceptação de rede: ataques on-path e ataques de repetição.

##### Ataques de backdoor

Um **ataque backdoor** é outro tipo de ataque do qual você precisa estar ciente como analista de segurança. Uma organização pode ter várias medidas de segurança em vigor, incluindo câmeras, verificações biométricas e códigos de acesso, para garantir que os funcionários não entrem e saiam sem serem vistos. No entanto, um funcionário pode contornar as medidas de segurança encontrando uma porta dos fundos do edifício que não seja tão fortemente monitorada, o que lhe permite sair sorrateiramente à tarde sem ser visto.

Em segurança cibernética, backdoors são pontos fracos deixados intencionalmente por programadores ou administradores de sistemas e redes que contornam os mecanismos normais de controle de acesso. As backdoors têm o objetivo de ajudar os programadores a realizar a solução de problemas ou tarefas administrativas. No entanto, as backdoors também podem ser instaladas por invasores depois que eles comprometem uma organização para garantir que tenham acesso persistente.

Depois que o hacker entra em uma rede insegura por meio de um backdoor, ele pode causar grandes danos: instalar malware, realizar um ataque de negação de serviço (DoS), roubar informações privadas ou alterar outras configurações de segurança que deixam o sistema vulnerável a outros ataques. Um ataque **DoS** é um ataque que tem como alvo uma rede ou um servidor e o inunda com tráfego de rede.

##### Possíveis impactos em uma organização

Como você já aprendeu, os ataques à rede podem ter um impacto negativo significativo em uma organização. Vamos examinar algumas possíveis consequências.

- **Financeiras**: Quando um sistema é colocado off-line com um ataque DoS ou outra tática, ele impede que a empresa realize tarefas que geram receita. Dependendo do tamanho da organização, as operações interrompidas podem custar milhões de dólares. Os custos de reparação para reconstruir a infraestrutura de software e pagar grandes somas associadas a um possível ransomware podem ser financeiramente difíceis. Além disso, se um agente mal-intencionado obtiver acesso às informações pessoais dos clientes ou consumidores da empresa, a empresa poderá enfrentar pesados custos de litígio e liquidação se os clientes recorrerem à justiça.

- **Reputação**: Os ataques também podem ter um impacto negativo sobre a reputação de uma organização. Se for de conhecimento público que uma empresa sofreu um ataque cibernético, o público poderá ficar preocupado com as práticas de segurança da organização. Ele pode deixar de confiar suas informações pessoais à empresa e escolher um concorrente para atender às suas necessidades.

- **Segurança pública**: Se ocorrer um ataque em uma rede governamental, isso pode afetar a segurança e o bem-estar dos cidadãos de um país. Nos últimos anos, as agências de defesa de todo o mundo estão investindo pesadamente no combate às táticas de guerra cibernética. Se um agente mal-intencionado obtivesse acesso a uma rede de poder, a um sistema público de água ou até mesmo a um sistema de comunicação de defesa militar, o público poderia sofrer danos físicos devido a um ataque de intrusão de rede.

#### Ler os registros do tcpdump

Um **analisador de protocolo de rede**, às vezes chamado de sniffer de pacotes ou analisador de pacotes, é uma ferramenta projetada para a captura e a análise do pacote de dados em uma rede. Eles são comumente usados como ferramentas de investigação para monitorar redes e identificar atividades suspeitas. Há uma grande variedade de analisadores de protocolos de rede disponíveis, mas alguns dos analisadores mais comuns incluem:

- Analisador de Tráfego SolarWinds NetFlow
- ManageEngine OpManager
- Observador de rede do Azure
- Wireshark
- tcpdump

Esta leitura se concentrará exclusivamente no tcpdump, embora você possa aplicar o que aprendeu aqui a muitos dos outros analisadores de protocolo de rede que usará como analista de segurança cibernética para se defender contra qualquer invasão de rede. Em uma próxima atividade, você analisará um registro de tráfego de dados do tcpdump e identificará um ataque DoS para praticar essas habilidades. 

##### tcpdump

O **tcpdump** é um analisador de protocolo de rede de linha de comando. Ele é popular, leve - o que significa que usa pouco espaço e tem baixo uso da memória - e usa a biblioteca libpcap de código aberto. O tcpdump é baseado em texto, o que significa que todos os comandos do tcpdump são executados no terminal. Ele também pode ser instalado em outros sistemas operacionais baseados em Unix, como o macOS®. Ele vem pré-instalado em muitas distribuições Linux.

O tcpdump fornece uma breve análise de pacotes e converte as principais informações sobre o Tráfego de rede em formatos facilmente lidos por humanos. Ele imprime informações sobre cada pacote diretamente em seu terminal. O tcpdump também exibe o endereço IP de origem, os endereços IP de destino e os números de porta que estão sendo usados nas comunicações. 

##### Interpretação da saída

O tcpdump imprime a saída do comando como interceptação de pacotes na linha de comando e, opcionalmente, em um arquivo de log, depois que um comando é executado. A saída de uma captura de pacote contém muitas informações importantes sobre o Tráfego de rede.

![Tipos de informações apresentadas em uma captura de pacote do tcpdump.](./public/img/tcpdump.png)

Algumas informações que você recebe de uma captura de pacote incluem:

- Registro de data e hora: A saída começa com o registro de data e hora, formatado como horas, minutos, segundos e frações de segundo.
- IPS de origem: a origem do pacote é fornecida por seu endereço IP de origem.
- Porta de origem: Esse número de porta é o local de origem do pacote.
- IP de destino: o endereço IP de destino é o local para onde o pacote está sendo transmitido.
- Porta de destino: Esse número de porta é o local para onde o pacote está sendo transmitido.

Observação: por padrão, o tcpdump tentará resolver os endereços de host para nomes de host. Ele também substituirá os números de porta por serviços comumente associados que usam essas portas.

##### Usos comuns

O tcpdump e outros analisadores de protocolo de rede são comumente usados para capturar e visualizar comunicações de rede e para coletar estatísticas sobre a rede, como na solução de problemas de desempenho da rede. Eles também podem ser usados para:

- Estabelecer uma Linha de Base para padrões de tráfego de rede e Métricas de utilização de rede.
- Detectar e identificar tráfego malicioso
- Criar alertas personalizados para enviar as notificações certas quando surgirem problemas de rede ou ameaças à segurança.
- Localizar mensagens instantâneas (IM), tráfego ou pontos de acesso sem fio não autorizados.

No entanto, os atacantes também podem usar os analisadores de protocolo de rede de forma maliciosa para obter informações sobre uma rede específica. Por exemplo, os atacantes podem capturar pacotes de dados que contenham informações confidenciais, como nomes de usuário e senhas de contas. AS como analista de segurança cibernética, é importante entender a finalidade e os usos dos analisadores de protocolo de rede.

#### Ataque DDoS na vida real

##### Um DDoS direcionado a um servidor DNS amplamente utilizado

Nos vídeos anteriores, você aprendeu sobre a Função de um servidor DNS. AS, os servidores DNS traduzem os nomes de domínio do site para o endereço IP do sistema que contém as informações do site. Por exemplo, se um usuário digitar o URL de um site, um servidor DNS o traduzirá em um endereço IP numérico que direciona o tráfego de rede para o local do servidor do site.

No dia do ataque DDoS que estamos estudando, muitas grandes empresas estavam usando um provedor de serviços de DNS. O provedor de serviços estava hospedando o sistema DNS para essas empresas. Isso significava que, quando os usuários da Internet digitavam a URL do site que queriam acessar, seus dispositivos eram direcionados para o lugar certo. Em 21 de outubro de 2016, o provedor de serviços foi vítima de um ataque DDoS.

##### Lead antes do ataque

Antes do ataque ao provedor de serviços, um grupo de estudantes universitários criou um **botnet** com a intenção de atacar vários servidores e redes de computadores de jogos. Um botnet é uma coleção de computadores infectados por malware que estão sob o Controle de um único agente de ameaça, conhecido como "bot-herder" Cada computador da botnet pode ser controlado remotamente para enviar um pacote de dados a um sistema-alvo. Em um ataque de botnet, os criminosos cibernéticos instruem todos os bots da botnet a enviar pacotes de dados para o sistema-alvo ao mesmo tempo, resultando em um ataque DDoS.

O grupo de estudantes universitários publicou o código da botnet on-line para que fosse Acessível a milhares de usuários da Internet e para que as Autoridades não pudessem rastrear a botnet até os estudantes. Ao fazer isso, eles possibilitaram que outros agentes mal-intencionados aprendessem o código da botnet e a controlassem remotamente. Isso incluiu os criminosos cibernéticos que atacaram o provedor de serviços DNS.

##### O dia do ataque

Às 7h da manhã do dia do ataque, o botnet enviou dezenas de milhões de solicitações de DNS ao provedor de serviços. Isso sobrecarregou o sistema e o serviço de DNS foi desligado. Isso significava que todos os sites que usavam o provedor de serviços não podiam ser acessados. Quando os usuários tentavam acessar vários sites que usavam o provedor de serviços, eles não eram direcionados para o site digitado no navegador. As interrupções de cada serviço da Web ocorreram em toda a América do Norte e Europa.

Os sistemas do provedor de serviços foram restaurados após apenas duas horas de inatividade. Embora os criminosos cibernéticos tenham enviado ondas subsequentes de ataques de botnet, a empresa de DNS estava preparada e conseguiu atenuar o impacto. 

#### Visão geral das táticas de interceptação

##### Uma análise mais detalhada da interceptação de pacotes

Se você aprendeu em um vídeo anterior, o **sniffing de pacotes** é a prática de captura e interceptação de pacotes de dados em uma rede. Em uma rede privada, os pacotes de dados são direcionados para o dispositivo de destino correspondente na rede.

A **Placa de interface de rede (NIC)** do dispositivo é uma peça de hardware que conecta o dispositivo a uma rede. A NIC lê a transmissão de dados e, se ela contiver o endereço MAC do dispositivo, aceita o pacote e o envia ao dispositivo para processar as informações com base no protocolo. Isso ocorre em todas as operações de rede padrão. Entretanto, uma NIC pode ser configurada para o modo promíscuo, o que significa que ela aceita todo o Tráfego na rede, mesmo os pacotes que não são endereçados ao dispositivo da NIC. Você aprenderá mais sobre as NICs mais adiante no programa. Agentes mal-intencionados podem usar softwares como o Wireshark para capturar os dados em uma rede privada e armazená-los para uso posterior. Em seguida, eles podem usar as informações pessoais em seu próprio benefício. Como alternativa, eles podem usar os endereços IP e MAC de usuários autorizados da rede privada para realizar o spoofing de IP.

##### Uma análise mais detalhada do spoofing de IPS

Depois que um agente mal-intencionado intercepta pacotes na rede, ele pode se passar por endereços IP e MAC de dispositivos autorizados para realizar um ataque de spoofing de IP. Os firewalls podem evitar ataques de spoofing de IP configurando-os para recusar pacotes IP não autorizados e tráfego suspeito. A seguir, você examinará alguns ataques comuns de spoofing de IP com os quais é importante estar familiarizado como analista de segurança.

###### Ataque no caminho

Um **ataque on-path** ocorre quando um hacker intercepta a comunicação entre dois dispositivos ou servidores que têm uma relação de confiança. A transmissão entre esses dois dispositivos de rede confiáveis pode conter informações valiosas, como nomes de usuário e senhas, que o agente mal-intencionado pode coletar. Um ataque no caminho às vezes é chamado de ataque man-in-the-middle porque o hacker está escondido no meio da comunicação entre duas partes confiáveis.

Ou pode ser que a transmissão interceptada contenha uma consulta ao sistema DNS. Você deve se lembrar de um vídeo anterior que um servidor DNS traduz nomes de domínio de sites em endereços IP. Se um agente mal-intencionado interceptar uma transmissão que contenha uma pesquisa de DNS, ele poderá spoofing a resposta de DNS do servidor e redirecionar um nome de domínio para um endereço IP diferente, talvez um que contenha código mal-intencionado ou outras ameaças. A maneira mais importante de se proteger contra um ataque no caminho é criptografar seus dados em trânsito, por exemplo, usando TLS. 

###### Ataque smurf

Um **ataque smurf** é um ataque de rede realizado quando um invasor descobre o endereço IP de um usuário autorizado e o inunda com pacotes. Quando o pacote spoofing atinge o endereço de transmissão, ele é enviado a todos os dispositivos e servidores da rede.

Em um ataque smurf, o spoofing de IP é combinado com outra técnica de negação de serviço (DoS) para inundar a rede com tráfego indesejado. Por exemplo, o pacote spoofing pode incluir um ping do Protocolo de Mensagens de Controle da Internet (ICMP). Como você aprendeu anteriormente, o ICMP é usado para solucionar problemas em uma rede. Mas se muitas mensagens ICMP forem transmitidas, as respostas de eco ICMP sobrecarregarão os servidores da rede e eles serão desligados. Isso cria uma negação de serviço e pode interromper as operações de uma organização.

Uma maneira importante de se proteger contra um ataque smurf é usar um firewall avançado que possa monitorar qualquer tráfego incomum na rede. A maioria dos firewalls de próxima geração (NGFW) inclui recursos que detectam anomalias na rede para garantir que as transmissões de tamanho excessivo sejam detectadas antes que tenham a chance de derrubar a rede.

###### Ataque DoS

Como você aprendeu, depois que o agente mal-intencionado fareja o Tráfego de rede, ele pode se passar por um usuário autorizado. Um **ataque de negação de serviço** é uma classe de ataques em que o invasor impede que o sistema comprometido realize atividades legítimas ou responda ao tráfego legítimo. No entanto, diferentemente do spoofing de IP, o ataque não receberá uma resposta do host visado. Tudo no pacote de dados é autorizado, inclusive o endereço IP no Cabeçalho do pacote. Nos ataques de spoofing de IP, o agente mal-intencionado usa pacotes IP que contêm endereços IP falsos. Os atacantes continuam enviando pacotes IP com endereços IP falsos até que o servidor da rede seja bloqueado.

**Dica profissional:** Lembre-se do princípio da defesa em profundidade. Não há uma estratégia perfeita para impedir cada tipo de ataque. Você pode criar camadas de defesa usando várias Estratégias. Nesse caso, o uso da criptografia padrão do setor fortalecerá sua segurança e o ajudará a se defender de ataques DoS em mais de um nível.

### Modulo 4:

#### Ataques de força bruta e proteção do sistema operacional

##### Ataques de força bruta

Um ataque de força bruta é um processamento de tentativa e erro para descobrir informações privadas. Há diferentes tipos de ataques de força bruta que os agentes mal-intencionados usam para adivinhar senhas, incluindo:

- Ataques de força bruta simples. Quando os atacantes tentam adivinhar as credenciais de login de um usuário, isso é considerado um ataque de força bruta simples. Eles podem fazer isso inserindo qualquer combinação de nomes de usuário e senhas que possam imaginar até encontrar uma que funcione.
- Os dictionary attacks usam uma técnica semelhante. Nos dictionary attacks, os atacantes usam uma lista de senhas comumente usadas e credenciais roubadas de violações anteriores para acessar um sistema. Esses ataques são chamados de ataques de "dicionário" porque os atacantes originalmente usavam uma lista de palavras do dicionário para adivinhar as senhas, antes que as regras de senhas complexas se tornassem uma prática de segurança comum.

O uso de força bruta para acessar um sistema pode ser um processo tedioso e demorado, especialmente quando é feito manualmente. Há uma série de ferramentas que os invasores usam para realizar seus ataques. 

##### Avaliação de vulnerabilidades

Antes de ocorrer um ataque de força bruta ou outro incidente de segurança cibernética, as empresas podem executar uma série de testes em sua rede ou aplicativos da Web para avaliar as vulnerabilidades. Os analistas podem usar máquinas virtuais e Sandboxes para testar arquivos suspeitos, verificar vulnerabilidades antes da ocorrência de um evento ou simular um incidente de segurança cibernética.

###### Máquinas virtuais (VMs)

As **máquinas virtuais (VMs)** são versões em software de computadores físicos. As VMs fornecem uma camada adicional de segurança para uma organização porque podem ser usadas para executar códigos em um ambiente isolado, impedindo que códigos maliciosos afetem o restante do computador ou do sistema. As VMs também podem ser excluídas e substituídas por uma imagem original após o teste de malware.

As VMs são úteis na investigação de máquinas potencialmente infectadas ou na execução de malware em um ambiente restrito. O uso de uma VM pode evitar danos ao seu sistema caso as ferramentas sejam usadas de forma inadequada. As VMs também oferecem a possibilidade de reverter para um estado anterior. No entanto, ainda há alguns Riscos envolvidos com as VMs. Ainda há um pequeno risco de que um programa mal-intencionado possa escapar da virtualização e acessar a máquina virtual.

É possível testar e explorar aplicativos facilmente com as VMs, e é fácil alternar entre diferentes VMs em seu computador. Isso também pode ajudar a simplificar muitas tarefas de segurança.

###### Ambientes Sandbox

Um sandbox é um tipo de ambiente de teste que permite a execução de software ou programas separados da sua rede. Elas são comumente usadas para testar patches, identificar e resolver Erros ou detectar vulnerabilidades de segurança cibernética. As Sandboxes também podem ser usadas para avaliar softwares suspeitos, avaliar arquivos com códigos maliciosos e simular cenários de ataque.

As sandboxes podem ser computadores físicos autônomos que não estão conectados a uma rede; no entanto, muitas vezes é mais demorado e econômico usar software ou máquinas virtuais baseadas em nuvem como ambientes de sandbox. Observe que alguns autores de malware sabem como escrever códigos para detectar se o malware é executado em um ambiente de VM ou sandbox. Os atacantes podem programar seu malware para se comportar como um software inofensivo quando executado dentro desses tipos de ambientes de teste. 

##### Medidas de prevenção

Algumas medidas comuns que as organizações usam para evitar a ocorrência de ataques de força bruta e ataques semelhantes incluem:

- Salting e hashing: o hashing converte informações em um valor Único que pode ser usado para determinar sua integridade. É uma função unidirecional, o que significa que é impossível descriptografar e obter o texto original. A salga adiciona caracteres aleatórios às senhas com hash. Isso aumenta o comprimento e a complexidade dos valores de hash, tornando-os mais seguros.
- Autenticação multifator (MFA) e autenticação de dois fatores (2FA): A MFA é uma medida de segurança que exige que o usuário verifique sua identidade de duas ou mais maneiras para acessar um sistema ou uma rede. Essa verificação ocorre usando uma combinação de fatores de autenticação: nome de usuário e senha, impressões digitais, reconhecimento facial ou uma senha única (OTP) enviada para um número de telefone ou e-mail. a 2FA é semelhante à MFA, exceto pelo fato de usar apenas duas formas de verificação.
- CAPTCHAe reCAPTCHA: CAPTCHA significa Completely Automated Public Turing test to tell Computers and Humans Apart (teste de Turing público totalmente automatizado para diferenciar computadores e humanos). Ele solicita que os usuários concluam um teste simples que prova que eles são humanos. O reCAPTCHA é um serviço CAPTCHA gratuito do Google que ajuda a proteger os sites contra bots e softwares mal-intencionados.
- Políticas de senha: As organizações usam políticas de senha para padronizar boas práticas de senha em toda a empresa. As políticas podem incluir diretrizes sobre a complexidade de uma senha, a frequência com que os usuários precisam atualizar as senhas, se as senhas podem ser reutilizadas ou não e se há limites para o número de vezes que um usuário pode tentar fazer o registro antes que sua conta seja suspensa.

#### Aplicativos de segurança de rede

Esta seção do curso aborda o tópico de hardening e monitoramento de rede. Cada dispositivo, ferramenta ou estratégia de segurança implementada pelos analistas de segurança protege ainda mais - ou hardening - a rede até que o proprietário da rede esteja satisfeito com o nível de segurança. Essa abordagem de adicionar camadas de segurança a uma rede é chamada de defesa em profundidade.

Nesta leitura, você aprenderá sobre a função de quatro dispositivos usados para proteger uma rede: firewalls, sistemas de detecção de intrusão, sistemas de prevenção de intrusão e ferramentas de gerenciamento de eventos e informações de segurança. Os profissionais de segurança de rede têm a opção de usar qualquer um ou todos esses dispositivos e ferramentas, dependendo do nível de segurança que desejam alcançar. 

Esta leitura discutirá os benefícios da segurança em camadas. Cada ferramenta mencionada é uma camada adicional de defesa que pode incrementar o hardening de uma rede, começando com o nível mínimo de segurança (fornecido apenas por um firewall) até o nível mais alto de segurança (fornecido pela combinação de um firewall, um dispositivo de detecção e prevenção de intrusões e monitoramento de eventos de segurança). 

![Uma imagem que mostra as diferenças entre um firewall, IPS e IDS.](./public/img/CS_R-055_Firewall-IDS-and-IPS.png)

Observe onde cada ferramenta está localizada na rede. Cada ferramenta tem seu próprio lugar na arquitetura da rede. Os analistas de segurança devem compreender as topologias de rede mostradas nos diagramas ao longo desta leitura.

##### Firewall

Até agora, neste curso, você aprendeu sobre firewalls sem estado, firewalls com estado e firewalls de próxima geração (NGFWs) e as vantagens de segurança de cada um deles.

A maioria dos firewalls é semelhante em suas funções básicas. Os firewalls permitem ou bloqueiam o tráfego com base em um conjunto de regras. À medida que os pacotes de dados entram em uma rede, o cabeçalho do pacote é inspecionado e permitido ou negado com base em seu número de porta. Os NGFWs também são capazes de inspecionar as cargas úteis dos pacotes. Cada sistema deve ter seu próprio firewall, independentemente do firewall da rede.

![Um firewall circulado por traços, protegendo a rede interna do tráfego da Internet que entra pelo modo.](./public/img/CS_R-055_Firewall.png)

##### Sistema de detecção de intrusão (IDS) 

Um **Sistema de detecção de intrusão (IDS)** é um aplicativo que monitora a atividade do sistema e alerta sobre possíveis intrusões. Um IDS alerta os administradores com base na assinatura do tráfego malicioso.

O IDS é configurado para detectar ataques conhecidos. Os sistemas IDS geralmente detectam pacotes de dados à medida que eles se deslocam pela rede e os analisam quanto às características de ataques conhecidos. Alguns sistemas IDS analisam não apenas as assinaturas de ataques conhecidos, mas também as anomalias que podem ser um sinal de atividade mal-intencionada. Quando o IDS descobre uma anomalia, ele envia um alerta ao administrador da rede, que pode investigar mais a fundo.

As limitações dos sistemas IDS são que eles só podem fazer a varredura de ataques conhecidos ou de anomalias óbvias. Ataques novos e sofisticados podem não ser detectados. A outra limitação é que o IDS não interrompe de fato o tráfego de entrada se detectar algo errado. Cabe ao administrador da rede detectar a atividade mal-intencionada antes que ela cause algum dano à rede.

![Um IDS circulado acima de uma imagem de uma troca de rede, que fica entre um firewall e a rede.](./public/img/CS_R-055_IDS.png)

Quando combinado com um firewall, um IDS acrescenta outra camada de defesa. O IDS é colocado atrás do firewall e antes de entrar na LAN, o que permite que o IDS analise os fluxos de dados depois que o tráfego de rede não permitido pelo firewall tiver sido filtrado. Isso é feito para reduzir o ruído nos alertas do IDS, também chamados de falsos positivos.

##### Sistema de prevenção de intrusão (IPS)

Um sistema de prevenção de intrusão (IPS) é um aplicativo que monitora a atividade do sistema em busca de atividades intrusivas e toma medidas para interromper a atividade. Ele oferece ainda mais proteção do que um IDS porque interrompe ativamente as anomalias quando elas são detectadas, ao contrário do IDS que simplesmente relata a anomalia a um administrador de rede.

Um IPS procura assinaturas de ataques conhecidos e anomalias de dados. Um IPS informa a anomalia aos analistas de segurança e bloqueia um remetente específico ou descarta pacotes de rede que pareçam suspeitos.

![Um IPS está situado entre um firewall e a rede interna.](./public/img/CS_R-055_IPS.png)

O IPS (como um IDS) fica atrás do firewall na arquitetura de rede. Isso oferece um alto nível de segurança porque os fluxos de dados arriscados são interrompidos antes mesmo de chegarem às partes sensíveis da rede. No entanto, uma possível limitação é o fato de ele estar em linha: Se ele quebrar, a conexão entre a rede privada e a Internet será interrompida. Outra limitação do IPS é a possibilidade de Falso positivo, que pode resultar na perda de tráfego legítimo.

##### Dispositivos de captura total de pacotes

Os dispositivos de captura total de pacotes podem ser incrivelmente úteis para administradores de rede e profissionais de segurança. Esses dispositivos permitem registrar e analisar todos os dados que são transmitidos pela rede. Eles também ajudam na investigação de alertas criados por um IDS. 

##### Gerenciamento de eventos e informações de segurança 

Um **sistema de gerenciamento de eventos e informações de segurança (SIEM)** é um aplicativo que coleta e analisa dados de registro para monitorar atividades críticas em uma organização. As ferramentas SIEM funcionam em tempo real para relatar atividades suspeitas em um painel de controle centralizado. Além disso, as ferramentas SIEM analisam os dados de registro de rede provenientes de IDSs, IPSs, firewalls, VPNs, proxies e registros DNS. As ferramentas SIEM são uma forma de agregar dados de eventos de segurança para que todos apareçam em um único local para análise dos analistas de segurança. Isso é chamado de painel único de controle. 

Abaixo, você pode ver um exemplo de um painel da ferramenta SIEM do Google Cloud, o Chronicle. **O Chronicle** é uma ferramenta nativa da nuvem projetada para reter, analisar e pesquisar dados.

![Imagem do painel de controle do Chronicle](./public/img/CS_R-055_Chronicle.png)

O **Splunk** é outra ferramenta SIEM comum. A Splunk oferece diferentes opções de ferramentas SIEM: Splunk Enterprise e Splunk Cloud. Ambas as opções incluem painéis detalhados que ajudam os profissionais de segurança a revisar e analisar os dados de uma organização. Há também outras ferramentas SIEM semelhantes disponíveis, e é importante que os profissionais de segurança pesquisem as diferentes ferramentas para determinar qual delas é mais benéfica para a organização.

Uma ferramenta SIEM não substitui a experiência dos analistas de segurança nem as atividades de hardening de rede e sistema abordadas neste curso, mas é usada em combinação com outros métodos de segurança. Os analistas de segurança geralmente trabalham em um Centro de operações de segurança (SOC), onde podem monitorar a atividade na rede. Em seguida, eles podem usar seus conhecimentos e experiência para determinar como responder às informações do painel e decidir quando os eventos atendem aos critérios para serem escalados para a supervisão.

#### Segurança na nuvem

##### Considerações sobre a segurança na nuvem

Muitas organizações optam por usar serviços em nuvem devido à facilidade de implantação, à velocidade de implantação, às Economias de custo e à escalabilidade dessas opções. A computação em nuvem apresenta desafios de segurança exclusivos dos quais os analistas de segurança cibernética precisam estar cientes.

###### Gerenciamento de acesso à identidade

O **Gerenciamento de identidade e acesso (IAM)** é um conjunto de processos e tecnologias que ajuda as organizações a gerenciar identidades digitais em seu ambiente. Esse serviço também autoriza como os usuários podem usar diferentes recursos da nuvem. Um problema comum que as organizações enfrentam ao usar a nuvem é a configuração inadequada das funções de usuário na nuvem. Uma função de usuário configurada incorretamente aumenta o risco ao permitir que usuários não autorizados tenham acesso a operações críticas na nuvem.

###### Configuração

O ecossistema de nuvem em expansão introduz uma complexidade significativa no gerenciamento da rede. Cada serviço em nuvem precisa de uma configuração precisa para manter os padrões de segurança e conformidade. Esse desafio se intensifica durante as migrações para a nuvem, em que é fundamental garantir uma configuração precisa para cada processo migrado. A negligência nessa área pode expor a rede a vulnerabilidades. Os serviços em nuvem mal configurados são uma fonte frequente de violações de segurança, o que ressalta a importância da atenção meticulosa aos detalhes por parte dos administradores e arquitetos de rede durante a migração e o gerenciamento contínuo dos serviços em nuvem.

###### Superfície de ataque

Os provedores de serviços de nuvem (CSPs) oferecem vários aplicativos e serviços para as organizações a um baixo custo.

Cada serviço ou aplicativo em uma rede tem seu próprio conjunto de riscos e vulnerabilidades e aumenta a superfície geral de ataque de uma organização. Uma superfície de ataque maior deve ser compensada com medidas de segurança maiores.

As redes em nuvem que utilizam muitos serviços introduzem muitos pontos de entrada na rede de uma organização. No entanto, se a rede for projetada corretamente, a utilização de vários serviços não introduzirá mais pontos de entrada no projeto de rede de uma organização. Esses pontos de entrada podem ser usados para introduzir malware na rede e apresentar outras vulnerabilidades de segurança. É importante observar que os CSPs costumam recorrer a opções mais seguras e foram submetidos a um exame mais minucioso do que uma rede tradicional no local.

###### Ataques de dia zero

Os ataques de dia zero são uma importante consideração de segurança para as organizações que usam soluções de rede na nuvem ou tradicionais no local. Um ataque de dia zero é uma exploração que era desconhecida anteriormente. É mais provável que os CSPs saibam da ocorrência de um ataque de dia zero antes que uma organização de TI tradicional saiba. Os CSPs têm maneiras de corrigir hipervisores e migrar cargas de trabalho para outras máquinas virtuais. Esses métodos garantem que os clientes não sejam afetados pelo ataque. Há também várias ferramentas disponíveis para aplicação de patches no nível do sistema operacional que as organizações podem usar.

###### Visibilidade e rastreamento

Os administradores de rede têm acesso a todos os pacotes de dados que cruzam a rede, tanto nas redes locais quanto na nuvem. Eles podem farejar e inspecionar pacotes de dados para saber mais sobre o desempenho da rede ou para verificar possíveis ameaças e ataques.

Esse tipo de visibilidade também é oferecido na nuvem por meio de registros de fluxo e ferramentas, como o espelhamento de pacotes. Os CSPs assumem a responsabilidade pela segurança na nuvem, mas não permitem que as organizações que usam sua infraestrutura monitorem o tráfego nos servidores do CSP. Muitos CSPs oferecem medidas de segurança robustas para proteger sua infraestrutura. Ainda assim, essa situação pode ser uma preocupação para as organizações que estão acostumadas a ter acesso total à sua rede e às suas operações. Os CSPs pagam por auditorias de terceiros para verificar o grau de segurança de uma rede em nuvem e identificar possíveis vulnerabilidades. As auditorias podem ajudar as organizações a identificar se alguma vulnerabilidade tem origem na infraestrutura local e se há algum lapso de conformidade por parte do CSP. 

###### As coisas mudam rapidamente na nuvem

Os CSPs são grandes organizações que trabalham arduamente para se manterem atualizados com os avanços tecnológicos. Para as organizações que estão acostumadas a ter o controle de todos os ajustes feitos em sua rede, isso pode ser um desafio potencial a ser acompanhado. As atualizações dos serviços na nuvem podem afetar as considerações de segurança das organizações que os utilizam. Por exemplo, as configurações de conexão talvez precisem ser alteradas com base nas atualizações do CSP.

As organizações que usam CSPs geralmente precisam atualizar seus processos de TI. É possível que as organizações continuem seguindo as práticas recomendadas estabelecidas para mudanças, configurações e outras considerações de segurança. No entanto, talvez seja necessário que a organização adote uma abordagem diferente, de modo a se alinhar às alterações feitas pelo CSP.

A rede em nuvem oferece várias opções que podem parecer atraentes para uma empresa de pequeno porte - opções que ela nunca poderia construir em suas próprias instalações. No entanto, é importante considerar que cada serviço acrescenta complexidade ao perfil de segurança da organização, e ela precisará de uma equipe de segurança para monitorar todos os serviços na nuvem.

##### Modelo de responsabilidade compartilhada

Um princípio de Segurança na nuvem comumente aceito é o **modelo de responsabilidade compartilhada**. O modelo de responsabilidade compartilhada afirma que o CSP deve assumir a responsabilidade pela segurança que envolve a infraestrutura de nuvem, inclusive centros de dados físicos, hipervisores e sistemas operacionais de host. A empresa que usa o serviço de nuvem é responsável pelos ativos e processos que armazena ou opera na nuvem.

O modelo de responsabilidade compartilhada garante que tanto o CSP quanto os usuários concordem sobre onde começa e termina a responsabilidade pela segurança. Um problema ocorre quando as organizações presumem que o CSP está cuidando da segurança pela qual elas não se responsabilizaram. Um exemplo disso são os aplicativos e as configurações de nuvem. O CSP assume a responsabilidade de proteger a nuvem, mas é responsabilidade da organização garantir que os serviços sejam configurados adequadamente de acordo com os requisitos de segurança da organização.

#### Criptografia e segurança na nuvem

##### Fortalecimento da segurança na nuvem

Há várias técnicas e ferramentas que podem ser usadas para proteger a infraestrutura e os recursos da rede de nuvem. Algumas técnicas comuns de reforço da segurança na nuvem incluem a incorporação de IAM, hipervisores, Linha de base, criptografia e apagamento criptográfico.

###### Gerenciamento de acesso à identidade (IAM)

O **Gerenciamento de identidade e acesso (IAM)** é um conjunto de processos e tecnologias que ajuda as organizações a gerenciar identidades digitais em seu ambiente. Esse serviço também autoriza como os usuários podem aproveitar os diferentes recursos da Nuvem.

###### Hipervisores

Um hipervisor faz a abstração entre o hardware do host e o ambiente do software operacional. Há dois tipos de hipervisores. Os hipervisores do tipo um são executados no hardware do computador host. Um exemplo de hipervisor do tipo um é o ESXi da VMware®. Os hipervisores do tipo dois operam no software do computador host. Um exemplo de hipervisor do tipo dois é o VirtualBox. Os provedores de serviços em Nuvem (CSPs) geralmente usam hipervisores do tipo um. Os CSPs são responsáveis pelo Gerenciamento do hipervisor e de outros componentes de virtualização. O CSP garante que os recursos e os ambientes de Nuvem estejam disponíveis e fornece patches e atualizações regulares. Vulnerabilidades em hipervisores ou configurações incorretas podem levar a fugas de máquinas virtuais (VM escapes). Uma fuga de VM é um exploit em que um agente mal-intencionado obtém acesso ao hipervisor principal, potencialmente ao computador host e a outras VMs. Como cliente de um CSP, você raramente lidará com hipervisores diretamente.

###### Linha de base

A Linha de base para redes de computadores e operações em nuvem abrange como o ambiente de nuvem é configurado e definido. Uma Linha de base é um ponto de referência fixo. Esse ponto de referência pode ser usado para comparar as mudanças feitas em um ambiente de nuvem. A configuração e a instalação adequadas podem melhorar muito a segurança e o desempenho de um ambiente de nuvem. Exemplos de estabelecimento de uma Linha de Base em um ambiente de nuvem incluem: restringir o acesso ao portal de administração do ambiente de nuvem, habilitar o gerenciamento de senhas, habilitar a criptografia de arquivos e habilitar serviços de detecção de ameaças para bancos de dados SQL.

##### Criptografia na Nuvem

A criptografia pode ser aplicada para proteger os dados que são processados e armazenados em um ambiente de nuvem. A criptografia usa criptografia e sistemas seguros de gerenciamento de chaves para fornecer integridade e confidencialidade dos dados. A criptografia de dados é uma das principais maneiras de proteger dados e informações confidenciais na nuvem.

A criptografia é o processamento de informações embaralhadas em Texto criptografado, que não pode ser lido por ninguém sem a chave de criptografia. A criptografia se originou principalmente da codificação manual de mensagens e informações usando um algoritmo para converter qualquer letra ou número em um novo valor. A criptografia moderna se baseia no sigilo de uma chave, em vez do sigilo de um algoritmo. A criptografia é uma ferramenta importante que ajuda a proteger as redes de nuvem e os dados em repouso para evitar o acesso não autorizado. Você aprenderá mais sobre criptografia em detalhes em um próximo curso.

##### Eliminação criptográfica

A eliminação criptográfica é um método de apagar a chave de criptografia dos dados criptografados. Ao destruir dados na Nuvem, os métodos mais tradicionais de destruição de dados não são tão eficazes. A destruição criptográfica é uma técnica mais recente em que as chaves criptográficas usadas para a descriptografia dos dados são destruídas. Isso torna os dados indecifráveis e impede que qualquer pessoa os descriptografe. Ao fazer a criptografia, todas as cópias da chave precisam ser destruídas para que ninguém tenha a oportunidade de acessar os dados no futuro.

##### Gerenciamento de chaves

A criptografia moderna depende de manter as chaves de criptografia seguras. Veja abaixo as medidas que podem ser tomadas para proteger ainda mais seus dados ao usar aplicativos em Nuvem:

- Módulo de plataforma confiável (TPM). O TPM é um chip de computador que pode armazenar com segurança senhas, certificados e chaves de criptografia.
- Módulo de segurança de hardware na nuvem (CloudHSM). O CloudHSM é um dispositivo de computador que fornece armazenamento seguro para chaves criptográficas e processa operações criptográficas, como criptografia e descriptografia.

As organizações e os clientes não têm acesso direto ao provedor de serviços em nuvem (CSP), mas podem solicitar auditorias e relatórios de segurança entrando em contato com o CSP. Normalmente, os clientes não têm acesso às chaves de criptografia específicas que os CSPs usam para criptografar os dados dos clientes. No entanto, quase todos os CSPs permitem que os clientes forneçam suas próprias chaves de criptografia, dependendo do serviço que o cliente está acessando. Por sua vez, o cliente é responsável por suas chaves de criptografia e por garantir que as chaves permaneçam confidenciais. O CSP está limitado em como pode ajudar o cliente se as chaves do cliente forem comprometidas ou destruídas. Uma das principais vantagens do modelo de responsabilidade compartilhada é que o cliente não é totalmente responsável pela manutenção da infraestrutura criptográfica. As organizações podem avaliar e monitorar o risco envolvido ao permitir que o CSP gerencie a infraestrutura, analisando a auditoria e os controles de segurança do CSP. Para os contratados federais, o FEDRAMP fornece uma lista de CSPs verificados.