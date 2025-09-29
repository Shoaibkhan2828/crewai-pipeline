🚀 Agentic Architecture for Automated Data Analysis using CrewAI 🤖📊

Welcome to a modular, agent-driven data analysis pipeline built with the CrewAI framework. This project demonstrates the power of autonomous, collaborative agents in performing end-to-end data analysis with minimal human intervention.

🧠 Overview

This system leverages CrewAI to orchestrate multiple specialized agents, each responsible for a distinct phase of the data analysis lifecycle. The architecture is designed to be extensible, interpretable, and capable of real-time collaboration between agents using structured task dependencies.

👥 Agents and Responsibilities

Each agent operates autonomously with its own mission and tools:

Data_Collection_Agent
Uses a custom Data_Collection_Tool to load and extract initial insights from the dataset.

Data_Cleaning_Agent
Utilizes a Data_Cleaning_Tool to handle missing values, normalize data, and ensure consistency.

Data_Analysing_Agent
Performs deeper statistical analysis to uncover patterns and trends in the cleaned data.

Data_Plotting_Agent (WIP)
Employs the CodeInterpreterTool to generate Python code for data visualizations and executes the code to render plots.

🛠️ Tech Stack & Tools

Framework: CrewAI

Languages: Python

Libraries: pandas, matplotlib, seaborn, numpy

AI Tools: Custom CrewAI tools, CodeInterpreterTool, Gemini

Dataset: california_housing_test.csv

🔁 Workflow

The system follows a clearly defined pipeline:

Data Collection ➡️ Data Cleaning ➡️ Data Analysis ➡️ (WIP) Visualization


Each step is executed by a dedicated agent.

The Crew object manages agent coordination and task sequencing.

Dependencies are enforced to maintain a logical flow.

📂 Use Case: California Housing Dataset

Tested on the california_housing_test.csv dataset, the system:

Extracted dataset shape, column data types, and null value analysis.

Cleaned and normalized the data automatically.

Performed exploratory data analysis (EDA) and presented structured insights.

(In progress) Visualized key patterns using auto-generated Python plotting code.

✅ Features

Modular agent design for scalability.

Structured and autonomous data analysis.

Easily extensible to new datasets or analysis steps.

Clear separation of concerns between collection, cleaning, analysis, and visualization.

📌 Next Steps

Finalize and integrate the Data_Plotting_Agent.

Expand analysis capabilities (e.g., correlation matrix, feature importance).

Introduce natural language querying for user interaction with the agents.

📬 Feedback & Contributions

Feel free to open issues or pull requests if you'd like to contribute or improve this project!
