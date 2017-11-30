# springbok

A minimalist functional programming utility library that ships with Flow types.

## Functions

- sort: `<T>( fn: (T) => number, list: T[] ) => T[]`
- reduce: `<T, R>( fn: (acc: R, x: T) => R, acc: R, list: $ReadOnlyArray<T> ) => R`
- reduceObj: `<T,R>( obj: {[key: string]: T}, acc: R, fn: (acc: R, key: string, x: T) => R ) => R`
- filter: `<T>( fn: (x: T) => boolean, list: $ReadOnlyArray<T> ) => Array<T>`
- map: `<T, R>( fn: (x: T) => R, list: $ReadOnlyArray<T> ) => Array<R>`
- mapIndexed: `<T, R>( fn: (i: number, x: T) => R, list: $ReadOnlyArray<T> ) => Array<R>`
- flatmap: `<T, R>( fn: (x:T) => $ReadOnlyArray<R>, list: $ReadOnlyArray<T> ) => Array<R>`
- concat: `<T>( a: $ReadOnlyArray<T>, b: $ReadOnlyArray<T> ) => Array<T>`
- clone: `<T>( obj: {[key: string]: T} ) => {[key: string]: T}`
- assoc: `<T>( key: string, val: T, obj: {[key: string]: T} ) => {[key: string]: T}`
- dissoc: `<T>( key: string, obj: {[key: string]: T} ) => {[key: string]: T}`
- fromPairs: `<T>( pairs: $ReadOnlyArray<[string, T]> ) => {[key: string]: T}`
- toPairs: `<T>( obj: {[key: string]: T} ) => Array<[string, T]>`
- find: `<T>( predicate: (x: T) => boolean, list: $ReadOnlyArray<T> ) => null | T`
- findIndex: `<T>( predicate: (x: T) => boolean, list: $ReadOnlyArray<T> ) => number`
- cond: `<T, R>( def: (x: T) => R, pairs: $ReadOnlyArray<[ (x: T) => boolean, (x: T) => R]>, x: T ) => R`
- contains: `<T>( element: T, list: $ReadOnlyArray<T> ) => boolean`
- all: `<T>( pred: (x: T) => boolean, list: $ReadOnlyArray<T> ) => boolean`
- uniq: `( list: string[] ) => string[]`
