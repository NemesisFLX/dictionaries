# Preprocessing commands

We want that case information is not taken into account so we change all characters that are high into low ones.

```cat alice.txt | tr 'ABCDEFGHIJKLMNOPQRSTUVWXYZ' 'abcdefghijklmnopqrstuvwxyz' > aliceTr.txt```

Afterwards for every special char:

```sed 's/`/ ` /' <aliceTr.txt >aliceTrSed.txt```