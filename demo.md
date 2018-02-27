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
	Konflikt auflösen	
11)	Wichtig!!! Immer commiten!
	user2: git commit -am "File changed"  //habne wir schon gemacht
13)	user2: git pull \\änderungen herunterladen
14)	user2: Konflikte auflösen
15)	User 2: git push 	< Jetzt geht es



1)	git branch branch-a
2)	git branch		
3) 	git checkout branch-A
4)	notepad textB.txt
5)	git add textB.txt
6)	git commit -am "new file textB.txt added"
7) 	git push --set-upstream origin branch-A
8)	git checkout master  
9)	git merge branch-A master
10)	git branch -D branch-A			//delete local branch
11)	git push origin --delete branch-A 	//delete remote branch