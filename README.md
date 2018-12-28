## Question 1

The *single_list* function below with the nested for loop processes a list of lists and flattens the elements into a single list. How to do the same thing in a single line using list comprehension?

#### Code
    def single_list(X):
        output = []
        for x in X:
            for a in x:
                output.append(a)
        return output

    X = [["1", "2"], ["a", "b"], ["3", "4", "p", "q"]]
    print(single_list(X))

#### Output
    ['1', '2', 'a', 'b', '3', '4', 'p', 'q']

## Answer 1

#### Code
    X = [["1", "2"], ["a", "b"], ["3", "4", "p", "q"]]
    list = [item for sublist in X for item in sublist]
    print(list)

#### Output
    ['1', '2', 'a', 'b', '3', '4', 'p', 'q']

--------------------------------------------------------------
## Question 2

Given 3 lists, make a new list consisting of the maximum values at each index for the 3 lists.

## Answer 2

#### Code
    A1 = [10, 11, 12, 13]
    A2 = [20, 15, 10, 5]
    A3 = [0, 10, 20, 30]
    maxs = [max(a) for a in zip(A1,A2,A3)]
    print(maxs)

#### Output
    [20, 15, 20, 30]

--------------------------------------------------------------
    
