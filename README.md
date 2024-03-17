# RCfunctions

## Funmction to expand and sort unique everything
nmap -sL -n -iL $1 | awk '/Nmap scan report/{print $NF}' | sort | sort -u | tee $1.-sorted 
