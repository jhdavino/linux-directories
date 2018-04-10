# Entendendo a estrutura de diretórios do Linux


Sistema de arquivos do Ubuntu Linux
## O diretório raiz (/)
Todos os arquivos e diretórios do sistema Linux instalado no computador partem de uma única origem: o diretório raiz. Mesmo que estejam armazenados em outros dispositivos físicos, é a partir do diretório raiz – representado pela barra (/) – que você poderá acessá-los.

Também vale lembrar que o único usuário do sistema capaz de criar ou mover arquivos do diretório raiz é o root, ou seja, o usuário-administrador. Isso evita que usuários comuns cometam erros e acabem comprometendo a integridade de todo o sistema de arquivos.

## Binários executáveis: /bin
No diretório /bin estão localizados os binários executáveis que podem ser utilizados por qualquer usuário do sistema. São comandos essenciais, usados para trabalhar com arquivos, textos e alguns recursos básicos de rede, como o cp, mv, ping e grep. Se você ainda não conhece esses comandos, não se preocupe: falaremos sobre eles em um artigo futuro, aqui no Canaltech.

## Binários do sistema: /sbin
Assim como o /bin, este diretório armazena executáveis, mas com um diferencial: são aplicativos utilizados por administradores de sistema com o propósito de realizar funções de manutenção e outras tarefas semelhantes. Entre os comandos disponíveis estão o ifconfig, para configurar e controlar interfaces de rede TCP/IP, e o fdisk, que permite particionar discos rígidos, por exemplo.

## Programas diversos: /usr
Se você não encontrar um comando no diretório /bin ou /sbin, ele certamente está aqui. O /usr reúne executáveis, bibliotecas e até documentação de softwares usados pelos usuários ou administradores do sistema. Além disso, sempre que você compilar e instalar um programa a partir do código-fonte, ele será instalado nesse diretório.

## Configurações do sistema: /etc
No diretório /etc ficam arquivos de configuração que podem ser usados por todos os softwares, além de scripts especiais para iniciar ou interromper módulos e programas diversos. É no /etc que se encontra, por exemplo, o arquivo resolv.conf, com uma relação de servidores DNS que podem ser acessados pelo sistema, com os parâmetros necessários para isso.

## Bibliotecas: /lib
Neste ponto do sistema de arquivos ficam localizadas as bibliotecas usadas pelos comandos presentes em /bin e /sbin. Normalmente, os arquivos de bibliotecas começam com os prefixos ld ou lib e possuem "extensão" so.

## Opcionais: /opt
Aplicativos adicionais, que não são essenciais para o sistema, terminam neste diretório.

## Aquivos pessoais: /home
No diretório /home ficam os arquivos pessoais, como documentos e fotografias, sempre dentro de pastas que levam o nome de cada usuário. Vale notar que o diretório pessoal do administrador não fica no mesmo local, e sim em /root.

## Inicialização: /boot
Arquivos relacionados à inicialização do sistema, ou seja, o processo de boot do Linux, quando o computador é ligado, ficam em /boot.

## Volumes e mídias: /mnt e /media
Para acessar os arquivos de um CD, pendrive ou disco rígido presente em outra máquina da rede, é necessário "montar" esse conteúdo no sistema de arquivos local, isso é, torná-lo acessível como se fosse apenas mais um diretório no sistema.

Em /media ficam montadas todas as mídias removíveis, como dispositivos USB e DVDs de dados. Já o diretório /mnt fica reservado aos administradores que precisam montar temporariamente um sistema de arquivos externo.

## Serviços: /srv
Dados de servidores e serviços em execução no computador ficam armazenados dentro desse diretório.

## Arquivos de dispositivos: /dev
No Linux, tudo é apresentado na forma de arquivos. Ao plugar um pendrive no computador, por exemplo, um arquivo será criado dentro do diretório /dev e ele servirá como interface para acessar ou gerenciar o drive USB. Nesse diretório, você encontra caminhos semelhantes para acessar terminais e qualquer dispositivo conectado ao computador, como o mouse e até modems.

## Arquivos variáveis: /var
Todo arquivo que aumenta de tamanho ao longo do tempo está no diretório de arquivos variáveis. Um bom exemplo são os logs do sistema, ou seja, registros em forma de texto de atividades realizadas no Linux, como os logins feitos ao longo dos meses.

## Processos do sistema: /proc
Lembra da história de que tudo funciona como um arquivo no Linux? Pois o /proc é a prova disso. Nesse diretório são encontrados arquivos que revelam informações sobre os recursos e processos em execução no sistema. Quer um exemplo? Para saber há quanto tempo o Linux está sendo usado desde a última vez em que foi iniciado, basta ler o arquivo /proc/uptime.

## Arquivos temporários: /tmp
Arquivos e diretórios criados temporariamente tanto pelo sistema quanto pelos usuários devem ficar nesse diretório. Boa parte deles é apagada sempre que o computador é reiniciado.
