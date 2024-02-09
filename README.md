# react-typescript
```typescript
type SignUpProps = {
    anyProps?: string;
}

const SignupPage = ({ anyProps = "Default Value" }: SignUpProps) => {
    return (
        <>
            <h1>Hello {anyProps}</h1>
        </>
    );
}

```
* It's a common convention in TypeScript to use PascalCase for type names. So, you might want to change signUpProps to SignUpProps for consistency.

```typescript
import React from 'react';

// Define the props interface
interface MyComponentProps {
  name: string;
}

// Define the function component
const MyComponent: React.FC<MyComponentProps> = ({ name }) => {
  return (
    <div>
      <h1>Hello, {name}!</h1>
    </div>
  );
};

export default MyComponent;

```
<br>
<br>

# How can I define an array of objects?
```typescript
let userTestStatus: { id: number, name: string }[] = [
    { "id": 0, "name": "Available" },
    { "id": 1, "name": "Ready" },
    { "id": 2, "name": "Started" }
];

```

<br>
<br>

# What is todo file in vscode?
https://stackoverflow.com/questions/71328373/how-to-use-todo-files-in-vs-code

<br>

# TypeScript - Declare a function callback type
https://trungvose.com/experience/typescript-function-callback-type/#:~:text=TL%3BDR%20To%20define%20the,)%20%7B%20callback('Hi!'

<br>
<br>

# Error Log: using React-helmet
* When I searched `react-helmet-typescript`, the official NPM page of the react helmet shows me how to install react!
```console
npm install --save @types/react-helmet
```
* Unfortunately, I kept getting this error: `Failed to resolve import "react-helmet"`. Why? I followed everything from the official document. Nothing was wrong! The fuck?
* After some research, LUCKILY I found the solution (again with a little clue, no solution found in docs).
* First, I have to install basic `react-helmet`, after that I can install `typescript @types` version of react-helmet.
* The @types/react-helmet needs basic `react-helmet` package to work.
* First, install basic 'react-helmet' then install @types/react-hemlet which is the typescript version of react helmet.
```console
npm install react-helmet

npm install --save-dev @types/react-helmet
```









