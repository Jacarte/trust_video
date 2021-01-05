# Script

Usually when a computer executes a program, this program first came from a compilation pipeline and what we execute in our program is an instantiation of the generated binary. Exactly the same instructions and exactly the same behavior are executed in the client computers. In a world scale, we have several equal million instances distributed to the clients. We call this "Software monoculture". 

Software monoculture has several benefits, such as maintenance, interroperability and certifications since you only need to make the changes to your application once and then distribute the binary. However, when you distribute the same binary along all your computers, you are also distribution unknown security flaws. A potential attacker can analyze this code, discover theese flaws and then create and attack. And following the same idea, the ttack can be delivered to the million deployed instances, exfiltrating data, for example. This this kind of attacks, we called "Break once Break everywhere".

How can we mitigate tis threat ? If we distribute a different binary, yet with the same functionality we can break potential attacks. For example, if we distribute different instructions making the same functionality of the orginal program, signature based attacks could be ineffective. The main limitation of this technique is that you need to scale the number of different variants to a real world scale as fast as a potential attacker can analyze and discover new flaws. Besides, you need to take care about creating new vulnerabilities. The technique needs to be safe and sound. We call this defense technique, "Software Monoculture"

 

