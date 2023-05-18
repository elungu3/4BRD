def count_letters_and_return_descending(x: str) -> str:
    '''
    :param x: a string
    :return: a string containing each element and the frequency of it from the string given as a parameter
    in descending order
    '''
    dict_hash = {}
    count_letters = ""
    for i in x:
        if i in dict_hash:
            dict_hash[i] += 1
        else:
            dict_hash[i] = 1
    lista_sort = sorted([f"{k}{v}" for k, v in dict_hash.items()], key=lambda x: x[1], reverse=True)
    for j in lista_sort:
        count_letters += j
    return count_letters


# print(count_letters_and_return_descending("testinnput"))


def reverse_words_with_len_bigger_than_5(y: str) -> str:
    '''
    :param y: a string that contains only letters and spaces (if contains multiple words)
    :return: the string given as parameter with the words of the string with len > or = 5 backwards
    '''
    if all(x.isalpha() or x.isspace() for x in y):
        y = y.split(" ")
        for i in y:
            if len(i) >= 5:
                y[y.index(i)] = i[::-1]
        return " ".join(y)
    else:
        raise Exception("Y parameter will consist of only letters and spaces")


# print(reverse_words_with_len_bigger_than_5("This is another test"))
