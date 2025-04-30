# counting-js
> Utility functions related to counting and combinatorial bit manipulation.

## Api

### Math
```
factorial(n: int): bigint
nChooseK(n: int, k: int): bigint
```

### Permutation
```
permutation(n: int, r: bigint): number[]
forEachPerm(n: int, callback: (perm: number[]) => boolean)
randomPermutation(n: int): number[]

shuffle(arr: any[]): any[]
```

### Combination
```
combo(n: int, k: int, r: bigint): number[]
forEachCombo(n: int, k: int, callback: (items: int[]) => boolean)
allCombos(n: int, k: int): number[][]
randomCombo(n: int, k: int): number[]

bitCombo(n: int, k: int, r: bigint): bigint
forEachBitCombo(n: int, k: int, callback: (bitCombo: bigint) => boolean)
allBitCombos(n: int, k: int): bigint[]
randomBitCombo(n: int, k: int): number[]
nextBitCombo(n: int, r: bigint): bigint

bitComboToR(n: int, k: int, bc: bigint): bigint
```

### Bigint
```
bitLength(bn: bigint): number
```

## Installing

Reference: [GitHub docs related to packages](https://docs.github.com/en/packages/learn-github-packages/installing-a-package)

GitHub packages require authentication to install.

1. Create a personal access token with the `read:packages` scope.
2. Add the GitHub package registry to a `.npmrc` file in your project like below, replacing `GH_PAT` with your PAT:
```
//npm.pkg.github.com/:_authToken=GH_PAT
@metal-pony:registry=https://npm.pkg.github.com
```
3. Then install in your project as normal:
```
npm install @metal-pony/counting-js
```
Do not commit your `.npmrc` file. Keep your access token secret.
