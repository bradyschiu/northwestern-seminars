Overview
This tool helps Northwestern University students find the best writing seminars based on historical CTEC (Course and Teacher Evaluation Council) data. First-year Weinberg students are required to take two seminars, and choosing the right one can significantly impact their educational experience.
Live Demo: https://poweringimaginations.github.io/northwestern-seminars/

Features:
Comprehensive Rankings: Sort seminars by course rating, instruction quality, hours required, and more
Search Functionality: Find courses by instructor name or course title
Wishlist System: Save interesting seminars to revisit later
Data Visualizations: See the relationship between workload and course ratings
Sentiment Analysis: Review sentiment scores based on student feedback
Seminar Filter: Easily distinguish between courses that were previously taught as seminars

The Problem We're Solving
Northwestern students face several challenges when selecting seminars:
The CTEC interface makes it difficult to compare multiple seminars
Some seminars lack CTECs because they're new or have new instructors
Manually reading through dozens of reviews for 30+ seminars is time-consuming
It's hard to objectively compare factors across all available seminars

This tool saves students hours of research by aggregating CTEC data and presenting it in an easy-to-use interface.

Methodology
We collected data from Northwestern's CTEC system with the following approach:
For each planned seminar, we identified the professor's previously taught courses
We prioritized courses that were:
Previous writing seminars
College seminars
Recently taught (within 5 years)
We extracted quantitative metrics and student reviews
For sentiment analysis, we applied RoBERTa models from Hugging Face to student comments

Data Processing
The included Python script (process_ctecs.py) processes raw CTEC data:

Extracts relevant metrics from each course
Performs sentiment analysis on student reviews
Generates a clean CSV for use in the web application

How to Use
Visit the Northwestern Writing Seminar Analysis Tool
Use the dropdown to sort by your preferred metric (course rating, hours required, etc.)
Use the search box to find specific instructors or course topics
Click the heart icon to add seminars to your wishlist
Visit the "Visualizations" tab to see data comparisons
Check your wishlist tab to review saved seminars
