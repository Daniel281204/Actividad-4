# Actividad-4
# Datos abiertos / BigQuery / LookerStudio
Jesus Daniel Muñoz Moscote

Introduccion a la Ingenieria de Sistemas - 2023_10

NRC: 4519

---
## Dataset usado:

<a href="https://www.datos.gov.co/Seguridad-y-Defensa/Homicidios-accidente-de-tr-nsito-Polic-a-Nacional/ha6j-pa2r">'Accidentes-transito_(2010-2023)'</a> Es un informe de accidentes de transito proporcionado por la DIJIN. En este se muestran los departamentos y municipios donde se presentan estos accidentes, ademas si fue realizado con moto o automovil. entre otros datos.

Con base a estos datos, respondere la pregunta planteada.

## ¿Cuáles son las áreas geográficas con la mayor cantidad de accidentes?

### Consulta SQL:

~~~ SQL
    SELECT Departamento, Municipio, SUM(Cantidad) AS TotalAccidentes
    FROM `proyecto-final-387917.Accidentes.Accidentes` 
    GROUP BY Departamento, Municipio
    ORDER BY TotalAccidentes DESC
~~~

## LookerStudio:

- <a href="https://lookerstudio.google.com/reporting/54cc64fa-5423-4298-8f93-30781fc33d29" target="_blank">Dashboard</a>

---

## Enlaces de Interes

- <a href="https://github.com/Daniel281204/Actividad-4" target="_blank">Repositorio de Github</a>

<center><img src="https://www.uninorte.edu.co/image/layout_set_logo?img_id=19855734&t=1682421319815"></center>
