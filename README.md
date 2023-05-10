<h1 align = "center">Typescript</h1>

<div align="center">  
   <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/victorpereiira/DockerNinja">
   <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/victorpereiira/DockerNinja">
</div>


<p align = "center">
    <a href="#about">About</a>   |
    <a href="#content">Content</a>   |
    <a href="#how-to-contribute">How to contribute</a>   
</p>


<div align="center">
    Translate for
    <a href="./github/readme_pt-br.md">PT-BR</a>
</div>


## About
🐱‍👤TypescriptNinha - Our Typescript discoverys. from [StudyVerse](https://github.com/VictorPereiira/StudyVerse)


## Project Targets

### Docker Study

1. To learning the fundamentals

### TypescriptTools

1. Abc


### Box 

- Doc
	- [Declare a function with an Object return type in TypeScript | bobbyhadz](https://bobbyhadz.com/blog/typescript-function-return-type-object)
- Youtube Videos
	- Abc
- Courses
    - [Typescript c/ React & Express](https://www.udemy.com/course/typescript-do-basico-ao-avancado-c-react-express/)



## Content

### What its?

1. Inference and Annotaion Types
   

### How to do

1. How to create a ...

- How to create a ...
    
    

### Notes

```tsx
Init ts config 
tsc --init 

Auto compiler
tsc -w
```

Inference and Annotaion Types 

```tsx
const ann: string = 'test'
const inf = 'test'
```

**Variables** **Types**

```tsx
// Array
const number_array: number[] = [1, 2, 3]
const string_array: string[] = ['a',  'b', 'c']
const number_array: Array<number> | Array<string> = [1, 2, 3, 'x', 'y']

// ReadOnlyArray

// Tupla
type FourNumbers =  [number, number, number, number]
```

**Type Alias**

```tsx
type ID = string | number

function showId(id: ID) {
	console.log(id)
}
```

******************Interface Object******************

```tsx
interface Point {
	x: number
	y: number
	readonly z?: number
}

function showPoint(obj: Point) {
	console.log(obj)
}

const coordObj:Point = { x: 45, y: 44 }
showPoint(coordObj)

OBS: "Use a interface quando quiser incrementar propriedades ao longo do código."

Others
// readonly
// Index Signature
// Herança
```

******************Literal types******************

```tsx
function showDirection(direction: "left" | "right" | "center") {
	console.log(direction)
}
```

**Dom**

```tsx
// Non null assertion operator
```

********Others********

```tsx
1. BigInt
2. Symbol
```

******************Narrowing ( Check data and type )******************

```tsx
// Typeof 
// Check is undefined
// Instanceof 
// Operator "in"
```

****************Functions****************

```tsx
:void -> return without
// Generic Function
// Constraint 
```

**************************Destructuring**************************

```tsx
interface Product {
    name: string
    price: number
    isAvailable?: boolean
}

function showProductDetails({ name, price, isAvailable = false }: Product): string {
    return `The product name is: ${name} and he cost R$:${price} and available is ${isAvailable}`
}

console.log(showProductDetails({ name: 'Short', price: 5.55 }));
console.log(showProductDetails({ name: 'T-Short', price: 45.55, isAvailable: true }));
```



## How to contribute
- Make a fork;
- Create a branch with your feature: `git checkout -b my-feature`;
- Commit changes: `git commit -m "feat: my new feature`;
- Make a push to your branch: `git push origin my-feature`.

<p>After meging your receipt request to done, you can delete a branch from yours.</p>

#
<p align = "center">
    Made by 👨🏾‍💻
    <a href="https://github.com/VictorPereiira">VictorPereira</a>
</p>


