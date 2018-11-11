---
title: "Taking Control with Switch Statement"
date: 2018-11-07T11:40:11+02:00
publishdate: 2018-11-07T11:40:11+02:00
image: "/images/blog/switch.svg"
tags: ["coding", "switch"]
comments: false
ReadingTime: "7"
AuthorName: "Akshay"
Description: "The Blog Creator"
Thumbnail: "/images/akshay.jpeg"
Summary: "This is gonna be a good read if you have just started coding recently or are not much familiar with switch Statement.This would be concept booster for your switch statement knowledge."
---
<!-- # Taking Control with Switch Statement -->

This is gonna be a good read if you have just started coding recently or are not much familiar with `switch Statement`.

If you are a pro or you think you are familiar with `switch statement` then scroll down to the link at the bottom, you may find something new.

  

So let us begin, when we begin to learn coding we come across topics like variable assignment, declaration, and control structures, loops and all.

  

I believe switch statement would be really confusing topic in control structures, so let’s simplify it

Switch statements are an other way to write if-else  code (but it's limited, you can only switch on integral values, or char value as it works for a single variable)

A thing to note is that C doesn't support switches on strings ,while other languages like Java support it.

The above explanation would become clear with this example

Example:

    if (a == 0) {  
    // First case  
    } else if (a == 1) {  
    // Second case  
    } else if (a == 2) {  
    // Third case  
    } else {  
    // Default case  
    }

  

With switches:

    switch (a) {  
    case 0:  
    // First case  
    break;  
    case 1:  
    // Second case  
    break;  
    case 2:  
    // Third case  
    break;  
    default:  
    // Default case  
    break;  
    }

  

Note an important thing:

`default` is essentially the same as else in an `if - else if - else` chain.

the `break;` statements at the end of every case. This means that after the code in that block is done we break out of the switch statement, and resume execution at the next statement after the switch.

If there's no `break`, it will continue running code line by line. The case statements are simply labels. For instance, in the example below, if a was 2, and as we removed all break statements, the code for statement 1,2, 3,4, and the default case would all run.

If you want to have the same code to execute for multiple cases you can leave the break off, like so:

    switch (a) {  
    case 1:  
    case 2:  
    // Code for first and second case  
    break;  
    case 3:  
    case 4:  
    // Code for third and fourth case  
    break;  
    default:  
    // Default case  
    break;  
    }

  

All the above points are summarised below, take note of this important points while dealing with switch statement.

 - The expression in the switch should be a constant value otherwise it
   would not be valid.
   
 - The Switch statement can work without default statement

    
 - The break statement is used inside the switch to terminate the
   sequence of code execution, the switch terminates, and the flow of
   control jumps to the next line following the switch statement

 - If there's no break, it will continue running code line by line
 - The default block can be placed anywhere.
 - You can write a switch statement inside another switch statement, but
   its not advisable as it can get real messy.

#### Whew that was too much of a switching for a day. I hope you understood  the topic..

**As I said above, the Pro folks have a look at [this article](https://embeddedgurus.com/stack-overflow/2010/04/efficient-c-tip-12-be-wary-of-switch-statements/) you may find something new. If you are beginner then don't read it, you may get confused**
