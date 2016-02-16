conseguir el conector (viene en zip)

src:
  https://github.com/wso2/esb-connectors/tree/master/distribution.
bin:
  https://storepreview.wso2.com/store/assets/esbconnector


instalar el esb

instalar el conector en el esb
  esb-mgmt-console > add
  (buscar el zip)
  (hacer el upload)
  [lo sube a wso2esb-4.9.0\repository\deployment\server\synapse-libs]
  
  habilitar el conector
  
crear el proxy
  services / add /proxy sequence 
  tipo: custom



crear usuario linkedin
andje
ahurtado.dj@gmail.com
confirmar mail

en edit profile, en la parte de skills & endorsements
adiconarl skills




#NOTA: 
# https://developer.linkedin.com/docs/fields#skills
# se debe aplicar para "Apply with LinkedIn program"
# https://www.quora.com/Can-one-access-the-skill-graph-of-LinkedIn-Skills-via-an-API-If-not-is-it-planned-for-the-future
# hay una alternativa a linkedin: http://api.itsyourskills.com/





en linkedin, crear la aplicacion
	https://www.linkedin.com/secure/developer?newapp=
	datos:
	cmpany: ANDJE
	name: wso2_access
	website-url: https://192.168.40.193:9446/carbon
	icon: icono_de_equilibrio


luego obtener el token de acceso

despues adicionar la url de acceso a authorized redirect URLS
  adicionar: https://192.168.40.193:8283
dar clikc en actualizar


prueba de datos:
	export CLIENT_ID=7765gnc0ysbctm
	export REDIRECT_URL=http://192.168.90.30:8283
	export STATE=andjestate2015
	export SCOPE=r_basicprofile
	echo $(echo https://www.linkedin.com/uas/oauth2/authorization?response_type=code\&client_id=$CLIENT_ID\&redirect_uri=$REDIRECT_URL\&state=$STATE\&scope=$SCOPE)

	colocar la url en el browser y solicitará credenciales

1. pedir access token


	

invocar el servicio
 {
"accessToken":"AQVT5aduaKoUktPuqxFD-KdGny8NyVOxY_F7wH53F050uf6SzqyfOSdxoU3wLgxLtQAnuskio7wWJIO9bIhxtJgikQ0DCX6ckNAAhDIx1yBpMOZsPtt7UvU0kgaxTdMGLk3X9Q7G_9NvvRNiliWx6UBY3Y_wCIQSfpu0KJrGyRCcT9_RAkE",
"apiUrl":"https://api.linkedin.com",
"publicUrl":"",
"fieldSelectors":"first-name,last-name",
"secureUrls":"true"
} 


request 
curl 


{
"accessToken":"AQVT5aduaKoUktPuqxFD-KdGny8NyVOxY_F7wH53F050uf6SzqyfOSdxoU3wLgxLtQAnuskio7wWJIO9bIhxtJgikQ0DCX6ckNAAhDIx1yBpMOZsPtt7UvU0kgaxTdMGLk3X9Q7G_9NvvRNiliWx6UBY3Y_wCIQSfpu0KJrGyRCcT9_RAkE",
"apiUrl":"https://api.linkedin.com",
"publicUrl":"",
"fieldSelectors":"first-name,last-name",
"secureUrls":"true"
} 




obtener token de acceso
- ir a https://apigee.com/console/linkedin?apig_cc=1
- en authentication selecciona oauth2
- (seleccionar signin with linkedin; provea un usuario y password)
- redireccionará de nuevo a apigee; 
- tratar de enviar el request de (retrieve basic profile)
- en el request estará el accessToken: 
	ejemplo=AQXtffY4rY0owx0zhfsVoTCGTYLhDPN20cnntguXLIBCWI5wv3aV6a8cjZAwnxRR6cheWh_niQ8ivvQJrJzMvWE_NneXzaAuKdhm9CzSCWIWazszv8Pn37NMOZS37zQd2g_Not9TiJbYkp2oO-54yr8rkdPsJl8O_045A1ZHIgu847gjnig
	
- debe configurarse el certificado de cliente de linkedin para tener acceso
Gener errores si el certificado no se encuentra configurado

	
	
	
  hacer un retrieve de basic-profile
-  





ref: instruccione sen https://github.com/wso2/esb-connectors/tree/master/linkedin/linkedin-connector/linkedin-connector-1.0.0


REFERENCIAS
- construir un conector: http://chanakaindrajith.blogspot.com.co/2014/04/getting-started-with-wso2-esb-connectors.html
- construir un conector: https://docs.wso2.com/display/ESBCONNECTORS/Creating+a+Connector

REFERENCIAS ----------------------------
Especialidades abogacia
 https://www.soloabogados.org/especialidades-abogacia
 
 
procesos
 doctrina aplicable 


 
pantallazos de dashboards  
https://www.google.com.co/search?q=case+law+dashboard&espv=2&biw=1364&bih=634&source=lnms&tbm=isch&sa=X&ved=0ahUKEwj1vJb93vDKAhUFXB4KHeCPCwoQ_AUIBigB#imgrc=CMxNSqMIYD-HsM%3A 
(automatic case characterization)
(The team used Python, Kibana, Elastic Search and Shiny toexplore, validate and visualize their data and results.)


abogado: habilidades generales
 analytical skills: 
 creativity
 research skills: 
 interpersonal skills: 
 logical thinking ability: 
 perseverance: 
 public speaking skills (oral): 
 pursues continuing education:
 reading comprehension skills:
 writing skills:
 
 liderazgo:
 medios digitales:
 lenguaje corporal:
 
 
 
REFERENCIAS
- http://environmentallawschools.org/resources/top-10-qualities-of-a-great-lawyer 