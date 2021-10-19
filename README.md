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

[Link to lab notebook template](https://docs.google.com/document/d/1QCl_kV826kfGlu4qfDkCSDaeJ779jycXACRg3zp-no8/copy) (Google Doc, ND users)

# Different types of Python environments

1. Up to this point, we have used the browser-based IDE [Replit](https://repl.it/).

2. What is an IDE? "An integrated development environment (IDE) is a software application that provides comprehensive facilities to computer programmers for software development. An IDE normally consists of at least a source code editor, build automation tools and a debugger" ([Wikipedia](https://en.wikipedia.org/wiki/Integrated_development_environment)).

3. An IDE can include features like syntax highlighting, code completion, version control, and debugging.

5. There are a WIDE range of IDEs that are proprietary or open-source, tailored to a specific language or able to work across languages.

5. Some common IDEs include Eclipse, Geany, Brackets, Atom, PyCharm, Spyder, RStudio, etc. For more in IDEs, visit Wikipedia's ["Comparison of integrated development environments"](https://en.wikipedia.org/wiki/Comparison_of_integrated_development_environments) page.

6. Replit (generally) worked for (most of) our needs. But it ran into problems with more complex programs or programs involving external files/datasets/etc. 

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

10. This lab introduces us to using Jupyter Notebooks through Anaconda. It also includes resources for [getting started in Google Colab](https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/google-colab-instructions.md), a browser-based Jupyter Notebooks environment.

# Installing Anaconda

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true" /></a></p>

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

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true" /></a></p>

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_5.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_5.png?raw=true" /></a></p>

24. It may take some time for the notebook to open in a browser window.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_6.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_6.png?raw=true" /></a></p>

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

<blockquote>To learn more about configuring Jupyter Notebooks to download notebooks as PDFs:
 <ul>
  <li><a href="https://pypi.org/project/notebook-as-pdf/">Jupyter extension documentation</a></li>
  <li>Cornellius Yudha Wijaya, "<a href="https://towardsdatascience.com/jupyter-notebook-to-pdf-in-a-few-lines-3c48d68a7a63">Jupyter Notebook to PDF in a few lines</a>", <em>Towards Data Science</em> (12 July 2020)</li>
 </ul>
 </blockquote>

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

50. In a previous lab, we mentioned how you can use modules, libraries, and packages to extend Python's functionality.

51. That previous lab used the built-in `csv` and `json` modules. 

52. We did not need to install those modules since they are already included in Python.

53. All we had to do was use an `import` statement to bring those modules into our Python program.

```Python
# sample import statement
import MODULE NAME
```

54. But, there are many situations in which we would need to install a Python module, package, or library before being able to use `import`.

55. Let's take a look at the installation instructions for a few common Python libraries.
- `NumPy` (scientific computing), ["Installing NumPy"](https://numpy.org/install/)
- `SciKit-Learn` (machine learning), ["Installing scikit-learn"](https://scikit-learn.org/stable/install.html)
- `pandas` (data wrangling/analysis) ["Installation"](https://pandas.pydata.org/docs/getting_started/install.html)
- `matplotlib` (data visualization) ["Installation"](https://matplotlib.org/stable/users/installing.html)

56. The documentation for each library includes sample code for installing the library in different Python environments and operating systems.

57. Many libraries/packages will include sample code for installing the package using `pip`, an installation method available through the Python Package Index.

58. Most libraries/packages will also include sample code for installing the package through Anaconda, sometimes referred to as `conda` in documentation.

58. BUT...these install commands are not something we should run within our Python program, whether we're working in a `.py` script or a `.ipynb` notebook.

59. You might see internet documentation that suggests you apply the install terminal syntax directly in a code cell.

```Python
!conda install --yes numpy

!pip install numpy
```

60. Resist this temptation!

61. We want to make sure the library is installed correctly in our Python environment, so we need to run the install command in a terminal/shell.

FIG_1

fig4

62. You can access a terminal/shell by launching the Anaconda Navigator and clicking the `Launch` button in the `CMD.exe Prompt` tile.

fig5

63. Then, within the terminal, we can run the install command.
- `pip` will work, but when possible `conda` is best

64. We can also open a terminal from within Jupyter Notebooks.

fig1

fig2

65. In the Jupyter Notebook main window (first browser tab that opens when you launch the program), click the `New` drop-down in the top right-hand corner.

66. Select `Terminal` under `Other` to open a terminal.

fig3

67. Then, within the terminal, we can run the install command.
- Again, `pip` will work, but when possible `conda` is best.

68. If you absolutely must install a package from within a notebook, we can use the `sys` module to install the package from within the notebook.

```Python
# sample code for installing numpy using conda

# import sys module
import sys

# line of code to install numpy using conda
!conda install --yes --prefix {sys.prefix} numpy
```

```Python
# sample code for installing numpy using pip

# import sys module
import sys

# line of code to install numpy using pip
!{sys.executable} -m pip install numpy
```

For more on installing Python packages in the Jupyter notebook environment:
- Jake VanderPlas, ["Installing Python Packages from a Jupyter Notebook"](https://jakevdp.github.io/blog/2017/12/05/installing-python-packages-from-jupyter/) *Pythonic Perambulations personal blog* (5 December 2017)

69. If you have already installed a package at the command line using `pip` or `conda`, launching Jupyter from the Anaconda navigator should not require installing the package again.

<blockquote>Q1: Use the Anaconda or Jupyter terminal to install the four libraries mentioned in step 55 (numpy, scikit-learn, pandas, matplotlib). Describe your experience installing these libraries using the available/provided documentation. What did you expect to happen? What challenges did you face? How did you solve them?</blockquote>

70. You can load the module/library/package in your Python program using `import`.

MODULE ERROR FIGURE

71. The `import` statements won't have an output, but the absence of a `ModuleNotFoundError` message is a good sign.

<blockquote>Q2: Write import statements for each of the libraries you installed in Q1. What did you expect to happen? What challenges did you face (if any)?</blockquote>

```Python
# import pandas 
import pandas

# import pandas using pd alias
import pandas as pd
```

```Python
# import numpy
import numpy

# import numpy using np alias
import numpy as np
```

```Python
# import scikit-learn
import sklearn

# import datasets module from scikit-learn
from sklearn import datasets

# import linear models from scikit-learn
from sklearn import linear_model
```

```Python
# import matplotlib
import matplotlib.pyplot

# import matplotlib using plt alias
import matplotlib.pyplot as plt
```

## ADD SECTION ON MODIFYING LAB PROCEDURE

## ADD SECTION ON EXPORT TO HTML/PDF

## OPTIONAL SECTION ON SPYDER

# Lab Notebook Questions

[Link to lab notebook template](https://docs.google.com/document/d/1QCl_kV826kfGlu4qfDkCSDaeJ779jycXACRg3zp-no8/copy) (Google Doc, ND users)

Q1: Describe your experience installing Anaconda using the available/provided documentation. What did you expect to happen? What challenges did you face? How did you solve them?

Q2: Compare your experience working in different Python IDEs. What seems appealing about each? What seems challenging? Based on this experience, what is your preference, or are there situations in which you'd prefer one over the other?
