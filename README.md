# springownconfiguration
Spring MVC framework: my own configuration that includes mysql connection dependencies with context, spring-security dependencies and context, service and dao context configuration

Things that u have to change:

1) project name and packagenames (obviously)

2) persistence-context: change 
            jndi-name="jdbc/chesspairing"  -> jndi-name="jdbc/yourownname"

3)web.xml 
            <description>DB Connection</description>
		        <res-ref-name>jdbc/chesspairing</res-ref-name>    ---> change chesspairing for the one that u set in 2)

4)security-context : change as u want, depends on your configuration, all is commented out

5)servlet-context: change  location="/resources/theme1/" /> ---> i set theme1 because i wanted to use a different pack of css, js, img easily. if u dont need it and u will only use one theme just set it as location="/resources/
                  
