# Hierarchical Clustering

This repository contains an implementation of the Hierarchical Clustering algorithm, a popular unsupervised learning technique used to group data into clusters based on their hierarchical relationships.

## Dataset

The dataset used in this implementation consists of unlabeled data points that need to be grouped into clusters. The data can be in any format, such as CSV, and typically includes numerical features.

## Contents

- **hierarchical_clustering.py**: The main script that implements the Hierarchical Clustering algorithm, including data preprocessing, model training, and visualization of the dendrogram and clusters.
- **data.csv**: The dataset file used for clustering.
- **requirements.txt**: A list of Python dependencies required to run the code.
- **plots/**: A directory containing visualizations of the clustered data.

## Implementation Details

The implementation follows these steps:

1. **Data Loading**: The dataset is loaded from `data.csv` and prepared for clustering.
2. **Data Preprocessing**: Preprocessing steps such as scaling the data and handling missing values are applied to ensure optimal clustering performance.
3. **Model Training**: The Hierarchical Clustering algorithm is applied to the preprocessed data. Both agglomerative (bottom-up) and divisive (top-down) clustering approaches can be used.
4. **Dendrogram Visualization**: A dendrogram is generated to visualize the hierarchical relationships between data points.
5. **Cluster Formation**: Clusters are formed by cutting the dendrogram at a chosen distance threshold.
6. **Evaluation**: Metrics such as silhouette score and cophenetic correlation coefficient are provided to evaluate the quality of the clustering.

## Usage

To use this code, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/mazimum86/hierarchical-clustering.git
    ```
2. Navigate to the repository directory:
    ```bash
    cd hierarchical-clustering
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Run the Hierarchical Clustering script:
    ```bash
    python hierarchical_clustering.py
    ```

## Dependencies

The following Python packages are required to run the code:

- pandas
- scikit-learn
- numpy
- matplotlib
- scipy
- seaborn

These dependencies are listed in the `requirements.txt` file and can be installed using `pip`.

## Results

The output includes:

- **Dendrogram**: A dendrogram showing the hierarchical relationships between data points.
- **Cluster Labels**: The cluster labels assigned to each data point.
- **Cluster Visualization**: Scatter plots showing the clusters formed by cutting the dendrogram.
- **Evaluation Metrics**: Metrics like the silhouette score and cophenetic correlation coefficient to assess the quality of the clustering.

## Contributing

Contributions are welcome! If you have any ideas for improvements or additional features, feel free to submit a pull request or open an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
