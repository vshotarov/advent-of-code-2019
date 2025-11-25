## All my solutions for [Advent of Code 2019](https://adventofcode.com/2019) in Python 2
Although I have used python 3 for some of them, I've not used any backwards incompatible features, so if anyone ever wants to run these solutions, make sure you are using python 2.

After all, AoC 2019 took place literally in the last month before Python 2 reached it's end of life.

![Screenshot of the final look of my Advent of Code 2019](AoC_2019.png)

### Reflections
#### Ones I struggled with
I am happy I was able to solve almost all of the tasks without having to look for help. The two that I had to look up are:

- [Day 16: Flawed Frequency Transmission](https://adventofcode.com/2019/day/16) - Although I had some inclination that at the middle point it's all ones and then zeroes start creeping in from the left, I wasn't able to fully wrap my head around it at the time. It all made sense when I saw some on the subreddit describing it with a diagonal matrix.

- [Day 22: Slam Shuffle](https://adventofcode.com/2019/day/22) - I solved part 1 with a very naive list implementation and, even though, I could see what needs to be done I wasn't aware of the *Modular inverse* operation, so I had to look up how to solve the *deal with increment* function.

#### Breadth-first search
Since there were a lot of path finding tasks I got to use it quite a bit which I enjoyed.

I had heard the term before, but I hadn't really put much thought in it. Once I solved the first path finding task (the oxygen one) and looked up people's solutions I realized what I was doing is actually BFS.

The one thing I was missing initially was that I was doing it recursively, so exploring each neighbour would fire off a recursion, but very quickly that reached python's recursion limits, which I didn't want to change as it felt a bit like cheating. It was fairly easy to convert the recursive implementation to an iterative one, though.

After looking up how other people do BFS in python I learned about heapq (Python's priority queue data structure).

