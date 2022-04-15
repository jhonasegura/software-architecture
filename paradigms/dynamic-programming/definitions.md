# Programación Dinámica

Es un método para reducir el tiempo de ejecución de un algoritmo mediante la utilización de subproblemas superpuestos y subestructuras óptimas.

```typescript
function recursiveFibo(n: number): number {
    console.log('calculado fibo', n);
    if (n <= 1) {
        return n;
    } else {
        return recursiveFibo(n - 1) + recursiveFibo(n - 2):
    }
}

console.log(recursiveFibo(5));
```

## Memoización

```typescript
let memo: number[] = [];

function memoizedibo(n: number, memo: numer[]): number {
    console.log(memo)
    if (memo[n] !== undefined) return memo[n];
    if (n <= 1) {
        memo[n] = n;
        return n;
    } else {
        let result = memoizedFibo(n - 1, memo) + memoizedFibo(n - 2, memo);
        memo[n] = result;
        return result;
    }
}

console.log(memoizedFibo(100, memo));
```

## Lineal

```typescript
function linearFibo(n: number): number {
    let memo = [0, 1];
    for (let actual = 2; actual <= n; ++actual) {
        memo[actual] = memo[actual - 2] + memo[actual - 1];
    }
    return memo[n]
}

console.log(recursiveFibo(5));
```

