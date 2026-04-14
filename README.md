## 📊 Implementation of Fairness-Aware Range Queries for Selecting Unbiased Data

**🚀 Overview:**

This project focuses on designing and implementing fairness-aware range query algorithms to reduce bias in data selection. It explores both unweighted and weighted fairness models using efficient search strategies like Best-First Search (BFS) and its optimized variants.

The goal is to ensure that query results are balanced across sensitive attributes (e.g., gender) while maintaining efficiency and accuracy.

**🎯 Key Objectives:**

1. Reduce selection bias in range queries
2. Support both unweighted and weighted fairness constraints
3. Optimize query performance using heuristic search algorithms
4. Compare brute-force vs heuristic approaches

**🧠 Core Concepts Implemented:**

**🔹 SPQA (Single Predicate Query Adjustment)**

Handles fairness in single-attribute queries

Supports:

✅ Unweighted fairness
✅ Weighted fairness

**🔹 BFSMP (Best-First Search Multi-Predicate)**

Extends fairness to multi-dimensional queries

Uses:

1. Priority queue-based exploration
2. Similarity-driven search

**🔹 IBFSMP (Improved BFSMP)**

Enhanced version of BFSMP with:

✅ U-threshold pruning (avoids unnecessary exploration)
✅ Visited set / graph structure (prevents redundant states)

✅ Range trees for efficient querying

✅ Supports both:

1. Weighted fairness

2. Unweighted fairness

**🔹 Additional Techniques**

1. Skyline Queries – for optimal result selection
2. Range Trees – for efficient multidimensional range search
3. Fairness Validation – using threshold-based checks

**📂 Dataset Used:**

📌 Math Dataset (~400 records)

📌 Credit Card Dataset (~3500 records)

**Features include:**

1. LIMIT_BAL (credit limit)
2. AGE

**Sensitive attribute: Gender**

**⚙️ Algorithms Covered:**

🔸 2D Case
BFSMP for fairness-aware range queries

🔸 3D Case
IBFSMP for improved performance and fairness

**🏗️ Project Structure:**

├── SPQA (Unweighted & Weighted)

├── BFSMP (2D Queries)

├── IBFSMP (3D Queries)

├── Range Trees

├── Skyline Implementation

├── Dataset Processing

└── Evaluation & Comparison

**🧪 How It Works:**

1. Define an initial query range
2. Evaluate fairness using a threshold (ε)
3. If unfair:
Expand/adjust query using BFS-based methods
Use:
Priority queues
Range trees
Heuristics
4. Return:
Fair and optimized query range

**📌 Key Features:**

1. Fairness-aware query processing
2. Multi-dimensional data handling
3. Efficient search using heuristics
4. Scalable for large datasets
5. Real-world dataset validation

**🛠️ Tech Stack:**

1. Python
2. NumPy / Pandas
3. Priority Queues (Heap)
4. Custom Algorithms (BFS, Heuristics)
5. Data Structures (Range Trees, Graphs)
   
**📊 Use Cases:**

1. Bias-free data selection
2. Fair AI / ML preprocessing
3. Financial risk analysis
4. Decision support systems
5. Ethical data querying
   
**🔮 Future Work:**

1. Extend to higher-dimensional datasets
2. Integrate with real-time databases
3. Improve approximation strategies
4. Apply to production-scale AI systems
