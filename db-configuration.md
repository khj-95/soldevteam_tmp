# DB CONFIGURATION

type: VENDER(ORACLE, MYSQL, MSSQL, POSTGRE, TIBERO, MARIA, DB2)

driver-class-name: net.sf.log4jdbc.sql.jdbcapi.DriverSpy

url: jdbc:log4jdbc:oracle:thin:@${db.config.ip}:${db.config.port}:${db.config.database-name}

url: jdbc:log4jdbc:mysql://${db.config.ip}:${db.config.port}/${db.config.database-name}

url: jdbc:log4jdbc:sqlserver://${db.config.ip}:${db.config.port};SelectMethod=cursor;DatabaseName=${db.config.database-name};encrypt=false;trustServerCertificate=false;

url: jdbc:log4jdbc:postgresql://${db.config.ip}:${db.config.port}/${db.config.database-name}

url: jdbc:log4jdbc:tibero:thin:@${db.config.ip}:${db.config.port}:${db.config.database-name}

url: jdbc:log4jdbc:mariadb://${db.config.ip}:${db.config.port}/${db.config.database-name}?useUnicode=true\&noAccessToProcedureBodies=true

url: jdbc:log4jdbc:db2://${db.config.ip}:${db.config.port}/${db.config.database-name}

table-space: TABLE-SPACE-NAME

table-index-space: TABLE-INDEX-SPACE-NAME
