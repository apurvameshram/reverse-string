# reverse-string
#Program to reverse each word in a document file
def print_words(filename):
    f = open(filename,'r')
    full_list = (f.read()).lower()
    print full_list
    list_content = full_list.split()
    reverse=[]
    for word in list_content:
        word = word[::-1]
        reverse.append(word)
    print " ".join(reverse)
print_words(filename)
