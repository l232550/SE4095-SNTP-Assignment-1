# SE4095 — Social Network Theory and Practice — Assignment #01

**Student ID:** L232550  
**Course:** SE4095 Social Network Theory and Practice

## Problem

Investigate how influence and brokerage appear in the political-blog hyperlink network, whether the link structure recovers the two known political orientations, and how the network's most central blogs affect the stability and quality of those communities.

## Dataset

Adamic, L. A., and Glance, N. (2005). *The Political Blogosphere and the 2004 U.S. Election: Divided They Blog.* Proceedings of the 3rd International Workshop on Link Discovery.

**Source:** https://public.websites.umich.edu/~mejn/netdata/

## Setup

```bash
python -m venv .venv

# Windows:
.venv\Scripts\activate

# macOS/Linux:
source .venv/bin/activate

pip install -r requirements.txt

python -m ipykernel install --user --name=sntp-assignment --display-name "SNTP Assignment"
````

## Data

Download `polblogs.zip` from the source URL above and unzip `polblogs.gml` into the project root (the same folder as the notebook).

## Run

Open `L232550_SNTP_Assignment1.ipynb` in Jupyter, select the **SNTP Assignment** kernel, and choose:

**Kernel → Restart & Run All**

Outputs are written to `outputs/`.

## Methods Chosen

* **Centralities:**

  * PageRank
  * Betweenness Centrality

* **Community Detection:**

  * Louvain Modularity Maximization

## Reproducibility

* **Global seed:** `42`
* **Louvain stability seeds:** `[1, 7, 13, 42, 99]`
* **Random removal seed:** `42`
