**OBS: '>' or '<' and '>>' or '<<' equal on linux**
# importar
mariadb -u &user_with_password -p &local_database < &.sql_to_import

# exportar
mariadb-dump -u &user_with_password -p &local_database > &.sql_to_exportation