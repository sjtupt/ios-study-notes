# Swift
Tested with Swift 3.0
## Function
### Something about outer parameters
* When call function without explict outer parameter should use internal parameter name instead of parameter label. eg:
 
		func greet(person:String, day:String)->String              --- function definition
		great(person: xx, day: xx)                                 --- when call
* When call function use _ instead of outer parameter cannot use any parameter label. eg:   

		func greet(person:String, _ day:String)->String            --- function definition
		great(person: xx, xx)                                      --- when call
* When call function with explict outer parameter should use outer parameter as label.eg:

		func greet(person person:String, onDay day:String)->String --- function definition
		great(person: xx, onDay: xx)                               --- when call
