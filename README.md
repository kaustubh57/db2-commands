# DB2 commands

- create schema [SCHEMA_NAME] authorization <inst_user>
- drop schema [SCHEMA_NAME] restrict


# Liquibase commands
liquibase --changeLogFile='xd-service/src/main/resources/migrations.xml' --username='xd' --password='xdpw' --url='jdbc:db2://localhost:50000/mojodb' --defaultSchemaName='xd2' --driver='com.ibm.db2.jcc.DB2Driver' --classpath='/Users/kkibm/.m2/repository/com/ibm/db2/jcc/db2jcc4/4.16.53/db2jcc4-4.16.53.jar' update

liquibase --changeLogFile='xd-files-service/src/main/resources/migrations.xml' --username='xd' --password='xdpw' --url='jdbc:db2://localhost:50000/mojodb' --defaultSchemaName='xd2' --driver='com.ibm.db2.jcc.DB2Driver' --classpath='/Users/kkibm/.m2/repository/com/ibm/db2/jcc/db2jcc4/4.16.53/db2jcc4-4.16.53.jar' update