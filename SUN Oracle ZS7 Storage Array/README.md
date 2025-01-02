# Sun Oracle ZS7 Appliance Storage
Este template foi criado a partir das MIBs disponibilizadas no appliance, segundo Doc ID 1593846.1. 

# Instalação
1. Confirme que o serviço SNMP está ativo e configurado no Storage Array ZS7 
2. Importe o template xml no Zabbix
3. Configure o host no Zabbix com interface SNMP

# Macros

* {$POOL.DISK.AVAI.CRIT} - Percentagem do espaço no pool disponivel para ser considerado como critico
* {$POOL.DISK.AVAI.WARN} - Percentagem do espaço no pool disponivel para ser considerado como atenção
* {$SNMP_COMMUNITY} - Community SNMP

# Objetos Suportados
* Harware Monitoring
  * Chassi State
  * Disk State
  * Cluster State
  * Module Status
  * Problem Identification
* Pools & RAID Groups
  * Discovery
  * Capacity/Utilization