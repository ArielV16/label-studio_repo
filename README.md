"# label-studio_repo" 
#Utilizar esto en Label-studio 

https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv

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
