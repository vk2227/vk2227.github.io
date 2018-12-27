## Question

The nested for loop below processes a set of lists and combines the elements into a single list. How to do the same thing in a single line using list comprehension?

def single_list(X):
    output = []
    for x in X:
        for a in x:
            output.append(a)
    return output

X = [["1", "2"], ["a", "b"], ["3", "4", "p", "a"]]

print(single_list(L))
