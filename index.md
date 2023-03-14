## Lab Report 5
# Using the `grep` command

1. `grep 'phrase' file` This looks inside of file and prints every line / paragraph containing the phrase

`grep 'devoted' Abernathy/ch1.txt`

![image](https://user-images.githubusercontent.com/122569112/224841104-10f8b50e-c1fd-4826-b039-6d9ee6cd9685.png)

Here's another example:

`grep 'Lucayans' travel_guides/berlitz2/Bahamas-History.txt`

![image](https://user-images.githubusercontent.com/122569112/224841311-748a42dd-a62c-4b71-b55d-cf95b6d06960.png)

This command is useful for finding instances of phrases in a file. Instead of having to open a file and search through it manually, the grep command
shows the instances if they are there, and tells you where as well.

2. `grep -c 'phrase' file` counts the number of times the phrase is used inside the file
`grep -c Lucayans written_2/travel_guides/berlitz2/Bahamas-History.txt`

![image](https://user-images.githubusercontent.com/122569112/224841968-827028d8-0120-4b17-96eb-b387a7ecd7a8.png)

Here's another example:

`grep -c In non-fiction/OUP/Abernathy/ch1.txt`

![image](https://user-images.githubusercontent.com/122569112/224842117-7b721c52-b5c1-4037-9523-ffb360c07295.png)

This helps us find how many times a certain phrase is within a file, and is useful for statistics purposes or just generally for counting when it would be
difficult to find all of the uses manually.

3. `grep -R phrase` finds the file path and lists where you could find the file 

`grep -R 'Just north of Puerto'`

![image](https://user-images.githubusercontent.com/122569112/224842602-a03f3619-ced0-4ae3-8998-675851d99d41.png)

Here's another example:

`grep -R 'Pirates Well harks back'`

![image](https://user-images.githubusercontent.com/122569112/224842785-c603daf5-57e3-4fc4-a34c-28b312dd16bc.png)

This helps to find instances of a phrase in an unknown file or location. This is useful in the case where a user doesn't know where they stored a specific
piece of information.

4. ` GREP_COLOR='1;35' grep --color=always 'word' file` This command finds the given phrase and highlights it in a given color.

`GREP_COLOR='1;35' grep --color=always 'Just north of Puerto' travel_guides/berlitz2/CanaryIslands-WhereToGo.txt`

![image](https://user-images.githubusercontent.com/122569112/224847149-dde8e579-7061-4a91-bcf1-7c8e3343f16c.png)

Here's one more example:

`GREP_COLOR='1;36' grep --color=always 'Lucayans' travel_guides/berlitz2/Bahamas-History.txt`

![image](https://user-images.githubusercontent.com/122569112/224847795-df85e498-f742-49aa-8499-53f06461dfb0.png)


Depending on the GREP_COLOR, the color of the found word in the file is changed. This helps save a little bit of time. Also, in a bash script this could be
used for advanced color coding of a given dataset.

# Research source: [this website](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/) .
