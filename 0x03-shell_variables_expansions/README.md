0. <o> obligatorio
Cree un script que cree un alias.

Nombre: ls
Valor: rm *
julien@ubuntu:/tmp/0x03$ ls
0-alias  file1  file2
julien@ubuntu:/tmp/0x03$ source ./0-alias 
julien@ubuntu:/tmp/0x03$ ls
julien@ubuntu:/tmp/0x03$ \ls
julien@ubuntu:/tmp/0x03$ 
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 0-alias

1. Hola, obligatorio
Cree un script que imprima hello user, donde user es el usuario actual de Linux.

julien@ubuntu:/tmp/0x03$ id
uid=1000(julien) gid=1000(julien) groups=1000(julien),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),113(lpadmin),128(sambashare)
julien@ubuntu:/tmp/0x03$ ./1-hello_you 
hello julien
julien@ubuntu:/tmp/0x03$ 
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 1-hello_you

2. El camino hacia el éxito es tomar una acción masiva y decidida obligatoria
Añadir /actiona la PATH. /actiondebe ser el último directorio en el que mira el shell cuando busca un programa.

julien@ubuntu:/tmp/0x03$ echo $PATH
/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
julien@ubuntu:/tmp/0x03$ source ./2-path 
julien@ubuntu:/tmp/0x03$ echo $PATH
/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/action
julien@ubuntu:/tmp/0x03$ 
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 2-path

3. Si el camino es hermoso, no preguntemos a dónde conduce obligatorio
Cree un script que cuente la cantidad de directorios en el PATH.

julien@ubuntu:/tmp/0x03$ echo $PATH
/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
julien@ubuntu:/tmp/0x03$ . ./3-paths 
11
julien@ubuntu:/tmp/0x03$ PATH=/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:::::/hello
julien@ubuntu:/tmp/0x03$ . ./3-paths 
12
julien@ubuntu:/tmp/0x03$ 
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 3-paths

4. Variables globales obligatorias
Cree un script que enumere las variables de entorno.

julien@ubuntu:/tmp/0x03$ source ./4-global_variables
CC=gcc
CDPATH=.:~:/usr/local:/usr:/
CFLAGS=-O2 -fomit-frame-pointer
COLORTERM=gnome-terminal
CXXFLAGS=-O2 -fomit-frame-pointer
DISPLAY=:0
DOMAIN=hq.garrels.be
e=
TOR=vi
FCEDIT=vi
FIGNORE=.o:~
G_BROKEN_FILENAMES=1
GDK_USE_XFT=1
GDMSESSION=Default
GNOME_DESKTOP_SESSION_ID=Default
GTK_RC_FILES=/etc/gtk/gtkrc:/nethome/franky/.gtkrc-1.2-gnome2
GWMCOLOR=darkgreen
GWMTERM=xterm
HISTFILESIZE=5000
history_control=ignoredups
HISTSIZE=2000
HOME=/nethome/franky
HOSTNAME=octarine.hq.garrels.be
INPUTRC=/etc/inputrc
IRCNAME=franky
JAVA_HOME=/usr/java/j2sdk1.4.0
LANG=en_US
LDFLAGS=-s
LD_LIBRARY_PATH=/usr/lib/mozilla:/usr/lib/mozilla/plugins
LESSCHARSET=latin1
LESS=-edfMQ
LESSOPEN=|/usr/bin/lesspipe.sh %s
LEX=flex
LOCAL_MACHINE=octarine
LOGNAME=franky
[...]
julien@ubuntu:/tmp/0x03$ 
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 4-global_variables

5. Variables locales obligatorias
Cree un script que enumere todas las variables locales y variables de entorno, y funciones.

julien@ubuntu:/tmp/0x03$ . ./5-local_variables
BASH=/bin/bash
BASHOPTS=checkwinsize:cmdhist:complete_fullquote:expand_aliases:extglob:extquote:force_fignore:histappend:interactive_comments:progcomp:promptvars:sourcepath
BASH_ALIASES=()
BASH_ARGC=()
BASH_ARGV=()
BASH_CMDS=()
BASH_COMPLETION_COMPAT_DIR=/etc/bash_completion.d
BASH_LINENO=()
BASH_REMATCH=()
BASH_SOURCE=()
BASH_VERSINFO=([0]="4" [1]="3" [2]="46" [3]="1" [4]="release" [5]="x86_64-pc-linux-gnu")
BASH_VERSION='4.3.46(1)-release'
CLUTTER_IM_MODULE=xim
COLUMNS=133
COMPIZ_CONFIG_PROFILE=ubuntu
COMP_WORDBREAKS=$' \t\n"\'><=;|&(:'
DBUS_SESSION_BUS_ADDRESS=unix:abstract=/tmp/dbus-Fg27Lr20bq
DEFAULTS_PATH=/usr/share/gconf/ubuntu.default.path
DESKTOP_SESSION=ubuntu
[...]
julien@ubuntu:/tmp/0x03$ 
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 5-local_variables

6. Variable local obligatoria
Cree un script que cree una nueva variable local.

Nombre: BETTY
Valor: Holberton
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 6-create_local_variable

7. Variable global obligatoria
Cree un script que cree una nueva variable global.

Nombre: HOLBERTON
Valor: Betty
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 7-create_global_variable

8. Toda adición al conocimiento verdadero es una adición al poder humano obligatorio.
Escriba un script que imprima el resultado de la adición de 128 con el valor almacenado en la variable de entorno TRUEKNOWLEDGE, seguido de una nueva línea.

julien@production-503e7013:~$ export TRUEKNOWLEDGE=1209
julien@production-503e7013:~$ ./8-true_knowledge | cat -e
1337$
julien@production-503e7013:~$
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 8-true_knowledge

9. Divide y gobierna obligatorio
Escriba un guión que imprima el resultado de POWERdividido por DIVIDE, seguido de una nueva línea.

POWERy DIVIDEson variables de entorno
julien@production-503e7013:~$ export POWER=42784
julien@production-503e7013:~$ export DIVIDE=32
julien@production-503e7013:~$ ./9-divide_and_rule | cat -e
1337$
julien@production-503e7013:~$
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 9-divide_and_rule

10. El amor es anterior a la vida, posterior a la muerte, inicial de la creación, y el exponente de la respiración es obligatorio.
Escriba un guión que muestre el resultado de BREATHal poderLOVE

BREATHy LOVEson variables de entorno
El script debe mostrar el resultado, seguido de una nueva línea.
julien@production-503e7013:~/$ export BREATH=4
julien@production-503e7013:~/$ export LOVE=3
julien@production-503e7013:~/$ ./10-love_exponent_breath
64
julien@production-503e7013:~/$
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 10-love_exponent_breath

11. Hay 10 tipos de personas en el mundo - Los que entienden binario y los que no lo hacen obligatoria
Escriba un script que convierta un número de la base 2 a la base 10.

El número en la base 2 se almacena en la variable de entorno BINARY
El script debe mostrar el número en la base 10, seguido de una nueva línea.
julien@production-503e7013:~/$ export BINARY=10100111001
julien@production-503e7013:~/$ ./11-binary_to_decimal
1337
julien@production-503e7013:~/$
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 11-binary_to_decimal

12. Combinación obligatoria
Cree un script que imprima todas las combinaciones posibles de dos letras, excepto oo.

Las letras son minúsculas, desde ahastaz
Una combinación por línea
La salida debe ser alfa ordenada, comenzando con aa
No imprimir oo
Su archivo de script debe contener un máximo de 64 caracteres.
julien@ubuntu:/tmp/0x03$ echo $((26 ** 2 -1))
675
julien@ubuntu:/tmp/0x03$ ./12-combinations | wc -l
675
julien@ubuntu:/tmp/0x03$ 
julien@ubuntu:/tmp/0x03$ ./12-combinations | tail -303 | head -10
oi
oj
ok
ol
om
on
op
oq
or
os
julien@ubuntu:/tmp/0x03$ 
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 12-combinations

13. Flotadores obligatorios
Escribe un guión que imprima un número con dos decimales.

El número se almacenará en la variable de entorno NUM.

ubuntu@ip-172-31-63-244:~/0x03$ export NUM=0
ubuntu@ip-172-31-63-244:~/0x03$ ./13-print_float
0.00
ubuntu@ip-172-31-63-244:~/0x03$ export NUM=98
ubuntu@ip-172-31-63-244:~/0x03$ ./13-print_float
98.00
ubuntu@ip-172-31-63-244:~/0x03$ export NUM=3.14159265359
ubuntu@ip-172-31-63-244:~/0x03$ ./13-print_float
3.14
ubuntu@ip-172-31-63-244:~/0x03$
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 13-print_float

14. Decimal a hexadecimal obligatorio
Escriba un script que convierta un número de la base 10 a la base 16.

El número en la base 10 se almacena en la variable de entorno DECIMAL
El script debe mostrar el número en la base 16, seguido de una nueva línea.
julien@production-503e7013:~/$ export DECIMAL=16
julien@production-503e7013:~/$ ./14-decimal_to_hexadecimal
10
julien@production-503e7013:~/$ export DECIMAL=1337
julien@production-503e7013:~/$ ./14-decimal_to_hexadecimal | cat -e
539$
julien@production-503e7013:~/$ export DECIMAL=15
julien@production-503e7013:~/$ ./14-decimal_to_hexadecimal | cat -e
f$
julien@production-503e7013:~/$
Repo:

Repositorio de GitHub: holberton-system_engineering-devops
Directorio: 0x03-shell_variables_expansions
Expediente: 14-decimal_to_hexadecimal

15. ¿Qué sucede cuando escribe ls * .c obligatorio?
Escribe una publicación de blog que describa paso a paso lo que sucede cuando escribes ls *.cy presionas Enter en tu shell. Intenta explicar cada paso que conozcas y da ejemplos. Un principiante total debe entender lo que ha escrito.

Tener al menos una foto, en la parte superior de la publicación del blog.
Publique su publicación de blog en Medium o LinkedIn
Comparte tu publicación de blog al menos en LinkedIn
Escribe de manera profesional e inteligible
Recuerde que estos blogs deben estar escritos en inglés para mejorar su capacidad técnica en una variedad de entornos.
Recuerde, los futuros empleadores verán sus artículos; tómelo en serio y produzca algo que sea un activo para su futuro

Cuando termine, agregue todas las URL a continuación (publicación de blog, publicación de LinkedIn, etc.)

Agregue URL aquí:

Repo:

Repositorio de GitHub: holberton-system_engineering-devops

16. ¿Cuál es la diferencia entre un enlace duro y un enlace simbólico? obligatorio
Escriba una publicación de blog que explique qué son los enlaces duros y simbólicos en Linux, cómo crearlos y cuál es la diferencia entre ambos. Use ejemplos para ilustrar.

Tener al menos una foto, en la parte superior de la publicación del blog.
Publique su publicación de blog en Medium o LinkedIn
Comparte tu publicación de blog al menos en LinkedIn
Cuando termine, agregue todas las URL a continuación (publicación de blog, publicación de LinkedIn, etc.)

Recuerde que estos blogs deben estar escritos en inglés para mejorar su capacidad técnica en una variedad de entornos.

Agregue URL aquí:

Repo:

Repositorio de GitHub: holberton-system_engineering-devops