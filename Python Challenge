# PC0 Hint: try to change the URL address.
#http://www.pythonchallenge.com/pc/def/0.html

print('\nPC0: 2**38=',str(2**38))
# 274877906944

#PC1 http://www.pythonchallenge.com/pc/def/map.html
"""
K>M
O>Q
E>G
everybody thinks twice before solving this.
g fmnc wms bgblr rpylqjyrc gr zw fylb. rfyrq ufyr amknsrcpq ypc dmp. bmgle gr gl zw fylb gq glcddgagclr ylb rfyr'q ufw rfgq rcvr gq qm jmle. sqgle qrpgle.kyicrpylq() gq pcamkkclbcb. lmu ynnjw ml rfc spj.

General tips:
Use the hints. They are helpful, most of the times.
Investigate the data given to you.
Avoid looking for spoilers.
"""
print('\nPC1 KOE2MQG')
strx="g fmnc wms bgblr rpylqjyrc gr zw fylb. rfyrq ufyr amknsrcpq ypc dmp. bmgle gr gl zw fylb gq glcddgagclr ylb rfyr'q ufw rfgq rcvr gq qm jmle. sqgle qrpgle.kyicrpylq() gq pcamkkclbcb. lmu ynnjw ml rfc spj. "
def KOE2MQG(strIn):
        strIn.lower()
        strO=''#lenthofstr1=len(strIn)
        for c in strIn:
                if c=='k':
                        c='m'
                elif c=='o':
                        c='q'
                elif c=='e':
                        c='g'
                strO+=c
        return strO
        '''while i<= lenthofstr1:
		if str1[i]=='k':
			#str1[i]='m'#TypeError: 'str' object does not support item assignment
		elif str1[i]=='o':
			str1[i]='q'
		elif str1[i]=='e':
			str1[i]='g'
		i+=1
		'''
#str1[i]='m'#TypeError: 'str' object does not support item assignment
def KOE2MQG2(strIn):
        StrO=strIn.replace('k','m')
        StrO=strIn.replace('o','q')
        StrO=strIn.replace('e','g')
        return StrO

def Map(strIn):
        ins=''
        for i in range(ord('a'),ord('z')+1):
                ins+=chr(i)
        out=ins[2:]+ins[:2]        
        table=strIn.maketrans(ins,out)
        strO=strIn.translate(table)
        return strO        
print(strx)
print(KOE2MQG(strx))
print(KOE2MQG2(strx))
print(Map(strx))
""" for c in strIn:
                if c in('y','z','Y','Z',' '):d=c
                else:d=chr(ord(c)+2)
                strO+=d"""
print(Map('map'))


#PC2
"""
recognize the characters. maybe they are in the book, 
but MAYBE they are in the page source.


General tips:
Use the hints. They are helpful, most of the times.
Investigate the data given to you.
Avoid looking for spoilers.

Forums: Python Challenge Forums, read before you post. 
IRC: irc.freenode.net #pythonchallenge 

To see the solutions to the previous level, replace pc with pcc, i.e. go to: http://www.pythonchallenge.com/pcc/def/ocr.html
"""
'''
find rare characters in the mess below:
'''
print('\nPC2 Rare chr')

focr=open('C:\Python33\pyGC\Python Challenge\ocr.txt','r')
ocr=focr.read()
def RareChr(strIn):
        ins=''
        rareChr=''
        for i in range(ord('a'),ord('z')+1):
                ins+=chr(i)
        for i in range(ord('A'),ord('Z')+1):
                ins+=chr(i)        
        for x in strIn:
             if x in ins:
                     rareChr+=x
        return rareChr
print(RareChr(ocr))
focr.close()

#PC3 One small letter, surrounded by <b>EXACTLY</b> three big bodyguards on each of its sides.
print('\n PC3 AAAiAAA')

with open('C:\Python33\pyGC\Python Challenge\s3B.txt', mode='r', encoding='utf-8') as fs3B:
        s3B=fs3B.read()

def rangex(n):
	for ii in range(2,n-2):
		print(i)
import re		
def s3b(strI):
        print('s3b is running')
        lows=ups=''
        for ll in range(ord('a'),ord('z')+1):
                lows+=chr(ll)
        for uu in range(ord('A'),ord('Z')+1):
                ups+=chr(uu)
        for i in range(len(''.join(strI.splitlines()))-1):
                if re.findall('[a-z][A-Z][A-Z][A-Z][a-z][A-Z][A-Z][A-Z][a-z]',s3B):
                        return re.findall('[a-z][A-Z][A-Z][A-Z][a-z][A-Z][A-Z][A-Z][a-z]',s3B)
'''     for i in range(len(strI)-1):
                if re.findall('[A-Z][A-Z][A-Z][a-z][A-Z][A-Z][A-Z]',s3B):
                        return re.findall('[A-Z][A-Z][A-Z][a-z][A-Z][A-Z][A-Z]',s3B)  '''                    
            
s3b=s3b(s3B)
print(s3b)
print(len(s3b))
def allin(lst): # all is key word
        s=''
        for i in lst:
                s+=i[4]
        return s        
print(allin(s3b))             

# PC4 follow the chain
'''urllib may help. DON'T TRY ALL NOTHINGS, since it will never 
end. 400 times is more than enough. '''
print('\nPC4:follow the chain')
import urllib.request #only urllib is not right!
url=['']
url[0]='http://www.pythonchallenge.com/pc/def/linkedlist.php?nothing=12345'
      
lltxt='C:\Python33\pyGC\Python Challenge\linkedlist.txt'

lltxtf=open(lltxt,'w') # you must know when to open
answer=[]
count=[]
for i in range(3):
        with urllib.request.urlopen(url[i]) as urlf:
                s=urlf.read().decode("utf8").split(' ')[-1]
                print('%d\t%s'%(i,(url[i].split('=')[-1])))
                url.append(url[0].split('=')[0]+'='+s) # don't forget +'='
        lltxtf.write('%d\t%s\n'%(i,url[i].split('=')[-1]))
        if not s.isnumeric():
                answer.append(s)
                count.append(i+1)
                '''break'''
             
lltxtf.close()        # you must know when to close a file, otherwise it's just rewritten.
s=''
if answer==[]:print('not get answer yet@@')
else:
        for i in answer:
                print('answer in ',(count[answer.index(i)],i))
                s+=i      # if you find invalid syntax and find nothing wrong, last line is short of a )
                print('answer is:\n',i)        

#网速好慢

# PC5 peak hell
'''
<peakhell src="banner.p"/>
C:\Python33\pyGC\Python Challenge\banner.p
<!-- peak hell sounds familiar ? -->
The clue here is that "peak hell" is a pointer towards "Pickle", a python serialization module. 
Fact 1: there is a refference to a file named banner.p in the html source, so we’ll download it and see
Pickle allows the programmer to generate a string representation of any object, very useful in saving complicated data types.

As for where the pickled information is stored, usually one would do:

with open('filename', 'w') as f:
    var = {1 : 'a' , 2 : 'b'}
    pickle.dump(var, f)
That would store the pickled version of our var dict in the 'filename' file. Then, in another script, you could load from this file into a variable and the dictionary would be recreated.

Another use for pickling is if you need to transmit this dictionary over a network (perhaps with sockets or something.) You first need to convert it into a character stream, then you can send it over a socket connection.

Also, there is no "compression" to speak of here...it's just a way to convert from one representation (in RAM) to another (in "text").
'''
import pickle
pf=r'C:\Python33\pyGC\Python Challenge\banner.p'
url=r'http://www.pythonchallenge.com/pc/def/banner.p' # use urllib.request(url,'rb')
with open(pf,'rb') as banner: # 'rb' as byte, 'r' as string s=pickle.load(banner)  TypeError: 'str' does not support the buffer interface
        s=pickle.load(banner)
        print(s)
        for line in s:
                print (''.join(map(lambda pair: pair[0]*pair[1], line)))
'''in case anyone else finds this post while wondering WTF the pickled data in Challenge 5 means,
it’s a list of lists where each sub-list represents a line of console output. The sublists consist
of pairs of characters and numbers of times to repeat the character.

print ”.join(map(lambda pair: pair[0]*pair[1], line))

map(F, line) means loop over each element (a pair here) in the list ‘line’, applying F to the element.
pair[0] is a character (length-1 string), and pair[1] is a long, so pair[0] * pair[1] produces the
character in pair[0] repeated pair[1] times.'''

# PC6 now there are pairs
dir0=r'C:\Python33\pyGC\Python Challenge\channel'
start=90052
dirx=[]
dirx.append(dir0+'\\'+str(start)+'.txt')
ctxtf=open(r"C:\Python33\pyGC\Python Challenge\channel.txt" ,'w')
for i in range(600):
        with open(dirx[i]) as f:
                s=f.read().split(' ')[-1]#ctxtf AttributeError: 'str' object has no attribute 'decode'
                print('%d\t%s'%(i,(dirx[i].split('\\')[-1]).split('.')[0]))
                new=''
                new='\\'.join(dirx[i].split('\\')[:-1])+'\\'+s+'.txt' # don't forget +'='
                dirx.append(new)
                ctxtf.write('%d\t%s\n'%(i,dirx[i].split('=')[-1]))
        if not s.isnumeric():
                answer.append(s)
                count.append(i+1)
                break

ctxtf.close()        # you must know when to close a file, otherwise it's just rewritten.
s=''
if answer==[]:print('not get answer yet@@')
else:
        for i in answer:
                print('answer in ',(count[answer.index(i)],i))
                s+=i      # if you find invalid syntax and find nothing wrong, last line is short of a )
                print('answer is:\n',i)        


#http://unixwars.com/2007/09/12/python-challenge-level-6-now-there-are-pairs/
#http://stackoverflow.com/questions/606191/convert-byte-array-to-python-string                
import zipfile,re
idx="90052"
file = zipfile.ZipFile("channel.zip",  mode='r')
history = []
while True:
    history.append(idx)
    data = file.read(idx+".txt",).decode(encoding='utf-8') # add str
    print( "File",idx+":\t"+ data) # add str()
    idx="".join(re.findall('[0-9.]',data)) 
    if len(idx)==1:
        break
#Collect the comments
print( ''.join([file.getinfo(i+'.txt').comment.decode(encoding='utf-8')  for i in history]))


# http://www.pythonchallenge.com/pc/def/oxygen.html
# PC7 smarty

