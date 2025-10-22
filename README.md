# LLM Evaluation Tasks for IFC Interpretation

This repository contains the supplementary data for the paper: **"Automating Building Model Preparation: A Comparison of LLM Performance on IFC-4x and IFC-5x"**.

## Overview

To ensure transparency and enable the replication of our research, we provide the complete list of 21 information extraction tasks used to evaluate the performance of Large Language Models (LLMs) on different Industry Foundation Classes (IFC) schema versions.

The tasks are designed to be relevant to Digital Building Permitting (DBP) and Automatic Compliance Checking (ACC), covering a range of categories from simple object identification to more complex logical inference.

## File Descriptions

This repository contains the tasks in two formats:

-   `tasks.json`: A machine-readable JSON file containing the full list of tasks, their categories, descriptions, and the ground-truth expected results.
-   `tasks.md`: A human-readable Markdown file that presents the same tasks in a clear, tabular format.

## Data Structure

Each task in the `tasks.json` file is an object with the following keys:
-   `task_id`: A unique identifier for the task.
-   `task_category`: The category of the evaluation task (e.g., "Geometric & Spatial Analysis").
-   `description`: The natural language question or prompt given to the LLM.
-   `expected_result`: The ground-truth answer used to evaluate the LLM's response.

## How to Cite

If you use these tasks in your research, please cite our paper:

```bibtex
@inproceedings{Iversen2025,
  author    = {Iversen, Odin and Hjelseth, Eilif and Fauth, Judith and Huang, Lizhen},
  title     = {Automating Building Model Preparation: A Comparison of LLM Performance on IFC-4x and IFC-5x},
  booktitle = {Proceedings of the Conference Name},
  year      = {2025},
  publisher = {Publisher Name},
  address   = {City, Country}
}
```
*(Note: Please update the BibTeX entry with the correct conference details upon publication.)*

## License

The contents of this repository are licensed under the MIT License. See the `LICENSE` file for details.
