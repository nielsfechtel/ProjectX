~\Desktop\ProjectX
⚡ mkdir docs

    Directory: C:\Users\Niels\Desktop\ProjectX



~\Desktop\ProjectX
⚡ mkdir reports

    Directory: C:\Users\Niels\Desktop\ProjectX



~\Desktop\ProjectX
⚡ cd reports


~\Desktop\ProjectX\reports
⚡ touch report_one.txt
touch: The term 'touch' is not recognized as a name of a cmdlet, function, script file, or executable program.
Check the spelling of the name, or if a path was included, verify that the path is correct and try again.


~\Desktop\ProjectX\reports
❌ notepad ./report_one.txt


~\Desktop\ProjectX\reports
⚡ notepad ./report_two.txt


~\Desktop\ProjectX\reports
⚡ mkdir images

    Directory: C:\Users\Niels\Desktop\ProjectX\reports



~\Desktop\ProjectX\reports
⚡ rmdir images


~\Desktop\ProjectX\reports
⚡ cd ..


~\Desktop\ProjectX
⚡ mkdir images

    Directory: C:\Users\Niels\Desktop\ProjectX



~\Desktop\ProjectX
⚡ mkdir src

    Directory: C:\Users\Niels\Desktop\ProjectX



~\Desktop\ProjectX
⚡ cd src


~\Desktop\ProjectX\src
⚡ mkdir html

    Directory: C:\Users\Niels\Desktop\ProjectX\src



~\Desktop\ProjectX\src
⚡ notepad html/index.html


~\Desktop\ProjectX\src
⚡ mkdir css

    Directory: C:\Users\Niels\Desktop\ProjectX\src


~\Desktop\ProjectX\src
⚡ notepad css/style.css


~\Desktop\ProjectX\src
⚡ mkdir js

    Directory: C:\Users\Niels\Desktop\ProjectX\src


~\Desktop\ProjectX\src
⚡ notepad js/script.js


~\Desktop\ProjectX\src
⚡ mkdir data

    Directory: C:\Users\Niels\Desktop\ProjectX\src


~\Desktop\ProjectX\src
⚡ rmdir data


~\Desktop\ProjectX\src
⚡ cd ..


~\Desktop\ProjectX
⚡ mkdir data

    Directory: C:\Users\Niels\Desktop\ProjectX


~\Desktop\ProjectX
⚡ notepad data/data.txt


~\Desktop\ProjectX
⚡ "Hello Data" | data/data.txt


~\Desktop\ProjectX
⚡ echo "Hello Data" | data/data.txt
InvalidOperation: Cannot run a document in the middle of a pipeline: C:\Users\Niels\Desktop\ProjectX\data\data.txt.


~\Desktop\ProjectX
❌ echo "Hello Data" | OutFile -FilePath data/data.txt
OutFile: The term 'OutFile' is not recognized as a name of a cmdlet, function, script file, or executable program.
Check the spelling of the name, or if a path was included, verify that the path is correct and try again.


~\Desktop\ProjectX
❌ echo "Hello Data" | Out-File -FilePath data/data.txt


~\Desktop\ProjectX
⚡ Get-Content .\data\data.txt
Hello Data


~\Desktop\ProjectX
⚡ git init
Initialized empty Git repository in C:/Users/Niels/Desktop/ProjectX/.git/


ProjectX on  main [🤷]
⚡ git status
On branch main

No commits yet

Untracked files:
(use "git add <file>..." to include in what will be committed)
data/ reports/ src/

nothing added to commit but untracked files present (use "git add" to track)


ProjectX on  main [🤷]
⚡ git add .


ProjectX on  main [++(6)]
⚡ git status
On branch main

No commits yet

Changes to be committed:
(use "git rm --cached <file>..." to unstage)
new file: data/data.txt
new file: reports/report_one.txt
new file: reports/report_two.txt
new file: src/css/style.css
new file: src/html/index.html
new file: src/js/script.js


ProjectX on  main [++(6)]
⚡ notepad ./images/.gitkeep


ProjectX on  main [++(6)]
⚡ git status
On branch main

No commits yet

Changes to be committed:
(use "git rm --cached <file>..." to unstage)
new file: data/data.txt
new file: reports/report_one.txt
new file: reports/report_two.txt
new file: src/css/style.css
new file: src/html/index.html
new file: src/js/script.js

Untracked files:
(use "git add <file>..." to include in what will be committed)
images/


ProjectX on  main [++(6)🤷]
⚡ git add images/


ProjectX on  main [++(7)]
⚡ git commit -m "initial setup"
[main (root-commit) 08b1b03] initial setup
7 files changed, 1 insertion(+)
create mode 100644 data/data.txt
create mode 100644 images/.gitkeep.txt
create mode 100644 reports/report_one.txt
create mode 100644 reports/report_two.txt
create mode 100644 src/css/style.css
create mode 100644 src/html/index.html
create mode 100644 src/js/script.js


ProjectX on  main
⚡ git switch -c feature/add-index.html-content
Switched to a new branch 'feature/add-index.html-content'


ProjectX on  feature/add-index.html-content
⚡ code .\src\html\index.html


ProjectX on  feature/add-index.html-content
⚡ git status
On branch feature/add-index.html-content
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: src/html/index.html

no changes added to commit (use "git add" and/or "git commit -a")


ProjectX on  feature/add-index.html-content [📝]
⚡ git add .\src\html\index.html


ProjectX on  feature/add-index.html-content [++(1)]
⚡ git switch main
M src/html/index.html
Switched to branch 'main'
