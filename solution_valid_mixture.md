```
# The algorithm is same here but there are few things to keep in mind.

def valid_strings(string):

    s = Stack()
    balanced = True  # Let's assume that is it balanced
    index = 0

    while  index < len (string) and balanced:
        symbol = string[index]
        if symbol in "([{":
            s.push(symbol)
        else:
            if s.isEmpty():
                balanced = False
            else:
                top = s.pop()
                if not matches(top,symbol):
                    balanced=False

        index+=1

    if balanced and s.isEmpty():
        return True
    else:
        return Fale

def matches(open, close):

    opens = "([{"
    closers = ")]}"

    return opens.index(open) == close.index(close)


```
