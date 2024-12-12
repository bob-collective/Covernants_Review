This review is done considering my main interest is to create Bitcoin L2s: 
- Inherit security from Bitcoin 
- Create a trust-minimized BTC bridge. The best way to do this is a bi-directional light client bridge e.g. via BitVM2. For this we need to build a light client for the L2 on Bitcoin, plus ideally introspection to for Bitcoin itself.

OP_CTV
```
- Not useful for BitVM2 because it cannot commit to inputs, meaning it cannot be used to simplify the connector-output construction. 

```

OP_CSFS
```
Evaluating
```

OP_PAIRCOMMIT

```
Evaluating
```

OP_INTERNALKEY
```
Evaluating
```

OP_CAT
```
Evaluating

The main pitch here is that we could implement a SNARK or START verifier in Bitcoin script. Evaluating if this is feasible in terms of executing proofs regularly and how this can improve the Bitcoin bridge design. My feeling is that we will need optimistic verification even with OP_CAT. 
```

OP_CCV
```
Evaluating```

OP_VAULT
```
Evaluating
```
More detaills: [https://github.com/bitcoin/bips/blob/master/bip-0345.mediawiki#user-content-Goals](https://github.com/bitcoin/bips/blob/master/bip-0345.mediawiki#user-content-Goals)

OP_TXHASH
```
Very useful for BitVM2
- Allow us to get rid of all pre-signing needed during BitVM setup
- Also improves peg-in UX for users
```

SIGHASH_APO
```
Evaluating
```

I will update this rationale and add more things when required
