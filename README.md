# TypeScript Optional Property Access Bug

This repository demonstrates a common, yet subtle, bug in TypeScript related to accessing optional properties.  The bug involves unexpected behavior when a property might not exist on an object, leading to runtime errors or unexpected results. The solution showcases how to effectively handle optional properties to prevent these issues.

## Bug Description
The provided `printCoord` function accepts an object with `x` and `y` coordinates. However, if the object doesn't contain these properties, or they're optional, accessing them directly can lead to runtime errors. TypeScript's type system doesn't always catch these errors during compilation if optional properties are not handled properly.

## Solution
The solution demonstrates how to safely access optional properties using optional chaining (`?.`) and nullish coalescing (`??`) operators. This approach ensures that the code gracefully handles cases where the properties might be undefined or missing, preventing runtime errors and producing more robust code.