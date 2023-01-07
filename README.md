# Struct


**Struct**
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

**Default Property**
```
struct Profile {
    var firstName: stringType
    var old: Int
    var state = "Miami" //Default property
    typealias stringType = String
}
var object2 = Profile(firstName: "Ahmet", old: 19)
```

**Computed property in struct**
```
struct StoredAndComputedPropertyStruct {
    //MARK: stored property
    var storedProperty: String
    
    //MARK: Computed property
    var computedProperty: String {
        return   "This is a computed property"
    }
}
let storedProperty = StoredAndComputedPropertyStruct(storedProperty: "Ali")
print(storedProperty.computedProperty)
```



