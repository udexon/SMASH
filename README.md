# SMASH

## Stack Machine Shell Programming

### Stack Machine Shell: the Most Overlooked Secret Weapon in Computer Programming

:: readers want to know the benefits (or purpose) by reading this article, not some abstract ideas that they cannot use, or need time to understand

> *Now imagine, LibreOffice has a "debug shell", with complete features of GDB, that can be brought up like a Browser JavaScript Console.*

Shell: developed by Unix in 1970s, for "large" computers. Forth was ported to "small" computers since 1968? dc ?

Shell, perhaps the first and the most common user interface any programmer would come across. 

Stack, perhaps the one of the most common and the first concepts any programmer would learn and never use it consciously again. 

What if you are presented with a shell whose fundamental mechanism is built upon a stack machine?

[ SMASH for Ajax ]( http://5gl.epizy.com/nsm/fgl.html?i=3 ): Describe ....

Stack machine is one of the most fundamental mechanisms in computer systems, which can be found in places from microprocessors to programming language interpreters. 

We demonstrated that a stack machine shell (SMASH) can be implemented in high level programming languages like JavaScript and PHP with as few as around 50 lines of code, and by extension, in other equivalent high level programmming languages. SMASH operates similarly to a Forth program, using Reverse Polish Notation. It uses indirect threaded code to access all functions within the host program. Consequently, SMASH enables a host program to be modified during live execution, with complete functionalities of a debugger.

So what does that mean to an "ordinary" reader who might be a programmer like you? 

Can you imagine having access to the source code of Google search engine or Facebook?

Theoretically, any and all source code that is worth learning, excluding perhaps Microsoft Office, are published on github.com or other open source repositories. 
As such, "having access to the source code" is not much a big deal.

However, having a GitHub repo set up and run locally, then attempting to modify it to produce useful result is another matter altogether. 
e.g. One might have a good idea on how to improve LibreOffice. 
However, the effort to set up and develop LibreOffice locally might put off 999 out of 1000 interested programmers.

Now imagine, LibreOffice has a "debug shell", with complete features of GDB, that can be brought up like a Browser JavaScript Console.

And, not only ALL open source programs like LibreOffice can have a stack machine shell (SMASH) which has the full functionatlities of GDB, the programming language that can be used to modify the host program is a Forth like Reverse Polish Notation (fRPN), a programming language whose difficulties to learn are no more than a reverse polish calculator, or a spreadsheet formula. 

Would that the best thing since the invention of the Internet itself?

Next, imagine the stack machine shell (SMASH) is not only available in LibreOffice, but any Facebook or Google "wannabe" open source clones. 
SMASH can be used as the interface on the web application or mobile application, to modify front end and back end functionalities, on the fly, without having to download the complete source code and set up the repo locally.

How long will it take for free software programmers to produce worthy clones of MAGA/F (Microsoft, Amazon, Goolge, Apple, Facebook) with SMASH if it is available "everywhere"?

Fastest way for Godot, or any other Programming Language,  to develop computer algebra system is CASPAROV?

Make this as main selling point in this article. 

Let us look at some issues surrounding Godot game development to illustrate the benefits of SMASH.

As programmer population and investment in open source projects grow, we witness many interesting breakthroughs such as the Godot game engine. 
Nevertheless, these projects invariably inherit many chronic ills in computer programming, which of course cannot be blamed on the core developers.

One of the primary tolerated ills would be the choice of programming language. From [ Godot's own web page ](https://docs.godotengine.org/en/3.1/getting_started/scripting/gdscript/gdscript_basics.html):

> In the early days, the engine used the Lua scripting language. Lua is fast, but creating bindings to an object oriented system (by using fallbacks) was complex and slow and took an enormous amount of code. After some experiments with Python, it also proved difficult to embed.

> The last third party scripting language that was used for shipped games was Squirrel, but it was dropped as well. At that point, it became evident that a custom scripting language could more optimally make use of Godot’s particular architecture.

Similar issues occur in other projects such as node.js, Angular etc.

In summary, every platform seems to have its own programming language. This seems to be a problem as entrenched as the biblical tower of Babylon (Babel). 
SMASH FRPN or ISYA as described in this article can be the be all and end all solution to the problem of the (programming) tower of Babylon. 

f.RPN F.RPN FRPN fRPN

> Just an unrelated joke to make readers remember the acronym FRPN: Bill Gate once wrote a paper on the pancake sorting algorithm. 
FRPN might sound like a frying pan, used to fry and flip (sort) the stack (!!) of pancakes

SMASH/FRPN might be the solution all API developers are looking for. 
It provies a language independent interface for programmers who intend to use a particular API, written in a particular programming language. 
API developers may continue to develop a library or API in a particular programming language. 
Programmers who are API users will only need to understand SMASH/FRPN in order to access the API.

Our proprosal for SMASH/FRPN does not require universal approval from all API developers.
A SMASH/FRPN interface to any API will typically take a week for a programmer working on part time to complete, as demonstrated with our JavaScript and PHP SMASH demo.

http://localhost/gltf_2019/g_rpn.html

Use mouse left (primary) button to select any two objects. Open JavaScript Console. Copy and paste the following commands:

```
ga_init(ga)
ga[0].p.v=new THREE.Vector3(1,0,0)
ga[1].p.v=new THREE.Vector3(0,0,0)
requestAnimationFrame( g_anim );
```

:: start new sentence on new line. easy to edit.

While writing this article, we attempt to reconcile a historical mystery concerning Unix shell and Forth (stack machine): Why has the stack mechanism used in Unix dc (desktop calculator) not succeeded in the various shells hence developed?

Could it be as simple as as "their paths did not cross", or was there some other more important reasons?

We may leave this mystery to readers with more resources or historical insights. A brief mention of it should present the readers with an interesting overview of issues concerned.


Programming Languages are like religions and ideologies, garnering enthusiastic followers while fragmenting the communities without anyone being concerned at the lost of productivity that has been accumulated over the decades. 

The fragmentation of Programming communities has not been in the limelight as the absolute base of programmers has been growing literally exponentially during the past few decades, only to be met with declining profit forecast by tech giants in recent quarters. 

Using a Forth like Reverse Polish Notation syntax, SMASH can be deployed as a "unifying script" across programming languages. 

Amongst the hundreds of Programming Languages that have been developed over the decades, Forth stood out as being frequently implemented as a "shell script" within a host Programming Language. Google "Forth" together with any other host programming language, you would find a GitHub project that implements Forth within the host programming language, from Java, JavaScript to PHP and Python. The list goes on to include Rust, Haskell, Go, C, C++, LISP and of course, the mandatory assembly language of any microprocessor. 

This would remain a mere curiosity in the relatively short history of computer programming had it not been formalized theoretically and found more useful applications. 

Formalized as inverse shunting yard algorithm

Dijkstra's 1961 paper describing the inverse shunting yard algortihm, as part of the ALGOL project, can be seen as the common ancestor of all programming language design. The inverse process, transforming Reverse Polish Notation (RPN) expressions into a host programming language, can be called the "inverse shunting yard algorithm" (ISYA). We believe ours is a novel attempt to describe ISYA formally, although implementations on individual programming language have existed independently, but most, if not all, have not been developed beyond the point of demonstrating how Forth can be implemented in a host programming language.

We believe that the Forth like Reverse Polish Notation employed  in stack machine shell (SMASH) has the potential to become a "universal script" which can be learned by programmers and non-programmers alike, including mathematicians and students studying mathematics. 


Show examples:

[ SMASH for Ajax ]( http://5gl.epizy.com/nsm/fgl.html?i=3 ): Describe ....

[ SMASH CASPAROV: Distributive law ]( http://5gl.epizy.com/var/www/html/gltf_2019/g_rpn.html )

Kotlin Android

Python?

etc?









