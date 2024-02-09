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









