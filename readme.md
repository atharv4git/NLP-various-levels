# What is Natural Language Processing ?
There’s something exceptional about humans.

We’re capable of doing unbelievably complex tasks. Even more amazing is that most of the things easiest for us are incredibly difficult for machines to learn.

The day to day activities that we do like talking or writing are in form of natural language.

We created coding programs to help us communicate on the same level as a computer. But can you imagine a world where humans talked to each other in the equivalent of code? It would be very dry…

A programmer is going to the grocery store and his wife tells him, “Buy a gallon of milk, and if there are eggs, buy a dozen.”

So the programmer goes, buys everything, and drives back to his house.

Upon arrival, his wife angrily asks him, “Why did you get 13 gallons of milk?” The programmer says, “There were eggs!”

Fortunately for us, there’s little chance that we’ll adopt Python as a spoken language. We can keep the beauty and complexity of the languages we speak and write, with their vast vocabulary, double-meanings, sarcasm, slang, abbreviations, and idiosyncrasies!

Natural language simply refers to the way we communicate with each other: speech and text.

Processing refers to making natural language usable for computational tasks.

Natural language processing, also referred to as text analytics, plays a very vital role in today’s era because of the sheer volume of text data that users generate around the world on digital channels such as social media apps, e-commerce websites, blog posts, etc. Natural Language Processing works on multiple levels and most often, these different areas synergize well with each other. This article will offer a brief overview of each and provide some example of how they are used in information retrieval.

# Morphological
Morphology has been a part of mainstream linguistics for sixty years or more.The morphological level of linguistic processing deals with the study of word structures and word formation, focusing on the analysis of the individual components of words. According to the classical approach in linguistics , words are formed of morphemes, which are the minimal (that is, non-decomposable) linguistics units that carry meaning

Many language processing applications need to extract the information encoded in the words – Parsers which analyze sentence structure need to know/check agreement between

# subjects and verbs
Adjectives and nouns
Information retrieval systems benefit from know what the stem of a word is and  machine translation systems analyze words to their components and generate words with specific features in the target language

Taking, for example, the word: “undesirableness”. It can be broken down into three morphemes (prefix, stem, and suffix), with each conveying some form of meaning: the prefix un- refers to “not being”, while the suffix -ness refers to “a state of being”. The stem desirable is considered as a free morpheme since it is a “word” in its own right. Bound morphemes (prefixes and suffixes) require a free morpheme to which it can be attached to, and can therefore not appear as a “word” on their own.

In Information Retrieval, document and query terms can be stemmed to match the morphological variants of terms between the documents and query; such that the singular form of a noun in a query will match even with its plural form in the document, and vice versa, thereby increasing recall.

# Lexical
It involves identifying and analyzing the structure of words and parts of speech. Lexicon of a language means the collection of words and phrases in a language. Lexical analysis is dividing the whole chunk of text into paragraphs, sentences, and words.This level of linguistic processing utilizes a language’s lexicon, which is a collection of individual lexemes. A lexeme is a basic unit of lexical meaning; which is an abstract unit of morphological analysis that represents the set of forms or “senses” taken by a single morpheme.

“Better”, for example, can take the form of a noun or a verb or a adjective but its part-of-speech and lexical meaning can only be derived in context with other words used in the phrase/sentence. This, in fact, is an early step towards a more sophisticated Information Retrieval system where precision is improved through part-of-speech tagging.

For a simple application like spam detection, lexical processing works just fine, but it is usually not enough in more complex applications, like, say, machine translation. For example, the sentences “My cat ate its third meal” and “My third cat ate its meal”, have very different meanings. However, lexical processing will treat the two sentences as equal, as the “group of words” in both sentences is the same. Hence, we clearly need a more advanced system of analysis.

# Syntactic
The next step after lexical analysis is where we try to extract more meaning from the sentence, by using its syntax this time. Instead of only looking at the words, we look at the syntactic structures, i.e., the grammar of the language to understand what the meaning is.

In Information Retrieval, parsing can be leveraged to improve indexing since phrases can be used as representations of documents which provide better information than just single-word indices. In the same way, phrases that are syntactically derived from the query offers better search keys to match with documents that are similarly parsed.

One example is differentiating between the subject and the object of the sentence, i.e., identifying who is performing the action and who is the person affected by it. For example, “Chris thanked Brett” and “Brett thanked Chris” are sentences with different meanings from each other because in the first instance, the action of ‘thanking’ is done by Chris and affects Brett, whereas, in the other one, it is done by Brett and affects Chris. Hence, a syntactic analysis that is based on a sentence’s subjects and objects, will be able to make this distinction.

There are various other ways in which these syntactic analyses can help us enhance our understanding. For example, a question answering system that is asked the question “Who is the Prime Minister of USA?”, will perform much better, if it can understand that the words “Prime Minister” are related to “USA”. It can then look up in its database, and provide the answer.

# Semantic
Lexical and syntactic processing don’t suffice when it comes to building advanced NLP applications such as language translation, chatbots etc.. The machine, after the two steps given above, will still be incapable of actually understanding the meaning of the text.

The semantic level of linguistic processing deals with the determination of what a sentence really means by relating syntactic features and disambiguating words with multiple definitions to the given context. This level entails the appropriate interpretation of the meaning of sentences, rather than the analysis at the level of individual words or phrases.

In Information Retrieval, the query and document matching process can be performed on a conceptual level, as opposed to simple terms, thereby further increasing system precision. Moreover, by applying semantic analysis to the query, term expansion would be possible with the use of lexical sources, offering improved retrieval of the relevant documents even if exact terms are not used in the query. Precision may increase with query expansion, as with recall probably increasing as well.

Such an incapability can be a problem for, say, a question answering system, as it may be unable to understand that PM and Prime Minister mean the same thing. Hence, when somebody asks it the question, “Who is the PM of USA?”, it may not even be able to give an answer unless it has a separate database for PMs, as it won’t understand that the words PM and Prime Minister are the same. You could store the answer separately for both the variants of the meaning (PM and Prime Minister), but how many of these meanings are you going to store manually? At some point, your machine should be able to identify synonyms, antonyms, etc. on its own.This is typically done by inferring the word’s meaning to the collection of words that usually occur around it. So, if the words, PM and Prime Minister occur very frequently around similar words, then you can assume that the meanings of the two words are similar as well.

Once you have the meaning of the words, obtained via semantic analysis, you can use it for a variety of applications. Machine translation, chatbots and many other applications require a complete understanding of the text, right from the lexical level to the understanding of syntax to that of meaning. Hence, in most of these applications, lexical and semantic processing simply form the “pre-processing” layer of the overall process. In some simpler applications, only lexical processing is also enough as the pre-processing part.

Some other Natural Language Processing (NLP) methods concerned with semantics include:

Using numbers to represent the meanings of words/sentences in text and how they relate to one another
Translating text from one language to another
Creating human readable text from structured data (rows and columns)
Determining the text in a given image (go from screenshot to Word document)
Forming answers to questions about a given set of data
Deciding on the positive or negative sentiment of a given text
Separating text into self-contained topics
Deciding on the meaning of an ambiguous word given the context (Roll over? Eat a sushi roll?)
Given an example like above, where we find proper nouns, figuring out the relationships between these (Melissa is Victor’s wife)
Semantics is a flourishing field — needless to say there is a lot of progress being made in helping our computers find meaning in text, and in turn helping us perform much more powerful analytics.
Discourse
Discourse processing is a suite of Natural Language Processing (NLP) tasks to uncover linguistic structures from texts at several levels, which can support many NLP applications.It deals with the analysis of structure and meaning of text beyond a single sentence, making connections between words and sentences. At this level, Anaphora Resolution is also achieved by identifying the entity referenced by an anaphor (most commonly in the form of, but not limited to, a pronoun). An example is shown below.

“I love dominoes pizza because they put extra cheese” , she said.

Here there are two entities she and dominoes, where she is in context of “I” and they is in context of “dominoes” so discourse will interpret this sentence has 2 entities ( I and dominoes ) and 2 anaphor ( she and they)

Much of discourse is used when trying to train chatbots to interact well with humans and be easily understandable. If you tell a chatbot on a cosmetics website that you’re looking for a good moisturizer, it’s unhelpful for the bot to ask what your favorite book is.

With the capability to recognize and resolve anaphora relationships, document and query representations are improved, since, at the lexical level, the implicit presence of concepts is accounted for throughout the document as well as in the query, while at the semantic and discourse levels, an integrated content representation of the documents and queries are generated.

Further methods of Natural Language Processing (NLP) that concern themselves with discourse include:

Which mentions are referring to which entities? (“they” refers to “Dominoes”)
Categorizing the type of text (Is it a question, statement, assertion?)
Grade the quality and coherence of text (automatic essay scoring)
# Pragmatic
Pragmatic means practical or logical. If someone calls you pragmatic, they mean that you tend to think in terms of the practical or logical rather than the ideal situation.

The pragmatic level of linguistic processing deals with the use of real-world knowledge and understanding of how this impacts the meaning of what is being communicated. By analyzing the contextual dimension of the documents and queries, a more detailed representation is derived.

Examples of Pragmatics:

Will you crack open the door? I am getting hot.
Semantically, the word “crack” would mean to break, but pragmatically we know that the speaker means to open the door just a little to let in some air.

I heart you!
Semantically, “heart” refers to an organ in our body that pumps blood and keeps us alive. However, pragmatically, “heart” in this sentence means “love”-hearts are commonly used as a symbol for love, and to “heart” someone has come to mean that you love someone.

If you eat all of that food, it will make you bigger!
Semantically, “bigger” in this sentence would mean larger than you are currently. Think about how this sentence, pragmatically, would mean something different depending on the context. If it is said to a young child, pragmatically, it would mean to grow bigger. If it is said to a grown person who is already obese, it would mean something entirely different.

In Information Retrieval, this level of Natural Language Processing primarily engages query processing and understanding by integrating the user’s history and goals as well as the context upon which the query is being made. Contexts may include time and location.

This level of analysis enables major breakthroughs in Information Retrieval as it facilitates the conversation between the IR system and the users, allowing the elicitation of the purpose upon which the information being sought is planned to be used, thereby ensuring that the information retrieval system is fit for purpose.
