# Clustering ML – Lab Assignment 3

This repository contains solutions for Lab Assignment 3 focused on **clustering algorithms** in machine learning. It includes both **from-scratch implementations** and **scikit-learn-based applications** on real and synthetic datasets.

---

## 📌 Contents

### Q1. K-Means from Scratch
- Implemented `k_means(X, k, max_iter, tol)` without using scikit-learn.
- Follows all steps: random initialization, distance calculation, centroid update, convergence check.
- Tested on 2D synthetic blob data and visualized results.

### Q2. Image Compression Using K-Means
- Loaded a small RGB image and reshaped it into pixel matrix.
- Applied `KMeans(n_clusters=16)` using scikit-learn.
- Compressed the image by replacing pixels with their cluster centroids.
- Displayed original and compressed images, reported file size reduction.

### Q3. Clustering Analysis on Iris Dataset
- Ran KMeans for `k=2 to 10`.
- Plotted Inertia and Silhouette Score vs `k`.
- Chose optimal `k` based on:
  - Elbow method (`k_elbow`)
  - Maximum silhouette score (`k_silhouette`)
- Printed and compared both values.

### Q4. KMeans vs MiniBatchKMeans Benchmarking
- Generated 1 million 10D samples with 10 true clusters.
- Compared:
  - Training time
  - Final inertia
  - Adjusted Rand Index (ARI)
- Wrapped into a function `benchmark_kmeans()` that returns a dictionary and prints a table.

### Q5. KMeans with Cosine Distance
- Implemented KMeans using cosine similarity.
- Applied to TF-IDF vectors from 20 Newsgroups (4 "sci" categories).
- Re-initialized empty clusters using max-min heuristic.
- Reported final cosine inertia and empty-cluster reinitializations.

---

## Technologies Used

- Python
- Jupyter Notebook
- NumPy
- scikit-learn
- Pillow
- Matplotlib
- SciPy

---

## Preview

- ✅ Cluster plots for blob data  
- ✅ Image compression results (Original vs Compressed)  
- ✅ Metrics vs `k` for Iris dataset  
- ✅ Performance benchmarking table  
- ✅ Cosine distance-based clustering stats

---

## License

This project is for academic/lab purposes. Feel free to reuse with credit.

---

## Contributions

Pull requests and suggestions are welcome. Happy learning! 😊
