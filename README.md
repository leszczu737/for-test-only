def anagram():
    res = []
    dictio_words = dict()
    with open(r'anagram.txt') as fin:
        words = fin.read()
    listed_words = words.split(',')
    for word in listed_words:
        # change word from file to list (for sorting)
        rea_word = word.strip().lower()
        # print (rea_word)
        res.append(rea_word)
        res.sort()
        dictio_words[rea_word] = dictio_words.setdefault(rea_word, len(rea_word))
        value = dictio_words[rea_word]
        for i in dictio_words:
            i
    # for rea_word in dictio_words:

    # for value in 

anagram()
