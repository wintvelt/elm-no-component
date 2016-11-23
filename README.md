# elm-no-component

An example of scaling Elm, showing how to scale a simple friendlist app.
With components, including drawbacks and pitfalls,
and an alternative - more Elm-like way to scale.

When you have a background in working with components, it can be hard to get used to the
workflow in Elm for organizing and scaling your app.
For me at least - coming from React &amp; Flux, it took quite some time to adapt to the
Elm way.



## Use case
As soon as your first elm app grows beyond one file, you need to make decisions: 
on how to break things down into smaller files.

One route to follow, is to make "components". Reusable fully functional bits of code.
React works this way, but there are surely many other frameworks and libraries
where thinking and scaling in components in the main pattern.

The Elm Architecture (TEA) does not really force you to do it one way or the other.
But using elm without components definitely is a lot easier, more efficient and faster.

Hopefully the example here will help you understand what the drawbacks and pitfalls of
components in elm are.

And more importantly, to provide an alternative approach to scaling and reusability.



## Example friendlist app
The scenario for both versions is the same:

1. Start with a simple page that shows details of 1 friend
2. Add editing functionality: change the details of this friend
3. Add validation to the fields
4. Add validation to the page
5. Add another page that displays a friend list, where you can click to edit details
6. Add functionality to add or delete a friend from the list
7. Improve messages
