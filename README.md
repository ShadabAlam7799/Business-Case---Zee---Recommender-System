# Zee Recommender System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-green)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow)

## Overview

This project implements a **content-based recommender system** for Zee Entertainment, designed to suggest relevant TV shows or movies to users based on their viewing preferences. Built using Python and popular data science libraries, the system leverages metadata such as genre, cast, director, and plot summaries to recommend items similar to those a user has previously enjoyed.

The solution is implemented in a Jupyter Notebook compatible with **Google Colab**, making it easy to run in the cloud with minimal setup.

---

## Features

- **Content-Based Filtering**: Recommends shows/movies based on item metadata and user preferences.
- **TF-IDF Vectorization**: Converts textual features (like plot summaries) into numerical vectors.
- **Cosine Similarity**: Measures similarity between items to generate recommendations.
- **Interactive Demo**: Includes sample function calls to demonstrate recommendation output.
- **Google Colab Ready**: Full compatibility with Google Colab for easy execution.

---

## Project Structure

```
Project 12 - Business Case - Zee_Recommender_System(google_colab).ipynb
```

- Single Jupyter Notebook containing:
  - Data loading and preprocessing
  - Feature engineering (e.g., combining metadata fields)
  - Model building using TF-IDF and cosine similarity
  - Recommendation function with usage examples

---

## Requirements

Ensure the following libraries are installed (automatically handled in Google Colab):

- `pandas`
- `numpy`
- `scikit-learn`
- `jupyter` (if running locally)

Install dependencies locally with:
```bash
pip install pandas numpy scikit-learn jupyter
```

---

## How to Use

### In Google Colab:
1. Upload the notebook to your Google Drive.
2. Open it in **Google Colab**.
3. Run all cells sequentially to:
   - Load and preprocess the dataset
   - Train the recommender model
   - Test recommendations using the `get_recommendations(title)` function

### Locally (with Jupyter):
1. Clone/download the notebook.
2. Open a terminal and start Jupyter:
   ```bash
   jupyter notebook
   ```
3. Navigate to and open the notebook.
4. Run all cells.

### Example Usage:
```python
# Get top 5 recommendations for "Kundali Bhagya"
get_recommendations("Kundali Bhagya")
```

---

## Dataset

The system assumes access to a metadata-rich dataset containing fields such as:
- `title`
- `genre`
- `cast`
- `director`
- `plot_summary` or `overview`

*(Note: The actual dataset file is not included in this repository. Ensure the required CSV or data source is available in the environment.)*

---

## Business Value

- **Personalized Content Discovery**: Helps users find relevant shows quickly, improving engagement.
- **Increased Watch Time**: Better recommendations lead to longer session durations.
- **Scalable Architecture**: The model can be extended to include user ratings or hybrid approaches.

---

## Future Enhancements

- Integrate **collaborative filtering** for a hybrid system.
- Add **user profile tracking** for dynamic recommendations.
- Deploy as a web app using **Flask** or **Streamlit**.
- Incorporate real-time viewing data for live personalization.

---

## Authors

- Prepared as part of **Project 12 – Business Case**  
- For educational and demonstration purposes  

---

## License

This project is for academic use. All rights related to Zee content and trademarks belong to their respective owners.

---

> **Note**: Replace placeholder dataset references with actual paths or APIs if deploying in production.
