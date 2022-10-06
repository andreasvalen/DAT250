# Excercise 2

### Report

- Installation failed as something was wrong with the paths

  - Solved: Dowloaded provided template folders and they worked perfectly

- Had some difficulties moving the projects to another git repo. Turns out i had to use the "Move" refactor function

I chose to create to db in the same folder as the java projects for easier accessability.
I used Jetbrains DataGrip as the database explorer to explore the created Apache Derby db.

- DB: Program would not run while the db explorer had an active connection
  - Solution: Deactivate the connection before running the program

Making the classes as described was pretty stright forward for everything but the bi-directional attributes. Their join tables were created in the databse as one would expect, but it was only possible to go from the owner class to the owned class. In short it acted as a uni-directional entity, even though it created the join_tables as expected. The solution was to bind the objects in the set functions in this fashion:

```java
owner.setOwned(Owned owned){
this.owned = owned;
owned.setOwner(this)
}
```

This feels like a workaround, and there is probably a spelling/syntax error somewhere that trips me up, but there is only created one join table in the db which is correct.

Screenshot of the many to many join table in the database:
![Alt text](resources/imgs/experiment-2-db-joinTableFocus.png?raw=true "Title")

- Unit test failed on bi-directional check

  - Solution?: changed setting functions

UNSOLVED: After rewriting an attribute relation in the entity, the db would fail to generate. I circumvented this by iterating the db name/version, but had to manually change url in explorer each time. Drop tables did not solve the issue.

Link to repo where experiment 2 unitTest runs: https://github.com/andreasvalen/expass2
