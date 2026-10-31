# ♟️ Lichess Spark Analysis

[![Open in Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jandreolli/lichess-big-data-analysis/blob/main/chess_game_analysis.ipynb)
![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-3.5.7-E25A1C?logo=apachespark&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-3.5.7-orange)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-F37626?logo=jupyter&logoColor=white)

Exploratory data analysis and machine learning on Lichess chess games using **Apache Spark (PySpark)**.

This project explores chess game outcomes, player ratings, opening strategies and game dynamics through distributed data processing, statistical analysis and machine learning.

The notebook supports both **Google Colab** and **local execution (VS Code)**.

---

## Project Overview

The objective of this project is to explore a large collection of chess games played on Lichess and investigate the factors that influence game outcomes.

Using Apache Spark, our project processes chess game data and applies analytical and machine learning techniques to identify patterns and relationships between different game characteristics.  

Our analysis explores several questions:

- **Player ratings and errors:** How do error rates vary according to players' ELO ratings?
- **Chess openings:** How do different openings influence winning probabilities?
- **Game outcome prediction:** Can match outcomes be predicted using player and game characteristics?
- **Game reversals:** What is the influence of chess openings on the likelihood of game reversals?

### Main objectives

- Process and analyze large-scale chess game data using PySpark.
- Perform exploratory data analysis and statistical aggregations.
- Investigate relationships between player ratings, openings and game outcomes.
- Build a machine learning model to predict chess game results.
- Visualize findings using Plotly.

---

## Technologies & Tools

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Apache Spark | Distributed data processing |
| PySpark | Python API for Apache Spark |
| Spark SQL | Data manipulation and transformations |
| Spark MLlib | Machine learning |
| Pandas | Data manipulation |
| Plotly | Interactive data visualization |
| KaggleHub | Dataset retrieval |
| Jupyter Notebook | Interactive development environment |  

---

## Dataset

**Source:** [Lichess September 2020 Dataset](https://www.kaggle.com/datasets/noobiedatascientist/lichess-september-2020-data)  

---

## Getting Started

You can execute the notebook in two different environments:

- Google Colab – recommended for users who want to get started without configuring a local Spark environment.
- Local execution – using Python, Java and VS Code.

### 1. Google Colab

The notebook includes an environment selector that automatically configures Spark depending on your choice.

**Step 1 – Open the notebook**

Click the badge at the top of this README:

[![Open in Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jandreolli/lichess-big-data-analysis/blob/main/chess_game_analysis.ipynb)

**Step 2 – Select the environment**

In the first configuration cell, set:

```python
ENVIRONMENT = "colab"
```

---

### 2. Local execution (VS Code)

Local execution is also supported.

#### Prerequisites

- Python 3.12
- Java 17
- VS Code
- Jupyter extension for VS Code

#### Step 1 – Clone the repository

```bash
git clone https://github.com/jandreolli/lichess-big-data-analysis.git

cd lichess-big-data-analysis
```

#### Step 2 – Create a virtual environment

```bash
python3 -m venv lichess_env

source lichess_env/bin/activate
```

#### Step 3 – Install Java

On Ubuntu:

```bash
sudo apt update
sudo apt install openjdk-17-jdk
```

Verify the installation:

```bash
java -version
```

#### Step 4 – Install Python dependencies

```bash
pip install --upgrade pip

pip install pyspark==3.5.7 kagglehub pandas plotly pyreadr
```

#### Step 5 – Configure the notebook

Open `chess_game_analysis.ipynb` in VS Code.

Select the Python interpreter associated with your `lichess_env` virtual environment.

In the first configuration cell, set:

```python
ENVIRONMENT = "local"
```  

---   

## Authors    

**Justine Andreolli**  _alias_ [@jandreolli](https://github.com/jandreolli)   
**Emilie Lardy**  _alias_ [@emilie.lardy](https://git.unistra.fr/emilie.lardy)