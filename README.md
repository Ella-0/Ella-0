
<!--
**Ella-0/Ella-0** is a āØ _special_ āØ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- š­ Iām currently working on ...
- š± Iām currently learning ...
- šÆ Iām looking to collaborate on ...
- š¤ Iām looking for help with ...
- š¬ Ask me about ...
- š« How to reach me: ...
- š Pronouns: ...
- ā” Fun fact: ...
-->

### Hi there š

I'm Ella (She/They) and I'm currently working on several projects mostly as part of the
[Iglunix](https://github.com/iglunix/) Linux distribution (Linux with none of
the GNU).

### Iglunix
Iglunix is a Linux (and in the future other kernels) distribution with no GNU
software included. It aims to become selfhosting with no GNU components
currently the only thing stopping that is the lack of a make implementation
that implements enough of the GNU extensions to build the Linux kernel and Musl
with no issues. The following are potential candidates for that:

 - [makers](https://code.boringcactus.com/makers/)
 - [kati](https://github.com/google/kati)
 - [lc-make](https://github.com/LightningCreations/lc-make)

### WebKit
As part of Iglunix, I'm working on a WebKit port (WPM) that aims to be portable
accross many *nix operating systems and not depend on any GNU software. Other
WebKit ports that would otherwise satisfy Iglunix's needs such as WPE depend on
GLib.

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
