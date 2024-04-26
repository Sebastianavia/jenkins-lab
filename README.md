# Jenkins Lab

## Ejecutar Docker Compose

Para ejecutar Docker Compose, asegúrate de que tengas Docker Compose instalado en tu sistema. Luego, sigue estos pasos:

1. Navega a la ubicación donde se encuentra tu archivo `docker-compose.yml`.

2. Ejecuta el siguiente comando en tu terminal para iniciar los contenedores definidos en el archivo `docker-compose.yml`:

```bash
docker-compose up -d
```

3. Extraer passwords

```bash
docker logs id_container
```

```bash
docker exec id_container cat /var/jenkins_home/secrets/initialAdminPassword
```

## Ejecucion 

<p align="justify">
4. Después de completar los pasos anteriores con éxito, el siguiente paso es ejecutar nuestro contenedor a través del puerto que elijamos y luego instalar los plugins predeterminados. Si en algún momento necesitamos más plugins, podemos añadirlos después de la instalación inicial.
</p>

---


![image](https://github.com/Sebastianavia/jenkins-lab/assets/71205906/d590a289-da10-44af-90f0-8e3960a88c20)


---

Corremos nuestra imagen.

![image](https://github.com/Sebastianavia/jenkins-lab/assets/71205906/cfde1fc4-f2ef-4178-bd53-7c6e1f78b906)

---
Ya que estamos trabajando en code space de GitHub, habilitamos el puerto 8080,  para acceder a Jenkins mediante una url generada.  

![image](https://github.com/Sebastianavia/jenkins-lab/assets/71205906/830f47f4-39c2-4a1a-b843-85adc6a15fe7)

---

Por medio de los logs obtenemos la contraseña y la registramos. 


<p align="center">
  <img src="https://github.com/Sebastianavia/jenkins-lab/assets/71205906/755460cb-475b-4569-84f7-af1e9a96dd2a" alt="Descripción de la imagen" width="400">
</p>

---
Instlamaos los pluguins.

<p align="center">
  <img src=https://github.com/Sebastianavia/jenkins-lab/assets/71205906/e78eedcb-0dd1-4f10-a917-7570cd4a561f alt="Descripción de la imagen" width="400">
</p>



---
Nos registramos...


<p align="center">
  <img src="https://github.com/Sebastianavia/jenkins-lab/assets/71205906/c05769c6-74da-4dcd-93c9-0b0deda7d6e6" alt="Descripción de la imagen" width="400">
</p>


---

Para que Jenkins funcione correctamente, es necesario crear un
token de API para el usuario conectado. Sigue estos pasos:
1. Ve al apartado de "Administrar Jenkins".
2. Haz clic en "Usuarios".
3. Selecciona tu usuario (o el usuario al que necesitas otorgar los
permisos).
4. Haz clic en tu nombre de usuario.
5. Vamos  a configuración.
6. Generamos un API (Token).


<p align="center">
  <img src=https://github.com/Sebastianavia/jenkins-lab/assets/71205906/b61004ec-4ded-4e5c-ad3c-0f5f99c56394
 width="400">
</p>

--- 
Para este proyecto necesitamos Node.js  
- Folders
- OWASP Markup Formatter
- ASM API
- JSON Path API
- Pipeline: Step API
- Token Macro
- Build Timeout
- Credentials
- Plain Credentials

Estos plugins se instalaron al principio “plugins recomendados”. 

Crearemos una tools.

<p align="center">
  <img src=https://github.com/Sebastianavia/jenkins-lab/assets/71205906/d8aaa285-58ff-4e6d-bc84-f6cea5a3f5ce width="400">
</p>


<p align="center">
  <img src=https://github.com/Sebastianavia/jenkins-lab/assets/71205906/85b29ea6-03e1-4c15-ae16-fef5b3d1d2ea width="400">
</p>

---

Creamos un proyecto de estilo libre.

- Descripción: test

<p align="center">
  <img src=https://github.com/Sebastianavia/jenkins-lab/assets/71205906/300bd3a5-063b-450c-bf77-32edf4f21674 width="400">
</p>

<p align="center">
  <img src=https://github.com/Sebastianavia/jenkins-lab/assets/71205906/d19b9c3c-459c-41de-8914-85feef78dc54 width="400">
</p>


<p align="center">
  <img src=https://github.com/Sebastianavia/jenkins-lab/assets/71205906/1c1d3bf9-5b05-4b7e-9b32-4139efc75bb0 width="400">
</p>

<p align="center">
  <img src=https://github.com/Sebastianavia/jenkins-lab/assets/71205906/2a243c68-cd74-43db-99dc-cd1bb0539562 width="400">
</p>

---

Guardamos..

<p align="center">
  <img src=https://github.com/Sebastianavia/jenkins-lab/assets/71205906/8de61759-2c18-4c36-b24e-493f1799273a width="400">
</p>

---

Una vez termina de construir, observamos el resultado.

<p align="center">
  <img src=https://github.com/Sebastianavia/jenkins-lab/assets/71205906/085b9055-de22-44e2-9b19-addf6b0858e7 width="400">
</p>


<p align="center">
  <img src=https://github.com/Sebastianavia/jenkins-lab/assets/71205906/fe5ea337-a764-4bfc-a889-789cfe77029d width="50">
</p>










