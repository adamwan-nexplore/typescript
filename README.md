# typescript


branded type

```typescript
declare const brand: unique sybmol;
export type Brand<T, TBrand> = T & { [brand]: Tbrand };
```
