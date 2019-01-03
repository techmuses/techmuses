---
title: "Lets Take Jump With Goto Statement"
date: 2018-11-07T11:40:11+02:00
publishdate: 2018-11-07T11:40:11+02:00
image: "/images/blog/goto.jpg"
tags: ["coding", "goto"]
comments: false
ReadingTime: "6"
AuthorName: "Adarsh"
Description: "The Evangelist"
Thumbnail: "/images/adarsh.jpg"
Summary: "This article will be beneficial for the rookies and will be a sure concept booster if you are encountering with goto statement first time."
---
Have you heard of goto? Goto statements are simple.

Goto statement is also said to be unconditional jump statement as it can jump forward as well as backward but here we are showing example of forward jump but backward jump is similar to foreward jump only.

You can imagine Goto as taking a jump to somewhere else in your code like in some fantasy terms I can say that teleporting form one point to another point but not random but where you have decided.

So first you have to decide where to teleport or jump by making a lable :-

First, you put a label somewhere:

    int x = 0;
    foo: x += 5;

Here,  `foo`  is a label for the  `x += 5;`  statement. If you jump to  `foo`, you jump directly to  `x += 5;`.

To jump to  `foo`, you can do  `goto foo;`,

 For example:




    if (x < 8)
    
    goto foo;

so here when your code will read `if` statement and it if will satisfy it then it will jump to our decided

    foo:
    
    x += 5;

so now value of x will be 5 as it was earlier decided as 0 and will add 5 to it as written in goto (foo) statement.

generally peoples get confuse between `goto` statement and switch statement but the difference between them is `switch` statements are controlled form of `goto` statements thats why they are known as controlled statements.

Its asctually better to have control in your program as you can direct its flow 





The switch body can contain special labels of the form case n or default, where n is a compile-time constant number, and can contain break; statements which jump to the end of the block. When the switch statement is entered, the corresponding case n label is jumped to depending on the value switched on; if none matches, then the default label is jumped to. If there is no default label, the whole statement is skipped.

You might have heard that goto is typically not a good idea in practice, and that's true. switch statements aren't as bad because you're far more limited in what you can do, but you still shouldn't do anything too crazy with them.



If your code goes in if statement and it satisfies it than it will jump back to the previous defined label of foo: and if false comes than there is no problem and your code will continue its actions.



