## V8, WebAssembly, and the **Future of JS and a Multi-Language Web**

---

## About Me

![left](./img/alladinsane.jpg)

* Robotics Author/Addict
* Developer 🥑
* Twitch streams hardware/software @nodebotanist

---

![left original](./img/ace.jpg)
![right original](./img/Arya.jpg)

---

#[fit] What even is **WebAssembly**?  

---

# What WebAssembly is **NOT**

* just a programming language (it's so much more than that)
* the death of JS (probably)
* something you can just ignore cause it's gonna go away

![inline](https://media.giphy.com/media/eenSmyv5VGhzUNTiWy/giphy.gif)

---

# What WebAssembly **IS**

* A compilation target for other languages to compile to, as well as a language in itself
* An augmentation of the abilities of JS by allowing other languages to operate in the browser
* But most importantly...

---

* Pretty literally\* **magic(k)**

![inline](https://media.giphy.com/media/3o84U6421OOWegpQhq/giphy.gif)

\* - no not really literally but I'll explain later

---

# WebAssmebly is a **compilation target**

* You write code in other languages and compile them into WebAssembly
* Rust, C/C++, Go, C#; these are just a few of the languages with WebAssembly as a compile target

---

## But the question you then have to ask is...

---

![fit](./img/WHAT.jpeg)

---

![fit](./img/WHY.jpeg)

---

## There are *so many reasons* you would want this in your life

---

# THIS IS **A NEW ERA FOR THE WEB**

---

![](https://media.giphy.com/media/h2OLfcSKKthRK/giphy.gif)

---

# No but seriously

WebAssembly is comprable to bringing the power of the JVM and the subsequent LLVM toolchain **into the browser**, creating an **evolution of the web as we know it**.


![inline](https://media.giphy.com/media/A9rtrLGbNZjgc/giphy.gif)

---

![](https://media.giphy.com/media/UnTC9o2HMyUta/giphy.gif)

---

![fit](./img/ancient.png)

---

![fit](./img/then.png)

---

![fit](./img/now.png)

---

![](https://media.giphy.com/media/mgqefqwSbToPe/giphy.gif)

---

# Why does this matter?

* Augmenting JS at its not-so-strong points
* Not rewriting entire codebases to use them on the web
* Fewer calls to the server, less latency, faster web apps

---

# Augmenting JS at its not-so-strong points

Who wants to write a banking app in JS?

If you're running *anything that relies on mathematical numerical accuracy or speed* that meant, until now, another AJAX call to have another language do alllllllll the math. *With WebAssembly*, we can do this in the browser, with, say, Rust.

---

# Other JS not-so-strong points

* Type coercion side-effects: `"" == 0 //true`
* API Overloads:

```
1 + document.getElementById("inputElem").value; // Concatenates
1 + Number(document.getElementById("inputElem").value); // Adds
```

* The mystery that is `typeof`

```
typeof {} === "object" //true
typeof "" === "string" //true
typeof [] === "array"; //false
```

---

## Using WebAssembly means *using the right tool for the job*

---

# BUT THIS WILL KILL JS!!!
![](https://media.giphy.com/media/bldbGnPJiJwli/giphy.gif)

---

# Probably not-- for most situations, it **makes JS better by letting it do what it is good at and ignoring the rest**.

However, WASM toolchains are gaining more and more abilities by the day, and some teams would like to have WASM be able to do everything JS does.

---

## It *makes the web better* by creating better browser experiences

![inline](https://media.giphy.com/media/SbtWGvMSmJIaV8faS8/giphy.gif)

---

# Let's *take a closer look* with a demo

---

# The Demo

* uses wasm-imagemagick
* manipulates images in the browser up to 10x faster than JS can
* Shows the real power of not having to rewrite code and being able to let us use the right tool for the job

---

# But what about *Node.JS*?

---

# Wait...

---

# What *ABOUT* Node.JS?!?!

![original](https://media.giphy.com/media/kaq6GnxDlJaBq/giphy.gif)

---

# Native. Heccin. Modules.

![inline](https://media.giphy.com/media/IYIlvuWc21U4g/giphy.gif)

---

# Why native modules are such a pain

* They have to be recompiled on download
* They either have to compile on every platform OR leave off platforms from support
* Node-Gyp (disclaimer: I respecc the hecc out of their work.)

---

# WebAssembly *Works on Node >= 8.0*

---

![](https://media.giphy.com/media/3o7btPCcdNniyf0ArS/giphy.gif)

---

# WebAssembly Modules in Node.JS

* Are *precompiled for Node.JS*, so they're portable to *any platform that runs Node.JS*.
* No more recompilation on every download on every architecture.
* FOR REALS.

---

> "Everyone wants to [deprecate] node-gyp and WebAssembly would allow us to do this"
-- Laurie Voss, a few weeks ago

---

# How do we get to this magickal land?

* WASI (Web Assembly System Interface) is being actively worked on an allows WASM to make system-level calls. It's by no means complete yet, but worth keeping an eye on!
* WASI is helped along by the fact that the Node V8 sandbox is the same sandbox being worked on in a few major browsers.

---

# WebAssembly is even invading serverless

![inline](./img/logo-wordmark-horizontal.png)

---

# We have a free tier now!

![inline](./img/qr.png)

(I'll show this again later)

---

# The point of this talk

* Try WebAssembly (I personally really like Rust)
* WebAssembly is the future of JS in all its forms
* If you are a hiring manager; *hire someone who is different from you*. Just go and do it.

---

![inline](https://media.giphy.com/media/jndc0TQq9fvK8/giphy.gif)

---

# Thanks for listening!

![right](./img/qr.png)

![inline](./img/carl-sagan-youre-awesome.gif)

* kas@cloudflare.com
* @nodebotanist
* https://github.com/nodebotanist/austinjs-july-2019
