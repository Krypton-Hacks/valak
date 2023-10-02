#!/bin/bash
# Creado y desarrollado por: Kevin Varsa (Krypton)
# Libre de modificaciones de codigo
# Uso de herramienta para fines legales
# Herramienta para informacion de una Linea de chip
# Sirve para Ingenieria Social
# Uso legal de un script de información de teléfono
# Este script está diseñado para ser utilizado de manera legal y ética.
# Su propósito principal es permitir a los usuarios acceder a información básica sobre un número de teléfono específico.
# Puede ser útil para identificar la ubicación geográfica, el operador de telefonía y otra información general asociada con el número.
# Se debe utilizar de acuerdo con las leyes y regulaciones de protección de datos y privacidad aplicables en tu jurisdicción.
# Es importante obtener el consentimiento adecuado del propietario del número de teléfono antes de utilizar este script.
# El uso inapropiado, ilegal o no ético de este script está estrictamente prohibido y puede tener consecuencias legales.
# El desarrollador Krypton no se responsabiliza del mal uso de esta herramienta
red="\e[1;31m"
green="\e[1;92m"
#Repeticion
repeat() {
#Banner
echo -e ${green} "" 
echo "------------------------------------------------"
echo "    __ __            ____  __                   "
echo "   / //_/_______  __/ __ \/ /_  ____  ____  ___ "
echo "  / ,<  / ___/ / / / /_/ / __ \/ __ \/ __ \/ _ \""
echo " / /| |/ /  / /_/ / ____/ / / / /_/ / / / /  __/"
echo "/_/ |_/_/   \__, /_/   /_/ /_/\____/_/ /_/\___/ "
echo "           /____/                               "
echo "                          (Creador:KevinVarsa)  "
echo "                          (GitHub:Krypton-Hacks)"
echo "                          (Instagram:varsa.tkd) " 
echo "------------------------------------------------"
echo -e ${green} "Seleccione una opcion"
echo ""
# Menu de Opciones
opcion=("1:Instalar_Requisitos" "2:Info_de_linea" "3:Salir")
for i in ${opcion[@]};do
echo $i
sleep 0.3
done
echo ""
read -p "opcion: " op
case $op in
[1-2-3])
# ESCOGIENDO SISTEMA OPERATIVO
if [ $op -eq 1 ];then
enigma() {
echo ""
echo "Ingrese su Sistema"
echo ""
sistema=("1:Kali-Linux" "2:Termux")
for s in ${sistema[@]};do
echo "$s";sleep 0.3
done
echo ""
read -p "sistema: " system
# Instalacion de Requisitos
case $system in
1)  echo "Instalando requisitos"
apt update -y
apt install nodejs -y
apt install npm -y
npm i -g install  truecallerjs -y
truecallerjs login
;;
2) echo "Instalando requsitos"
pkg update -y
apt update -y
apt install nodejs -y
pkg install nodejs -y
apt install npm -y
npm i -g install truecallerjs -y
truecallerjs login
;;
*)echo -e ${red} ""
 echo "Sistema incorrecto"
sleep 1
clear
enigma
;;
esac
}
enigma
# Opcion para el Hackeo
elif [ $op -eq 2 ];then
echo ""
echo -e ${green} "Ingrese el numero de telefono para hackear"
echo ""
read -p "Numero de la victima (Ej:+59175817266): " numero
echo "|------------------------------------------------|"
echo "| [+] Buscando Linea...                          | "
sleep 5
echo "| [+] Linea de telefono encontrada               | "
sleep 2
echo "| [+] Hackeando informacion de la Victima...     | "
echo "|------------------------------------------------|"
sleep 2
truecallerjs -s $numero --text
echo ""
echo -e ${red} "Hackeo completo!!!"
elif [ $op -eq 3 ];then
echo "Saliendo"
sleep 1.3
exit
fi
;;
*)echo -e ${red} ""
 echo "Opcion Incorrecta"
sleep 1
clear
repeat
;;
esac
}
repeat
