# ReportISW2-ModuloSWTesting
## Compilazione ed esecuione dei test per il progetto Bookkeeper

Esecuzione dei test e generazione dei report di JaCoCo:
'''bash
mvn clean verify
'''

Esecuzione dei test e generazione dei report di ba-dua:
'''bash
mvn clean verify -Dba-dua-dir=/path/to/ba-dua-master/ba-dua-agent-rt/target -P data-flow-test
'''
Il report di ba-dua viene generato nella directory '''./bookkeeper-server/'''


Esecuzione del mutation test:
'''bash
mvn clean verify -P pit-test
'''
Il report di pit viene generato nella directory '''./bookkeeper-server/target/'''

## Compilazione ed esecuione dei test per il progetto OpenJPA

Esecuzione dei test e generazione dei report di JaCoCo:
'''bash
mvn clean verify
'''

Esecuzione dei test e generazione dei report di ba-dua:
'''bash
mvn clean verify -Dba-dua-dir=/path/to/ba-dua-master/ba-dua-agent-rt/target -P data-flow-test
'''
Il report di ba-dua viene generato nella directory '''./openjpa-kernel/'''


Esecuzione del mutation test:
'''bash
mvn clean verify -P pit-test
'''
Il report di pit viene generato nella directory '''./openjpa-kernel/target/'''
