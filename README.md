**Debugging with Cursor**

In this practice, you'll identify bugs in a Python file and use Cursor to debug it. 

1. Download the files from this repo.
2. Install the required packages: `pip install -r requirements.txt`.
3. Open Cursor. 
4. Try running the broken code: `python brokencode/sales_analyzer.py`.
5. Choose one error message from the output. Copy the entire error and paste it into the Cursor chat with this prompt:
    
    <aside>
    
    I'm getting this error with my Python code: 
    
    `<paste the error type, e.g. filenotfound error>`
    
    The code is trying to process sales data from a CSV file. Here's the problematic code:
    
    `< paste the relevant lines here and tag the file for context: @sale_analyzer.py >` 
    
    Please identify the issue and suggest a fix.
    
    </aside>
    
6. If you like the suggestion, use Cursor's Agent Mode to apply the fix directly.
7. Use this prompt to fix the rest of the bugs: 
    
    <aside>
    
    `<filename>` is throwing errors when I run it. The input file is `<another filename>` with columns: `date`, `product`, `region`, `sales_amount`, `quantity`. Please review and fix the issues.
    
    </aside>
    
8. Upload your debugged code to the platform for validation.

HINT

Try using the debugging prompt pattern:


**Problem + expected vs actual + context files**

**Example prompt**
Problem: My file organiser crashes with "KeyError" when processing files.

**Expected:** Should handle unknown file types gracefully.
**Actual**: Program crashes and stops processing.

**Context files:**
- file_organizer.py (main logic)
- test_files/ (sample files that cause crashes)

**Error message:**
KeyError: '.xyz' in get_file_category() function


You may also ask Cursor to find bugs for you using Ask mode, then switch to Agent Mode to implement solutions.
