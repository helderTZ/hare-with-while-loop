# Hare-with-while-loop

A patch that when applied to the Hare lang repo adds while loop functionality to the Hare compiler.

Because Hare lang does not exist in Github, I can't fork it. So I only commit the patch, this README and an example file that when compiled with the patched Hare compiler demonstrates the while loop working.

> Disclaimer: this was just an experiment for learning purposes.

## References:

- Hare lang: [https://harelang.org/](https://harelang.org/)
- Hare lang repo: [https://sr.ht/~sircmpwn/hare/sources](https://sr.ht/~sircmpwn/hare/sources)

## Instructions

1. Follow the normal installation instructions from the Hare lang homepage (clone `harec`and `hare`, build `harec`)

2. Apply the patch in the `hare` folder (not the `hacec` folder, that is the bootstrap compiler) with `git apply while.patch`.

3. Now you can build `hare` with `harec`.

4. That's it, you can now build the example with `hare build -o while_exm while_exm.ha`.
