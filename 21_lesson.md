### Objects, Constructors, context(this) 


#### Example for context:

```
function isContextEqualTo(contextLink, currentContext) {
   console.log(contextLink === currentContext);
}

function Person(name, age) {
    this.name = name;
    this.age = age;
    
    this.getName = function () {
       isContextEqualTo(window, this); // ??
       isContextEqualTo(user, this); // ??
       return this.name;
    };
}

Person.getAge = function () {
    isContextEqualTo(window, this); // ??
    return this.age;
};

var user = new Person("erer", 45);

var getAge = Person.getAge;
var getName = user.getName;

consoe.log(getAge()); //  в каком контексте вызана функция?
consoe.log(getName()); //  в каком контексте вызана функция?
consoe.log(user.getName()); //  в каком контексте вызана функция?

Person.getAge = function() {
    isContextEqualTo(Person, this); // ??
    return this.name;
}

user.getAge = getAge;
consoe.log(user.getAge()); //  в каком контексте вызана функция?
```

1. Create function getName, that takes a 'name' from it's current context, and returns it to user. Then create an object, with 'name' key
and call 'getName' in context of object, and then in context of global window.

2. Create a funnction 'getDoubled' that will double a 'number' property in current context (depends on context) and multiply it to 2, then create funnction 'getDoubledTrippled' that will use getDoubled function result and multiplied it to 3. Use bind || call || apply in this cases. 

3. Create a constructor that will describe 'City'. It should
  - have 'name', 'population', 'country' (passed as arguments to functions;
  - have methods 'getPopulation'(return population), 'getCityName' (return city name);
  - have constant: 'AREA' tht cannot me modified or deleted
  - have 'addCitizen' method that increments 'popular' +1

4. Create function sum, that will return sum of different count of asrguments passed to it. It should work like this:

```
sum(2)(5)(6)(7)(2)(3)(4)( ); //29 
sum(56)(-10)(3)(1)( ); //50
```

Or like this:

```
sum(2)(5)(6)(7)(2)(3)(4)
```
