GCAT

Требования:
1. tomcat - не ниже 8
2. java - не ниже 1.8
3. БД postgresql

Настройки:
1. Развернуть БД gcat (скрипт в файле gcat_DB.txt)
2. Создать файл GCAT.properties с полями (файл GCAT.properties):
	dbName = gcat - имя БД
	dbIp = 127.0.0.1 - ip БД
	dbPort = 5432 - порт БД
	dbLogin = login - логин
	dbPassword = pass - пароль
	dbTimeout = 3600 - время ожидания
3. В развернутом tomcat, в файл catalina.properties добавить поле 
	GCATConfigPath=путь до файла GCAT.properties
4. В tomcat, через Manager App загрузить GCAT.war


Файл лога формируется автоматически в "/tmp/GCAT.log"