# Explanation
When calling Constructors
	- new Empty Object is created
	- `this` refers to this empty Object
	- return object linked to [[Prototypes|Prototype]] of constructor
- Don't Create methods inside constructors
	- lead to method duplication (method is an object) which fucks memory
	- Instead attach it to Prototype
# Sources
- Extends [[OOP In JS#sources]]