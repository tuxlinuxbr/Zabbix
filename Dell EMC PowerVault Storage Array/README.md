# Dell EMC PowerVault Storage Array
Este template foi criado a partir das MIBs disponibilizadas sitio da Dell na área de Downloads (Dell ME Series Storage Array MIB).

Obs: 

Conforme indicado em https://www.dell.com/support/kbdoc/en-us/000219988/powervault-me5-information-about-snmp-support-and-mibs-location, as MIBs snmp disponíveis somente permitem acesso a management interfaces, environmental monitoring, uptime, and array health status.

# Instalação
1. Confirme que o serviço SNMP está ativo e configurado no Storage PowerVault
2. Importe o template xml no Zabbix
3. Configure o host no Zabbix com interface SNMP

# Macros

* {$SNMP_COMMUNITY} - Community SNMP

# Objetos Suportados
* Harware Monitoring
  * Chassi State
  * Network Interface State
  * Overall State
  * Sensor Check
  * Problem Identification
