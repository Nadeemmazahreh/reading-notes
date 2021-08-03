## What is list comprehensions? 
    List comprehensions provide a concise way to create lists. It consists of brackets containing an expression followed by a for clause, then zero or more for or if clauses. 

## Differnece between a normal for loop a list comprehension for loop 

    new_list = []
    for i in old_list:
        if filter(i):
            new_list.append(expressions(i))
    

    new_list = [expression(i) for i in old_list if filter(i)]




