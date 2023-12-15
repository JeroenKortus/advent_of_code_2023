# Advent of Code 2023
This repository contains my solutions for the advent of code challenges of 2023. My first year participating in this event!

# Reflection (29/30⭐)
I was made aware of the existence of this cool challenge by a colleague who thought this would be fun for me... She was right! In this file I'll briefly reflect on each day of the challenge. Going into this my goal is just to try to complete the challenges each day using my own ideas and skills and not worry too much about being among the first to complete it or write beautiful and optimized code. I do however, want to complete the daily challenges on the day of the release, by myself.

## Day 1 ⭐⭐
The first day was about learning how advent of code works. I read the fun introduction texts, rules and learned that everyone has their own input and respective output. The challenge itself was very simple.

## Day 2 ⭐⭐
The second day was also an easy challenge. All information needed per line was neatly organized in the input and was easily usable.

## Day 3 ⭐⭐
The third day was a bit more tricky. The input was no longer just some lines with all information neatly presented, instead it was a 2D grid. Taking some time to set up a function that would correctly perform a check around a certain location on the grid made solving the first part not that difficult. For part two working with what I already had made me go overkill to set up two classes to store some information in. All in all not too much trouble on day 3, just some extra lines of code.

## Day 4 ⭐⭐
The first part of the challenge on day 4 was very easy again. By not thinking too much and just jotting down some code I ended up with the correct answer. Looking back at it, calculating the answer could have been done a lot easier. The second part was a bit more tricky. Keeping track of the new cards and processing them all individually showed me that in this challenge, writing efficient code, and more importantly, coming up with efficient solutions was something that could play a role in certain challenges. Still, I solved part two by brute forcing my way to an answer. (and having to wait 1m 29s for my code to finish...)

## Day 5 ⭐⭐
With the lesson learned from yesterday's part two I tackled day 5. Part one, as usual, was relatively easy. Checking the numbers one by one across the categories lead to an answer in no time. Part two proved to be the first real challenge in advent of code. Using the code I already had, I naively adjusted it a little to check all numbers in the ranges one by one. After noticing it took quite some time to process the input and doing some calculations, I realized that the code would need to run for about 18 hours for it to find an answer. Wanting to be done with the challenge the same day and not have my laptop work extra hours, I instead went with the approach of checking ranges of numbers. The implementation of it took some effort as my brain, tired from working that day, kept messing up the indexing of ranges. In the end the code ran in less than a second which is a lot faster than 18 hours, according to my calculations!

## Day 6 ⭐⭐
Day 6 is the day with the least lines of code so far. Reading the challenge I started thinking back to math class and how parabola's and intersections worked, but before thinking too hard opted to try the brute force approach first. This turned out to be very easy for both parts, part two still only taking 10 seconds to run.

## Day 7 ⭐⭐
The entirety of day 7 was pretty simply solvable by using a function to dictate the outcome based on the number of unique cards. Sorting the cards using a lambda function was something I hadn't done before, but was happy to have learned.

## Day 8 ⭐⭐
Part one, again, simple. Part two I continued with the code created in part one. This meant I was on the path of brute forcing it again... Who would have thought. After running it and thinking about what I had started, I realized this could take a while and started considering other options. I quickly checked what was happening and noticed that the paths from the different starting locations all looped past the end point in different sized loops. So by finding the least common multiple I eventually got the answer. Which saved me a couple of trillion loop iterations (not something that would have been done running the same day).

## Day 9 ⭐⭐
Day 9 was one of the easiest of all days. Part one I created some simple code to go down the sequence to the list of zeros and back up again adding an extra entry to every list. To my surprise, part two required the same thing only at the start of the list. This was easily done by changing a few indexes in my code.

## Day 10 ⭐⭐
This challenge is my favorite so far and might turn out to be my favorite of the challenge. For part one I created a function that would return the next step based on the current pipe configuration. This meant defining the connections for the six different types of pipes. My favorite part was part two. After reading the challenge I had no idea how to go about doing it, but after doing some thinking I came up with a plan. I expanded the grid and connected the pipes back up again so that all 'outside' cells would always be connected and making sure no edge coordinates contained part of the loop. Then I extracted the region that included [0,0] (as it is sure to be an outside cell). This gave me a grid where every cell is known to be either inside, outside, or part of the loop. In the end I downscaled the grid to its original size while keeping the information, giving me the number of inside cells.

## Day 11 ⭐⭐
The entirety of day 11 was knowing how Manhattan distance works. Knowing this, solving both parts is easy. For part one I opted to expand the array, as it couldn't get too big to handle. For part two I changed this approach because it wouldn't fit in memory if done the same way. But because the expansion only happened on the empty rows and columns, performing the calculation on the original array and just adding 999999 for each empty row/column crossed worked perfectly.  

## Day 12 ⭐✖️
Day 12 was again a classic "brute force part one, gets too big for part two" scenario. This time I could not figure out how to do the second part. After trying some bits and bobs I gave up for the day and looked up solutions of others. All of them used something called dynamic programming, which is something I wasn't familiar with. So for this advent of code I was not able to use it to solve part two of day 12. But I will look into it in the future as it seems like a useful skill to learn.

## Day 13 ⭐⭐
Day 13 did not give me too many problems. For part one I split up the code in finding the duplicate rows and columns that are next to each other and in the next step determining if it was a mirror image. This code I used again in part two to get the "original" mirroring rows/columns. In the next step I found all rows and columns that are next to each other that have a maximum of 1 differing character. Final step was to determine for all matching pairs that were not the original if they could be a mirror image if only one thing was changed (or just checking if it has exactly one different character).

## Day 14 ⭐⭐
For part one I made three nested loops that would iteratively move all rounded rocks. I made sure to start at the north so that a place could become free for a rock in the next layer. For part two it was impossible to run it a billion times using the same method. Just like in day 8 it was key to find where the grid would turn into a configuration that was seen earlier and using this repeating pattern to calculate what it would look like at cycle 1.000.000.000. I did have some trouble getting this right as my first cycle was cycle zero and not one, which gave me the wrong answer.

## Day 15 ⭐⭐
On day 15 both parts were easy. In python the `ord()` function can be used to get ASCII values, which makes it easy just to create a simple loop and compute the answer. For part two a bit of organizational skills were needed. But using nested dictionaries and relying on the fact that they have an order to them made it easy to compute the answer for part two.

## Day 16 

## Day 17 

## Day 18 

## Day 19 

## Day 20 

## Day 21 

## Day 22

## Day 23 

## Day 24 

## Day 25  
