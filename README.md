# ResBaz Arizona 2021 | Basics of text processing with spaCy

- [ResBaz Arizona 2021 | Basics of text processing with spaCy](#resbaz-arizona-2021--basics-of-text-processing-with-spacy)
  - [- Final Notes](#--final-notes)
  - [Overview](#overview)
  - [Repository Structure](#repository-structure)
  - [Installation Instructions](#installation-instructions)
    - [Requirements](#requirements)
    - [If you don't have a `conda` environment](#if-you-dont-have-a-conda-environment)
  - [Using spaCy](#using-spacy)
    - [Run the program](#run-the-program)
  - [License](#license)
  - [Resources](#resources)
-------------------------

## Overview

In this workshop, we will dive into the basics of [spaCy](https://spacy.io/) for text processing. spaCy is a free Natural Language Processing Python library developed specifically for production environments.

The first part of the workshop will be dedicated to introducing spaCy and navigating through its documentation. The objective here is both to become familiar with the building blocks of spaCy, and to acquire documentation-reading skills (good for starting/intermediate pythonistas).

During the second part of the workshop, we will work in small groups and code. Using Jupyter notebooks, we will create a pipeline for text tokenization, part-of-speech tagging, parsing, and extracting named entities. Here, the objective is to put into practice what we learned from the documentation.

We will dedicate the last 15 minutes to discussing the advantages of using spaCy and its ecosystem (Prodigy, Thinc, and other tools).

*Instructor:* Damian Romero

*Level:* Intermediate

## Repository Structure
    .
    ├── README.md
    ├── LICENSE
    ├── data
    │   ├── processed
    │   └── raw
    ├── notebooks
    ├── solutions


## Installation Instructions

Follow the instructions below to install and run spaCy and Jupyter Notebooks on your computer. Alternatively, you can take a look at the [spaCy](https://spacy.io/usage) and/or [Jupyter](https://jupyter.org/install) documentation directly.

You will find two types of installation instructions: one for `pip` and one for `conda`. If you don't know the difference, you can take a look at [this brief post](https://modelpredict.com/how-not-to-break-your-python-environment-again/).

***Important Note:*** do not change your default system Python. If you are not sure how to install a new version of Python, please look at [this post](https://realpython.com/effective-python-environment/).


### Requirements

- Python (>=3.6)
- Unix/Linux, macOS/OS X or Windows
- (Optional) [conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html)
- About 1GB of free storage for language models (you can eliminate these later).


### Install without a [`conda` environment](https://realpython.com/effective-python-environment/)

1. [Install a working version of Python (>=3.6) or above.](https://realpython.com/installing-python/)
2. Open the command prompt or terminal in your computer
3. Install spaCy by typing `pip install -U spacy` and enter on your console
4. Install two of the English language models `python -m spacy download en_core_web_sm` and `python -m spacy download en_core_web_trf`
5. Install Jupyter by typing `pip install notebook` and enter on your console
6. Check that your installations were successful with `pip freeze`


#### Install with a [`conda` environment](https://realpython.com/effective-python-environment/)

1. Create a new conda environment. To be on the same page, we will use Python 3.7.6 and name our environment `spacy_test`. Do: `conda create -n spacy_test python=3.7.6`
2. Activate your new environment with `conda activate spacy_test`
3. Check your conda version has a spaCy 3.0 distribution `conda search spacy`. If so, do: `conda install spacy=3.0.6`
4. Install spaCy. I recommend doing so from pip to avoid issues on the next step:  `pip install spacy=3.0.6`. Alternatively, do: `conda install -c conda-forge spacy=3.0.6`.
5. Install two of the English language models `python -m spacy download en_core_web_sm` and `python -m spacy download en_core_web_trf`
6. Install Jupyter `conda install notebook`
7. Check your installations by running `conda list`.

## Using Jupyter

This section is just for practice. On the day of the workshop, you will find all the notebooks we will use uploaded to this repo.

Let's get started with our first notebook. Open your terminal and navigate to the folder for this repository:

```bash
# On Windows
> cd \path\to\this_repo\folder
> jupyter notebook # This may take a while, so be patient

# On MacOS
$ cd /path/to/this_repo/folder
$ jupyter notebook # This may take a while, so be patient
```

A browser window should have opened. Now, navigate to the `notebooks` folder and open the `first_notebook` file. Follow the instructions on the notebook.


## License

All code is licensed under the [MIT License](https://opensource.org/licenses/MIT) - see the [LICENSE](LICENSE) file for details.

For the data used in this repository, please consult the original license.

## Resources

- [spaCy documentation](https://spacy.io/)
- [Jupyter documentation](https://jupyter.org/)
- From Real Python: [An Effective Python Environment: Making Yourself at Home](https://realpython.com/effective-python-environment/)
- From Real Python: [Running Python "from the command line"](https://realpython.com/run-python-scripts/)
- From Real Python: [Introduction to Jupyter Noebooks](https://realpython.com/jupyter-notebook-introduction/)
- [Conda: Myths and Misconceptions](https://jakevdp.github.io/blog/2016/08/25/conda-myths-and-misconceptions/) by Jake VanderPlas 
- [The difference between conda and pip and how not to break your environment again?](https://modelpredict.com/how-not-to-break-your-python-environment-again/) by Mario Kostelac.


------------

<!-- ![visitors](https://visitor-badge.glitch.me/badge?page_id=damian-romero.ResBaz21_spaCy_basics) -->