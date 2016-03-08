# Agents

Les agents sont les process chargés de collecter les logs sur les serveurs.

FileBeat a volontairement été exclu car il est jeune, et pas présent en standard sur Linux.
C'est en effet un critère important au niveau des exploitants de ne pas impacter les serveurs déjà en production. Rsyslog étant installé en standard dans bon nombre de distributions, c'est un choix naturel ici.

