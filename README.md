"# label-studio_repo" 


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

