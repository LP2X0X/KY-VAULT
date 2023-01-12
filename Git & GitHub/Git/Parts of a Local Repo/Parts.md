- The Git repository itself is divided into two parts — the first part is called the “Index”, and the second part is what we will refer to as the “Object Database”. Include the "Working Directory", these three parts are what we work with when using Git.
- When we run git add < filename >, Git makes a copy of the file and puts it in the index. We can think of the index as the “staging area,” wherein we can put things till we are sure we want to commit to them.
- Now when we run the git commit command, it takes the contents of the staging area and stores those in the object database, also known as Git’s memory bank.
![[Capture.png|center]]