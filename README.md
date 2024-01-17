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
