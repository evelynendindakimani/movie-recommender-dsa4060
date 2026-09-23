# Movie Recommender System — DSA 4060

## Project Description
A personalised movie recommender system that uses a user's rating history
and movie genre features to suggest unseen films that match their taste.
The system implements and compares multiple recommendation approaches:
a popularity baseline, content-based filtering, item-based collaborative
filtering, and matrix factorization.

## Author
| Name | Student ID |
|---|---|
| Evelyne Kimani | 666813 |

## Dataset
- **Name:** MovieLens Latest Small
- **Source:** https://grouplens.org/datasets/movielens/
- **Interactions:** Ratings (1–5 stars), tags
- **Attributes:** Movie title, release year, genres (18 types)
- **Usage:** Research and educational purposes only

## Proposed Approaches
- **Baseline:** Popularity-based ranking
- **Method 1:** Content-based filtering (genre matching)
- **Method 2:** Item-based collaborative filtering
- **Advanced:** Matrix factorization

## Evaluation Metrics
- Precision@10
- Recall@10
- NDCG@10
- Catalogue coverage
- Diversity

## Milestones
- [x] Week 1–2: Proposal + GitHub repository setup
- [ ] Week 3–4: Data preparation + popularity baseline + content-based prototype
- [ ] Week 5–6: Item-based collaborative filtering + preliminary evaluation
- [ ] Week 8–10: Matrix factorization + parameter tuning
- [ ] Week 11–12: Streamlit interface + final evaluation + documentation
- [ ] Week 13: Presentation and demonstration
## Project Structure
movie-recommender-dsa4060/
├── data/
│ ├── raw/ # original MovieLens files
│ └── processed/ # cleaned and split data
├── notebooks/
│ ├── 01_data_inspection.ipynb
│ ├── 02_baseline.ipynb
│ ├── 03_content_based.ipynb
│ ├── 04_collaborative_filtering.ipynb
│ └── 05_matrix_factorization.ipynb
├── src/
│ ├── data_loader.py
│ ├── baseline.py
│ ├── content_based.py
│ ├── collaborative.py
│ ├── matrix_factorization.py
│ └── evaluate.py
├── app/
│ └── app.py
├── requirements.txt
└── README.md

## How to Run
1. Download MovieLens Latest Small from https://grouplens.org/datasets/movielens/
2. Place `ratings.csv` and `movies.csv` in `data/raw/`
3. Install dependencies:
   pip install -r requirements.txt
4. Run the Streamlit app:
   streamlit run app/app.py

## Requirements
pandas
numpy
scikit-learn
matplotlib
seaborn
streamlit
jupyter
surprise

## References
Harper, F. M., & Konstan, J. A. (2015). The MovieLens Datasets:
History and Context. ACM TiiS, 5(4), Article 19.
