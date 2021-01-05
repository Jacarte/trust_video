# Script

Usually when a computer executes a program, this program first came from a compilation pipeline and what we execute in our program is an instantiation of the generated binary. Exactly the same instructions and exactly the same behavior are executed in the client computers. In a world scale, we have several equal million instances distributed to the clients. We call this "Software monoculture". 

Software monoculture has several benefits, such as maintenance, interroperability and certifications since you only need to make the changes to your application once and then distribute the binary. However, when you distribute the same binary along all your computers, you are also distribution unknown security flaws. A potential attacker can analyze this code, discover theese flaws and then create and attack. And following the same idea, the ttack can be delivered to the million deployed instances, exfiltrating data, for example. This this kind of attacks, we called "Break once Break everywhere".

How can we mitigate tis threat ? If we distribute a different binary, yet with the same functionality we can break potential attacks. For example, if we distribute different instructions making the same functionality of the orginal program, signature based attacks could be ineffective. The main limitation of this technique is that you need to scale the number of different variants to a real world scale as fast as a potential attacker can analyze and discover new flaws. Besides, you need to take care about creating new vulnerabilities. The technique needs to be safe and sound. We call this defense technique, "Software Monoculture"

 
The web context is probably the greatest example of what a monoculture is. Every time you load a page, this page contains the same resources gathered from a server. All of them are executed the same way with the same expected functionality. In 2017 a new language was added to this context, WebAssembly. WebAssembly is meant to be used as a fast language, fast enough to have native performance in the web. In fact, the community is growing ots adoption and several languages and frameworks are being migrated to WebAssembly. For example, C, C++, Go and Rust or  QEmu and Blazor.  It is also meant to be safe, but recent works show that WebAssembly is not excempt of vulnerabilities. Our approach to tackle, yet undiscovered, porential vulnerabilities, by providing several variants of Webassembly given a program source code.

Going back to how Web works, every client that ask for a WebAssembly program to the servers, we can serve a different variant each time. This is the goal of our approach. To provide software diversiy to the web through WebAssembly.
 
