# Bingo-Game

bingolist=[[1,2,3,4,5],[6,7,8,9,10],[11,12,13,14,15],[16,17,18,19,20],[21,22,23,24,25]]

while True:
	n=int(input())
	
	for i in bingolist:
		if n in i:
			l=i.index(n)
			i[l]=-1		
	for i in bingolist:
		sum=0
		for a in i:
			sum+=a
		if sum==-5:
			print("Bingo")
			break
	sum=0		
	for i in bingolist:
		sum+=i[0]
		if sum==-5:
			print("Bingo")
			break
	sum=0		
	for i in bingolist:
		sum+=i[1]
		if sum==-5:
			print("Bingo")
			break
	sum=0		
	for i in bingolist:
		sum+=i[2]
		if sum==-5:
			print("Bingo")
			break
	sum=0		
	for i in bingolist:
		sum+=i[3]
		if sum==-5:
			print("Bingo")
			break
	sum=0		
	for i in bingolist:
		sum+=i[4]
		if sum==-5:
			print("Bingo")
			break
	sum=0		
	for i in bingolist:
		sum+=i[bingolist.index(i)]
		if sum==-5:
			print("Bingo")
			break
	sum=0		
	for i in bingolist:
		sum+=i[4-bingolist.index(i)]
		if sum==-5:
			print("Bingo")
			break
