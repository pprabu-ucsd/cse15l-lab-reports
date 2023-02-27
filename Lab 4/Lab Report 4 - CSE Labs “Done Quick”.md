# Lab Report 4 - CSE Labs “Done Quick”

**By Pranav Prabu**

## Task #1: Log into ieng6
`CTRL+R` to start a search

Used `ssh` as the query

`<enter>` to finish the search and get:

`ssh cs15lwi23aaw@ieng6.ucsd.edu`

`<enter>` to log into the remote server

## Task #2: Clone your fork of the repository from your Github account
Copied the SSH key from GitHub:
`git@github.com:pprabu-ucsd/lab7.git`

Pasted it into the terminal to get:
`git clone git@github.com:pprabu-ucsd/lab7.git`

`<enter>` to clone the fork of the repository

## Task #3: Run the tests, demonstrating that they fail
`CTRL+R` to start a search

Used `javac` as the query

`<enter>` to finish the search to get:

`javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`

`<enter>` to compile the tests

`CTRL+R` to start a search

Used `TestL` as the query

`<enter>` to finish the search to get:
`java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples`

`<enter>` to run the tests

## Task #4: Edit the code file to fix the failing test
`CTRL+R` to start a search

Used `sed` as the query

`<enter>` to finish the search to get:

`sed -i '43 s/1/2/1' ListExamples.java`

`<enter>` to make the edit

## Task #5: Run the tests, demonstrating that they now succeed
`CTRL+R` to start a search

Used `javac` as the query

`<enter>` to finish the search to get:

`javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`

`<enter>` to compile the tests

`CTRL+R` to start a search

Used `TestL` as the query

`<enter>` to finish the search to get:
`java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples`

`<enter>` to run the tests

## Task #6: Commit and push the resulting change to your Github account

For this final step, I typed out the following commands:
`git add *`
`git commit -m "fixed file"`
`git push`

I found it easier and faster to just type them out rather than using arrow keys to find them.
