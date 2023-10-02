#!/bin/bash
#Script hecho para ver el dominio de una pagina web y de ahi extraer informacion de ello
#Usarlo con fines legales
#colors
RED="$(printf '\033[31m')"  GREEN="$(printf '\033[32m')"  ORANGE="$(printf '\033[33m')"  BLUE="$(printf '\033[34m')"
MAGENTA="$(printf '\033[35m')"  CYAN="$(printf '\033[36m')"  WHITE="$(printf '\033[37m')" BLACK="$(printf '\033[30m')"
REDBG="$(printf '\033[41m')"  GREENBG="$(printf '\033[42m')"  ORANGEBG="$(printf '\033[43m')"  BLUEBG="$(printf '\033[44m')"
MAGENTABG="$(printf '\033[45m')"  CYANBG="$(printf '\033[46m')"  WHITEBG="$(printf '\033[47m')" BLACKBG="$(printf '\033[40m')"
RESETBG="$(printf '\e[0m\n')"



lookup() {

nslookup ${domainweb}

}

who-is() {

whois ${website}
}
repeat() {
cat <<- EOF

${CYAN}    ____                  _____           _       __ 
${CYAN}   / __ \____  _____     / ___/__________(_)___  / /_
${CYAN}  / / / / __ \/ ___/_____\__ \/ ___/ ___/ / __ \/ __/
${CYAN} / /_/ / / / (__  )_____/__/ / /__/ /  / / /_/ / /_  
${CYAN}/_____/_/ /_/____/     /____/\___/_/  /_/ .___/\__/  
${CYAN}                                       /_/           
${MAGENTA}                                   (By:KevinVarSa)
${MAGENTA}                                   (Gh:Krypton-Hacks)


${CYAN}Ingrese una Opcion
1:Extraer IP de una Pagina Web
2:Extraer Informacion confidencial de una Pagina Web o IP
3:Salir

EOF

read -p "<<<<<---: "

        case ${REPLY} in

        1|uno) echo "Ingresa la pagina web para extraer su Dominio";read -p "Domain: " domainweb
                    echo -n "      Buscando Dominio de ${domainweb}..."
                   for i in {0..100}; do
                sleep 0.1  # Simula un proceso en curso
                   echo -ne "\r[$i%]"
                   done
                  sleep 2
                  clear
                   echo ""
                    lookup
                 echo -e  ""
              echo -e "\nDominio encontrado"
                     ;;
        2|dos) echo "Ingrese la IP o la ruta web para extraer la informacion";read -p "Web: " website
                     echo -n "      Hackeando informacion de ${website}..."
                   for i in {0..100}; do
                sleep 0.1  # Simula un proceso en curso
                   echo -ne "\r[$i%]"
                   done
                  sleep 2
                  clear
                   echo ""
                    who-is
                 echo -e  ""
              echo -e "\nHackeo completo"
                          ;;
        3|tres) exit 11
           ;;
         *) echo " Opcion incorrecta. Intente nuevamente..."
           sleep 1.5
           clear
           repeat
          ;;
        esac
}
repeat






