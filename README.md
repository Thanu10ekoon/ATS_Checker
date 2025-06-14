# ATS Resume Checker (CLI)

A command-line tool to analyze and summarize PDF resumes for ATS (Applicant Tracking System) compatibility. It extracts key information, scores ATS-friendliness, and highlights common mistakes.

## Features
- **Extracts text** from PDF resumes
- **Summarizes candidate details**: Name, profession, and skills
- **Scores ATS-friendliness** (0-100)
- **Detects common issues** (e.g., missing contact info, tables, images)
- **Rich CLI output** with color and tables

## Requirements
Download Python
- Python 3.8+ (download python by https://www.python.org/downloads/)


Install PIP
```bash
python -m pip install --upgrade pip
```

Download
```bash
pip install git
git clone https://github.com/Thanu10ekoon/ATS_Checker.git
```

Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage
1. Place your PDF resume in the same directory as `ats_checker.py`.
2. Run the script:
   ```bash
   python ats_checker.py
   ```
3. Enter the filename when prompted (e.g., `my_resume.pdf`).
4. View the summary, ATS score, and detected issues in your terminal.

## Example Output
```
===== CV SUMMARY =====
┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃ Field      ┃ Value                                ┃
┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
┃ Name       ┃ John Doe                             ┃
┃ Profession ┃ Software Engineer                   ┃
┃ Skills     ┃ Python, Java, SQL                   ┃
└────────────┴──────────────────────────────────────┘

ATS Friendly: Yes (Score: 90/100)

Mistakes / Issues Detected:
- No phone number found
- Uses special bullet characters
```

## Notes
- Only PDF files are supported.
- The tool uses heuristics for name/profession detection and may not be 100% accurate.
- For best results, use a simple, text-based resume format.

## Dependencies
- [PyPDF2](https://pypi.org/project/PyPDF2/)
- [nltk](https://pypi.org/project/nltk/)
- [rich](https://pypi.org/project/rich/)

## License
MIT 
