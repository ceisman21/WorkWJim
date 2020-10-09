Cooper Eisman and James Fahey
10/9/2020

Q1 - What does clone set the variable origin to represent?
	The clone command sets the local origin as the repository that is cited in the command and then makes a branch.

Q2 - What does the command git push --set-upstream origin master do? What does remote tracking mean in this context?
	This command moves the origin of the local computer to equal the "master" branch of the git repo

Q3 - Explain and illustrate what's happening in the commit tree when this command executes.
	The next commit will move toward the specified branch, all further pushes and commits will be made to this branch

Q4 - Are your commits overwritten by the remote master?
	No, they are merged

Q5 - Is this a merge or a rebase?
	I believe this is a merge. It takes the info from both files and yucks them together

Q6 - Person B: checkout the local master branch. Is it updated as well, or still behind remote master?
	Still behind the master branch by 1 commit

Q7 - Run git branch. Did your local copy of your branch delete when Person A deleted the remote branch?
	No, it did not

Q8 - Use git log --graph --all to view the branching structure and copy and paste the result into the README.md formatted as a code segment (see markdown cheatsheet).



Structure:

*   commit 2196ba8a35f4197ebef1680b1ae1af73cfbb0e8c (HEAD -> main, origin/main)
|\  Merge: d2446d9 19d1a36
| | Author: ceisman21 <ceisman21@kentdenver.org>
| | Date:   Thu Oct 8 10:18:23 2020 -0600
| |
| |     Merge
| |
| * commit 19d1a36fe8ceb267ab22fc99ce65009c36fe779a
| | Author: James <jfahey21@kentdenver.org>
| | Date:   Thu Oct 8 10:06:02 2020 -0600
| |
| |     Added a line to hello
| |
* | commit d2446d92025812b72a44f2e11a55ec9bb2e86073
|/  Author: ceisman21 <ceisman21@kentdenver.org>
|   Date:   Thu Oct 8 10:13:16 2020 -0600
|
|       Hello World
|
* commit eb8aac19bf3ee04cee5c95b9350fd81f66fb740b (origin/Feature2, Feature2)
| Author: James <jfahey21@kentdenver.org>
| Date:   Thu Oct 8 09:59:20 2020 -0600
|
|     Added dab
|
* commit 13568c6ea6cabe57e5a58ad5c99c8f4eee3f8caa
| Author: ceisman21 <ceisman21@kentdenver.org>
| Date:   Thu Oct 8 09:44:13 2020 -0600
|
|     Test for Main2
|
* commit cc3009ea25da678f6225e1c9bd4581b72d7c0321 (origin/master, origin/JimsBranch)
| Author: ceisman21 <ceisman21@kentdenver.org>
| Date:   Thu Oct 8 09:36:12 2020 -0600
|
|     Cheese
|
* commit 7f044cf69c381ea81ec33038ff5e247adbc45afe
  Author: ceisman21 <ceisman21@kentdenver.org>
  Date:   Thu Oct 8 09:33:44 2020 -0600

      Cheese