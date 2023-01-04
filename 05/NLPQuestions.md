**Why is the matrix in Figure 1.1 called binary incident matrix?**
Because the only values are 0 and 1. 1 = contain, 0 = does not contain

**What is the difference between "word" and "term"?**
All terms are words, but not all words are terms. Words have a universal meaning to the speaker of that particular language. A term does not have a universal meaning. It has a special meaning in a specific situation.

**What concept does the term "corpus" denote?**
Body of texts

**Which terms are used as synonym for "vocabulary"?**
Set of terms

**What are the differences between "token", "type" and "term"?**
Token:
A token is an instanceTOKEN of a sequence of characters in some particular document that are grouped together as a useful semantic unit for processing.
Type:
A type is the class of allTYPE tokens containing the same character sequence.
Term:
A term is a type that is included in the IR system’s dictionary.

**Find out what the standard encoding is in Python.**
ASCII

**Which preprocessing step described in section 2.2 do you think is mandatory for most applications?**
tokenization and case folding

**Find examples (that were not listed in the book) in your native language where tokenization is not straightforward, i.e. simply splitting at non-alphanumeric characters might not be enough.**
compound words like: Freundeskreis, Wohnugnsbesichtigung
words with inflections: lesen (to read), ließ (read), gelesen(read)

**Which preprocessing steps decrease the size of the vocabulary?**
stemming and stop word removal

**Is stemming or lemmatization more resource-intense?**
lemmatization because it requires more complex processing of the text

**In your native language, find another example where normalization might be useful.**
Hühner, Huehner 
Strasse, Straße

**What is the bag-of-words representation of a document?**
Detecting similar bag of words by the number of occurrences of each term. 

**What is the problem with raw term frequency?**
high frequency words get a high weight --> raw frequncy words get a lower weight

**Why is document frequency preferred to collection (or corpus) frequency?**
This is because in trying to discriminate between documents for the purpose of scoring it is better to use a document-level statistic (such as the number of documents containing a term) than to use a collection-wide statistic for the term.

**What is the inverted document frequency ( idf ) of a term that occurs in every document?**
idf = log(N/df)
Thus the idf of a rare term is high, whereas the idf of a frequent term is likely to be low.

**Can the tf-idf weight of a term in a document exceed 1?**
yes it can exceed 1

**Make sure to be able to follow the computations in Example 6.2 and Example 6.3.**
