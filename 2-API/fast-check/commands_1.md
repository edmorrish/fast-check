[Home](/) &gt; [fast-check](../fast-check.md) &gt; [commands](commands_1.md)

## commands() function

For arrays of [AsyncCommand](AsyncCommand.md) to be executed by [asyncModelRun](asyncModelRun.md)

This implementation comes with a shrinker adapted for commands. It should shrink more efficiently than  for [AsyncCommand](AsyncCommand.md) arrays.

<b>Signature:</b>

```typescript
declare function commands<Model extends object, Real, CheckAsync extends boolean>(commandArbs: Arbitrary<AsyncCommand<Model, Real, CheckAsync>>[], maxCommands?: number): Arbitrary<Iterable<AsyncCommand<Model, Real, CheckAsync>>>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  commandArbs | <code>Arbitrary&lt;AsyncCommand&lt;Model, Real, CheckAsync&gt;&gt;[]</code> | Arbitraries responsible to build commands |
|  maxCommands | <code>number</code> | Maximal number of commands to build |

<b>Returns:</b>

`Arbitrary<Iterable<AsyncCommand<Model, Real, CheckAsync>>>`
