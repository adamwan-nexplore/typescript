# typescript


branded type

```typescript
declare const brand: unique symbol;
export type Brand<T, TBrand> = T & { [brand]: TBrand };
```


```typescript
export type Email = Brand<string, "Email">;
export const validateEmail = (email: string): email is Email => {
  if (!email.includes("@")) {
    throw new Error("Email invalid");
  }
  
  return true;
}



```
