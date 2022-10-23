# Human Benchmark

https://humanbenchmark.com
This website has 8 games where you can test various skills you have ranging from your reaction time to short term memory, you can save your results to compare yourself to friends or the entire world with the percentile stat on your profile. As someone who's pretty good at these games, <details><summary>(my stats)</summary>
<p>

![image](https://user-images.githubusercontent.com/96302110/197370437-55811916-0efe-4eec-b034-7a5e101a9f4c.png)

</p>
</details>

i've had my fair share of fun playing them. I thought it would be interesting to put my programming skills to the test by recreating them. 

What started just as a fun exercise for myself soon turned into a challenge as my unhealthy obsession with finishing projects i have started took control over me and forced me to stay up until 2 am fixing errors before the day of my math quiz while suffering from a terrible sickness causing me to have constant coughing fits and headaches. 

(Note to any future employers that might be reading this: Do NOT expect me to jeopardize my own health and wellbeing for your demands just because I have history of doing that even for completely useless projects)

# DAY 1 [(Reaction Time Test)](https://github.com/EgeEken/Reaction)

At this point, i had no concept of "day one" since this is before i made this into a challenge for myself, i decided to make a reaction time test thinking it would be easy enough, and all things considered, it was, the only problem was that this required a lot of precision with your click and the classic time.sleep() function has a lot of issues that come with inputs, most importantly, it saves your input and plays it as soon as the sleep period is over, which meant that by clicking early, you could get basically 0 ms every single time, so i had to improvise and make something that drains a lot of memory and computing power in exchange for fixing this one issue. In hindsight there was probably a way to fix it properly but i was more concerned about getting it done before collapsing in my bed so i'll let it slide.

<details><summary>Demonstration (click here to open)</summary>
<p>

![reaction time gameplay fix](https://user-images.githubusercontent.com/96302110/195985409-5692d1ed-3abd-4a85-bd95-c5d28024be7c.gif)

</p>
</details>

# DAY 2 [(Sequence Memory Test)](https://github.com/EgeEken/Sequence)

For this one, most of my effort went into the planning and design, the bugfixing and tweaking part was surprisingly easy afterwards since i made the base pretty solid. A lot of the code in this served as a baseline for the following three days so i guess you could count some of that planning as part of the other days as well.

<details><summary>Demonstration (click here to open)</summary>
<p>

![sequence](https://user-images.githubusercontent.com/96302110/196301263-31e1ed65-89d0-48f2-b758-50373a658580.gif)

</p>
</details>

# DAY 3 [(Aim Speed Test)](https://github.com/EgeEken/Aim)

This one was easier than the last, but at this point my sickness was getting really bad so it was a struggle nonetheless. Not a lot to note about this one besides that this is the point where i realised "Wow i made 3 of these in 3 days, how about that", still under the illusion that I was in charge and not my crippling obsessive tendencies.

<details><summary>Demonstration (click here to open)</summary>
<p>

![Aim](https://user-images.githubusercontent.com/96302110/196504214-85d8775a-e413-4084-919b-cc26d1671a84.gif)

</p>
</details>

# DAY 4 [(Visual Memory Test)](https://github.com/EgeEken/Visual)

This one was mostly straightforward thanks to the borrowed code from day 2, however, there was one small issue that took me about 3 hours of debugging, erasing and rewriting code, taking breaks due to crippling coughing fits and headache attacks until i eventually settled on a slight improvement and collapsed into my bed. This issue was that your inputs from the previous round would be saved, once again due to, i'm assuming, time.sleep(). While the problem i was attempting to fix is still not fully gone, i believe it is now small enough to not cause any issues in the gameplay of anyone on the off chance that someone actually plays these instead of just going on the human benchmark website.

<details><summary>Demonstration (click here to open)</summary>
<p>

![visual memory gameplay_Trim](https://user-images.githubusercontent.com/96302110/196817239-f9d0f27a-9d6b-4f45-92cf-a2c9b146aa92.gif)

</p>
</details>

# DAY 5 [(Chimp Test)](https://github.com/EgeEken/Chimp)

This one was probably the hardest one conceptually among all of the tests, however, i was feeling much better at this point, so the added boost of concentration from my head NOT feeling like its gonna crack at any moment allowed me to finish up the code fast enough, but as is tradition with these tests, one issue causing boxes to overlap took about an hour of debugging, replanning, rewriting and testing code to be fully fixed.

<details><summary>Demonstration (click here to open)</summary>
<p>

![chimp test gameplay_Trim](https://user-images.githubusercontent.com/96302110/197075859-fe431622-1aae-41fd-baae-e9ab8a9c5fd7.gif)

</p>
</details>

# DAY 6 [(Number Memory Test ](https://github.com/EgeEken/Numbers)and[ Verbal Memory Test)](https://github.com/EgeEken/Verbal)

These two were possibly the easiest ones so i decided to do two in one day, but for number memory i decided to add a nice looking animation for the timer instead of letting the player just guess when it's going to be over or adding an ugly text timer, that took some time but i think the result was worth it. Plus i spent a significant amount of time going through my code over and over again to fix errors, although i ended up finding a solution to the problem thats been in most of the previous ones, which was that the inputs in the waiting period carried over to the play period. This is a problem caused by time.sleep() and the solution was a very crude one but it worked so i'll take it. Verbal memory didn't really have anything fancy that i had to invent workarounds for so it was pretty straightforward. 

<details><summary>Demonstrations (click here to open)</summary>
<p>

![number memory gameplay_Trim](https://user-images.githubusercontent.com/96302110/197221144-029c8fe8-9b3e-40a1-afa8-0dcc2ac0d58b.gif)

![Verbal memory test trim](https://user-images.githubusercontent.com/96302110/197283609-a442cd38-e99d-46c1-aac8-21b7eeed0fd4.gif)

</p>
</details>

# DAY 7 [(Typing)](https://github.com/EgeEken/Typing)

I expected this one to be the easiest, but turns out it is shockingly hard, first off, there is no built in way to wrap text around a screen or even just a given section in PyGame, which is insane already, but also the way i implemented text wrapping made it impossible to make new words wrap the way they should even if we know the length they're going to have, which causes this irritating visual error where the new words will just continue without wrapping until you hit the edge where they suddenly snap to where they were supposed to be from the start, i spent so much time trying to fix this error and i couldn't achieve anything. This is definitely the day where i had the biggest disconnect between the amount of time and effort i expected to spend versus the amount i actually ended up spending. But i am very proud to say that i did it, i achieved my goal, in a week, i recreated all 8 human benchmark games on pygame.

<details><summary>Demonstrations (click here to open)</summary>
<p>

![typing gameplay trim (2)](https://user-images.githubusercontent.com/96302110/197369222-66c8fb94-851f-4f1b-9451-ac3bdea7244c.gif)

</p>
</details>
