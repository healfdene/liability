# Code is a Liability
Business people treat computer source code as an asset, but if you program yourself, you will one day discover that code is a liability. You may refer to “technical debt” as a specific problem that occurs after a rushed job, but the ugly reality is that almost *all* code is technical debt. Here are some simple guidelines for how to manage that heavy millstone around your neck: this is, the liability of all the code you’ve had to write.

## Don’t love your code
It follows that one of the best ways to avoid technical debt is to avoid writing code. To make this work, you have to learn NOT to love your own code. Sure, writing code is fun at first pass. It can even be fun to get all the bugs out and clean your code up.  Adding on to that code is where you get into trouble. If you feel like adding code, just take a deep breath, maybe stop for a cup of coffee, then try deleting some code instead.

Seriously, when you find you need to add a feature to your code, you’ve probably also learned that some existing feature turned out to be unneeded.  Excise those lines first. Then figure how to add your new feature using fewer lines than you deleted. If you get your new feature in while having deleted more code than you added, congratulate yourself: you are indeed a wizard!

It helps sometimes to focus a little antipathy on your code. Sit with it for a few hours, stare at it and tell it, “if you’re going to make my life difficult, there will be a price to pay!” Every line of that code is just sitting there waiting to ruin something fun you would have otherwise enjoyed.

Now spend some time thinking of how to break that code. Write another program to break the one you just wrote. The lines of code in your new program don’t count against your quota – the test code doesn’t add to your technical debt unless you decide to adopt the test like a new puppy. Remember: don’t love your code.

## Other people’s stuff
An important subtext to this is that you can’t delete code unless you know what you are doing. If you are not sure which code paths are obsolete, then you won’t know whether you can delete code. If you find this is the case, then you almost certainly shouldn’t add code either.

One of the fastest ways to incur technical debt is messing with stuff you don’t fully understand. Stay away from other people’s code when you can. If you must work with it, learn it well enough to be able to comfortably delete it a few lines at a time.
If that is not possible, delete whole files at a time (of other people’s code) to avoid the uncertainty.

## Learning things
Is there something you wanted to learn about? Wanting to learn new things is often a danger sign that you are about to take on some technical debt.  Avoid learning on anyone else’s schedule. Don’t learn new tech for an existing project unless you have to (you will know when you have to, since it happens often enough anyway.)

The problem with learning new tech is that you will find yourself messing with things you don’t fully understand, and taking on technical debt unexpectedly when you try to change things (see “other people’s stuff” above.)

When you want to learn something new, relax in your recliner at home and read about it on your iPad. Then grab a laptop and write a bit of code that you plan on throwing away. Savor the experience, and put it out of your mind until you actually need it for a real, hard requirement.

Taking a dependency on a tech that you didn’t really need is a good way to guarantee you won’t enjoy your next vacation. OTOH, cleaning out obsolete dependencies is one of the most enjoyable ways to delete code.

## Generalizing nothing
How do you generalize from a set with one element? Meaningless question, right?

It is a good idea to understand at least two or more complete cases before generalizing. Writing code that appears to be general, prior to having complete knowledge of the cases it must handle, is another way to quickly incur tech debt. When coding, don’t generalize as you go – wait to get at least one complete case right, end to end, before generalizing. In the meantime, keep deleting code so you don’t try to generalize stuff you didn’t need.

## Reuse
The joys of reusing code are way over-hyped. It is far nobler to delete code than to reuse code. Reuse of code that you didn’t need is a false economy. Just because you didn’t write new lines of code doesn’t mean they won’t come back to bite you. Unnecessary code reuse can rapidly expand the number of potential paths through your code. Extra code paths, even when they are dead code paths, will cost you time when you are debugging and troubleshooting code.

All that said, don’t write the same thing twice! Copy and paste is an OK way to lay down a pattern, as long as you have a plan to delete same code later.

## Imaginary users
Thinking about users you don’t already have is another way to get into trouble with tech debt. A common misconception is imagining that there is a programmer in the future that will want to use your general code. If you don’t know someone, right now, who wants to use you code, then there probably isn’t anybody who will really want it now, or ever.

A worse misconception is the imaginary person who will finish your work: that person will see the pattern you laid down, add their special knowledge, and finish the job. That person doesn’t exist either.

## Tools
Tools are wonderful things. We love and hate our tools. Tools are incredibly difficult to do well. Little tools, that aren’t too general and that you know you can use, are great things to write for yourself as you go. The problem is when you expect other people to use a tool you wrote. If other people are going to use the tool, then they will need to have some input: does it work for them? Do they understand it? What do they do when it does not work?

A common feature of tools that that they don’t always work. Writing tools that work for most people, most of the time, is very, very time consuming.

Most programmers have a tendency to like tools: customizing their own tools and writing special purpose tools when it makes sense. Writing tools for someone you haven’t met, or someone in the future, is not likely to come out the way you expect.

## What to do when you want to do stuff
I keep telling you not to do stuff, but you need to finish your project, right? The trick is to not think up new things to do. Instead, figure out what your project needs and do it in the simplest way possible while avoiding technical debt.  Don’t do anything you don’t have to do. If you have extra time, find instead something that you know you will eventually have to do, and do it early (again, in the simplest way possible.) When you get far enough ahead, just start testing your stuff and beating on it in more elaborate ways. When that’s done, test a colleague’s stuff. You may have to be careful with that, and stick to testing stuff written by friends who take criticism well. On no account should you add to your own code just because you have the time. If you feel you really must mess with your stable code, delete stuff from it instead.

## Net value
Notice there is no source code in this Github project? That means it has, at least, a net value of zero, as opposed to the negative net value it would have if I had included code. If you disagree, send me a pull request. ;-)
