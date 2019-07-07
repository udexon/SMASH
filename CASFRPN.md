Next, we use an ongoing project of ours to illustrate how SMASH/FRPN may offer a more concise solution (in terms of line of code) to Godot or similar game engine:

http://5gl.epizy.com/gltf_2019/g_rpn.html

This web page is taken from a three.js tutorial. Modification has been made such that, you follow the instructions below, one of the selected object will start moving:

- Use mouse left (primary) button to select any two objects. 
- Open JavaScript Console. 
- Copy and paste the following commands:

```
ga_init(ga)
ga[0].p.v=new THREE.Vector3(1,0,0)
ga[1].p.v=new THREE.Vector3(0,0,0)
requestAnimationFrame( g_anim );
```

I am sure this is a typical game programming scenario.

What is not typical is the following: instead of "hard coding" the criteria for the objects to "bounce off" the "wall", we wish to *create a computer algebra system which can solve simultaneous linear equations governing the motion of the objects.*

At this point, some readers might dismiss this as overly ambitious. However, as there has been JavaScript computer algebra system like [Algebrite](http://algebrite.org/), porting it to Godot should not be rocket science.

Nevertheless, as the fragmenting programming tools disinetegrate the programmer communities, few programmers would find time to work on extra curricular projects, as they would spend too much time "fire fighting" -- learning and coping with differences of programming tools and platforms -- which is showing no signs of diminishing.

The following are fragments of SMASH/FRPN code for expanding expressions `(a + b)*(c + d)` and `(a + b)*c`, also written in RPN:


```
S.push('a b + c d + *'); 
F("space: explode: hgm: : top_edges t t2sn: cx: over: cx: 1 - \
i: e ix: ; ")
F(": left_terms dup: 1 ix: 5 pick: swap: i: e i: dup: 0 i: \
subt: over: 1 i: subt: ;");
F(" top_edges left_terms 3 pick: 0 i: subt: \\* 1 pick: 4 pick: \
\\* \\+ 7 mss:")

a d c + \* d c + b \* \+


S.push('a b + c *'); 
F("space: explode: hgm: : top_edges t t2sn: cx: over: cx: 1 - \
i: e ix: ; ")
F(": left_terms dup: 1 ix: 5 pick: swap: i: e i: dup: 0 i: \
subt: over: 1 i: subt: ;");
F(" top_edges left_terms 3 pick: 0 i: subt: \\* 1 pick: 4 pick: \
\\* \\+ 7 mss:")

a c \* c b \* \+
```
