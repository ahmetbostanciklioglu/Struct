# Struct


**Struct:**
```
struct Family {
    var son: String
    var daughter: String
    var father: String
    var mother: String
    var grandmother: String
    var grandfather: String
}

var object1 = Family(son: "Ahmet", daughter: "Asiye", father: "Ali", mother: "Marie", grandmother: "Natalie", grandfather: "Marcus")
object1.son = "Ali"
```

**Default property in struct:**
```
struct Profile {
    var firstName: stringType
    var old: Int
    var state = "Miami" //Default property
    typealias stringType = String
}
var object2 = Profile(firstName: "Ahmet", old: 19)
```

**Computed property in struct:**
```
struct StoredAndComputedPropertyStruct {

    var storedProperty: String  // stored property
    
    var computedProperty: String {  // Computed property
        return   "This is a computed property"
    }
}
let storedProperty = StoredAndComputedPropertyStruct(storedProperty: "Ali")
print(storedProperty.computedProperty)
```

**Property observers in struct:**
```
struct propertyObserverStruct {
    var storedProperty: String
    var propertyObserver: Int {
        
        didSet { // this code block will run after first propertyObserver value applied (after  'propertyObserver: 20' value )
            print("\(storedProperty) is \(propertyObserver)% improved")
        }
    }
}

var propertyObject = propertyObserverStruct(storedProperty: "Property observer", propertyObserver: 20)
propertyObject.propertyObserver = 50   // print("Property observer is 50% improved")
propertyObject.propertyObserver = 70   // print("Property observer is 70% improved")
propertyObject.propertyObserver = 100  // print("Property observer is 100% improved")
```

**Method in struct:**
```
struct MethodStruct {
    var property: Int
    
    func method(type: Int) -> Int {
        return property * 10
    }
}
let methodObject  = MethodStruct(property: 10)
methodObject.method(type: 12) // 100
methodObject.property  // 10
```


**Mutating method in struct:**
```
struct MutatingMethods {
    var property: String = "Mehmet"
    
    mutating func mutatingFunction() { //to change the value of property with function in struct use mutating keyboard before the 'func' keyboard
        property = "Ahmet"
    }
    
var test = MutatingMethods() 
print(test.property) // "Mehmet"

var mutatingObject = MutatingMethods(property: "Ali") 
print(mutatingObject.property) //"Ali

mutatingObject.mutatingFunction()
print(mutatingObject.property) //Ahmet
```


