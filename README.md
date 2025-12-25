Resume Optimizer & Formatter

This project is designed to take an existing resume (PDF or DOCX) and automatically transform it into a clean, ATS-friendly, single-page professional resume. Most resumes — especially student resumes — have problems like:
i) inconsistent formatting
ii) random placement of sections
iii) long paragraphs instead of bullet points
iv) missing summary or structured skills
v) badly extracted text when converted manually

This project solves those problems automatically using Python.

What the System Does

1️.Extract Resume Content
The system first reads the resume file
If it is PDF, it extracts text using pdfplumber
If it is DOCX, it converts it to Markdown using mammoth
Then it stores everything in a temporary Markdown text file, making it easier to edit.

2️.Clean & Optimize Resume Content
The program rewrites bullet points into more impactful sentences
ensures every bullet looks professional
adds default profile summary when missing
detects possible name, email, phone, and gender
organizes content into logical sections
It mimics what top-performing resumes usually follow.

3️.Auto-Generate Resume Layout
The project converts structured content into a clean HTML layout with CSS styling:
left column → contact + personal info + skills
right column → main resume content
Then, using WeasyPrint, it exports this HTML into a final PDF resume.

The final resume is:
neat
professional
ATS-friendly
single-page

Objective of the Project is to automatically convert unformatted resumes into a clean, structured, professionally styled resume PDF using Python.This reduces manual formatting and helps students/freshers quickly generate high-quality resumes.

Where This Project Can Be Used:
university placement cells
resume builders
job portal integrations
student project submissions
ATS compatibility improvement tools

Technologies Used
Python
pdfplumber → extract text from PDFs
mammoth → convert DOCX to text
regex → extract info (email, phone, headings)
HTML + CSS → resume layout
weasyprint → convert HTML → PDF

Final Output
The output is:
optimized Markdown resume
structured HTML resume
final polished PDF resume
