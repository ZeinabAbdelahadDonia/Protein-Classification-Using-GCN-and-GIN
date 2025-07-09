# Protein-Classification-Using-GCN-and-GIN
This project performs graph classification to determine whether a protein structure (represented as a graph) corresponds to an enzyme or non-enzyme. It leverages Graph Convolutional Networks (GCN) and Graph Isomorphism Networks (GIN) and explores data augmentation using Cayley Graph Propagation.

# Dataset
- Uses the PROTEINS dataset from TUDataset.
- Each sample is a protein represented as a graph:
    - Nodes: Atoms or amino acid units.
    - Edges: Chemical or structural bonds.
    - Labels: Binary class — Enzyme (1) or Non-Enzyme (0).


# Project Structure

- **Data Exploration**
    - Visual inspection and preliminary statistics of protein graph data (from the TUDataset collection).

- **Preprocessing**

    - Cayley Graph Propagation (Cayele): Graph augmentation method that introduces virtual nodes to improve learning.

    - Visualization: Effects of Cayele expansion shown through before/after graph samples.

    - Data Augmentation: Techniques to expand and enrich the training data.

- **Modeling**

    - Implementations of GCN and GIN architectures.

    - Training loop and performance metrics.

- **Hyperparameter Tuning**

    - Grid search across model depth, learning rates, dropout rates, and hidden units.

- **Fine-tuning**
  
    -  Fine-tuning on the PROTEINS dataset from TUDataset.
    -  Best model selection and final performance evaluation.
 
# Results & Insights

- Graph classification performance is improved by augmenting data with Cayele transformation.

- Visual inspection supports the structural advantages of Cayele-expanded graphs.

- Fine-tuned GIN generally performs better on enzyme classification than vanilla GCN.

# Contributors
- https://github.com/KonouzA
- https://github.com/omaar28
- https://github.com/Retaj12003
- Myself
