# Prokka
Este GitHub es para instalar prokka
## Instalación
Primer paso: instalar dependencias
$ sudo apt-get update

$ sudo apt-get upgrade

$ sudo apt-get install bedtools ncbi-blast+ mcl cd-hit mafft prank fasttree parallel

$ sudo perl -MCPAN -e shell

En este momento se abre un programa en terminal, y se debe anotar la siguiente sentencia:

> install Array::Utils Bio::Perl Exception::Class File::Basename File::Copy File::Find::Rule File::Grep File::Path File::Slurper File::Spec File::Temp File::Which FindBin Getopt::Long Graph Graph::Writer::Dot List::Util Log::Log4perl Moose Moose::Role Text::CSV PerlIO::utf8_strict Devel::OverloadInfo Digest::MD5::File

Para sair de este programa apretar "q"

## Instalar Roady
Descargar del siguiente link: (https://github.com/sanger-pathogens/Roary/tarball/master) 
luego ingresar a la carpeta descargas e instalar
$ cd Downloads

$ tar xvzf sanger-pathogens-Roary-xxxx.tar.gz

$ cd sanger-pathogens-Roary-db

$ ./install_dependencies.sh

chequear si esta bien instalado
$ roary -w
Si aparece que no esta instalado ingresar la sugerencia del terminal que es
$ sudo apt install roady
Si ve vuelve a intentar el chequeo, tira un error de que falta un paquete que se instalara a continuacion:

$ sudo apt-get install libdatetime-perl libxml-simple-perl libdigest-md5-perl git default-jre bioperl

$ sudo cpan Bio::Perl

$ git clone https://github.com/tseemann/prokka.git $HOME/prokka

$ $HOME/prokka/bin/prokka --setupdb

ahora ya estaría todo OK **Nota: el prokka se instalará con el guion anterior, eso quiere decir que cada vez que se llame a prokka se tiene que llamar de esta forma: $ $HOME/prokka/bin/prokka **

#correr archivo prokka
