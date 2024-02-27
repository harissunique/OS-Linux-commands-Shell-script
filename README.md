# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
### Display the content of the files
cat < file1
## OUTPUT
![WhatsApp Image 2024-02-12 at 11 29 19 AM](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/c94c4a76-49f4-46f7-97a8-de321ce85120)



cat < file2
## OUTPUT
![WhatsApp Image 2024-02-12 at 11 29 19 AM](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/c72ff23e-df20-4c08-8a16-4840261eac1f)


# Comparing Files
cmp file1 file2
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/c7f60bc8-07bb-43c7-88f6-f77c518174a6)

comm file1 file2
 ## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/e1c1fa6a-7eb5-4573-a2f7-d332c63707c4)

 
diff file1 file2
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/14a11e10-748c-4837-8f8c-98a7bb7c54e8)


#Filters

### Create the following files file11, file22 as follows:

cut -c1-3 file11
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/40d880c3-4eeb-421a-a564-29e45404475f)

cut -d "|" -f 1 file22
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/436a7501-c522-4b02-ae39-ba1a391c5031)

cut -d "|" -f 2 file22
## OUTPUT
cat < newfile 
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/bb19a3e7-3f12-483f-a0fc-377586c7019b)

## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/dc16d4c9-3743-44b5-a7cd-f3d9282df0df)

grep hello newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/92152c61-8f4a-4e64-ab25-e1da4a78772e)

grep -v hello newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/553fa073-7703-4184-a309-2861a3940b15)

cat newfile | grep -i "hello"
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/9f98cf1b-0b69-462d-be37-661b91058c6d)

cat newfile | grep -i -c "hello"
## OUTPUT

grep -R ubuntu /etc
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/b86a6b5a-83f8-403b-adc9-b8ce7073234e)

grep -w -n world newfile   
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/eb24b560-ea0d-4000-939b-f5f2fd01719d)

egrep -w 'Hello|hello' newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/91e9ca2e-80d8-40af-879f-7d162fd1f81a)

egrep -w '(H|h)ello' newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/2aef2ecf-efd6-414a-806b-565f5a352e42)

egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/d4683644-1bb0-4e3c-aba6-e8ad1e7b6235)

egrep '(^hello)' newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/e84ff546-0bb2-4673-89d2-e063ab52b79c)

egrep '(world$)' newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/d0f30de0-6f36-44d6-b179-9038cf64011a)

egrep '(World$)' newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/61277461-c803-4651-97a2-44b2f2249941)

egrep '((W|w)orld$)' newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/8407e750-360d-4618-bcf1-a15397ac5679)

egrep '[1-9]' newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/11d2f11a-d9dd-4031-ae76-4a1e5d45cbab)

egrep 'Linux.*world' newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/aea04219-9477-4c77-8869-7e5a236b52cd)

egrep 'Linux.*World' newfile 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/57a931c1-b4a9-474b-85f6-673a6677fa74)

egrep l{2} newfile
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/0b0e3818-ad4a-4457-8d48-bb0b9781d525)

## OUTPUT 


cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/15f71b7d-9de1-486b-95f9-d0a47edd4cb2)

sed -n -e '3p' file23
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/935e41ac-cef7-4004-86bd-8468ce609fd9)

sed -n -e '$p' file23
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/fde3c44c-c67b-4577-add4-04f19672d4c7)

sed  -e 's/Ram/Sita/' file23
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/515073f9-5a64-4e95-b71e-d79c8587acf6)

sed  -e '2s/Ram/Sita/' file23
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/438d0526-e72c-48a8-b2c2-02c72d41d513)

sed  '/tom/s/5000/6000/' file23
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/6aa011d2-186a-414f-b514-00debb8a44e1)

sed -n -e '1,5p' file23
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/82c39cbc-3d3d-4513-ab1d-6a6005fd5c57)

sed -n -e '2,/Joe/p' file23
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/b7e023e8-c5e4-4af6-bbcd-6438f58cad6b)

sed -n -e '/tom/,/Joe/p' file23
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/1430b248-5100-409c-b0f7-a6ad12c5f959)

seq 10 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/1f5d6e2f-1a7b-4eea-8552-acff8c81523b)

seq 10 | sed -n '4,6p'
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/eb525a7e-43b5-4916-af88-3bc8c6b4cdca)

seq 10 | sed -n '2,~4p'
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/84f84424-6a15-4d3b-a285-941d3fe16861)

seq 3 | sed '2a hello'
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/7bea0f04-279e-4903-a337-d4902ebd4032)

seq 2 | sed '2i hello'
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/eafaeb58-e136-4d78-8e1f-bd4de3e2ff9d)

seq 10 | sed '2,9c hello'
## OUTPUT

![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/18284ae2-1458-43d2-adf9-c938b0e768e3)

## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/12731e6d-a860-400f-a9bb-2f5065523170)

sed -n '2,4{s/$/*/;p}' file23


#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/e5d6736e-cf4e-41a3-b67d-1782fb4559b3)

## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/c09905f2-fb18-476a-96fc-e262f634d64e)

cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin 
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/5f25712f-0ef9-4879-9d54-e78ff0d86f5e)

#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/a0e3114f-c0d9-439d-9d0a-240feb23dfe9)

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```

```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
 ## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/aef9e430-000a-4eca-a90b-5c110a4f8b44)

cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/c3162aaa-49f9-4871-975f-c899bad6ddad)

#Backup commands
tar -cvf backup.tar *
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/259a58b1-5889-4760-8ec0-f67ea57c7483)
mkdir backupdir
mv backup.tar backupdir 
tar -tvf backup.tar
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/27f00a78-61df-4953-b159-2234ef1e8472)

tar -xvf backup.tar

## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/daaccfa5-068f-4c51-88a6-1334d3eb57cd)

# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/0873e9e1-fc55-454b-9b95-af81ffff5b78)

cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT


cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/5afd01d6-bc49-420d-9376-f1d88e9b0178)

echo $?
## OUTPUT 
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/e7518e15-b5da-412c-a1ed-a9f6bc85220d)

./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
 ![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/475f954a-2446-4788-b1e9-341e2605a36b)

abcd
 
echo $?

 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
## OUTPUT
vi ![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/2266709f-d5df-4e6e-8825-f7a4e29cf7d0)

chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/0f088335-0b68-436e-b56e-a413b3316a37)

# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/3194dc09-c476-4167-a39e-779103ef8029)

# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/cfa8b86b-0e65-478d-aeaa-5a507d5bedc9)

# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/49a3408b-2e23-4f73-9cf2-407575a726c6)
vi

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/fe1af2ba-772b-44ba-938f-01691ae96134)

# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/969d3670-be61-4d5b-81d2-d53103223e8d)

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/4f69c2a2-0a5d-47db-af34-ce60e46db3b5)

# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/3ba0b9af-a6b9-433f-8acf-dd42ecf4932d)

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 
 ## Output
 
cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
 
  ## Output

cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
 
 
 ## Output
 ![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/f7fe8180-dde0-4567-b576-c29d30b63b55)

cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
 
 ## Output
 ![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/169b4ed1-16f1-4f17-b7cc-e3cd3d5ab22a)

cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
## Output
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/b46800a0-8101-495c-a66b-7c12c548322e)

cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 
  ## Output
![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/885626ba-ec97-4b35-8972-68e3f4d814ab)

cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
  ## Output
 ![image](https://github.com/deepika3095/OS-Linux-commands-Shell-script/assets/151625159/169b4ed1-16f1-4f17-b7cc-e3cd3d5ab22a)

cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

## OUTPUT

cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file ="cities"
for state in 'cat $file'
do
echo "Visit beautiful $file"
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT


cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT

 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT

$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
 
cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT


 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT



$ ./exread1.sh 
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
 ./funcex.sh 

 
 ./funcex.sh 1 2

 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
 
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 
cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
 ./argshift.sh 1 2 3
 
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
 
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 


# RESULT:
The Commands are executed successfully.
