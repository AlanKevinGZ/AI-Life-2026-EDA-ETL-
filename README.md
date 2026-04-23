# 🤖 How AI is Changing Life | AI and Student Life 2026

> A clean, synthetic dataset tracking how students use AI for grades, productivity, and career readiness.

---

## 📌 About the Dataset

This dataset explores the intersection of **Artificial Intelligence and higher education in 2026**. As AI tools become standard in every classroom, this synthetic data was created to help fellow students and researchers analyze the real-world impact of LLMs on **academic performance** and **mental well-being**.

📥 Source: [Kaggle — AI and Student Life 2026](https://www.kaggle.com/)

---

## 📊 Key Features

| Feature | Description |
|---|---|
| 🎓 Academic Metrics | Baseline GPA vs. Post-AI GPA |
| 🤖 Student Behavior | Primary AI tools used (Claude, ChatGPT, Copilot) and daily usage frequency |
| 💡 Trendy Insights | Ethics concerns and AI Career Readiness scores |

---



## 🔍 Potential Use Cases

- 📈 **Predict** a student's career confidence based on their AI usage patterns
- 🏫 **Analyze** which majors are adopting AI tools the fastest
- 📉 **Build a regression model** to measure the impact of AI on GPA
- 🧠 **Explore** ethical concerns and their relationship to academic performance

---

## 🧪 Key Findings (EDA)

- Average GPA **increased ~8.77%** after AI adoption (`GPA_Baseline` → `GPA_Post_AI`)
- All majors showed a **positive GPA change**, though the magnitude varied
- Top AI tools in use: **Claude**, **ChatGPT**, **Copilot**

---

## 🛠️ Requirements

```bash
pip install pandas matplotlib seaborn scikit-learn
```

---

## 🚀 Quick Start

```python
import pandas as pd

df = pd.read_csv("ai_student_life_2026.csv")

# Rename columns to Spanish
df.rename(columns={
    'Student_ID': 'ID_Estudiante',
    'Age': 'Edad',
    'Major': 'Carrera',
    'Primary_AI_Tool': 'Herramienta_IA_Principal',
    'Task_Frequency_Daily': 'Frecuencia_Tareas_Diaria',
    'Main_Usage_Case': 'Caso_Uso_Principal',
    'GPA_Baseline': 'Promedio_Base',
    'GPA_Post_AI': 'Promedio_Post_IA',
    'Time_Saved_Hours_Weekly': 'Horas_Ahorradas_Semanal',
    'AI_Ethics_Concern': 'Preocupación_Ética_IA',
    'Career_Confidence_Score': 'Puntuación_Confianza_Laboral'
}, inplace=True)

# GPA impact
print(df[['Promedio_Base', 'Promedio_Post_IA']].mean())
```

---

## 📁 File Structure

```
📦 ai-student-life-2026
 ┣ 📜 README.md
 ┣ 📊 ai_student_life_2026.csv
 ┗ 📓 analysis.ipynb
```

---

## 📄 License

This is a **synthetic dataset** created for educational and research purposes.
