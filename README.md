# Quantum codes do not fix qubit independent errors

This notebook complements the homonymous article written by the authors, by proving several claims made in the article with the assistance of a symbolic calculus library for Python, as well as in wxMaxima.

## Table of Contents

1. [Authors](https://github.com/rafamartinc/qec_qip_5q#1-authors)
2. [Python Implementation](https://github.com/rafamartinc/qec_qip_5q#1-python-implementation)
    1. [Online visualization](https://github.com/rafamartinc/qec_qip_5q#2-1-online-visualization)
    2. [Local execution and editing](https://github.com/rafamartinc/qec_qip_5q#2-2-local-execution-and-editing)
        1. [Code download](https://github.com/rafamartinc/qec_qip_5q#2-2-1-code-download)
        2. [Installation](https://github.com/rafamartinc/qec_qip_5q#2-2-2-installation)
        3. [Execution](https://github.com/rafamartinc/qec_qip_5q#2-2-3-execution)
3. [wxMaxima Implementation](https://github.com/rafamartinc/qec_qip_5q#3-wxmaxima-implementation)

---

## 1. Authors

- **J. Lacalle**, Dep. de Matemática Aplicada a las TIC, ETS de Ingeniería de Sistemas Informáticos, Universidad Politécnica de Madrid, C/ Alan Turing s/n, 28031, Madrid, Spain ([jesus.glopezdelacalle@upm.es](mailto://jesus.glopezdelacalle@upm.es)).

- **L. M. Pozo-Coronado**, Dep. de Matemática Aplicada a las TIC, ETS de Ingeniería de Sistemas Informáticos, Universidad Politécnica de Madrid, C/ Alan Turing s/n, 28031, Madrid, Spain ([lm.pozo@upm.es](mailto://lm.pozo@upm.es)).

- **A. L. Fonseca de Oliveira**, Facultad de Ingeniería, Universidad ORT, Montevideo, Uruguay ([fonseca@ort.edu.uy](mailto://fonseca@ort.edu.uy))

- **R. Martin-Cuevas**, Programa de Doctorado en Ciencias y Tecnologías de la Computación para Smart Cities, ETS de Ingeniería de Sistemas Informáticos, Universidad Politécnica de Madrid, C/ Alan Turing s/n, 28031, Madrid, Spain ([r.martin-cuevas@alumnos.upm.es](mailto://r.martin-cuevas@alumnos.upm.es)).

---

## 2. Python Implementation

This version of the code has been developed using [Python 3](https://www.python.org/). Additionally, it uses SymPy ([Official website](https://www.sympy.org/en/index.html), [GitHub repo](https://github.com/sympy/sympy)), a Python library for symbolic mathematics, to perform the calculations described in the article. It also uses Jupyter Notebook ([Official website](https://jupyter.org/), [GitHub repo](https://github.com/jupyter/notebook)) to shape the document that contains the code and make it more readable, attaching all associated explanations and references to the main article.

You may choose to just visualize this document online, or to download it in your system if you intend to run it locally and/or edit it.

> The files associated to this implementation can be found in the folder ```jupyter```.

### 2.1. Online visualization (without installation)

The latest version of the implementation in Python can be seen from Jupyter's online tool for Notebook visualization and sharing, nbviewer:

[Notebook on Jupyter's nbviewer](https://nbviewer.jupyter.org/github/rafamartinc/quantum_codes_do_not_fix_qubit_independent_errors/blob/main/jupyter/main.ipynb)

The cache duration on nbviewer.jupyter.org is approximately 10 minutes. Therefore, if a commit to this repository has been done in the last 10 minutes, you may not be seeing the last version of the code. To invalidate the cache and force nbviewer to re-render a notebook page, append ```?flush_cache=true``` to the URL.

### 2.2 Local execution and editing

#### 2.2.1 Code download

You may get this software by downloading this repository in a ZIP compressed file, directly from [this link](https://github.com/rafamartinc/quantum_codes_do_not_fix_qubit_independent_errors/archive/main.zip), and extracting it in the folder of your choice. Alternatively, you may also use the following git command (after installing Git on your system: [Linux and Unix](https://git-scm.com/download/linux), [Git for Windows](https://gitforwindows.org/))

##### Using HTTPS:

```shell
git clone https://github.com/rafamartinc/qec_qie_5q.git
```

##### Using SSH:

```shell
git clone git@github.com:rafamartinc/qec_qie_5q.git
```

##### 2.2.2 Installation

Begin by making sure that [Python 3](https://www.python.org/) is installed in the system that you intend to use to run the code. After installing it, you may use the following command to install the specific libraries used by this repository, after placing your terminal in the same folder where the repository files are located.

```shell
pip install -r jupyter/requirements.txt
```

##### 2.2.3 Execution

After the installation has been completed, and from the same terminal, you may run either one of the following commands to initialize the notebook. A web server will be hosted temporarily on your system in order to render the Jupyter Notebook in your usual web browser. Your web browser should open automatically once you run either one of the following lines:

```shell
python -m notebook jupyter/main.ipynb
```

```shell
jupyter notebook jupyter/main.ipynb
```

If your web browser does not open itself, follow the instructions provided by the command in your terminal. Once the Notebook is ready, you will be able to run the code locally, and apply any modifications.

---

## 3. wxMaxima implementation

You may find the same proceedings implemented in wxMaxima as well. [wxMaxima(https://wxmaxima-developers.github.io/wxmaxima/) is a document based interface for the computer algebra system [Maxima](https://maxima.sourceforge.io/). **Maxima** is a system for the manipulation of symbolic and numerical expressions, including differentiation, integration, Taylor series, Laplace transforms, ordinary differential equations, systems of linear equations, polynomials, sets, lists, vectors, matrices and tensors. Maxima yields high precision numerical results by using exact fractions, arbitrary-precision integers and variable-precision floating-point numbers. Maxima can plot functions and data in two and three dimensions. **wxMaxima** provides menus and dialogs for many common maxima commands, autocompletion, inline plots and simple animations.

You may find more information about how to install and use wxMaxima in different systems at: https://wxmaxima-developers.github.io/wxmaxima/download.html

Alternatively, a PDF version of the code has also been included, should you want to read the code without installing the software.

> The files associated to this implementation can be found in the folder ```wxmaxima```.
