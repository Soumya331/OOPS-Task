Ans1)
```python
class car:
    def __init__(self , name_of_vehicle, max_speed , average_of_vehicle ) :
        self.name_of_vehicle = name_of_vehicle
        self.max_speed = max_speed
        self.average_of_vehicle = average_of_vehicle
        
        def return_car_details(self):
            return self.name_of_vehicle, self.max_speed, self.average_of_vehicle
```


```python
obj_car = car("toyota" , 67 , 56)
```


```python
obj_car.max_speed
```




    67




```python
obj_car.name_of_vehicle
```




    'toyota'




```python
obj_car.average_of_vehicle
```




    56



Ans2)
```python
class car1(car):  
    def __init__(self, seating_capacity) :
        self.seating_capacity = seating_capacity
        print(self.seating_capacity, obj_car.name_of_vehicle)
```


```python
car2 = car1(7)
```

    7 toyota


Ans 3)When a class is derived from more than one base class it is called multiple inheritance. The derived class inherits all the features of the base case.


```python
class Class1:
    def m(self):
        print("In Class1")
       
class Class2(Class1):
    pass
 
class Class3(Class1):
    def m(self):
        print("In Class3")   
      
class Class4(Class2, Class3):
    pass      
 
obj = Class4()
obj.m()
```

    In Class3


Ans4) We use getters & setters to add validation logic around getting and setting a value and to avoid direct access of a class field .


```python
class age:
	def __init__(self, age = 0):
		self._age = age
	
	# getter method
	def get_age(self):
		return self._age
	
	# setter method
	def set_age(self, age):
		self._age = age

soumya = age()

# setting the age using setter
soumya.set_age(21)

# retrieving age using getter
print(soumya.get_age())


```

    21


Ans 5) Method overriding is an ability that allows a child class to provide a specific implementation of a method that is already provided by one of its parent classes.


```python
class number:
      
    def message(self):
        print('number')
    
class age(number):
  
    def message(self):
        print('Age is a number')
        
num = number()
num.message()

num1 = age()
num1.message()
```

    number
    Age is a number



```python

```

