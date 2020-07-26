the_list = ["디자인등록출원을 하려는 자는","제40조제1항에도","불구하고"
            ,"디자인을","1디자인등록출원(이하'복수디자인등록출원'이라 한다)으로 할 수 있다."
            ,"이 경우","디자인마다 분리하여","표현하여야","한다."]
key_word = "디자인"
sentence = "1디자인디자등록인출원(이하'복수디자인등록출원'이라 한다자자자자)으로인인인 할 수 있다.디자인마다 디디 분리한다"

def searching_TextInList(key_word):
    N = 0
    for word in the_list:
        while key_word in word:
            N += 1
            word = word.strip(key_word)
            
    return N

def searching_TextInText(sentence,key_word):
    key_word_list = list(key_word)
    sentence_list = list(sentence)
    print(key_word_list,sentence_list)
    for i in range(len(key_word_list)):
        key_word_index = []
        for j in range(len(sentence_list)):
            if sentence_list[j] == key_word_list[i]:
                key_word_index.append(j)
        key_word_list[i] = key_word_index
    count = 0 
    for i in range(len(key_word_list[0])):
        for j in range(len(key_word_list)):
            Check = True
            the_number = key_word_list[0][i]+j
            if not the_number in key_word_list[j]:
                Check = False
        if Check :
            count += 1
    return count

answer = searching_TextInText(sentence,key_word)
print(answer)
