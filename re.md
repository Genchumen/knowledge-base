---
title: Reverse Engineering
---

# GNU Debugger

# Cutter


# Address Space Layout Randomization

As the name suggests, ASLR randomizes the address space of a
program. Doing so helps mitigate the use of buffer overflow
jumps into functions and NOP sleds.

## Disabling

ASLR can be disabled with `echo 0 | sudo tee /proc/sys/kernel/randomize_va_space`


# Stack Protection

Buffer overflows cannot be performed on binaries compiled
with most modern toolchains with default settings.

## Disabling

For gcc and clang, stack protection can be disabled with the
`-fno-stack-protector` option.
