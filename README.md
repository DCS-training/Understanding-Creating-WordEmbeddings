# Understanding and Creating Word Embeddings
This repository contains the materials for the **Silent Disco: Understanding and Creating Word Embeddings** workshop.

The tutorial introduces the basic concepts behind **word embeddings** and demonstrates how they can be explored using computational methods.

The workshop is available in **both Python and R**:

* If you would like to follow the **Python version**, please navigate to:
  **[[Programming Historian](https://programminghistorian.org/en/lessons/understanding-creating-word-embeddings)]**

* If you would like to follow the **R version**, the materials are provided in this repository and described below.

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

## Code Files

The repository contains the **R tutorial** for the workshop:

```
word_embeddings.Rmd
```

This RMarkdown file contains the full tutorial, including theoretical explanations and executable code.

Participants can open this file in **RStudio** and run the code sections sequentially.

---

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

