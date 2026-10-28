AttLightGNN: Post-Pruning Node-Level Attention for Lightweight GNN-based Recommendation

This repository contains the implementation of the **AttLightGNN** model for the Gowalla dataset, as part of my Master's thesis: *Scalable and Efficient Graph Neural Network-Based Recommendation Systems*.

Contents
* `gowalla-attlightgnn.ipynb`: The main Kaggle notebook containing the code for the AttLightGNN model, training loop, pruning, and evaluation.

Important Requirements (Data & Pretrained Models)
Because the datasets and pretrained teacher/intermediate models are too large, they are **not** included in this repository. The notebook relies on two external components:

1. **LightGNN Pretrained Models**: 
   Download the `example_checkpoints.zip` and place the `gowalla` folder into `inModels/gowalla/`. 
   *(Source: Official LightGNN Repository)*

2. **Gowalla Dataset**:
   The notebook expects the dataset to be in `Datasets/sparse_gowalla/` containing `trnMat.pkl`, `tstMat.pkl`, and `valMat.pkl`.
   *(Source: Official LightGNN Repository)*

How to Run
1. Open `gowalla-attlightgnn.ipynb` in Kaggle or Jupyter Notebook.
2. Ensure you have the required dependencies installed (PyTorch, PyTorch Geometric, torch-scatter, torch-sparse).
3. Upload the missing data and models to the respective directories as described above.
4. Run the notebook cells sequentially.

Key Results (Gowalla)
* **AttLightGNN**: Recall@20 = 0.2667 | NDCG@20 = 0.1737
* **LightGNN Baseline**: Recall@20 = 0.2610 | NDCG@20 = 0.1684

## 📝 Citation
