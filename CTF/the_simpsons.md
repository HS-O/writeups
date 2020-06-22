## The Simpsons
Challenge link: https://ctflearn.com/challenge/160


Challenge category: Cryptography, hard 

Challenge points: 80 points

Challenge description:

Ya know, I was thinking... wouldn't the Simpsons use octal as a base system? They have 8 fingers... Oh, right! The problem! Ummm, something seems odd about this image... https://mega.nz/#!yfp1nYrQ!LOz_eucuKkjAaDqVvz3GWgbfdKWn8BhussKZbx6bUMg

Challenge solution:

1. firstly, go to the link provided and download it as jpg.
2. open the jpg with notepad -- in case there is something hidden 
3. at the button there are lines of python code 
4. decode the encoded and key using octal mentioned in the description 
5. get encoded as 'jrjerwhzkrexar', get key as 'How much did Maggie originally cost? (Divided by 8, to the nearest integer, and then plus four)'
6. search the ans of the qn in key online and do calculation get 110
7. follow the key - use chr(the result of the key) get key = n
8. then the line below gives a new value of key = key + key + chr(ord(key)-4), get new key as nnj
9. finally, use the new key to decipher the encoded text "jrjerwhzkrexar" 
10. get the flag "wearenumberone", submit 
11. problem solved 
