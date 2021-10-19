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
  * [Authoring in Jupyter notebooks](#authoring-in-juyter-notebooks)
  * [Jupyter notebook export options](#jupyter-notebook-export-options)
- [IF NEEDED: Getting Started With Google CoLab](getting-started-with-google-colab)
- [Other Lab Notebook Questions](#other-lab-notebook-questions)
- [OPTIONAL: Python in Spyder](#optional-python-in-spyder)
- [Lab Notebook Questions](#lab-notebook-questions)


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

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/Figure_1.png?raw=true" /></a></p>

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig4.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig4.jpg?raw=true" /></a></p>

62. You can access a terminal/shell by launching the Anaconda Navigator and clicking the `Launch` button in the `CMD.exe Prompt` tile.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig5.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig5.jpg?raw=true" /></a></p>

63. Then, within the terminal, we can run the install command.
- `pip` will work, but when possible `conda` is best

64. We can also open a terminal from within Jupyter Notebooks.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig1.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig1.jpg?raw=true" /></a></p>

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig2.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig2.jpg?raw=true" /></a></p>

65. In the Jupyter Notebook main window (first browser tab that opens when you launch the program), click the `New` drop-down in the top right-hand corner.

66. Select `Terminal` under `Other` to open a terminal.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig3.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig3.jpg?raw=true" /></a></p>

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

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/module_error.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/module_error.png?raw=true" /></a></p>

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

## Authoring in Jupyter Notebooks

72. Remember there are three types of Jupyter notebook cells.
- ***Code cells*** allow you to edit and write code with full syntax highlighting and tab completion.
- ***Markdown cells*** allow you to document the computational process using descriptive text formatted using the markdown language.
- ***Raw cells*** allow you to write output directly. These cells are not evaluated by the notebook and render unmodified.

73. There are a few ways you can change a cell's type.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig6.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig6.jpg?raw=true" /></a></p>

74. One option is to select the cell type from the drop-down options.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig7.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig7.jpg?raw=true" /></a></p>

75. Another option is to select `Cell Type` from the `Cell` menu tab.

76. You'll also notice there are keyboard shortcuts for changing cell type.
- `y` (code)
- `m` (markdown)
- `r` (raw)

77. A couple of notes on keyboard shortcuts...
- When a cell is highlighted in green (click inside the cell's text box), this indicates you are editing in the cell.
- When a cell is highlighted in blue (click to the left of the cell's text box), this indicates you are modifying the entire cell.

A few other useful keyboard shortcuts:
- `x` (delete a cell)
- `a` (insert cell above, default is code cell)
- `b` (insert cell below, default is code cell)

78. To put that another way:
- Green: Typing code, adding text to a markdown cell, etc.
- Blue: Changing the type of cell using keyboard shortcuts

<blockquote>Q3: In a markdown cell, add text that includes the following style or formatting components:
 <ul>
  <li>Heading (h1, h2, h3, etc)</li>
  <li>Italics or bold text formatting</li>
  <li>Unordered (or bulleted point) list</li>
  <li>Link</li>
 </ul>
 NOTE: You will want to reference Adam Pritchard's <a href="https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet">Markdown Cheatsheet</a> resource when working on this question.
 </blockquote>

<blockquote>Q4: In a code cell, write a simple Python program (or programs) that includes the following functions:
 <ul>
  <li><code>input()</code></li>
  <li><code>print()</code></li>
 </ul>
 You are welcome to use a program (or programs) you've written for previous labs- original code is not required for this question. The main point for this question is to see how a Jupyter Notebook code cell executes a program.</blockquote>
 
## Jupyter Notebook Export Options

79. You can download a Jupyter notebook as a `.ipynb` file (this is the default option).

80. You can also use the `File` - `Download as` menu options to download the notebook in a number of other formats, including `.py`, `.pdf`, or `.html`.

81. NOTE: The PDF export options require additional configuration.

82. Specifically, we're going to install the `notebook-as-pdf` and `pyppeteer` libraries. These allow HTML and PDF export and are much easier than trying to set up and configure LaTeX.

83. Open a terminal (through Anaconda or Jupyter) and type the following commands (hitting `Enter` or `Return` after each line).

```
python -m pip install -U notebook-as-pdf
pyppeteer-install
```

84. Once both installation processes have completed, you can close the terminal.

85. You will need to restart the Python Kernel for the new export options to be available.

<p align="center"><a href="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig8.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/images/fig8.jpg?raw=true" /></a></p>

86. Click one of the `Restart` options under the `Kernel` menu tab.

87. If needed, re-run any code cells.

<blockquote>To learn more about configuring Jupyter Notebooks to download notebooks as PDFs:
 <ul>
  <li><a href="https://pypi.org/project/notebook-as-pdf/">Jupyter extension documentation</a></li>
  <li>Cornellius Yudha Wijaya, "<a href="https://towardsdatascience.com/jupyter-notebook-to-pdf-in-a-few-lines-3c48d68a7a63">Jupyter Notebook to PDF in a few lines</a>", <em>Towards Data Science</em> (12 July 2020)</li>
 </ul>
 </blockquote>

# Getting Started With Google CoLab

Anaconda is a hefty software program that may not run (or run well) on your personal computer.

"'Colaboratory,' or 'CoLab' for short, is a product from Google Research. Colab allows anybody to write and execute arbitrary python code through the browser, and is especially well suited to machine learning, data analysis and education. More technically, Colab is a hosted Jupyter notebook service that requires no setup to use, while providing free access to computing resources including GPUs." ([Google Colaboratory, "Frequently Asked Questions"](https://research.google.com/colaboratory/faq.html))

If Jupyter Notebooks through Anaconda is not a good fit, Google CoLab is a robust alternative.

["Google CoLab Instructions"](https://github.com/kwaldenphd/python-jupyter-notebooks/blob/main/google-colab-instructions.md), developed by Spring and Fall 2021 graduate teaching assistant [Subhadyuti Sahoo](https://github.com/SDSAHOO703).

See also:
- ["Welcome to Colaboratory"](https://colab.research.google.com/notebooks/intro.ipynb) notebook from Google CoLab

# Other Lab Notebook Questions

Q5: Compare your experience working in different Python IDEs. What seems appealing about each? What seems challenging? Based on this experience, what is your preference, or are there situations in which you'd prefer one over the other?

Q6: After working through the previous steps, export your notebook for this lab as a PDF. Submit both the Jupyter Notebook (.ipynb) and PDF file on Canvas.

# OPTIONAL: Python in Spyder

88. If you've got extra time and want to explore another Python IDE included in Anaconda...

89. What is Spyder? "Spyder is a free and open source scientific environment written in Python, for Python, and designed by and for scientists, engineers and data analysts. It features a unique combination of the advanced editing, analysis, debugging, and profiling functionality of a comprehensive development tool with the data exploration, interactive execution, deep inspection, and beautiful visualization capabilities of a scientific package" ([Spyder documentation](https://www.spyder-ide.org/)).

90. Spyder's core components include:
- Editor
- IPython console
- Variable explorer
- Plots
- Debugger
- Help

91. These robust Python features in Spyder are incredibly useful as you start to do more work with datasets, visualizations (plots), and debugging in more complex programming environments.

<p align="center"><a href="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_1.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_1.png?raw=true" /></a></p>

<p align="center"><a href="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_2.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_2.png?raw=true" /></a></p>

92. Open the Anaconda navigator and select the option to launch Spyder.

<p align="center"><a href="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_2a.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_2a.png?raw=true" /></a></p>

93. Spyder has three default panes that show up when you launch the program.

94. Your `.py` file shows up on the left-hand side of the program window. This is where you will write Python code. You can have multiple `.py` files open in Spyder and navigate between the tabs. 

95. The top-right pane has four default options:
- Variable explorer, which lets you see named variables in your program
- Help, which provides additional documentation, information, or resources
- Plots, which will show visualizations generated by your program
- Files, which will show all files currently open or active in your Spyder workspace

96. The bottom-right pane is the Console, which lets you execute and test Python commands. You can have multiple consoles open simultaneously.

97. So how is the Console different from your `.py` file?

98. In the `.py` file you are writing a Python program that will run or execute when the file is called. You make updates to that file, save changes, etc.

99. The Console lets you execute Python commands but is not saving those commands as part of a `.py` file. 

100. Great for testing. Less great for building out complex programs.

101. NOTE: When we were working in Replit, all files that were part of our Python project were in the same virtual workspace. 

102. That's not going to be the case when working in a desktop IDE like Spyder. 

103. Think of this as the difference between working with files in Google Drive versus on your local computer. 

104. You can set a working directory, which is where Spyder will look for external files you are wanting to access from within a Python program. The working directory is also where Python will save `.py` files you build.

<p align="center"><a href="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_2c.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_2c.png?raw=true" /></a></p>

105. Click on the folder icon in the top-right hand corner of Spyder (next to the arrow icon) to set a working directory. It doe--where you save `.py` files and other files (think data files) you might be wanting to access as part of a Python program.

106. Now, files don't have to be in your current working directory for you to access them in Python. But you'll need to provide the full file path (i.e. location information or directory information for where that file is located on your computer).

107. Go ahead and create an `EoC_II` folder and set that folder as your working directory in Spyder. It might also be a good idea to start creating lab-specific sub-folders within your `EoC_II` parent folder. 

108. This will help with organization as we move through labs and work with a variety of sample files and datasets.

109. Work through the ["First Steps with Spyder" resources](https://docs.spyder-ide.org/current/first-steps-with-spyder.html) provided by Spyder. That includes two 3.5 minute videos that introduce you to the basics of the Spyder IDE and how to get started with Python in Spyder.

<blockquote>QA: How is Spyder different than previous IDEs? What do you see as strengths/advantages? What do you see as possible challenges?</blockquote>

<blockquote>OPTIONAL: Take a <code>.py</code> lab notebook file and load it into Spyder. Explore how the program runs in a different IDE. In particular, explore Spyder's options to run portions or a selection of the larger program. How does this change the way you interact with the program?</blockquote>

# Debugging

110. To paraphrase an old programming joke, writing code is 90% of the work of programming. Debugging is the other 90%.

111. You've been working on a program for hours, your head hurts, and something still isn't working. We all know a version of that feeling.

112. There's no easy solution that will prevent all problems (or "bugs") in your code. But having strategies for testing your code, recognizing and making sense of error messages, and methodically debugging your code can help immensely.

113. Python errors will usually fall into three types: syntax, runtime, and semantic.

114. Syntax refers to the structure of a program and rules about that structure. 

115. ***Syntax errors*** involve things like indentation, parenthesis, etc. The Python interpreter expects the language to be structured a specific way, and throws a syntax error when it's not.

116. ***Runtime errors***, or ***exceptions***: appears after a program has started running. These errors indicate something unexpected has happened that interrupts or stops the program execution. 

117. Things that can cause a runtime error include:
- Misspelled or incorrectly capitalized variables or function names
- Dividing by zero
- Mismatched data types (i.e. attempting to perform operations on data of the wrong type)
- Attempting to use a type conversion function on a value that can't be converted

118. Semantic: relates to meaning. 

119. ***Semantic errors*** have to do with the meaning (or purpose/intent) of your code. Semantic errors don't show up as error messages-but the program will not do what you expect it to do. 

120. The debugging strategies discussed here will focus on semantic errors but are useful for all types of errors.

## Stepwise debugging in Spyder

121. Spyder will catch many syntax and runtime errors. 

122. Hover over a red `X` by any of your lines of code to see more information about a possible error.

123. Spyder integrates the enhanced `ipdb` debugger, which gives you robust options for troubleshooting or debugging your code.

124. Specifically, the debugger will let you run a program line by line, running a single line of code and waiting for you to tell it to continue.

125. Running your program through this kind of debugging is immensely valuable for tracking down bugs or catching complex issues in a program.

126. This mode of debugging includes the following possible steps or "moves":
- Continue (run the program until the next breakpoint)
- Step in (executes the next line of code; if the next line of code is a function, the debugger will 'step into' the first line of that function)
- Step over (executes the next line of code, but will not go line-by-line through the function; the debugger 'steps over' the function code and waits for the function call to return)
- Step out (lets you step out of a function if you used step in and want to 'step out' of the function)
- Stop (stops debugging and terminates the program)

<p align="center"><a href="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_3.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_3.png?raw=true" /></a></p>

<p align="center"><a href="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_4.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/python-spyder/blob/main/images/Figure_4.png?raw=true" /></a></p>

127. Let's use this approach and Spyder functionality to debug a number adding program..

```Python
print('Enter the first number to add: ')
first = input()
print('Enter the second number to add: ')
second = input()
print('Enter the third number to add: ')
third = input()
print('The sum is ' + first + second + third)
```

128. First run the program without the debugger enabled. What happens?

129. Debug the file going line-by-line. Remember to use `Step Over` to execute functions without going into each line of the function code.
- Functions in this sample program include `print()` and `input()`
- You can always `Step Out` if you accidently step into a function

<blockquote>QB: What type of error does this program return (syntax, runtime, semantic) and why? How would we go about modifying the program to address this error?</blockquote>

## Other approaches to debugging

130. If you've never put a `print()` statement in your code to output a variable's value while the program is running, you have used a form of `logging` to debug your code.

131. Python's `logging` module lets you record custom messages that output as part of your program. 

132. These `log` messages describe when the program reaches a point where a logging function is called and what variables have been specified at that point.

133. Step one is to import the `logging` module and set up basic configuration for the module at the top of your `.py` file.

```Python
import logging
logging.basicConfig(level=logging.DEBUG, format=' %(asctime)s - %(levelname)s - %(message)s')
```

134. This configuration information instructs Python to create a `LogRecord` object when a logging function is called, and to include specific information about that event in the `LogRecord` object.

135. So how would we use the `logging` module when writing a program?

136. Say we were creating a function that calcualted the factorial of a given number.
- Factorial 4 is 1 x 2 x 3 x 4 = 24
- Factorial 7 is 1 x 2 x 3 x 4 x 5 x 6 x 7 = 5040

```Python
import logging
logging.basicConfig(level=logging.DEBUG, format=' %(asctime)s - %(levelname)s - %(message)s')
logging.debug('Start of program')

def factorial(n):
  logging.debug('Start of factorial(%s%%)' % (n))
  total = 1
  for i in range(n + 1):
    total *= i
    logging.debug('i is ' + str(i) + ', total is ' + str(total))
  logging.debug('End of factorial(%s%%)' % (n))
  return total

print(factorial(5))
logging.debug('End of program')
```

137. Anytime we call the `logging.debug()` function, the configuration information from the start of the file governs the log formatting and messages.

<blockquote>QC: What happens when we run this program? What kinds of log messages do we get, and what information do they give us?</blockquote>

<blockquote>QD: Is this program doing what we expect? Where would you go next with debugging or addressing the error?</blockquote>

## But why can't I debug using `print()`

138. It can seem unwieldy to configure the `logging` module and write lines of code dedicated just to logging what's happening in your program.

139. But think about the factorial example. Log messages led us right to the program's issue. 

140. Trying to debug using `print()` calls means you'll have to go back through each line of your program to remove `print()` statements used for debugging (while also making sure you aren't removing `print()` statements that are a component of the actual program).

141. Think of the `logging` module as a report that generates alongside your program output as it executes. The program executes and you also have useful log information about what happened along the way.

142. Once you're done debugging the program, you can add the `logging.disable()` function to the start of your program to supress the log messages without actually having to modify your program.

<blockquote>Visit Python's <a href="https://docs.python.org/3/howto/logging.html">Logging HOWTO</a> documentation to learn more about the logging module.</blockquote>

<blockquote>QE: What are your thoughts on this approach to identifying what's happening in your program? What seems appealing? What seems challenging? When or how could this approach be useful?</blockquote>

# Lab Notebook Questions

NOTE: As Q5 specifes, remember to submit two versions of your lab notebook on Canvas- a Jupyter Notebook (`.ipynb`) file and a PDF (a process we work through in an earlier section of the lab).

Q1: Use the Anaconda or Jupyter terminal to install the four libraries mentioned in step 55 (numpy, scikit-learn, pandas, matplotlib). Describe your experience installing these libraries using the available/provided documentation. What did you expect to happen? What challenges did you face? How did you solve them?

Q2: Write import statements for each of the libraries you installed in Q1. What did you expect to happen? What challenges did you face (if any)?

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

Q3: In a markdown cell, add text that includes the following style or formatting components:
- Heading (h1, h2, h3, etc)
- Italics or bold text formatting
- Unordered (or bulleted point) list
- Link

NOTE: You will want to reference Adam Pritchard's [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) resource when working on this question. 

Q4: In a code cell, write a simple Python program (or programs) that includes the following functions:
- `input()`
- `print()`

You are welcome to use a program (or programs) you've written for previous labs- original code is not required for this question. The main point for this question is to see how a Jupyter Notebook code cell executes a program.

Q5: Compare your experience working in different Python IDEs. What seems appealing about each? What seems challenging? Based on this experience, what is your preference, or are there situations in which you'd prefer one over the other?

Q6: After working through the previous steps, export your notebook for this lab as a PDF. Submit both the Jupyter Notebook (.ipynb) and PDF file on Canvas.

OPTIONAL SPYDER QUESTIONS:

QA: How is Spyder different than previous IDEs? What do you see as strengths/advantages? What do you see as possible challenges?

QB: What type of error does this program return (syntax, runtime, semantic) and why? How would we go about modifying the program to address this error?

QC: What happens when we run this program? What kinds of log messages do we get, and what information do they give us?

QD: Is this program doing what we expect? Where would you go next with debugging or addressing the error?

QE: What are your thoughts on this approach to identifying what's happening in your program? What seems appealing? What seems challenging? When or how could this approach be useful?
