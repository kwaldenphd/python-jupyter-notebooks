# Python and Jupyter Notebooks

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>
This tutorial is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

## Lab Goals

By the end of this lab, students will be able to:
- Install Anaconda in their local environment
- Understand the core components of the Jupyter Notebooks environment
- Compare and contrast Python IDEs

## Acknowledgements

The documentation for Google Colab was developed by Spring 2021 graduate teaching assistant [Subhadyuti Sahoo](https://github.com/SDSAHOO703).

Peer review and editing was provided by Spring 2021 graduate teaching assistants [Subhadyuti Sahoo](https://github.com/SDSAHOO703) and [Aidan Draper](https://github.com/adraper2).

The author consulted the following texts when writing this tutorial:
- Allen Downey, [*Think Python: How to Think Like a Computer Scientist*](https://www.oreilly.com/library/view/think-python-2nd/9781491939406/) (O'Reilly, 2015).
  * Chapter 2 "Variables, Expressions and Statements" (11-20)
- Quinn Dombrowski, Tassie Gniady, and David Kloster, "Introduction to Jupyter Notebooks," *The Programming Historian* 8 (2019), https://doi.org/10.46430/phen0087

# Table of Contents

- [Different types of Python environments](#different-types-of-python-environments)
- [Installing Anaconda](#installing-anaconda)
- [Python in Jupyter notebooks](#python-in-jupyter-notebooks)
  * [Installing packages in Jupyter notebooks](#installing-packages-in-jupyter-notebooks)
- [Lab Notebook Questions](#lab-notebook-questions)

# Different types of Python environments

1. Up to this point, we have used the browser-based IDE [Replit](https://repl.it/).

2. What is an IDE? "An integrated development environment (IDE) is a software application that provides comprehensive facilities to computer programmers for software development. An IDE normally consists of at least a source code editor, build automation tools and a debugger" ([Wikipedia](https://en.wikipedia.org/wiki/Integrated_development_environment)).

3. An IDE can include features like syntax highlighting, code completion, version control, and debugging.

5. There are a WIDE range of IDEs that are proprietary or open-source, tailored to a specific language or able to work across languages.

5. Some common IDEs include Eclipse, Geany, Brackets, Atom, PyCharm, Spyder, RStudio, etc. For more in IDEs, visit Wikipedia's ["Comparison of integrated development environments"](https://en.wikipedia.org/wiki/Comparison_of_integrated_development_environments) page.

6. Replit (generally) worked for (most of) our needs in Elements I. But it ran into problems with more complex programs or programs involving external files/datasets/etc. 

7. Now, we're going to install Python on your local computer, using a distribution called Anaconda.

8. What is Anaconda? "Anaconda is a open-source distribution of the Python and R programming languages for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment. The distribution includes data-science packages suitable for Windows, Linux, and macOS. It is developed and maintained by Anaconda, Inc., which was founded by Peter Wang and Travis Oliphant in 2012" ([Wikipedia](https://en.wikipedia.org/wiki/Anaconda_(Python_distribution))).

9. The Anaconda environment includes a number of specific tools and programs, including:
- JupyterLab
- Jupyter Notebook
- Qt Console
- Spyder
- Glue
- Orange
- RStudio
- Visual Code Studio

10. This semester, we'll be using the Jupyter Notebook and Spyder components of Anaconda.

# Installing Anaconda

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/Figure_1.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/Figure_1.png?raw=true" /></a></p>

11. Windows/PC instructions:
- Anaconda Documentation, ["Installing on Windows"](https://docs.anaconda.com/anaconda/install/windows/) *Anaconda* (2020).
- ProgrammingKnowledge, ["Install Anaconda Python, Jupyter Notebook and Spyder on Windows 10"](https://youtu.be/5mDYijMfSzs) *YouTube video* (4 September 2018).

12. Mac OS instructions:
- Anaconda Documentation, ["Installing on macOS"](https://docs.anaconda.com/anaconda/install/mac-os/) *Anaconda* (2020).
- Understanding Data, ["Easily Install Anaconda Python Distribution On Mac OS X"](https://youtu.be/V6ZAv7hBH6Y) *YouTube video* (16 October 2019).

13. Chromebook instructions:
- Alex P. Miller, ["Data Science on a Chromebook: How to run Jupyter, Python, and R locally in ChromeOS"](https://alex.miller.im/posts/data-science-chromebook-pixelbook-jupyter-python-r/) *personal blog* (6 March 2019).
- Noebrian, ["Installing Anaconda on a Chromebook"](https://chromebook.home.blog/2019/01/20/installing-anaconda-on-a-chromebook-no-dev-beta-or-crouton-needed/) *ChromeBooks* (20 January 2019).

<blockquote>Q1: Describe your experience installing Anaconda using the available/provided documentation. What did you expect to happen? What challenges did you face? How did you solve them?</blockquote>

# Python in Jupyter notebooks

14. What is Jupyter?

15. "Project Jupyter is a non-profit, open-source project, born out of the IPython Project in 2014 as it evolved to support interactive data science and scientific computing across all programming languages. Jupyter will always be 100% open-source software, free for all to use and released under the liberal terms of the modified BSD license" (["About Us"](https://jupyter.org/about), *Jupyter.org*)

16. Project Jupyter receives funding from a range of non-profit foundations and corporate partners that include:
- Alfred P. Sloan Foundation
- Gordon and Betty Moore Foundation
- Google
- Microsoft

17. Institutional partners for Project Jupyter include:
- Apple
- Bloomberg
- Netflix
- Cal Poly
- Berkeley
- Amazon Web Services (AWS)

18. The name Jupyter is a reference to the three core languages supported by the project: **Ju**lia, **Py**thon, and **R**.

19. And what is a Jupyter notebook?

20. According to "[The Jupyter Notebook](https://jupyter-notebook.readthedocs.io/en/stable/notebook.html)" documentation:

<blockquote>The notebook extends the console-based approach to interactive computing in a qualitatively new direction, providing a web-based application suitable for capturing the whole computation process: developing, documenting, and executing code, as well as communicating the results. The Jupyter notebook combines two components:
 <ul>
  <li>A web application: a browser-based tool for interactive authoring of documents which combine explanatory text, mathematics, computations and their rich media output.</li>
  <li>Notebook documents: a representation of all content visible in the web application, including inputs and outputs of the computations, explanatory text, mathematics, images, and rich media representations of objects</li>
 </ul>
 </blockquote>

21. A Jupyter notebook is a file (the notebook document) that displays or renders in a web browser.

22. We'll be launching Jupyter Notebooks through Anaconda. 

23. The web application component of the notebook will be hosted on your local computer and the notebook document will save to a file directory on your local computer.

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/Figure_1.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/Figure_1.png?raw=true" /></a></p>

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/Figure_5.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/Figure_5.png?raw=true" /></a></p>

24. It may take some time for the notebook to open in a browser window.

<p align="center"><a href="https://github.com/kwaldenphd/python-refresh/blob/main/figures/Figure_6.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-refresh/blob/main/figures/Figure_6.png?raw=true" /></a></p>

25. When in a new notebook document, you have four main components to the user interface:
- Notebook name
- Menu bar
- Toolbar
- Code cell

26. The notebook name is what the `.ipynb` file created via the Jupyter notebook will be saved as.

27. Click on the default notebook name (usually `Untitled`) to rename the notebook.

28. The menu bar includes drop-down options used to manipulate the notebook functionality.

29. The toolbar icons give you quick access to the most commonly-used features of the notebook environment.

30. Code cells are the default type of cell.

31. But why are there cells?

32. Jupyter notebooks consist of a sequence of cells.

33. A cell is a multiline text input field. 

34. You can execute the contents of a cell by using `Shift-Enter`, clicking the `Play` button in the toolbar, or the `Cell` and `Run` icons in the menu bar.

35. How a cell executes is determined by its type.

36. There are three types of Jupyter notebook cells.

37. ***Code cells*** allow you to edit and write code with full syntax highlighting and tab completion.

38. ***Markdown cells*** allow you to document the computational process using descriptive text formatted using the markdown language.

39. ***Raw cells*** allow you to write output directly. These cells are not evaluated by the notebook and render unmodified.

40. You can edit or work within a code cell until you get the desired output, then move on to a new cell.

41. You can use markdown cells along the way to document your process using narrative text (alongside or in addition to code comments used in code cells).

42. To learn more about formatting text in markdown, visit Adam Pritchard's ["Markdown Cheatsheet"](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) resource page.

43. You can download a Jupyter notebook as a `.ipynb` file (this is the default option).

44. You can also use the `File` - `Download as` menu options to download the notebook in a number of other formats, including `.py`, `.pdf`, or `.html`.

45. There's a lot to love about Jupyter notebooks. 

46. A few challenges or drawbacks:
- Version control especially in collaborative environments is virtually impossible
- Jupyter lacks the debugging tools and autocompletion features of an IDE
- Testing and debugging code is virtually impossible
- Installing third-party packages or modules can be tricky 
- Jupyter's non-linear workflow limits transparent reproducible code
- Jupyter doesn't play well with external big data applications (spark/dask/distributed)

<blockquote>Citation: Alexander Mueller, <a href= "https://towardsdatascience.com/5-reasons-why-jupyter-notebooks-suck-4dc201e27086">"5 reasons why jupyter notebooks suck"</a>, <i>Towards Data Science</i> (24 March 2018)</blockquote>

47. So when could you use Jupyter notebooks? 

48. Jupyter notebooks are fantastic tools for exploration. 

49. They also work well for documenting process, or in situations when you might need to alternate between code and other kinds of text (like say in a lab notebook).

### Installing packages in Jupyter notebooks

50. You might see internet documentation that suggests you apply the install terminal syntax directly in a code cell.
```Python
!conda install --yes numpy

!pip install numpy
```

51. Resist this temptation!

52. When installing a package in a notebook environment, you want to make sure the package is installed in the currently-running Jupyter kernel.

53. We can do this by loading the package and the adding a line of code to install the package in the current Jupyter kernel if needed.

```Python
# sample code for installing numpy using conda

# import sys module
import sys

# line of code to install numpy
!conda install --yes --prefix {sys.prefix} numpy
```

```Python
# sample code for installing numpy using pip

# import sys module
import sys

# line of code to install numpy
!{sys.executable} -m pip install numpy
```

54. If you have already installed a package at the command line using `pip` or `conda`, launching Jupyter from the Anaconda navigator should not require installing the package again.

55. For more on installing Python packages in the Jupyter notebook environment:
- Jake VanderPlas, ["Installing Python Packages from a Jupyter Notebook"](https://jakevdp.github.io/blog/2017/12/05/installing-python-packages-from-jupyter/) *Pythonic Perambulations personal blog* (5 December 2017)

<blockquote>Q2: Compare your experience working in different Python IDEs. What seems appealing about each? What seems challenging? Based on this experience, what is your preference, or are there situations in which you'd prefer one over the other?</blockquote>

# Lab Notebook Questions

Q1: Describe your experience installing Anaconda using the available/provided documentation. What did you expect to happen? What challenges did you face? How did you solve them?

Q2: Compare your experience working in different Python IDEs. What seems appealing about each? What seems challenging? Based on this experience, what is your preference, or are there situations in which you'd prefer one over the other?
