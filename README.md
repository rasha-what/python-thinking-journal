# python-thinking-journal
A collection of my Python learning journey, coding experiments, and programming thoughts. 

Thinking in Python 🐍
Why this repository?

I started learning Python from scratch. Instead of only uploading projects, I wanted to document the moments where my way of thinking changed.

This repository contains:

- Programming exercises
- Small projects
- Questions I asked
- Better solutions I discovered
- Things that surprised me
- My own observations while learning

My goal isn't to become someone who memorizes Python. My goal is to become someone who thinks like a programmer.

=========================================

First Thought 💡 

While solving a problem that printed even numbers from 0 to 10, I noticed something. The common solution was:

for i in range(11):
    if i % 2 == 0:
        print(i)

Then I asked myself: Why should Python check every number if I already know that every even number plus 2 is another even number? So I rewrote it as:

for i in range(0, 11, 2):
    print(i)

Because? Every even number + 2 = another even number! 
Instead of visiting every number, it simply skips the odd number. 

While solving a problem to print even numbers, I realized that I didn't need to check every number. Since every even number is exactly 2 greater than the previous one, I could use range(0, 11, 2) instead of looping through every number and testing i % 2 == 0.

Here comes the topic of Code Optimization...

While solving a simple problem of printing even numbers, I realized something interesting. My first solution checked every number one by one to see if it was even. Then I stopped and asked myself:

"Why should Python check every number when I already know where all the even numbers are?"

That led me to a different solution using range(0, 11, 2), where Python jumps directly from one even number to the next. The output is exactly the same, but Python performs less work because it skips all the odd numbers instead of checking them individually.

===================================
**Of course, I understand that not every problem can be solved through pattern recognition or optimization. However, exploring these possibilities is part of what makes learning Python so fascinating to me.**
===================================
