# Answers to selected Delftse Foundations of Computation exercises
These are the solutions to exercises given as homework for the [Reasoning & Logic course (CSE1300)] using the free textbook [Delftse Foundations of Computation].
With every new version of the book, changes applied on this repository will be included in the new version of the book.

## Quickstart

1. Download a TeX installation, see requirements below. We also recommend a rich editor such as [TexStudio](https://www.texstudio.org/).
1. Create an account [here on GitLab](https://gitlab.ewi.tudelft.nl/users/sign_in) using your TUD student e-mail and your netid as your username.
1. [Add an SSH key to your account](https://gitlab.ewi.tudelft.nl/profile/keys)
1. [Fork the repository](https://gitlab.ewi.tudelft.nl/reasoning_and_logic/book_solutions/-/forks/new)
1. Download a git installation; For example: [Git Bash](https://git-scm.com/downloads) or just `apt install git` on Ubuntu/Debian
1. In git configure your e-mail address: `git config --global user.email=<your-student-email-address>` where `<your-student-email-adres>` is your TUD address. E.g `git config --global user.email=s.hugtenburg@student.tudelft.nl`.
1. Clone your fork; Go to your fork on Gitlab and hit the "clone" button on the top right. Copy the SSH-url and perform the following command in git: `git clone <the url you copied>`, e.g. `git clone git@gitlab.ewi.tudelft.nl:reasoning_and_logic/book_solutions.git`.
1. Open index.tex in your tex installation. You should be able to compile this document to a pdf. (On Linux systems, you can install `make` and run the `make` command to compile the document.)
1. Make any changes/additions to the proper files. Remember that index.tex is the one you should compile for the document.
1. Make sure to also add your name to the contributors.tex and README.md files.
1. Commit your changes in git: `git add . && git commit -m '<A summary of your changes>'`
1. Push your changes to your fork: `git push`
1. [Create a merge request](https://gitlab.ewi.tudelft.nl/reasoning_and_logic/book_solutions/merge_requests/new) to get your changes into our version of the book solutions.
1. Process any comments we leave on your merge request.
1. Enjoy your contribution to the book!

## Requirements
- LaTeX ([texlive](https://www.tug.org/texlive/), [miktex](https://miktex.org/) or [MacTex](https://www.tug.org/mactex/))
- [GNU Make](https://www.gnu.org/software/make/) (GNU/Linux & Mac)
- [unzip](http://infozip.sourceforge.net/UnZip.html) (GNU/Linux & Mac)
- [wget](https://www.gnu.org/software/wget/) (GNU/Linux & Mac)
- [Garamond Math*](https://ctan.org/pkg/garamond-math) (Windows)
- [xelatex*](http://xetex.sourceforge.net/)

\* Included in most LaTeX releases

## Known issues
- *LaTeX Error: Command \XeTeX already defined*

Comment out line 62 with the value **\usepackage{bidi}**

## Credits
These answers written by Stefan Hugtenburg (@MrHug) with contributions
from:

- Valentijn van de Beek (@valentijn)
- Max van Deursen (@mvandeursen)
- Julian Kuipers (@Misterjuul)
- Jindrich Pohl (@jpohl)

The Delftse Foundation of Computation is written by [Stefan Hugtenburg] and
[Neil Yorke-Smith] and is released under the [Creative Commons Attribution
NonCommercial-ShareAlike-4.0 International License]

[Stefan Hugtenburg]: https://www.tudelft.nl/ewi/over-de-faculteit/afdelingen/software-technology/distributed-systems/people/stefan-hugtenburg/
[Neil Yorke-Smith]: https://www.tudelft.nl/ewi/over-de-faculteit/afdelingen/software-technology/algorithmics/people/neil-yorke-smith/
[Reasoning & Logic course (CSE1300)]: https://studiegids.tudelft.nl/a101_displayCourse.do?course_id=51302
[Delftse Foundations of Computation]: https://textbooks.open.tudelft.nl/index.php/textbooks/catalog/book/13
[Creative Commons Attribution NonCommercial-ShareAlike-4.0 International License]: http://creativecommons.org/licenses/by-nc-sa/4.0/
