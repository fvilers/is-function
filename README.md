# @fvilers/is-function

A TypeScript type guard that validates if the given value is a function

## Installation

```
npm install @fvilers/is-function
```

or

```
yarn add @fvilers/is-function
```

## Usage

```ts
import isFunction from "@fvilers/is-function";

const variable: any = (): string => {
  return "Hello, world!";
};

if (isFunction(variable)) {
  // From here, variable is strongly typed as a function
  console.log("Variable is a function that returns", variable());
} else {
  console.log("Variable is not a function");
}
```

It will output:

```
Variable is a function that returns Hello, world!
```
