java c
Faculty of Arts  Science 
Fall 2024 Quiz 5 - V2 
CSC 110 Y1F
Question 1. Tabular Data [6   marks]
Consider   the   following   sample   list   representing   student   scores.   Each   row   contains   a   student   ID,   their   name,   and   their   scores   on   three   quizzes.
student_scores =   [
[1099752,   '   Alice   ' , 85,   90, 88],
[1087711,   '   Bob   ' , 78,   85,   92],
[1000023,   '   Priya   ' , 90,   92,   87],
[100048,   '   Muchen   ' , 82, 88,   85],
[109943,   '   Chirly   ' , 88,   84,   90]
]
Part (a) [3   marks]
What   would   the   following   pieces   of   code   evaluate   to?   Write   your   answers   in   each   blank   space   provided.
>>> len(student_scores[0])
>>> student_scores[3][1]
>>> max([row[0] for   row   in   student_scores])
Part (b) [3   marks]
Complete   the   function   below,   based   on   the   provided   speciﬁcation.
def student_quiz1_meets_threshold(data: list[list], student_id: int, goal_score:   int)   -> bool:
"""Return whether the student with student_id   scored at   least   goal_score   on   quiz   1   .
If the student_id does not   exist   in   data,   return   False   .
Preconditions:
- goal_score   >   0
- data is a valid   list of   student   scores,   structured   the   way   we   described   above
- quiz 1   scores   appear   at   index   2   in   each   student   data   sublist
>>> student_quiz1_meets_threshold(student_scores, 1099752, 80)   True
>>> student_quiz1_meets_threshold(student_scores, 1087711, 90)   False
>>> student_quiz1_meets_threshold(student_scores, 1,   90)
False
"""
Question 2. Python Dataclasses [3   marks]
We   want   to   represent   each   student’s   data   using   data   classes   instead.   Complete   the   StudentData   class   below.   Each   StudentData   instance   should   have   the   following   attributes   for   a   student:    id,   name   and   list   of   integer quiz_scores.   When   declaring   the   data   type   of   each   attribute,   make   it 代 写CSC 110 Y1F Fall 2024 Quiz 5 - V2Python
代做程序编程语言  as   speciﬁc   as   possible.   You   should   also   include   the   following   representation   invariants: 
•   There   are   a   total   of three   scores   in   the   quiz_scores   list
•   All   scores   in   the   quiz_scores   list   are   greater   than   or   equal   to   0   from dataclasses import   dataclass
@dataclass
class StudentData:
"""Data about a   student   '   s performance   on three   quizzes   .
Representation Invariants:
# TODO: Write the two representation invariants below, as   Python   expressions
Instance Attributes:
# TODO: Write each instance attribute   '   s   variable   name   and   description   below
"""
# TODO: Write each instance attribute   '   s variable   name   and   specific   data   type   below
Question 3. Debugging / For Loops [3   marks]The   function   below   is   an   incorrect   attempt   to   return   True   if a   string   s   is   made   up   of only   uppercase   vowels   (that   is,   a A, E,   I,   O   or a U).   Your   friend   Bob   believes   the   function   is   correct   because   he   tried   calling   the   function   with   some   string   arguments   which   the   code   did   work   correctly   for.   Answer   the   questions   below.
def   all_upper_vowel(s: str)   ->   bool:
"""Return True if and   only   if   s   consists   of   all uppercase   vowels   ."""
for   char   in   s:
if   char   in   '   AEIOU   ' :
return True
return False
Part (a) [1   mark]
Give   an   example   of   a   valid   argument   for   all_upper_vowels   where   this   function   will   return   the   correct   expected value   (according   to   the   docstring):
Part (b) [1   mark]
Give   an   example   of a   valid   argument   for   all_upper_vowels   where   this   function   will   NOT   return   the   correct   expected   value:
Part (c) [1   mark]
Brieﬂy   explain   (in   1–2   sentences)   why   this   function   is   incorrect   (identify   the   issue   in   the   code):



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
