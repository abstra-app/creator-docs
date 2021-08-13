# References

When using expression mode you might stumble upon a difficult task: how to reference something other than [variables](https://docs.abstra.app/docs/front-end/variables), something that is not in the context?

For this task Abstra has a different approach: we use references. A reference is a "link" that points to another entity and exposes its properties and methods in a context-like variable accessible in expression mode.

You can reference four types of entities:

* Variables
* Components
* Interfaces

For example:

In the `Page or component` argument of a [Subview element](../elements/subview.md) you can enter expression mode and create references to other [components](../components.md) and create a logic to dynamically switch them with code:

![](../../../.gitbook/assets/referenceinteface.gif)

