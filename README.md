Steps to reproduce bug:
1. Create a label, for example "old"
2. Assign that label to a PR
3. Search for PRs that do not contain that label, for example, "is:merged -label:old".  The PR should not show up.
4. Rename the label, for example "old"->"new".
5. Search for PRs that do not contain the renamed label, for example, "is:merged -label:new". 

Expected:
The PR should not show up because it has the new label.

Actual:
The PR shows up in the search.  
