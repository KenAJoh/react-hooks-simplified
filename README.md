# React-snippets: simplified

A collection of snippets without the bloat.

## Features

Made for daily use when developing react-applications.

## Snippets

| Snippet           |                   |
| ----------------- | ----------------- |
| `useEffect`       | useEffect         |
| `useLayoutEffect` | useLayoutEffect   |
| `useState`        | useState          |
| `useCallback`     | useCallback       |
| `useContext`      | useContext        |
| `useMemo`         | useMemo           |
| `useRef`          | useRef            |
| `useTransition`   | useTransition     |
| `useEvent`        | custom event hook |
| `cla`             | className         |
| `cl`              | console.log       |

## Exmplanation

### **useEffect**

```javascript
useEffect(() => {

  return () =>
}, [])
```

### **useLayoutEffect**

```javascript
useLayoutEffect(() => {

  return () =>
}, [])
```

### **useState**

```typescript
// JS
const [state, setState] = useState();

// TS
const [state, setState] = useState<type>();
```

### **useCallback**

```javascript
const callback = useCallback(() => {
  func(a);
}, [a]);
```

### **useContext**

```typescript
// JS
const context = useContext(ctx);

// TS
const context = useContext<type>(ctx);
```

### **useMemo**

```typescript
// JS
const value = useMemo(() => calc(a), [a]);

// TS
const value: type = useMemo(() => calc(a), [a]);
```

### **useRef**

```typescript
// JS
const ref = useRef(null);

// TS
const ref = useRef<type>(null);
```

### **useTransition**

```javascript
const [isPending, startTransition] = useTransition();
```

### **useEvent**

Not used often, but when needed its a pain to boilerplate.

```typescript
const callback = useCallback(() => {
  calc(a);
}, [a]);

useEffect(() => {
  window.addEventListener(event, callback);

  return () => {
    window.removeEventListener(event, callback);
  };
}, [callback]);
```

### **cla**

For the extra lazy (like me)

```javascript
className = "";
```

### **cl**

Logs output in object format

```javascript
console.log({ value });
```
