# Agents

Les agents sont les process charg�s de collecter les logs sur les serveurs.

FileBeat a volontairement �t� exclu car il est jeune, et pas pr�sent en standard sur Linux.
C'est en effet un crit�re important au niveau des exploitants de ne pas impacter les serveurs d�j� en production. Rsyslog �tant install� en standard dans bon nombre de distributions, c'est un choix naturel ici.

