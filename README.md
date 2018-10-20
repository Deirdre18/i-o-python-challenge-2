(Solution Code from Code Institute tutorial - Challenge 2 (I/O))

#Challenge 2

1) Create a sample file consisting of four lines of text.

2) Using the r+ mode, overwrite the first line. 

3) Then, move the file cursor to overwrite the third line. 

4) Finally, append a line to the file.


Console Output:

~/workspace $ python3
Python 3.4.3 (default, Nov 17 2016, 01:08:31) 
[GCC 4.8.4] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> f = open('myfile.txt', 'r+')
>>> f.write('Line 0')
6
>>> current_position = f.tell()
>>> f.seek(current_position + 8)
14
>>> f.write('Line 6')
6
>>> f.seek(0, 2)
27
>>> f.write('\nLine 5')
7
>>> f.close()
>>> 
