# Pandas-Data-Analyst-AI-Copilot
Explore Data with ease.


This Streamlit application is designed to act as a Pandas Data Analyst AI Copilot, allowing users to upload CSV or Excel files, ask questions about the data, and receive either data tables or interactive visualizations in response. Below is a breakdown of the key components and functionality of the app:

Key Features
OpenAI API Integration:

![alt image](https://github.com/boprosv/Pandas-Data-Analyst-AI-Copilot/blob/main/Screenshot%202025-03-11%20140759.png?raw=true)

Users must input their OpenAI API key to use the app.

The app validates the API key by attempting to fetch the list of available models from OpenAI.

Users can select between different OpenAI models (e.g., gpt-4o-mini, gpt-4o).

![alt image](https://github.com/boprosv/Pandas-Data-Analyst-AI-Copilot/blob/main/Screenshot%202025-03-11%20140851.png?raw=true)

File Upload and Data Preview:

Users can upload CSV or Excel files.

The app previews the first few rows of the uploaded dataset using st.dataframe.

![alt image](https://github.com/boprosv/Pandas-Data-Analyst-AI-Copilot/blob/main/Screenshot%202025-03-12%20123219.png?raw=true)

AI Agent Setup:

The app uses a PandasDataAnalyst agent, which includes:

A DataWranglingAgent for data manipulation and transformation.

A DataVisualizationAgent for generating interactive charts using Plotly.

The agent processes user queries and returns either tables or visualizations.

Chat Interface:

Users can input questions in a chat interface.

![alt image](https://github.com/boprosv/Pandas-Data-Analyst-AI-Copilot/blob/main/Screenshot%202025-03-12%20125437.png?raw=true)

The app maintains a chat history using StreamlitChatMessageHistory.

Responses are displayed in the chat interface, including tables, charts, or error messages.

Dynamic Output Handling:

If the agent decides to return a chart, the app uses Plotly to render the visualization.

If the agent decides to return a table, the app displays the data in a DataFrame.

Charts and tables are stored in session state for persistence across interactions.

![alt image](https://github.com/boprosv/Pandas-Data-Analyst-AI-Copilot/blob/main/Screenshot%202025-03-12%20120812.png?raw=true)

Error Handling:

The app includes error handling for invalid API keys, file upload issues, and agent processing errors.

If chart generation fails, the app falls back to returning a table.

![alt image](https://github.com/boprosv/Pandas-Data-Analyst-AI-Copilot/blob/main/Screenshot%202025-03-12%20120841.png?raw=true)

The Chart is fully interactive, so you can have detailed analysis.

![alt image](


