# 💻 Developer Portfolio Gateway

**Author:** Gabriel Dilley
**Course:** CIS352 – Intro to Enterprise Computing

---

## 👋 About Me

Welcome to my GitHub portfolio repository!
I am currently studying Computer Information Systems at Wayne State College.
This repository serves as a central directory for navigating my coursework and projects.

---

## 👤 Profile

### Gabriel Dilley

<img src="assets/headshot_1000.jpg" alt="Gabriel Dilley" width="200" style="border-radius: 8px;"/>

[GitHub](https://github.com/gawdilley) • [Email](mailto:gadill01@wsc.edu)

---

## 📚 Table of Contents

| Project | Tech | Category | Description | Repo |
| --- | --- | --- | --- | --- |
| [CALC2000](#calc2000) | COBOL / JCL | CIS352 Intro to Enterprise Computing | Calculates future investment values using compound growth and repeated doubling logic | [COBOL-Chapter-1-Assignment](https://github.com/gawdilley/COBOL-Chapter-1-Assignment) |
| [UTIL2000](#util2000) | COBOL / JCL | CIS352 Intro to Enterprise Computing | Tiered electric utility billing program that calculates customer bills based on kWh usage | [COBOL-Chapter-2-Assignment](https://github.com/gawdilley/COBOL-Chapter-2-Assignment) |
| [RPT2000](#rpt2000) | COBOL / JCL | CIS352 Intro to Enterprise Computing | YTD sales report with year-over-year comparison, percent change, and grand totals | [COBOL-Chapter-3-Assignment](https://github.com/gawdilley/COBOL-Chapter-3-Assignment) |
| [RPT3000](#rpt3000) | COBOL / JCL | CIS352 Intro to Enterprise Computing | Multi-page YTD sales report with branch-level control breaks and automatic pagination | [COBOL-Chapter-4-Assignment](https://github.com/gawdilley/COBOL-Chapter-4-Assignment) |
| [RPT5000](#rpt5000) | COBOL / JCL | CIS352 Intro to Enterprise Computing | Three-level YTD sales report with sales rep and branch control breaks using EVALUATE | [COBOL-Chapter-5-Assignment](https://github.com/gawdilley/COBOL-Chapter-5-Assignment) |
| [RPT6000](#rpt6000) | COBOL / JCL | CIS352 Intro to Enterprise Computing | Table-driven sales report with indexed lookups, copybooks, and PACKED-DECIMAL storage | [COBOL-Chapter-6-Assignment](https://github.com/gawdilley/COBOL-Chapter-6-Assignment) |
| [SEQ3000](#seq3000) | COBOL / JCL | CIS352 Intro to Enterprise Computing | Sequential and indexed employee file maintenance with add, change, and delete transactions | [COBOL-SEQ3000](https://github.com/gawdilley/COBOL-SEQ3000) |

---

## CALC2000

A foundational `COBOL` program that `calculates and displays the future value of an investment` using predefined input values. The investment amount is doubled on each iteration to demonstrate program flow and numeric computation.

**Key Concepts:** COMPUTE statements | Numeric editing | Reusable PERFORM paragraphs | Removing ACCEPT input | Formatted output | Program header documentation

**Tech Stack:**
![COBOL](https://img.shields.io/badge/COBOL-Enterprise-blue)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-000000.svg?style=for-the-badge&logo=GitHub)

### 🚦 Status
✅ Completed

### 📄 Example Output

```
Calculating Future Values

Future Value   =  1,628.89
Investment Amount:   1,000
Number of Years:        10
Yearly Interest Rate:  5.5%

Future Value   =  3,257.79
Investment Amount:   2,000
Number of Years:        10
Yearly Interest Rate:  5.5%

End of session.
```

[CALC2000 Repo](https://github.com/gawdilley/COBOL-Chapter-1-Assignment)

🔙 [Back to TOC](#-table-of-contents)

---

## UTIL2000

A `COBOL` utility billing program that `calculates and displays electric bills` for three predefined customers using a `tiered kilowatt-hour (kWh) rate system` and a fixed service fee.

**Key Concepts:** Tiered rate calculations | Conditional logic | Arithmetic operations | Formatted output | Multi-record processing

**Tech Stack:**
![COBOL](https://img.shields.io/badge/COBOL-Enterprise-blue)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-000000.svg?style=for-the-badge&logo=GitHub)

### 🚦 Status
✅ Completed

### 📄 Example Output

```
********************************
*** UTIL2000 - CUSTOMER BILL ***
********************************

--------------------------------
CUSTOMER: CUST-ALPHA
--------------------------------
KWH USED       :   350
SERVICE FEE    : $14.95
TIER 1 CHARGE  : $42.00
TIER 2 CHARGE  :  $0.00
TIER 3 CHARGE  :  $0.00
--------------------------------
TOTAL BILL     : $56.95
--------------------------------

--------------------------------
CUSTOMER: CUST-BRAVO
--------------------------------
KWH USED       :   925
SERVICE FEE    : $14.95
TIER 1 CHARGE  : $60.00
TIER 2 CHARGE  : $63.75
TIER 3 CHARGE  :  $0.00
--------------------------------
TOTAL BILL     : $138.70
--------------------------------
```

[UTIL2000 Repo](https://github.com/gawdilley/COBOL-Chapter-2-Assignment)

🔙 [Back to TOC](#-table-of-contents)

---

## RPT2000

An intermediate `COBOL` reporting program that reads `customer financial records` from a master file and generates a `formatted Year-To-Date (YTD) Sales Report`. Introduces file I/O, selective record filtering, and year-over-year sales comparison.

**Key Concepts:** Sequential file I/O | COMPUTE / SUBTRACT | Percent change calculations | Division-by-zero protection | Pagination | Grand totals

**Tech Stack:**
![COBOL](https://img.shields.io/badge/COBOL-Enterprise-blue)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-000000.svg?style=for-the-badge&logo=GitHub)

### 🚦 Status
✅ Completed

### 📄 Example Output

```
DATE:  02/19/2026           YEAR-TO-DATE SALES REPORT            PAGE:    1
TIME:  14:35                                                      RPT2001

BRANCH SALES  CUST   CUSTOMER NAME         SALES          SALES        CHANGE    CHANGE
 NUM    REP   NUM                         THIS YTD       LAST YTD      AMOUNT   PERCENT
------  -----  -----  --------------------  ----------  ----------  ----------  ------
 01      10   10001  ACME SUPPLY CO          25,450.75   20,125.50    5,325.25    26.5
 01      12   10015  METRO INDUSTRIAL        18,900.00   19,500.00     -600.00    -3.1
 02      08   20002  SOUTHERN MATERIALS      45,300.25   30,100.00   15,200.25    50.5
                                           ===========  ===========  ===========  ======
                              GRAND TOTAL   89,651.00    69,725.50   19,925.50    28.6
```

[RPT2000 Repo](https://github.com/gawdilley/COBOL-Chapter-3-Assignment)

🔙 [Back to TOC](#-table-of-contents)

---

## RPT3000

A `COBOL` reporting program that processes customer financial records and generates a `multi-page YTD Sales Report` with `branch-level control breaks`, accumulator resets, and automatic pagination. Built collaboratively with Garrett Finke.

**Key Concepts:** Control break processing | Multi-level totals | FUNCTION CURRENT-DATE | Signed numeric fields | ROUNDED option | Report-style output formatting

**Tech Stack:**
![COBOL](https://img.shields.io/badge/COBOL-Enterprise-blue)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-000000.svg?style=for-the-badge&logo=GitHub)

### 🚦 Status
✅ Completed

[RPT3000 Repo](https://github.com/gawdilley/COBOL-Chapter-4-Assignment)

🔙 [Back to TOC](#-table-of-contents)

---

## RPT5000

An advanced `COBOL` reporting system that generates a `three-level YTD Sales Report` with control breaks at the sales rep and branch level. Uses `EVALUATE TRUE` for clean decision logic and introduces level-88 condition names. Built collaboratively with Garrett Finke.

**Key Concepts:** Three-level control break processing | EVALUATE TRUE | 88-level condition names | WITH TEST AFTER | INITIALIZE | SPACE-CONTROL variable line spacing | Field suppression on detail lines

**Tech Stack:**
![COBOL](https://img.shields.io/badge/COBOL-Enterprise-blue)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-000000.svg?style=for-the-badge&logo=GitHub)

### 🚦 Status
✅ Completed

[RPT5000 Repo](https://github.com/gawdilley/COBOL-Chapter-5-Assignment)

🔙 [Back to TOC](#-table-of-contents)

---

## RPT6000

An advanced `COBOL` program that introduces `in-memory table processing` with a sales rep lookup table loaded from a reference file. Uses `SEARCH`, `OCCURS`, `INDEXED BY`, `COPY`, and `PACKED-DECIMAL` storage for a professional-grade sales report.

**Key Concepts:** Table loading from file | OCCURS / INDEXED BY | SEARCH statement | COPY copybooks | INITIALIZE | PACKED-DECIMAL | REDEFINES | ON SIZE ERROR | Floating $ and +++ edit patterns

**Tech Stack:**
![COBOL](https://img.shields.io/badge/COBOL-Enterprise-blue)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-000000.svg?style=for-the-badge&logo=GitHub)

### 🚦 Status
✅ Completed

[RPT6000 Repo](https://github.com/gawdilley/COBOL-Chapter-6-Assignment)

🔙 [Back to TOC](#-table-of-contents)

---

## SEQ3000

A `COBOL` file maintenance project containing three programs that demonstrate `sequential and indexed file maintenance`. Processes employee transaction files to perform adds, changes, and deletes against both sequential and indexed master files, with full error transaction handling.

**Key Concepts:** Sequential file maintenance pattern | HIGH-VALUE sentinel | Indexed file organization | ORGANIZATION IS INDEXED | ACCESS IS RANDOM | I-O open mode | READ INVALID KEY / NOT INVALID KEY | DELETE | REWRITE | FILE STATUS IS | DISPLAY diagnostics

**Tech Stack:**
![COBOL](https://img.shields.io/badge/COBOL-Enterprise-blue)
![JCL](https://img.shields.io/badge/JCL-Mainframe-lightgrey)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-000000.svg?style=for-the-badge&logo=GitHub)

### 🚦 Status
✅ Completed

[SEQ3000 Repo](https://github.com/gawdilley/COBOL-SEQ3000)

🔙 [Back to TOC](#-table-of-contents)

---

*CIS352 – Intro to Enterprise Computing · Wayne State College*
