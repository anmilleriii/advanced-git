# git-commands

Library of advanced git commands

## Commands

**Show behind/ahead commits from `develop`**

````sh
git rev-list --left-right --count develop...$(git branch --show-current)
````

*Output:*

````
8       212
````

<https://stackoverflow.com/questions/20433867/git-ahead-behind-info-between-master-and-branch>

**Sort branches by date worked on**

````sh
git for-each-ref --sort=-committerdate refs/heads/ --format='%(authordate:short) %(color:red)%(objectname:short) %(color:yellow)%(refname:short)%(color:reset) (%(color:green)%(committerdate:relative)%(color:reset))'
````

*Output:*

````
2021-09-15 ef1a390 scratch/example (3 weeks ago)
2021-09-15 c96773f feature/example (3 weeks ago)
2021-08-05 c4d4a45 feature/example (9 weeks ago)
2021-08-04 a0b3d61 release/example (9 weeks ago)
2021-08-03 abccaf7 feature/example (9 weeks ago)
````

<https://stackoverflow.com/questions/20433867/git-ahead-behind-info-between-master-and-branch>

**Show behind/ahead commits from `develop`**

````sh
git rev-list --left-right --count develop...$(git branch --show-current)
````

*Output:*

````sh
8       212
````

<https://stackoverflow.com/questions/20433867/git-ahead-behind-info-between-master-and-branch>
