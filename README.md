# Orbit=1

Orbit is a bit processor.

The core concept of the Orbit processor is to
remove the artfice of a word size. Modern processors
perform computations on a fixed number of bits,
whether it be 8, 16, 32, 64 or in rare cases some
other specific size.

Since there is no predetermined word size, Orbit's
memory layout is also bitwise.

Operands for processing instructions must be in
the form of FROM and TO address pairs, or FROM an
address plus a SIZE.

    ADD A10F:A11F B891:B8A1

    ADD A10F+16 B891+16

[Where to store rsult?]

Stack operations?

    ADD +16 +16

This adds the top 16 bits to the subsequent 16 bits
and puta the result on the top of the stack, which
would be 17 bits including the carey bit.
