To connect to the Level 0 of Bandit on OverTheWire, you will need to use SSH (Secure Shell). Here's a step-by-step guide:

1. Open your command line or terminal.
2. Type in the following command: 
    1. `ssh bandit0@bandit.labs.overthewire.org -p 2220`.
3. When prompted, enter the password. For level 0, the password is `bandit0`.
4. You are now connected to the Bandit Level 0.

### level 0

just connecting `ssh bandit0@bandit.labs.overthewire.org -p 2220`
password for user bandit0 is `bandit0`

### level 0 to 1

**commands**:

1. ls
2. cat readme

- **password -  NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL**

### level 1 to 2

**commands**:

1. ls
2. cat ./-

- **password -  rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi**

### level 2 to 3

**commands**:

1. ls 
2. cat ./spaces\ in\ this\ filename

- **password -  aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG**

### level 3 to 4


**commands**:

1. ls
2. cd inhere
3. ls -a
4. cat .hidden

- **password -  2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe**



### level 4 to 5

**commands**:

1. ls
    1. inhere
2. cd inhere
3. ls
    - file00 -file01 -file02 -file03 -file04 -file05 -file06 -file07 -file08 -file09
4. file ./-file0*
    1. 
    
    ./-file00: data
    ./-file01: data
    ./-file02: data
    ./-file03: data
    ./-file04: data
    ./-file05: data
    ./-file06: data
    ./-file07: ASCII text
    ./-file08: data
    ./-file09: data
    
5. cat ./-file07

- **password -  lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR**

### level 5 to 6

**commands**:

1. ls
    1. inhere
2. cd inhere 
3. ls
- **maybehere00**  **maybehere04**  **maybehere08**  **maybehere12**  **maybehere16 maybehere01**  **maybehere05**  **maybehere09**  **maybehere13**  **maybehere17 maybehere02**  **maybehere06**  **maybehere10**  **maybehere14**  **maybehere18 maybehere03**  **maybehere07**  **maybehere11**  **maybehere15**  **maybehere19**
1. find -type f -size 1033c ! -executable
    1. ./maybehere07/.file2
2. cd ./maybehere07
3. cat .file2

- **password -  P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU**

### level 6 to 7

**commands**:

1. find / -user bandit7 -group bandit6 -size 33c 2>&1 | grep -F -v Permission | grep -F -v directory
    1. /var/lib/dpkg/info/bandit7.password
2. cat /var/lib/dpkg/info/bandit7.password

- **password -  z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S**

### level 7 to 8

**commands**:

1. ls
    1. data.txt
2. cat data.txt | grep millionth
    1. **millionth**	TESKZC0XvTetK0S9xNwm25STk5iWrBvP

- **password -**  TESKZC0XvTetK0S9xNwm25STk5iWrBvP

### level 8 to 9

**commands**:

1. ls
    1. data.txt
2. cat data.txt | sort | uniq -c -u
    1. 1 EN632PlfYiZbn3PhVK3XOGSlNInNE00t

- **password -**  EN632PlfYiZbn3PhVK3XOGSlNInNE00t

### level 9 to 10

**commands**:

1. ls
    1. data.txt
2. strings data.txt | grep '^=’
    1. 
        
        **=**2""L(
        
        **=**========= passwordk^
        
        **=**========= is
        
        **=**Y!m
        
        **=**========= G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
        
        **=**r=_
        
        **=**uea
        

- **password -**  G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

### level 10 to 11

**commands**:

1. ls
    1. data.txt
2. base64 -d data.txt
    1. The password is 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

- **password -**  6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM


### level 11 to 12

**commands**:

1. ssh [bandit11@bandit.labs.overthewire.org](mailto:bandit2@bandit.labs.overthewire.org) -p 2220
    1. 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
2. ls
    1. data.txt
3. cat data.txt
    1. Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi
4. echo "Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi" | tr '[A-Za-z]' '[N-ZA-Mn-za-m]’
    1. The password is JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
- **password -**  JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv


### level 12 to 13

- password - wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw



### level 17 to 18 diff

password to login to from bandit17 - VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e

**commands**:

1. ls
    1. passwords.new  passwords.old
2.  diff passwords.old passwords.new
    
    42c42
    < p6ggwdNHncnmCNxuAt0KtKVq185ZU7AW
    
    hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg
    

- **password -  hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg**

### level 18 to 19 .bashrc modified

**commands**:

1. ssh [bandit18@bandit.labs.overthewire.org](mailto:bandit18@bandit.labs.overthewire.org) -p 2220 cat readme
    1. hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg

- **password -  awhqfNnAbc1naukrpqDYcF95h7HoMTrC**



