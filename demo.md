# Demo #

1)	mkdir gitdemo_user1
2)	mkdir gitdemo_user2
	Beide user1 und user2 
3)	git clone https://github.com/codemapper/GIT-Demo.git

	Beide user1 und user2 ändern den Text auf der selben Zeile
4)	notepad text1.txt  //user1
5)	notepad text1.txt  //user2

## Konflikte lösen ##
	
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

## Arbeiten mit Branches ##

1)	git branch branch-a
2)	git branch		
3) 	git checkout branch-a
4)	notepad textB.txt
5)	git add textB.txt
6)	git commit -am "new file textB.txt added"
7) 	git push --set-upstream origin branch-a  //git push -u origin branch-a
8)	git checkout master  
9)	git merge branch-a master
10)	git branch -D branch-a			//delete local branch
11)	git push --delete branch-a 	//delete remote branch //short: git push -d origin branch-a


## Reset ##
git reset --hard old-commit-id //see e.g. git log

## Clone inkl. switch Branches ##

1) git clone https://github.com/ICT-BBC/mvc.git
2) git checkout controller