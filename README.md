# Algorithms-and-its-elements
ALGORITHM Sentence Analysis

VAR
    sentence: string
    length , word_count , vowel_count  : integer
    current_char: char

BEGIN

WRITE ('write your sentence')
Read (sentence)
length := 0
word_count := 1
vowel_count := 0
FOR i := 1 to length(sentence) DO
    current_char := sentence[i]
    length := length + 1
    
    IF current_char = ' ' THEN
        word_count := word_count + 1
    ELSE IF current_char IN ['a','e','i','o','u','A','E','I','O','U'] THEN
        vowel_count := vowel_count + 1
    END IF
    
END FOR

word_count := word_count - 1 

WRITE ("Length of sentence: ", length)
WRITE ("Number of words: ", word_count)
WRITE ("Number of vowels: ", vowel_count)

END
