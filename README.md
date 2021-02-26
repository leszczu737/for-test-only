# test anagram list of words

def anagram():
    with open(r'anagram.txt') as fin:
        words = fin.read()
    words_sort = list(words)
    print (words_sort)

anagram()

