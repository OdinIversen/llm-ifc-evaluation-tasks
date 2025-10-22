# Evaluation Tasks for LLM-based IFC Interpretation

This document lists the 21 evaluation tasks used in our study, categorized by the BIM model they apply to.

## Model 1: hello-wall
*Description: A simple IFC model representing a wall structure with two windows.*

| Task ID | Category | Description | Expected Result |
|---|---|---|---|
| task_1_1 | Model Summarization & Domain Identification | Provide a very brief high-level summary of the model's content and purpose. | Content: This model represents a wall structure with two windows. Purpose: Testing IFC, software development and education. |
| task_1_2 | Geometric & Spatial Analysis | What is the height, width, and thickness of the wall. | Height: 3.0 m, Width: 10.0 m, Thickness: 0.1 m |
| task_1_3 | Property & Attribute Retrieval | What materials are used in the model? | Concrete, wood, and glass. |
| task_1_4 | Object Identification & Enumeration | How many windows are present in the wall? | 2 |
| task_1_5 | Object Identification & Enumeration | How many doors are present in the wall? | 0 |
| task_1_6 | Object Identification & Enumeration | How many walls are present in the model? | 1 |
| task_1_7 | Geometric & Spatial Analysis | What is the height of the windows? | 1.2 |
| task_1_8 | Geometric & Spatial Analysis | What is the distance between the floor and the bottom of the glass of the windows? | 1.1 m |
| task_1_9 | Logical Inference & Constraint Checking | Does the space have a satisfactory view out from the building? | Yes, the space has a satisfactory view out from the building as it has two windows to the outside. |
| task_1_10 | Geometric & Spatial Analysis | What is the volume of the wall? | 2.78 |
| task_1_11 | Logical Inference & Constraint Checking | Is there room for one more window in the wall? | Yes, there is room for one more window in the wall. |

## Model 2: domestic-hot-water
*Description: An IFC model representing a domestic hot water system with various components.*

| Task ID | Category | Description | Expected Result |
|---|---|---|---|
| task_2_1 | Model Summarization & Domain Identification | Provide a very brief high-level summary of the model's content and purpose. | Content: This model represents a domestic hot water system, including pipes, a water heater tank, a sink, a bathtub, faucets, and a floor. Purpose: Testing IFC, software development and education. |
| task_2_2 | Object Identification & Enumeration | How many pipe segments are present in the model? | 9 (10 if you count the pipe fitting as a segment) |
| task_2_3 | Geometric & Spatial Analysis | What is the length, width, and thickness of the floor. | Length: 10 m, Width: 4.1 m, Thickness: 0.15 m |
| task_2_4 | Object Identification & Enumeration | How many sinks are present in the model? | 1 |
| task_2_5 | Object Identification & Enumeration | How many bathtubs are present in the model? | 1 |
| task_2_6 | Geometric & Spatial Analysis | How far above the floor is the top of the sink? | 1.05 |
| task_2_7 | Object Identification & Enumeration | How many water heater tanks are present in the model? | 1 |
| task_2_8 | Topological & Relational Analysis | What pipe segments are used to connect the water heater tank to the sink? | PIP_20 or #1403, PIP_20_001 or #1865, PIP_20_002 or #1770, PIP_20_003 or #1705, PIP_20_005 or #1455, PIP_20_007 or #1529 (TEE_20 or #2059 if you count the pipe fitting as a segment) |
| task_2_9 | Topological & Relational Analysis | What pipe segments are used to connect the water heater tank to the bathtub? | PIP_20 or #1403, PIP_20_004 or #2132, PIP_20_005 or #1455, PIP_20_006 or #1621, PIP_20_007 or #1529 (TEE_20 or #2059 if you count the pipe fitting as a segment) |
| task_2_10 | Logical Inference & Constraint Checking | Is the model satisfactory for a bathroom? | No, the model lacks a toilet, which is essential for a bathroom. |
