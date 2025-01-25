
Personalized Student Recommendations

## Project Overview
This project analyzes quiz performance to provide students with personalized recommendations for improving their preparation. The application uses data from current and historical quiz submissions, highlighting weak topics, improvement trends, and performance gaps. It also assigns students to personas based on their performance metrics.

## Key Features
1. Data Analysis:
   - Identifies weak topics and highlights performance trends.
   - Analyzes topics and difficulty levels based on response data.

2. Recommendations:
   - Provides actionable advice based on weak areas.
   - Focuses on improvement strategies.

3. Insights and Personas:
   - Generates creative insights like average scores and common weak areas.
   - Assigns personas such as "High Achiever" or "Needs Improvement" for better understanding.

4. Visualizations:
   - Weak Topics Distribution: Bar chart showing the frequency of mistakes by topic.
   - Performance Trends: Line charts for score and accuracy trends over time.
   - Student Personas: Clustering scatter plot based on performance metrics.

## Setup Instructions
### Prerequisites
- Python 3.8 or higher
- Installed Python libraries:
  ```bash
  pip install pandas matplotlib seaborn scikit-learn requests
  ```

### Files and APIs
- APIs:
  - Current Quiz Data: `https://api.jsonserve.com/rJvd7g`
  - Historical Quiz Data: `https://api.jsonserve.com/XgAgFJ`
- Output Files:
  - `recommendations.csv`: Contains recommendations for each student.
  - `insights_summary.txt`: Summarizes insights like average scores and weak areas.
  - Graph files:
    - `performance_trends.png`
    - `weak_topics_distribution.png`
    - `student_personas.png`

### Steps to Run the Project
1. Clone or download the project repository.
2. Install the required Python libraries.
3. Run the Python script:
   ```bash
   python student_recommendations.py
   ```
4. Outputs will be saved in the project directory:
   - `recommendations.csv`
   - `insights_summary.txt`
   - Graph images as PNG files.

## Approach Description
### Data Handling
- Fetch data from the provided API endpoints.
- Process the historical quiz data to extract response analyses, weak topics, and performance metrics.
- Handle errors gracefully for missing or invalid data.

### Insights Generation
- Calculate average weak areas, scores, and accuracy.
- Identify performance gaps and trends over time.

### Recommendation System
- Use weak topics and trends to generate personalized recommendations.
- Assign personas based on accuracy, score, and improvement metrics.

### Visualization
- Generate insightful graphs for better understanding:
  - Weak topics frequency (bar chart).
  - Performance trends over time (line graphs).
  - Clustering-based personas (scatter plot).

---