### Awesome List of PLT Papers

#### Interpreters and VMs


+ _"A Portable VM-based Implementation Platform for non-restrict Functional Programming Languages"_ by Jan Martin Jensen & John van Gronigan. This paper discusses implementation of `asm.js` which was widely used to run C code (such as DOOM) in browser pre-WASM. Discusses architecture of the VM which you can use to implement your own.

+ _"Optimizing code-copying JIT compilers for virtual stack machines"_ by David Gregg and Antol Ertl. This paper discusses how you can use C code to create JIT. Basically, instead of using an Assembly framework like libkeystone to just-in-time compile your JIT code, you can use C code instead, hence "Code-copying". Ertl is one of GForth's authors by the way, and creator of VMGen. So he knows something about language VMs.

+ _"The Essence of Meta-Tracing JIT Compilers"_, a thesis by Maarten Vandercammen. This thesis explains whatever there is to know about Meta-tracing. PyPy is, for example, a meta-tracing Python interpreter. In a simple Tracing-JIT interpreter, you 'trace' busy parts of the code (mostly loops) and you generate machine code for them, and optimize it as you go. In a 'Meta-tracing' JIT, you hand it off to another interpreter to trace it for ya. PyPy uses a subset of Python to do that.

Have fun reading.
