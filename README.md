# Exno.7-Prompt-Engineering
# Date:19-09-2025
# Register no.212223080041

Aim:
To develop a prompt-based application tailored to personal needs, fostering creativity and practical problem-solving skills while leveraging the capabilities of large language models.

Algorithm:
Identify a personal requirement (e.g., daily task organization).

Design simple prompts to collect basic information from the user.

Gradually refine prompts to include:

Prioritization of tasks
Time allocation suggestions
Reminders and motivational notes
Implement the prompt-based application using ChatGPT.

Display outputs showing progression from basic to advanced prompt designs.

Evaluate usability and insights provided by the application.

Python Code:
# Daily Task Organizer using ChatGPT

import openai

# Set API Key
openai.api_key = "your_openai_api_key"

# Function to query ChatGPT
def ask_chatgpt(prompt):
    try:
        response = openai.ChatCompletion.create(
            model="gpt-4",
            messages=[{"role": "user", "content": prompt}]
        )
        return response.choices[0].message.content
    except Exception as e:
        return f"Error: {e}"

# Step 1: Basic Prompt - Simple Task List
prompt1 = "List 5 tasks I should complete today for productivity."
print("=== Basic Prompt ===")
print(ask_chatgpt(prompt1), "\n")

# Step 2: Intermediate Prompt - With Priorities
prompt2 = "Organize my daily tasks into High, Medium, and Low priority categories."
print("=== Intermediate Prompt ===")
print(ask_chatgpt(prompt2), "\n")

# Step 3: Advanced Prompt - With Time Allocation and Motivation
prompt3 = ("Create a structured daily plan for my tasks with estimated time allocations, "
           "short breaks, and a motivational quote at the end.")
print("=== Advanced Prompt ===")
print(ask_chatgpt(prompt3))
Sample Output:
=== Basic Prompt ===
1. Check and reply to important emails  
2. Complete the project report draft  
3. Study one chapter of AI textbook  
4. Exercise for 30 minutes  
5. Plan tomorrow’s agenda  

=== Intermediate Prompt ===
High Priority:  
- Finish project report  
- Study AI textbook  

Medium Priority:  
- Reply to emails  
- Plan tomorrow’s agenda  

Low Priority:  
- Exercise  

=== Advanced Prompt ===
9:00–10:30 AM → Work on project report  
10:30–11:00 AM → Short break  
11:00–12:30 PM → Study AI textbook  
12:30–1:00 PM → Lunch  
1:00–2:00 PM → Reply to emails  
5:30–6:00 PM → Exercise  

"Stay consistent. Small daily progress leads to big results!"  
Result:
The prompt-based application for organizing daily tasks is developed successfully, demonstrating progression from simple to advanced prompts and showcasing the practical use of LLMs.


# Algorithm: Develop a prompt-based application using ChatGPT - To demonstrate how to create a prompt-based application to organize daily tasks, showing the progression from simple to more advanced prompt designs and their corresponding outputs.




# Result: The Prompt is executed successfully


