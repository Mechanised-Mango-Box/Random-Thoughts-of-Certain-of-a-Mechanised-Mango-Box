# GDScript - First Impressions
> A review of my first impressions of Godot's scripting DSL

---

## Preface
Having now used GDScript now for two game jams and attempted to use it for side projects, I believe now would like reflect on my experiences of Godot 4. And what better than GDScript. That said, I feel it is best to explain my use cases to add context to by opinions.

### Projects made with GDScript
- **Side Project** (Arena, Couch PvP, Side-scroller)
- **Game Jam 1** (Strategy, Casual/Simple)
- **Game Jam 2** (Strategy, Casual/Simple, Surival)
> Note: Web export only works for GDScript at the time that this was written (Godot 4.2.1)

## Experience
### The Positives
- The initial development speed with GDScript was indeed quite fast, and there were not too many complaints overall.
- The extra features such as being able to get a node via its local path being quite useful for rapid prototyping.
- Editor intergrations with the built-in editor also were nice QoL.
- Lots of helper nodes to fill in the feature gaps
- Explicit declaration
### The Negatives
- Not having static typing leads to issues as a project grows
	- Type hinting does not offer enough safety
	- Dictonaries are not typed
	- Refactoring is much more dangerous
	- Duck typing's benefits do not outweigh its detriments
- Only one battery included, the standard library while it does cover most use cases, still lacks support for lots of commonly used items
- Having to use autoload to fix the issue of singletons
- No access to external frameworks/libraries

## Summary
While I do appreciate the ability to rapidly prototype, I cannot see myself using GDScript in the future for any project that is code heavy. Additionally, prototyping in C# is often no slower than in GDScript while offering far greater scalbility leading to even less of a reason to use it. The few advantages that GDScript does have over C# do not justify its usage.

That said amazing things can happen in any language!

---

## Additional Notes
### For Beginners
While most sources that I have come across mentioned that GDScript is easier to learn (perhaps due to its similarity to Python), I disagree with that and argue that C#'s stricter compliler helps engrain good habits and ideas that may not be immediately obvious in GDScript. However, the lack of resources and documentation to Godot specific issues in C# may be an issue. However one should aim to learn 「programming」 not 「a language」.
### Insignificant Issues
*There are some issues that I take with GDScript that I did not mention above, however I have deemed them to be mostly preference / not worth arguing for*
- Significant Whitespace - Personally dislike this but it is not a dealbreaker, just an inconvenience
- Performance - Not that big of an issue given that C# will GC, adn that more gains can be generally made through better optimised code
- Export Platforms - While not insignificant per say, it should not be taken that GDScript is better due to it having web export but rather that C# is missing web exports and that the goal should be to have platform parity.
- Learning Resources - this will come in due time for C# and can be converted from GDScript with ease, on the other hand, programming knowledge is also not language dependent (although the ease of application may)
