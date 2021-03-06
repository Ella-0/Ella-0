
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
-->

### Hi there 👋

I’m currently working on [Iglunix](https://github.com/iglunix/), a Linux (and in the future other kernels) distribution with no GNU components. This includes work on a reimplementation of GLib and a simple, WIP bootloader that can be built with an LLVM toolchain. Currenty GNU make is the only GNU package included; unfortunately there are no complete reimplementations of GNU make however [kati](https://github.com/google/kati) has implemented a fair portion of GNU make, [Lightning Creations](https://github.com/LightningCreations) aims to implement GNU extensions in LC-Make and [toybox](https://github.com/landley/toybox/) aims to have an implementation of GNU make. I have got simple GUI applications running with various Wayland compositors however there are still some issues here. I some of the issues are caused by a lack of udev. Instead I'm using [libudev-zero](https://github.com/illiliti/libudev-zero) which does implement everything yet but I do plan on contributing to it when I wrap my head around the way udev works. Currently no web browsers run; I'm currently working on implementing the various GNU APIs required by the WebKit WPE (and maybe GTK if I get around to reimplementing that) port to get that running. This means reimplementing GLib and Fribidi (I'll probably make a wrapper around [Servo's Bidi](https://github.com/servo/unicode-bidi) implementation for this).

I'm also working on a programming language called [grime](https://github.com/Ella-0/grimec). Unfortunately the compiler isn't really in a very usable state and I've changed the syntax quite a bit. The following is a classic example:
```grime
mod!(test::hello_world)

use!(std::Env)

pub fn main(env: &Env) -> Result((), NotZero(u32)) {
  env.stdout.println("Hello, World!");
  Ok(())
}
```
The syntax is very similar to Rust and will have a similar borrow checker but also intends to include the compile time flexibility of Zig.
