# Understanding and Creating Word Embeddings
This repository contains the materials for the **Silent Disco: Understanding and Creating Word Embeddings** workshop, developed by Dr. Aybuke Atalay.

The tutorial introduces the basic concepts behind **word embeddings** and demonstrates how they can be explored using computational methods.

The workshop is available in **both Python and R**:

The goal of this workshop is to introduce how word embeddings represent relationships between words in a corpus and how these representations can be explored to investigate patterns in language use.

Participants will work through a step-by-step workflow that includes:

* preparing a textual corpus
* cleaning and tokenising text
* understanding how embedding models are trained
* exploring relationships between words using vector similarity
* interpreting and validating embedding results

The scripts contain explanations and commented code so that participants can follow the analytical workflow step by step and experiment with different queries.

---

# Workshop Aims

By the end of this workshop, participants should be able to:

* Understand the basic principles behind **word embeddings**
* Understand how **word vectors represent language in vector space**
* Prepare a corpus for embedding analysis
* Explore relationships between words using **cosine similarity**
* Perform simple vector arithmetic to query embedding models
* Interpret the results produced by embedding models

---

# Workshop Files

## Code Files (R)

This RMarkdown file below contains the full tutorial, including theoretical explanations and executable code.

```
word_embeddings.Rmd
```

Participants can open this file in **RStudio** and run the code sections sequentially. Alternatively, they can use Noteable (please see below for further details)

---

## Code Files (Python)

Python users will follow the pre-designed workshop: [Programming Historian](https://programminghistorian.org/en/lessons/understanding-creating-word-embeddings#corpus-size). 
You can directly follow the workshop using the link. However, it is important to note that this tutorial has some important setup requisites for working locally on your PC and depending on your experience with Python this could become a hassle. 
Therefore for those who would like to follow the tutorial using the University [Noteable](https://noteable.edina.ac.uk/launch) cloud service, we have added core materials from the tutorial to this repository so it can be cloned with a file structure and important installs pre-embedded.

The code file below contains the full tutorial in Python:
```
understanding-creating-word-embeddings.ipynb
```

## Data Files

The workshop uses a small corpus of **nineteenth-century American recipes**.

The texts are provided as `.txt` files stored in the following folder:

```
data/
  recipes/
    recipe_1.txt
    recipe_2.txt
    recipe_3.txt
    ...
```

Each file contains the text of one recipe. The tutorial demonstrates how these texts can be loaded, cleaned, and used to explore relationships between words in the corpus.

---

## Model Files

To ensure the workshop runs quickly on different machines, a **pre-trained word embedding model** is provided.

```
models/
  recipe_embeddings.rds
```

Instead of training a model during the session, participants will load this file and use it to explore the relationships between words in the corpus.

The tutorial also includes the training code so that participants can see how such models are normally created.

---
# Getting Started in Python (for R, please scroll down)

### Setting up for the word embedding tutorial in python

- The self guided tutorial is fully encompassed in the html link sent to you and it has some setup instructions requiring you to install some tools and have some pre-knowledge of working with Python locally on your PC. 
- Depending on whether you are a newcomer to programming or intermediate, you may or may not have an existing local setup suitable for working through the tutorial. 
- This current readme file will present a useful options for your setup following the necessary requisites of the tutorial and you are welcome to choose this to get started.

**Original tutorial guide**
[Tutorial link with descriptives & process](https://programminghistorian.org/en/lessons/understanding-creating-word-embeddings#corpus-size)


## Simplest approach for University members

Using Noteable --> (https://noteable.edina.ac.uk/launch) ---> Standard Python 3 ---> Clone ---> Paste this in (https://github.com/DCS-training/Understanding-Creating-WordEmbeddings.git)

- We have placed the necessary python codebook (ipynb) connected to the tutorial on this repository and a zipped data folder which you can clone and open in Noteable using EASE credentials. This way you will have an exact copy of the repository and work from the paths designed in there as follows:

```
├── understanding-creating-word-embeddings.ipynb
│
├── data/
│   └── recipes/
│       recipe_1.txt
│       recipe_2.txt
│       recipe_3.txt
│       ...
```

One everything is cloned onto Noteable. You can start by clicking on the python notebook which we have adjusted slightly to add some necessary installs. A secondary addition is a codeblock which unzips the data from the associated folder so that remaining code can be completed on the text corpora. Use the original tutorial link as you work through the codebook, since the tutorial has detailed explanations of each step and the linked methods for the code.

NOTE: the original authors of the tutorial are listed in the DOI link above, here we have simply added some small setup blocks for ease of access to run the tutorial on University cloud systems. The original codebook was downloaded from [here](https://nbviewer.org/github/programminghistorian/jekyll/blob/gh-pages/assets/understanding-creating-word-embeddings/understanding-creating-word-embeddings.ipynb) and the text corpora folder with data was downloaded from [here](https://programminghistorian.org/assets/understanding-creating-word-embeddings/ViralTexts-nineteenth-century-recipes-plaintext.zip)


#### Alternative Set-Up 

- Google Colab is a similar working space to the above option.

You can use this option by following:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
(https://colab.research.google.com/github/DCS-training/Understanding-Creating-WordEmbeddings/blob/main/understanding-creating-word-embeddings.ipynb)

**Ensure to place this in the first cells in the codebook so you have all the necessary file**

```
!git clone https://github.com/DCS-training/Understanding-Creating-WordEmbeddings.git
%cd Understanding-Creating-WordEmbeddings
```

# Getting Started in R

### Option 1 (Recommended): Noteable

If you are part of the **University of Edinburgh**, you can use
[https://noteable.edina.ac.uk](https://noteable.edina.ac.uk)

Noteable provides a cloud-based computational environment that allows you to run R without installing anything locally.

#### Start Noteable

1. Open: [https://noteable.edina.ac.uk/login](https://noteable.edina.ac.uk/login)
2. Login with your **EASE credentials**
3. Under **RStudio**, click **Start**

#### Clone the Repository

1. Click **Project (None)** → **New Project**
2. Select **Version Control**
3. Select **Git**
4. Paste the repository URL:

```
https://github.com/DCS-training/Understanding-Creating-WordEmbeddings
```

5. Click **Create Project**

This will clone the repository and make all files available in Noteable.

You can then open:

```
word_embeddings.Rmd
```

and follow the tutorial.

---

### Option 2: Running Locally with RStudio

If you prefer to run the workshop on your own computer:

#### Install R

1. Go to
   [https://www.r-project.org](https://www.r-project.org)
2. Download the version appropriate for your operating system
3. Follow the installation instructions

#### Install RStudio

1. Go to
   [https://posit.co/download/rstudio-desktop/](https://posit.co/download/rstudio-desktop/)
2. Download the version for your operating system
3. Install the software

#### Clone the Repository

Download or clone this repository and open the project folder in **RStudio**.

Then open:

```
word_embeddings.Rmd
```

Run the code chunks sequentially from top to bottom.

---

# Repository Structure

The repository is organised as follows:

```
├── word_embeddings.Rmd
│
├── data/
│   └── recipes/
│       recipe_1.txt
│       recipe_2.txt
│       recipe_3.txt
│       ...
│
└── models/
    └── recipe_embeddings.rds
```

* **word_embeddings.Rmd** – the main tutorial
* **data/recipes/** – the corpus used in the workshop
* **models/** – the pre-trained embedding model used for analysis

---

