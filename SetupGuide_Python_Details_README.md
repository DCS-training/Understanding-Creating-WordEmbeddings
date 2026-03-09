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


#### Alternate option

- Google Colab is a similar working space to the above option.

You can use this option by following:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
(https://colab.research.google.com/github/DCS-training/Understanding-Creating-WordEmbeddings/blob/main/understanding-creating-word-embeddings.ipynb)

**Ensure to place this in the first cells in the codebook so you have all the necessary file**

```
!git clone https://github.com/DCS-training/Understanding-Creating-WordEmbeddings.git
%cd Understanding-Creating-WordEmbeddings
```