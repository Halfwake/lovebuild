You can use -d and -o flags to pick the working directory to build in and the love file to create.

Here's the input with flags.
````
C:\Users\andrew\Desktop\gitter\lovebuild>python lovebuild -d test -o my_test.love
Building file <my_test.love> from dir C:\Users\andrew\Desktop\gitter\lovebuild\test
````

And here's the output with flags.
````
C:\Users\andrew\Desktop\gitter\lovebuild\test
Writing: C:\Users\andrew\Desktop\gitter\lovebuild\test\.gitignore
To: .gitignore
Writing: C:\Users\andrew\Desktop\gitter\lovebuild\test\main.lua
To: main.lua
Finished
````

Without a directory it'll use the directory it's called from. Without a specified output name it will generate a file named 'test.love'.
This can be useful if you'd rather just throw the file into the top of your project folder and call it as needed.

Here's the input without flags.
````
C:\Users\andrew\Desktop\gitter\lovebuild\test>python lovebuild
Building file <test.love> from dir C:\Users\andrew\Desktop\gitter\lovebuild\test
````

And here's the output without flags.
````
C:\Users\andrew\Desktop\gitter\lovebuild\test
Old file <test.love> was removed
Writing: C:\Users\andrew\Desktop\gitter\lovebuild\test\.gitignore
To: .gitignore
Writing: C:\Users\andrew\Desktop\gitter\lovebuild\test\main.lua
To: main.lua
Finished
````