# Challenge 5: Extracting specific sections of text
Using the `cut` command to cut out columns from text
## Solution
Invoke `/challenge/run` 
```
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run
20558 p
18025 w
16500 n
4655 .
26221 c
3605 o
3573 l
3629 l
24462 e
28191 g
26778 e
2312 {
32537 U
19647 T
8257 N
15274 H
5859 K
8408 7
23638 N
13639 u
24012 l
31821 q
23980 a
23098 G
14236 v
5955 L
13807 2
7020 w
23394 i
11223 e
25903 -
6644 Q
5285 O
27982 F
14595 W
3673 V
8352 6
6497 R
25850 F
23413 .
32323 0
32565 1
516 N
32417 x
7379 E
5913 z
1333 N
24955 x
21179 w
7213 i
20643 M
32140 w
29987 A
29859 z
5906 N
9291 z
19642 E
32760 z
5870 W
28089 }
```
Now, we invoke the command again but _pipe_ its output to `cut`, using which we clear out the first column by defining the column delimiter with `-f` to be `" "` and extract the `2nd` column, which we _pipe_ to `tr` to delete the _newline_ characters  
```
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{UTNHK7NulqaGvL2wie-QOFWV6RF.01NxEzNxwiMwAzNzEzW}
```
## Flag
`pwn.college{UTNHK7NulqaGvL2wie-QOFWV6RF.01NxEzNxwiMwAzNzEzW}`
### Notes
- learnt about the `cut` command, which can be used to _"cut"_ out columns from its input
  - using `-d` we specify the column delimiter (the characters by which the columns are separated)
  - using `-f` we specify _which_ column we want to extract by giving the column no. with the argument