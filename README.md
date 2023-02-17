# -TypescriptNinja
🐱‍👤 TypescriptNinja - Our TypescriptVerse discoverys.

### Input Content

[Declare a function with an Object return type in TypeScript | bobbyhadz](https://bobbyhadz.com/blog/typescript-function-return-type-object)

****************************Init ts config****************************

```tsx
tsc --init
```

**************************Auto compiler**************************

```tsx
tsc -w
```

******************************************************Inference and Annotaion Types******************************************************

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
