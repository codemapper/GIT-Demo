1)	mkdir gitdemo_user1
2)	mkdir gitdemo_user2
	Beide user1 und user2 
3)	git clone https://github.com/codemapper/GIT-Demo.git

	Beide user1 und user2 ändern den Text auf der selben Zeile
4)	notepad text1.txt  //user1
5)	notepad text1.txt  //user2

	
6)	User 1: git commit -am "File changed"
7)	User 2: git commit -am "File changed"
8)	User 1: git push
9)	User 2: git push	< Fehler!!!  You may want to first integrate the remote changes
10)	Konflikt auflösen
11)	User 2: git push	< Fehler!!!  You may want to first integrate the remote changes
12)	Wichtig!!! Immer commiten!
12)	user2: git commit -am "File changed"
13)	User 2: git push 	< Jetzt geht es
