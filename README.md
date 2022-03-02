### sample
## React Testing repo

## Typescript Tutorial
- "Superset" of JS. Adds static typing (type defined vars)
- Primitives: number, string, boolean. let age: number
- Complex Types: arrays, objects. let arr: string[]; arr = ['a','b']; \
let person: {name: string; age: number}; person = {name: 'Max', age: 12}
- Type Inference: let course = 'React'; !Xcourse = 123;X!
- Union Types: let course: string | number (|boolean) = 'React';
- Type Aliases: type Person = = {name:string, age: number}; custom data type, providing maintainability and ease reusability
- Functions and Types: function add(a: number, b:number): (-mostly not using return type definition-number (or any other)) { return a+b; }
- function print(value :any) { constole.log(value);}: This would class with JS's built-in 'print'.So! \
function print(value :any):void { constole.log(value);}
- Generics
function insertAtBeggining(array: any[], value: any){
    const newArray = [valu, ...array];
    return newArray;
}
const demo = [1,2,3];
const UpdatedArray = insertAtBeggining(demo, -1); // [-1,1,2,3]

updatedArray[0].split(''); //split a number :/ There's where Generics feature gets in
+++---: function insertAtBeggining<T>(array: T[], value: T){ ... }
eg:
const demo = [1,2,3];
const UpdatedArray = insertAtBeggining(demo, -1); // [-1,1,2,3] (valid)
const stringArray = insertAtBeggining(['a','b','c'], 'd'); // Valid!

## React - TS
- React.FC: declared function that is a functional component
- const Todos: React.FC<{items: string[]}> = (props) => {}: To pass custom properties to Todos function
