## ASPECTOS A TENER EN CUENTA:

* El código relativo al modelo de elementos finitos se ha ejecutado en una estación de trabajo externa. Por favor, si quieres ejecutar el código para hacer alguna simulación presta mucha atención a las rutas del código y adáptalas a las tuyas. Lo importante es mantener la referencia a la carpeta `inputs-APDL`, que contiene todos scripts requeridos por MAPDL. Revisa también que tu sistema operativo sea compatible con PyANSYS (https://github.com/pyansys), es bastante problemático.
   
* El contenido de la carpeta `case-studies-inputs` se corresponde con el de la carpeta `data/preprocessed/files-to-ansys` o `data/preprocessed/files-to-ml/inputs` (sin contar las condiciones de contorno).

* El contenido de la carpeta `case-studies-outputs` se corresponde con el de la carpeta `data/preprocessed/files-to-ml/outputs` o `inputs-APDL/Resultados`. Son precisamente las salidas del modelo de elementos finitos, que después se usan como target variable en los modelos de machine learning. 
