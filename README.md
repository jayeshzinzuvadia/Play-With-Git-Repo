# Play-With-Git-Repo
For learning GitHub and Git commands

## A. Basic GitHub Commands
* Create New Repository from the GitHub
* Open the git bash terminal or CMD in your local machine
* Copy the GitHub link of your newly created repository and run the following command:-
    ```
        git clone <Repository Url>
    ```
* **git clone** will clone the repo i.e. copy the github repo code to your local machine
* Now, let's define staging area. It's an area which contains files that are ready to commit
* To add/remove files into/from the staging area, run the command:-
    ```
        git add <Filename>
        git rm <Filename>
    ```
* To commit the changes, run:-
    ```
        git commit -m "Type your commit message"
    ```
* **git commit** will add your changes to local version control database
* To push the commited changes into remote server i.e. your GitHub repository
    ```
        git push
    ```
* Use **git pull** to fetch the repository code into the local machine if repo contains the files NOT present in the local machine. So, first grab the repo files and then push it. 
* **git log** will show all your logs of commit history
* **git difftool** will show the difference between the local changes and previous version of the file. You can use tools like meld for merging the code. By default, vmdiff is used.
* To undo uncommited changes, run:
    ```
        git checkout -- <filename> 
                or
        git restore <filename>
    ```
* To undo commited changes, run:
    ```
        git revert <commit id>      // It will be committed 
        git revert -n <commit id>   // To commit manually using the command
    ```
* To reset the changes, run:
    ```
        git reset --hard <commit id>    // Dangerous operation
    ```
* To perform branch operations, run:
    ```
        git branch      // Show the list of branches and branch marked as * is active

        git branch <branch name>        // Create a new branch
        git checkout -b <branch name>   // Create new branch and switch to that branch

        git checkout <branch name>      // Switch to the specified branch

        git checkout master                   // Switch to master branch before deleting a branch       
        git branch -D <branch name to delete> // Delete branch name
    ```

## B. Some useful resources to learn GitHub:-
1. Prerequisites : [Cryptographic Hash Function used by Git](https://www.tutorialspoint.com/cryptography/cryptography_hash_functions.htm)
2. [Git SCM book](https://git-scm.com/book/en/v2)
This is a open source book. Read chapter 1, 2, 3 and 10 from this book. Chapter 1, 2, and 3 are must to use git practically. And you can skip chapter 10 which describes it's internal working. But chapter 10 is one of my favourite and if you want to admire the beauty of git, chapter 10 is highly recommended.
3. [Git internals](https://m.youtube.com/watch?v=lG90LZotrpo)
This is really good talk which describes git internals in elegant way.
4. [Git Playlist](https://www.youtube.com/playlist?list=PLpcSpRrAaOarEpNz71TSfNVd0eQmsZSgN)  
            * [Video 1](https://www.youtube.com/watch?v=uR6G2v_WsRA)  
            * [Video 2](https://www.youtube.com/watch?v=FyAAIHHClqI&t=1512s)  
            * [Video 3](https://www.youtube.com/watch?v=Gg4bLk8cGNo)  
5. [CodeBasics GitHub tutorials](https://youtube.com/playlist?list=PLeo1K3hjS3usJuxZZUBdjAcilgfQHkRzW)
6. [Git immersion](http://gitimmersion.com/)
7. [Open Source Contribution](https://youtu.be/OCR_7I6Bjzo)

## C. How to write README.md file:-
* To display text for different styles :-<br> 
    1) Italics :  _type between a pair of underscores_<br>
    2) Bold : **type between a pair of two asterisk**<br>
    3) Strikethrough : ~~type between pair of two tilde~~<br>
    4) Simple : simply type the text<br>
* For Headings use # before the title. Adjust the size using #'s from 1 to 6:-<br>
    # Heading 1
    ## Heading 2
    ### Heading 3
    #### Heading 4
    ##### Heading 5
    ###### Heading 6
* Quote:-<br>
    > "Arise, Awake, Stop not until your goal is achieved"
* Copyright:-<br>
    Write "\&copy;" to create &copy;
* Hyperlink:-<br>
    [YouTube](https://www.youtube.com/ "Youtube videos")
* To add image, type ![imageName](image path):-<br>
    ![Earth](earth.png)
    <!-- <img src="earth.png" alt="drawing" width="200"/> -->
* To add single line of code, type it between a pair of backquote:<br>
    `printf("Hello");`<br>
    `System.out.println("Hello");`<br>
    `print("Hello")`<br>
* To add multiple lines of code in a .md file, type it between a pair of 3 backquote:<br>
    ```
    #include<iostream>
    void main()
    {
        cout << "Hello" << endl;
    }
    ```
* To add table:-<br>
    |Name|Email|Address|
    |----|-----|-------|
    |Jayesh|jayeshzinzuvadiya099@gmail.com|Rajkot|
* List:-  
  1. Item 1
  2. Item 2
  3. Item 3
    * Sub item 1
    * Sub item 2
* Line (Use *** or ---)  
    ***
    End of the file
    ***
