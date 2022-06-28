Crear base de datos

CREATE ROLE banxico WITH PASSWORD 'banxico' LOGIN;
CREATE DATABASE efirma ENCODING 'UTF8' OWNER banxico;

-- jdbc:postgresql://localhost:5432/efirma

create table certificado_operador(
numero_serie varchar(100),
nombre_comun varchar(100),
certificado_pem varchar(100)
);

select *
from certificado_operador;

El proyecto debe estar corriendo el localhost api call front

References:
https://mkyong.com/spring-boot/spring-boot-spring-data-jpa-postgresql/
https://www.baeldung.com/spring-data-jpa-query
https://www.baeldung.com/java-bouncy-castle
https://docs.hidglobal.com/auth-service/docs/buildingapps/javascript/read-different-certificate-key-file-formats-with-javascript.htm
https://github.com/digitalbazaar/forge
https://github.com/digitalbazaar/forge#rsa



