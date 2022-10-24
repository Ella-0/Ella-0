
<!--
**Ella-0/Ella-0** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...


### Grime

I'm also working on a programming language called
[grime](https://github.com/Ella-0/grimec). Unfortunately the compiler isn't
really in a very usable state and I've changed the syntax quite a bit. The
following is a classic example:

```grime
mod test::hello_world;

use std::Env;

pub fn main(env: &Env) -> Result((), NotZero(u32)) {
  env.stdout.println("Hello, World!");
  Ok(())
}
```
The syntax is very similar to Rust and will have a similar borrow checker but
also intends to include the compile time flexibility of Zig.

-->

### Hi there 👋

I'm Ella (She/They) and I'm currently working on several projects mostly as part of the
[Iglunix](https://github.com/iglunix/) Linux distribution (Linux with none of
the GNU).

### AGXV
AGXV is a Vulkan driver for Apple Silicon Macs intended to be used in Asahi Linux.

### Iglunix
Iglunix is a Linux (and in the future other kernels) distribution with no GNU
software included. It aims to become selfhosting with no GNU components
currently the only thing stopping that is the lack of a make implementation
that implements enough of the GNU extensions to build the Linux kernel and Musl
with no issues.
