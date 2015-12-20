# microsoft-sqlserver-sqljdbc4
The JAR is not included within maven central, so you will need to follow the below:

1. Visit the MSDN[2] site for SQL Server and download the latest version of the JDBC driver for your operating system.
2. Unzip the package
3. Open a command prompt and switch into the expanded directory where the jar file is located.
4. Execute the following command. Be sure to modify the jar file name and version as necessary:
5. mvn install:install-file -Dfile=sqljdbc41.jar -Dpackaging=jar -DgroupId=com.microsoft.sqlserver -DartifactId=sqljdbc4 -Dversion=4.1

[1] http://claude.betancourt.us/add-microsoft-sql-jdbc-driver-to-maven/
[2] https://msdn.microsoft.com/en-us/sqlserver/aa937724
