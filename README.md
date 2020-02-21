# midterm

## First Section

**Cloning** : when we clone something to our local machine from remote repository, we own that repository

**Fetch** : when we fetch something, we are bringing changes made on remote repository to our local repository to compare. we are not actually merging that changes.

**Pull** : when we pull something, that means we are merging the changes made on remote repository to our local repository. Pull is like doing "fetch" and "merge" in one step.
## Second Section
### Differnece between Trello and Asana

| **Trello**    |   **Asana**       |
|---------------|:-----------------:|
| Expensive plans| Cheaper plans|
|Better UI | Not better UI|
|can change Background| can not change Background|
|Only board view| Both board and list view|
|Restricts number of boards|Limits number of user|
|Built-in Feature | Don't have built-in Feature|

## Third Section

**Question 1**:

The . git folder_ contains all the information that is necessary to keep track of you projects. It has all the information about you commits, have tags refering to different version of your project.

The object database is located in "objects" folder inside the .git folder

**Question 2**:

The git hash object function takes any text as input and generates a key using hash algorithim. It user SHA-1 algorithim to change any text to fixed length key which can not be reversed and we can refer to the data using that key.
```
echo "hello world" | $git hash-object --stdin
```

In above line of code, we are telling git to take text "hello world" and generates the hash key for it.
```
echo "hello world" | $git hash-object --stdin -w
```

when we mention -w flag with the hash-object function, then we telling git to write that key to objects folder in .git folder.

**Question 3**:

git does not store file name for the files. It always refer to the file using hash key. It generates the key by combining content, size and type of the object so hash key has all the information about the file.
