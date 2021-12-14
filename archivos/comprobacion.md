# Comprobación  

Vamos a asegurarnos de que K0S funciona correctamente y para ello vamos a crear un Pod y ver que este funciona.  

## Creación del Pod  
Creamos un Pod sencillo mediante el siguiente comando:  
![](https://github.com/anamontejo95/Instalaci-n-K0S-en-remoto/blob/main/imagenes/crear-pod.PNG)  

## Comprobación del Pod  
Nos aseguramos que el pod se ha creado bien, tenemos que asegurarnos de que el estado de este sea "Running".  
Lo podemos ver con el comando k0s kubectl get all.  
![](https://github.com/anamontejo95/Instalaci-n-K0S-en-remoto/blob/main/imagenes/comprobar-pod.PNG)  

## Acceso al Pod  
A continuación, vamos a acceder al Pod y de forma sencilla vamos a crear un contenido en nuestra web, será algo sencillo por lo que con la herramienta de redireccionamiento generaremos ese contenido.  
![](https://github.com/anamontejo95/Instalaci-n-K0S-en-remoto/blob/main/imagenes/acceso-pod.PNG)  
![](https://github.com/anamontejo95/Instalaci-n-K0S-en-remoto/blob/main/imagenes/contenido.PNG)  

## Tmux  
Por último, para asegurarnos de que todo funciona correctamente vamos a crear una pasarela para comunicarnos con el Pod. Para ello utilizaremos la herramienta tmux, ya que esta nos permite tener abierto más de un terminal a la vez.
El procedimiento es el siguiente. Primero instalamos la herramienta tmux (si no la tenemos ya instalada) y a continuación crearemos dos terminales. 
Como podemos ver en la foto, en el terminal superior creo la paserela de comunicación (port-forward) y en el inferior hacemos la comprobación mediante el comando curl.  
![](https://github.com/anamontejo95/Instalaci-n-K0S-en-remoto/blob/main/imagenes/tmux.PNG)
