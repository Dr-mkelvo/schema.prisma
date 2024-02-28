$ bunx prisma generate

STEP 2:
$ bunx prisma db push 


ERROR
###############
Environment variables loaded from .env
Prisma schema loaded from prisma/schema.prisma
Datasource "db": MySQL database "sql6687185" at "sql6.freemysqlhosting.net:3306"
Error: Unknown column 'datetime_precision' in 'field list'
   0: sql_schema_connector::flavour::mysql::connection::describe_schema
             at schema-engine/connectors/sql-schema-connector/src/flavour/mysql/connection.rs:34
   1: schema_core::commands::schema_push::Calculate `from`
             at schema-engine/core/src/commands/schema_push.rs:29
   2: schema_core::state::SchemaPush
             at schema-engine/core/src/state.rs:433

##############
while :
DATABASE_URL="mysql://sql6687185:Y5YuHw529x@sql6.freemysqlhosting.net:3306/sql6687185"
PROD_DATABASE_URL="mysql://sql6687185:Y5YuHw529x@sql6.freemysqlhosting.net:3306/sql6687185"
LOCAL_DATABASE_URL="mysql://sql6687185:Y5YuHw529x@localhost:3306/sql6687185"



STEP 2:
$ bunx prisma db push 


ERROR
###############

Environment variables loaded from .env
Prisma schema loaded from prisma/schema.prisma
Datasource "db": MySQL database "defaultdb" at "mysql-33dafe04-takeoffokwemba-8d33.a.aivencloud.com:19093"
Error: Unable to create or change a table without a primary key, when the system variable 'sql_require_primary_key' is set. Add a primary key to the table or unset this variable to avoid this message. Note that tables without a primary key can cause performance problems in row-based replication, so please consult your DBA before changing this setting.
   0: sql_schema_connector::apply_migration::migration_step
           with step=CreateTable { table_id: TableId(23) }
             at schema-engine/connectors/sql-schema-connector/src/apply_migration.rs:21
   1: sql_schema_connector::apply_migration::apply_migration
             at schema-engine/connectors/sql-schema-connector/src/apply_migration.rs:10
   2: schema_core::state::SchemaPush
             at schema-engine/core/src/state.rs:433


#####################
while:
    DATABASE_URL="mysql://avnadmin:AVNS_ij8Y_tzefS4f0OMwJbM@mysql-33dafe04-takeoffokwemba-8d33.a.aivencloud.com:19093/defaultdb?ssl-mode=REQUIRED"
    PROD_DATABASE_URL="mysql://avnadmin:AVNS_ij8Y_tzefS4f0OMwJbM@mysql-33dafe04-takeoffokwemba-8d33.a.aivencloud.com:19093/defaultdb?ssl-mode=REQUIRED"
    LOCAL_DATABASE_URL="mysql://avnadmin:AVNS_ij8Y_tzefS4f0OMwJbM@mysql-33dafe04-takeoffokwemba-8d33.a.aivencloud.com:19093/defaultdb?ssl-mode=REQUIRED"
