# snarkjs-generate-solidity

Provides generator functions for verifiers as Solidity Smart Contracts.

This generator plugin supports the `groth16`, `plonk`, and `fflonk` protocols and
follows the conventions of the generator plugins for SnarkJS, such that it provides:

```js
export const verifiers = {
    groth16(vkey, logger): string,
    plonk(vkey, logger): string,
    fflonk(vkey, logger): string,
};

export const calldata = {
    groth16(proof, publicInputs, logger): string,
    plonk(proof, publicInputs, logger): string,
    fflonk(proof, publicInputs, logger): string,
};
```
