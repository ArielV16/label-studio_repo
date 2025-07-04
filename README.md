"# label-studio_repo" 
## instalacion de git
1. ingresar a la paguina de git

   ```
   https://git-scm.com/downloads/win
   ```
2. una vez descargado debe ejecutarlo dando a todo siguiente (o next)
3. Puede ver la version con el siguiente codigo para verificar la instalacion
   
   ```
   git --version
   ```
  
5. para iniciar deberán indicar su nombre

   ```
   git config --global user.name "Juanito Perez"
   ```
Luego indicar su correo que usan en GutHub
   ```
   git config --global user.email juanito.perez@gmail.com
   ```
y estaria listo para comenzar a subir carpetas a los repositorios


## Instalación

1. dirigirse a Anaconda Prompt
2. crear una carpeta en el escritorio (O en algun otro lado) con el nombre "label-studio_repo"
3. dirigirse a la carpeta creada con el codigo siguiente (es un ejemplo)
   ```
   cd C:\Users\AVILLALOBOS\Desktop\label-studio_repo 
   ```
4. instalar label-studio con el siguiente codigo en la terminal
   
   ```
   pip install label-studio
   ```

5. una vez instalado iniciar en el entorno virtual

```
    label-studio start
```
6. una vez iniciado le pedira iniciar sesion (tendra que crear una cuenta)


## Utilizar esto en Label-studio 

en este link se encuentra la database que tendran que importar en label studio

```
https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv
```

Aqui se encuentra las opciones ingresadas en la clase 

```
<View>
    <Header value="Table with {key: value} pairs"/>
    <Table name="table" value="$item"/>
    <Text name="passenger_info" value="Passenger ID: $PassengerId \n Name: $Name \n Class: $Pclass \n Age: $Age\n Sex: $Sex"/>
  	<Choices name="choice" toName="table">
        
    <Choice value="Child"/>
    <Choice value="Adult"/>
    <Choice value="Elder(60+)"/>
</Choices>
</View>
```

Cada uno de los datos debe ser etiquetado con las opciones basandose en la edad 

