SpendDNA: Financial Archetype Analyzer
SpendDNA is a pure-Python financial analytics pipeline designed to process raw, unstructured banking transaction data and transform it into actionable financial insights.

While most data cleaning and anomaly detection pipelines rely heavily on external libraries, this project was built under strict programmatic constraints to demonstrate a foundational mastery of Data Structures, mathematical logic, and core Python processing.

⚙️ The Engineering Challenge
To prove raw coding proficiency without relying on "black box" libraries, this pipeline strictly adheres to the following constraints:

No Regular Expressions (re): All currency scrubbing and text parsing is handled via native Python string manipulation.

No ML or Statistical Libraries (scipy): Statistical outliers are flagged by calculating Z-scores manually through core Pandas aggregation formulas.

No Visualization Libraries (matplotlib / seaborn): Data presentation is achieved through a custom-built, terminal-based ASCII reporting engine utilizing f-string alignments.

🔍 Key Features
Algorithmic Parser: Ingests messy CSVs, standardizes multi-format date strings, and scrubs irregular currency symbols (₹, Rs., commas) natively.

Heuristic Categorization Engine: Acts as a lightweight NLP tagger, mapping chaotic UPI and payment gateway descriptions to canonical vendors and categories using iterative boolean matching.

Mathematical Anomaly Detection: Computes the standard deviation and mean for individual spending categories to detect and flag high-variance transactions (Z-Score > 2).

Financial Archetyping: Applies conditional logic to the processed analytics to generate a user personality profile (e.g., The Foodie, The YOLO Spender) and outputs a "Spotify Wrapped" style terminal dashboard.

🚀 Getting Started
Prerequisites
You only need Python and its core data manipulation libraries installed to run this pipeline.

Python 3.8+

Pandas

NumPy

Installation & Execution
Clone this repository to your local machine.

Ensure your transaction data is saved as Data set for DADS June.csv in the root directory (or update the file path in the script).

Run the Jupyter Notebook or Python script to execute the pipeline.

View the generated ASCII report directly in your terminal or output cell.

📁 Project Structure
SpendDNA.ipynb : The core analytical pipeline and logic engine.

Data set for DADS June.csv : The raw transaction dataset (replace with your own export).

README.md : Project documentation.

👤 Author
Tanishq Pardeshi
B.Tech in Computer Science and Engineering (Business Systems)
