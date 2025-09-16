Level 0: 
`cat readme.txt`. The password is ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
Lesson: make sure you know how to use SSH and display the contents of a file

Level 1: 
`cat ./-`. The passsword is 263JGJPfgU6LtdEvgfWU1XP5yac29mFx
Lesson: Learn how to work with dashed filenames (since many Unix commands use - for arguments)

Level 2: 
`cat ./--spaces\ in\ this\ filename--`. The password is MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
Lesson: Learn how to work with spaces in filenames

Level 3: 
`cd inhere`
`ls -a` to reveal the hidden file, which will not appear if you just use `ls`
`cat ...Hiding-From-You`. The password is 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
Lesson: Learn how to view and interact with hidden files

Level 4: 
`cd inhere`
`cat ./-file07` (this is the only human-readable file in the folder). The password is 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
Lesson: Learn to distinguish between human-readable and non-human-readable files

Level 5:
`cd inhere`
`find -readable -size 1033c` (will find only one file that matches the properties in the instructions)
`cat ./maybehere07/.file2`. The password is HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
Lesson: Learn how to use `find` to search for file properties

Level 6:
`cd ../..` to go to root folder
`find -user bandit7 -group bandit6 -size 33c` (following instructions)
`cat ./var/lib/dpkg/info/bandit7.password` (the one file that matches). The password is morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
Lesson: Learn how to use `find` to search for files owned by users and groups

Level 7:
`cat data.txt | grep "millionth"`. The password is dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
Lesson: Learn how to use `grep` to search through large files
