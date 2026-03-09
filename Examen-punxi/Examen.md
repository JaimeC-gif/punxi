` `![ref1]![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.002.png)
|2 ASIX:    -  **Tema** |
| - |
|**PRACTICA   // //** |



|**Nombre: Nombre professor**|Jaime Climent Cardona Espe|**Grupo: 2 ASIX Grupo: 2 ASIX**|
| :- | :- | - |

**EXAMEN IAW![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.003.png)**

**Accedir al teu server per nom de domini**

Primer pas tindre instalat nginx que es el servidor web

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.004.png)

Dins de /var/www/html hi ha un index per defecte de nginx, aquest es el que es mostra cuando posem url en el navegador

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.005.png)

Revisar si el /etc/nginx/sites-available, el root redirigeix a /var/www/html i veure si esta fet l’enllaç simbòlic![ref2]

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.007.jpeg)

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.008.png)

*16/09/24 Página **1** de **7***

|2ASIX:    -  **Tema** |
| - |
|**PRACTICA  //** -  Jaime Climent Cardona|

Indica com podria accedir a la url amb el meu nom![ref3]

Desde un client entrem al ficher /etc/hosts i anyadim la següent línia

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.010.jpeg)

I ara en el navegador posem [http://examen.com](http://examen.com/) i deuria de funcionar tal que així

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.011.jpeg)

S’hauria de accedir amb la url: [**http://examen.com**](http://examen.com/) en este cas **Implantació 1**

Creem fitxer dins de /var/www/html/ nomenat nota.html![ref2]

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.012.jpeg)



|2ASIX:    -  **Tema** |
| - |
|**PRACTICA  //** -  Jaime Climent Cardona|

Creem el fitxer resultat perq es redirisxca desde nota.html![ref3]

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.013.jpeg)

Mostrem el nota.html en el navegador![ref2]

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.014.jpeg)



|2ASIX:    -  **Tema** |
| - |
|**PRACTICA  //** -  Jaime Climent Cardona|

**Implantació 2![ref3]**

Crea una base de dades per a guardar la configuració i les dades de dolibarr Crea un usuari amb privilegis per a gestionar la base de dades

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.015.png)

Dolibarr necesita les extension PHP:

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.016.jpeg)

Descarreguem el .zip i fem un rsync per a pasarlo al nostre servidor![ref2]

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.017.png)



|2ASIX:    -  **Tema** |
| - |
|**PRACTICA  //** -  Jaime Climent Cardona|

Obtenim el arxiu de la aplicació![ref3]

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.018.jpeg)

Descomprimim el arxiu

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.019.jpeg)

Li cambiem el nom la arxiu i li donem els permisos adequats

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.020.png)

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.021.png)

Creem arxiu conf.php i estbalim permisos

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.022.png)

Creem carpeta documents i establim permisos![ref2]



|2ASIX:    -  **Tema** |
| - |
|**PRACTICA  //** -  Jaime Climent Cardona|

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.023.png)

Servidor Nginx

Creem un nou fitxer en /etc/nginx/sites-available

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.024.jpeg)

Activem el lloc

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.025.png)

Comprobem que esta correcte i reiniciem![ref2]

![](Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.026.png)



|2ASIX:    -  **Tema** |
| - |
|**PRACTICA  //** -  Jaime Climent Cardona|

*Página ***8*** de ***8****

[ref1]: Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.001.png
[ref2]: Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.006.png
[ref3]: Aspose.Words.51783f1a-c266-4b62-8a9d-28614e85f259.009.png
