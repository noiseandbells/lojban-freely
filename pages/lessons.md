# The Xextbook
a primer for Xextan, the compact logical language
Version 1.1 by Rachel Isabel Gardener
Last updated 4/21/2024

## Table of Contents ##

- [Lesson 1: Predicates](#lesson-1-predicates)
- [Lesson 2: Arguments](#lesson-2-arguments)
- [Lesson 3: Illocutions](#lesson-3-illocutions)
- [Lesson 4: Adverbs](#lesson-4-adverbs)
- [Lesson 5: Determiners](#lesson-5-determiners)
- [Lesson 6: Prepositions](#lesson-6-prepositions)
- [Lesson 7: Tags](#lesson-7-tags)
- [Lesson 8: Connectives](#lesson-8-connectives)
- [Lesson 9: Scope](#lesson-9-scope)
- [Lesson 10: Serialization](#lesson-10-serialization)
- [Lesson 11: Lambda](#lesson-11-lambda)
- [Lesson 12: Transmogrification](#lesson-12-transmogrification)

## Part 1: Beginner

### Lesson 1: Predicates

Like most logical languages, Xextan is almost entirely devoid of nouns as a distinct part of speech. Rather, most semantic concepts in Xextan are expressed in the form of a verb phrase or function, otherwise known as a [predicate](?page=predicate). In order to be used as a noun, a predicate must first be converted into an [argument](?page=argument).

This can be achieved in various ways, but the simplest is by placing a [case marker](?page=case-marker) immediately before the predicate in question:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***o len***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*a human*

When any predicate is converted into a noun, the resulting noun is understood as something which does the action or has the quality described by the predicate. Notably, the case marker o not only changes the predicate len into a noun, but also marks it as the subject of the sentence. To mark the direct object of a sentence, **e** is used, while **a** marks the indirect object.

Observe the following sentence using the predicate **don** (“give”), which has both a direct object, which we will call “E”, and an indirect object, “A”:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***don o len e buk a len not.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“A person gives a book to another person.”*

This sentence also demonstrates the default verb-subject-object word order, or VSO. Nearly any word order is permissible, however, provided a few rules are followed: in particular, the verb marker **u** is needed to achieve certain word orders. However, in most VSO sentences, it may be elided. In this case, we know that the first word in the sentence, don, is the verb of the sentence because it is an unmarked predicate.

Second, note the indirect object, **a len not**. When a predicate immediately follows another predicate, the second predicate becomes a modifier acting on the first, and the predicate with modifiers then acts as a single unit. Here, the predicate **not** (“other”) modifies **len** to create a serial predicate meaning “to be another person”, which is then converted into an indirect object noun with **a**. Serial predicates in Xextan fill the role occupied by adjectives and adverbs in natural languages. This combining behavior of predicates is also the primary reason why **u** is necessary in certain word orders, as unintended serial predicates may form if one is not careful.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***e buk u don o len a len not.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“A book was given by a person to another person.”*

This means exactly the same thing as the previous example, but **u** is needed to prevent **buk** from forming a serial predicate with **don**, which would result in the sentence becoming a nonsensical fragment meaning something like “A giving-book a person another person.” Remember, however, that while every Xextan predicate has a subject O, not all have a direct object E or indirect object A. In short, case markers allow for highly free word order within sentences without sacrificing clarity or conciseness.

The particle **no** can be used to negate predicates, including those which have been converted into nouns, as well as nearly any other kind of Xextan word.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***no dal o dan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“The building is not large.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***tet o xta e no kol.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“An animal tries \[something\] not easy.”*

**tu** is the deictic (definite/demonstrative) particle, and can mean “this \[X\]” or “that \[X\]” depending on context. It belongs to the same grammatical class as **u**, and requires a case marker or preposition in order to use it in a noun phrase. However, **tu** is one of many Xextan particles which contracts/combines with other particles for conciseness. When used with one of the case markers **o**, **e**, or **a**, it contracts to form **to**, **te**, or **ta**.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***dzo xne to len.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“This person walks fast.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***no nel o dze te kep.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“A parent does not like that idea.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***tup o nan e xto ta dan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“A man throws rocks at that building.”*

Note that Xextan does not distinguish between definite and indefinite nouns. To specify that you are referring to a certain specific instance of something, possibly something recently mentioned, the deictic construction is used instead.

### Lesson 2: Arguments

In the previous chapter, we learned that the vast majority of concepts in Xextan are expressed with predicates, whether used as the verb of a sentence or converted into nouns with case markers. Pronouns are the primary exception to this rule: they act as nouns by default, and do not form serial predicates. Consider the following example, using the first and second person pronouns **ni** and **vo**, respectively:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***tak o ni e vo.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I talk to you.”*

Although they are written in the above example for clarity, since pronouns act as nouns by default, they also do not require a case marker in order to be used in a sentence, and therefore **tak ni vo** would be exactly equivalent to the above. Keep in mind, however, that unmarked nouns still possess an implied case marker, or role. The rule is that an unmarked noun will always take the highest priority role which has not already been filled, either expressly or implied, according to the case hierarchy O > E > A.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***a len bel u don le go.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“They gave it to a beautiful person.”*

Here, the only noun with an explicit case marker is **a len bel**, “to a beautiful person”. The verb **don** is marked with **u**, and is followed by an unmarked third-person pronoun **le**. Since the O role has not been filled, we know that **le** has an implied O case marker, making it the subject of the sentence. Then, the only role left to be filled is E, which is taken by **go**, giving us a sentence which literally means “To a beautiful person they gave it.”

Xextan distinguishes three kinds of animacy in pronouns, with an animate third person pronoun **le**, an inanimate third person pronoun **go**, and an abstract third person pronoun **du**. The latter is typically used to refer to a situation or thing that the speaker or another person has recently mentioned, e.g. **no dun ni du** (“I do not know that.”)

### Lesson 3: Illocutions

Any time you want to speak Xextan, you must announce yourself using a special word, or else you get bonked on the head with a wiffle bat.

Just kidding, only an absolute walnut would believe that. You do, however, need to separate your sentences with illocutions. These are special words that do the double duty of specifying the grammatical mood of a sentence while also preventing sentences from running into each other and making a giant mess of things.

The most basic illocution is **i**, which has no meaning of its own and serves only to separate sentences, or more accurately, independent clauses. As you have seen before, it may be dropped at the beginning of an utterance.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***(i) xek ni, i vit ni, i sna ni.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I came, I saw, I conquered.”*

Other illocutions change the meaning of a sentence completely: **ja** turns a sentence into a yes/no question and **jo** is used to form commands.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***ja nel vo e ban Xextan?***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Do you like Xextan?”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***jo get vo e xut!***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Get some water!”*

Meanwhile, **je** and **ju** indicate that the following sentence contains related or contrasting information, respectively. As such, they do not make any sense when used at the start of an utterance.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***no ten ni su pan, je txi ni e buk xextan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I don’t have any grain, so I’m eating a Xextan book.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***fik o loqban, ju kol o xextan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Lojban is hard, but Xextan is easy.”*

The last illocution is **ji**, which is used for performative speech – statements which become true merely by being said.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***ji kle ni vo.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I forgive you.”*

And that’s pretty much all there is to it.

### Lesson 4: Adverbs

While serial predicates serve the function of adverbs in many situations, there are a few true adverbs at our disposal that ought to be mentioned. These particles modify an entire clause, and may be placed anywhere within the clause in question with no change in meaning; the most common or “default” position is immediately before or after the predicate. The most important are the tense markers, namely **pa**, **na**, and **fa**, which represent the past, present, and future tense, respectively.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***pa vit ni e kit.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I saw a bug.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***zal ni na e tsazon.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I am currently at the park.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***zuk ni du fa.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I’ll do that later.”*

Another important set of adverbs are the five attitudinals, which as the name implies, express the speaker’s attitude or emotion. These include:

**wa**, which means understanding or realization: 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***wa, sendun ni na.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Oh, I understand now.”*

**we**, which expresses surprise, wonder, or fear:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***we! bálu!***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Whoa! A bear!”*

**wi**, which indicates happiness, gratefulness, or enjoyment:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***vit ni e lit, wi.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I can see light, fortunately.”*

**wo**, which conveys anger, annoyance, or discomfort:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***wo, txe pil ni…***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*Ugh, I’m so tired…”*

and **wu**, which denotes sadness, regret, or pity:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***no dun ni, wu.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I don’t know, sorry.”*
    
The words **qeu** and **nai** are used to mean “yes” and “no”, but are grammatically adverbs. They can be used both in response to a question and also in an adverbial role to affirm or deny a statement:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***sik ni e sundan sin, qeu.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I’m looking for a new house, indeed.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***lup le ni… nai.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“He loves me… not.”*

Finally, there is a special particle **fe** which converts any predicate into an adverb or adverbial phrase. Like other adverbs, a **fe**- adverb can technically be placed anywhere in the sentence, but watch out for unwanted serial predicates! The second example below uses the verb marker **u** to prevent the adverb from forming a serial with **qde**.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***jo got vo e xildan fexné!***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Get yourself to school quickly!”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***fextí, u qde ni e plevak.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*Quietly, I waited for the bus.*

Adverbial phrases formed with **fe** and **fi** and a predicate are typically written as one word, with an added acute accent above the core vowel of the predicate: e.g. **fesák**, **fizán**, etc.

Adverbs are one of the simplest yet most powerful pieces of Xextan grammar. Use them wisely, and you shall benefit most greatly.
This concludes our exploration of the basic foundations of Xextan. Future lessons will cover more advanced concepts; for now, live long and prosper, and **jo tak xextan**!

## Part 2: Intermediate

### Lesson 5: Determiners

A determiner is a word which expresses the intended referent of a given word or phrase. In Xextanic terms, a determiner converts a predicate into a noun, or adds additional information to an existing noun. The most basic determiners in Xextan are numbers, or quantifiers. Although Xextan lacks a singular-plural distinction, you can convey this distinction by directly specifying a number. The numbers from zero to nine are:

- nu (0)
- ne (1),
- duo (2)
- tie (3)
- kua (4)
- pei (5)
- lio (6)
- qai (7)
- bui (8)
- giu (9)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***got (o) ni (e) duo vendan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I go to two stores.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***vit (o) vo (e) pei sol.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“You see five stars.”*

In the above examples, the case markers may be dropped, as noun phrases formed from a determiner and a predicate automatically take implied case roles in accordance with the case hierarchy, just like pronouns. Nonetheless, as with pronouns, it is permissible to include the case marker for clarity or emphasis.
Xextan also features a set of possessive determiners, which create a possessive noun phrase. These include:

- **nia** - (“my”/”our”) 
- **vua** - (“your”) 
- **lia** - (“his”/”her”/”their”)
- **gua** - (“its”)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***pon (o) nia nandze (e) vua papkin (a) lia padqbu.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“My dad put your bag on his desk.”*

The determiner **po** converts a predicate or noun into an abstraction, or a subordinate clause. As with all other determiners, the resulting phrase is treated as a noun. This is similar to how the infinitive and participle forms of English predicates are used to convert predicates into nouns, like how the predicate “work” (**gun**) becomes “to work” or “working” (**po gun**):

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***fik (o) po gun.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Working is hard.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***nel (o) vo (e) po dul.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“You like to read.”*
    
The usefulness of simple **po** + predicate phrases is somewhat limited, but can be expanded with tags (ch. 7) and long scope (ch. 9).

Other determiners include **la**, which introduces “native” Xextan names, and **lu**, which converts a Xextan word or phrase into a noun representing the word/phrase itself. To introduce foreign names and quotes, the particles **lau** and **lou** are instead used, and the foreign word itself is surrounded by the delimiter phoneme, denoted by a tilde **~** as below. (The tilde may be realized as any sound not otherwise present in the quoted text.)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***sku la Bíli lu “bon!”***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Billy said, ‘Good!’”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***tin ni lau ~ Beatles ~ .***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I listen to the Beatles.”*

The determiner **lo** specifies that the referenced predicate is used in a gnomic or archetypal/stereotypical sense. It is not strictly necessary, as the generic case markers also cover this sense, but it may be applied for clarity or emphasis. To specify the opposite, i.e. that you are referring to a specific instance of the predicate, use the demonstrative **tu** (or its contracted variants) or apply a quantifier.

### Lesson 6: Prepositions

Having already learned the case markers **o**, **e**, and **a**, we can build on our knowledge with a closely related concept: prepositions. These are quite similar to case markers, but they can be added to any sentence regardless of the alignment of the main predicate. 

A fairly straightforward example is **peu**, the topic marker:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***ja dun vo peu kísékit?***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Do you know about elm seed bugs?”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***fip ni nu nan. ju, peu tu bek… u fip ni go.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I fear no man. But as for that thing… I fear it.”*

The preposition **za** (cf. **zal**, "to be at") is used to describe the location, context, or environment in which something takes place:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***pa vit ni le za dindan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I saw her at church.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***za ban xextan, u zat peixiduo zakvla.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“In the Xextan language, there are 500 root words.”*

To state that an action was performed using a certain tool or implement or by a certain method or technique, you can make use of **fo** (cf. **fol**, "to use").

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***pal ni e tik dal fo xlotul.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I’m building a huge machine using a hammer.”*

Another useful set of prepositions are **pau**, **nau**, and **fau**, which mean before, during, and after, respectively. Notice that they follow the same P-N-F pattern as **pa**, **na**, and **fa**. Unlike **peu**, though, these are primarily useful when used to encapsulate an entire clause, which requires the use of scope management. (See chapter 9, “Scope”, for details.)

There are many other prepositions to learn, including the vocative voi and the directional **fai**, but since they all behave exactly the same way, we do not need to cover all of them in detail at the moment. Remember though that while not necessarily grammatically incorrect, not all prepositions may make rational sense in a given sentence.

### Lesson 7: Tags
So far, we have mostly dealt with simple sentences, i.e. sentences consisting solely of one or more independent clauses. We will now examine a few devices which will allow us to construct more complex sentences.

Tags are particles which attach additional information to a predicate or noun phrase in the form of a secondary argument. The simplest of these is **pe**, which indicates that the following noun or predicate is associated with the former in some way.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***tak ni e len pe la Nípon.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I talk to a person from Japan.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***po qip u zon pe sui pel.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Life is a place of many dangers.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***xik o xta pe tun zin.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Animals from the tundra are strange.”*

Similar to **pe** is **ke**, a tag which attaches a relative phrase or clause. When applied to a noun, it has the effect of asserting that the following argument is equivalent to or represents a quality of the previous argument:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***zbu ni e sup ke txe vut.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I found a substance which is very explosive.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***fel o len ke tak xextan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Happy is the person who speaks Xextan.”*

As you may have noticed, many of these examples using **ke** are nearly equivalent to simply attaching the predicate as a serial, and **ke** here is therefore somewhat redundant. The real power of **ke** comes in combination with scope management, which we will not encounter for a few chapters. 

However, we have a similarly powerful mechanism at our disposal through the use of the binding tags **do**, **de**, and **da**. These special tags allow us to add a subject, object, or indirect object to the simple subordinate clause represented by the argument of **ke**- or any predicate, really. If that sounds confusing, the following examples should (hopefully) clarify things:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***xil vo peu ban ke pal do ni.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“You are learning about a language that I made.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***ja vit vo e txi de nia qba?***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Did you see the one who ate my fruit?”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***ti len ke sku da le.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“That’s the person who told them.”*

Note that **do** operates a little bit differently than **de** and **da**, in that in a **ke**-phrase it reverses the expressed relation between the tagged argument and the predicate: a “**len ke lup do ni**” is a person whom I love whereas a “**len ke lup de ni**” is a person who loves me. Outside of a **ke**-phrase, **do** retains this inversion behavior: while “**o txi**” is “something which eats”, “**o txi do ni**” is “something which I eat”.

### Lesson 8: Connectives

Before we dive into the more advanced grammar specific to logical languages and unambiguity, we need to cover one more basic part of speech common to nearly all languages: namely, connectives. In natural languages, this class of word is more commonly known as conjunctions. Xextan includes two categories of connectives, distinguishing between logical and non-logical variants. While both kinds of connective share an identical grammar, they serve somewhat different functions.

Logical connectives, as their name implies, serve a parallel function to logical operators in mathematics. Nonetheless, they are applied to the same kind of everyday situations as their counterparts in natural languages. The three logical connectives are **qe** (AND), **qa** (OR), and **qo** (XOR).

The AND operator **qe** is fairly self-explanatory: it corresponds closely to the English conjunction “and.”

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***dal qe bel to xan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“This mountain is large and beautiful.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***get vo e qba qe e pan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“You get fruit and grain.”*

(Note the repeated **e** in the second example above. This is necessary in order to ensure that the two arguments **qba** and **pan** remain distinct rather than combining their case alignment to form a single predicate **qba qe pan**, which would mean “[to be] both fruit and grain.”)

The OR operator **qa** predictably corresponds to English “or,” or more accurately “and/or”:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***fa dqu la Líli qa la Áiden.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Lily and/or Aiden will help.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***fo tu buk, u xil vo su nit qa sin.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“With this book, you are learning something interesting and/or new.”*

The XOR operator **qo** also means “or,” but specifically in the sense of “either A or B, but not both.”

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***zal o fendze e lia dan, qo e gunzon.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“The mother is either at home, or at work.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***vel qo blu to vak xne.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“The fast car was either red or blue.”*

Note that the same operators can be applied to connect virtually any part of speech, provided that the elements on either side of the operator belong to the same type. By default, any connective joins the element immediately to its right with the most recent element to its left of the same type. It is not possible to connect sentence elements of different types; rather, one of the elements must be converted to match the type of the other. Connectives can even join independent clauses when applied directly to the verb marker **u** or an opening illocution:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***na spalil ni, qo u na ske su txe xik.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Either I am dreaming, or something very strange is going on.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***txi o kával e xával; qe ju, txi o bálu e álu.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Horses eat rice; meanwhile, bears eat potatoes.”*

Last but not least, let’s take a look at non-logical connectives. As previously mentioned, non-logical connectives work the same way as logical connectives, but have different formal and semantic meanings. Most critical among these is **ze**, which joins elements into a single mass. ze may be used in contrast with **qe** in order to specify that the action described by a sentence is performed or received jointly by two or more entities, rather than individually. Consider the following examples:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***jo xle ni ze vo te piáno.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Let’s you and I \[together\] carry this piano.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***jo xle ni qe vo te piáno.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Let’s you and I \[each/individually\] carry this piano.”*
    
In addition to disambiguating joint and individual actions, **ze** also offers a convenient option for translating certain uses of the conjunction “with”:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***pal o fen ze o nan e sundan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“A woman builds a house \[together\] with a man.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***zgitak o xilnik ze lia xillen.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“A teacher sings \[together\] with his student.”*

Another non-logical connective is **kai**, which can be used to express literal or figurative comparisons. Note that unlike its English counterparts “like” and “as,” the position of **kai** in the sentence explicitly affects the nature of the comparison:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***jo no tak vo e ni kai lo sinpok.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Don’t talk to me like \[you would talk to\] a child.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***jo no tak vo kai lo sinpok e ni.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Don’t talk to me like a child \[would talk\].”*

Finally, as with logical connectives, a comparison can be expanded to a full clause to achieve clarity, by placing **u** or an illocution after the connective:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***pa fel lia xin kai u ben o dalsol.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Her heart rejoiced like the sun blazes.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***bonvet ni vo kai u bonvet ni nia fendze ze ne xlotul.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I trust you like I trust my mother with a hammer.”*

## Part 3: Advanced

### Lesson 9: Scope

Perhaps the most critical concept in all of logical language theory, and certainly the mechanism which sets logical languages apart from all other languages both natural and constructed, is the ability to explicitly delimit the scope of sentence elements. True mastery over a logical language, especially in spoken conversation, requires a thorough knowledge of both how to proactively manage scope, and also how to avoid becoming entangled in excessively complex sentence structures in the first place.

The term scope management, as I use it in this book, refers to the ways in which a logical language explicitly binds sentence elements (including nouns, adverbs, prepositional phrases, and others) to the clause to which they  properly belong. Simple sentences, i.e. those which consist of a single independent clause, typically do not require extensive scope management in order to remain syntactically ambiguous.

Rather, explicit scope management becomes a necessity in complex sentences which include one or more subordinate clauses, especially where clauses occur embedded or nested within other clauses. Xextan, like most logical languages, primarily handles scope through the use of particles which “step down” a level of scope, and other particles (called terminators) whose sole function is to explicitly close that scope in order to return to the “top level,” i.e. the main independent clause.

In Xextan, only particles which take an argument, known as operators, can introduce their own levels of scope. Operators include determiners, prepositions (including case markers), tags, and connectives. Each of these classes of particles carries short scope by default, meaning that they accept a single noun phrase as their argument. For the purpose of short scope, a single noun phrase can consist of an individual noun or predicate, a serial predicate of arbitrary length, or a noun or predicate with trailing arguments of its own tagged with **pe**, **ke**, or **do**/**de**/**da**.

In the following examples, any particles carrying short scope and the extent of their scope is denoted with curly braces **{ }**:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***sik {o len} {e xta sin}.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“A person searches for a new animal.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***zal ni {e xtevak {ke xle {de qipxto}}}.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I am on a train that is carrying coal.”*

Every example sentence we have encountered up to this point has made exclusive use of short scope constructions. As the name implies, short scope is limited by its very nature, and constructions carrying short scope tend to resolve themselves without much forethought on the part of the speaker. For this reason, short scope is a highly powerful tool for maintaining syntactic unambiguity with little cost.

That said, of course, there are times when you may need to construct a more convoluted sentence, perhaps one with multiple subordinate clauses which each contain their own complex constructions. For this, it is typically more effective to apply long scope. Any particle which can carry short scope can also carry long scope: to introduce long scope, the vowel or diphthong of the particle in question is nasalized, indicated with a tilde diacritic (**~**) over the vowel (for particles with diphthongs, over the first letter of the diphthong; for particles with a glide, over the non-glide vowel).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***vet ni põ bel qe nit o ban Xextan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I think that Xextan is beautiful and interesting.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***zat o fen lal kẽ pa sun e katnokfuk.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“There was an old lady who lived in a shoe.”*

While short scope takes a single noun phrase as its argument, and closes automatically as soon as this argument has ended, long scope instead takes an entire clause as its argument, and ends only when the speaker begins a new sentence with an illocution, or else explicitly closes the scope using the long scope terminator **ku**. Note that **ku** only closes a single long scope clause; however, because it is difficult to keep track of nested levels when speaking aloud, we also have the universal terminator **xu**, which closes all open clauses and returns to top level.

Observe how the scope of the subordinate clause in the following examples completely changes the meaning of the sentence:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***pa tin ni {põ fol vo e piáno za nia danzi}.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I heard you playing the piano [while you were] in my room.”*
    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***pa tin ni {põ fol vo e piáno ku} za nia danzi.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I heard you playing the piano [while I was] in my room.”*

### Lesson 10: Serialization

Although you can certainly construct complex sentences and make yourself understood with explicitly delimited scope using **po**-clauses in both short and long scope variants, this can become cumbersome and may feel somewhat unnatural to those of us not bestowed with the blessing of speaking a logical language as one’s native tongue. To remedy this, Xextan allows some subordinate clauses to be serialized. That is, certain predicates provide for implicit subordination when additional predicates are chained. This is similar to expressly invoking a subordinate clause with long-scope **po**.

Recall from way back in chapter 1 that a predicate which occurs directly adjacent to another predicate will combine to form a serial predicate. For most predicates, the trailing predicate simply acts as a modifier or descriptor to the initial predicate, and the resulting serial inherits an identical case alignment to that of the initial predicate.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***dan***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*O is a building*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***qbi***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*O is nearby to E*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***dan qbi***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*O is a nearby building*

However, this basic “modifier” behavior is not the only way in which serial predicates combine. Every predicate belongs to a particular class, and the class of a predicate determines its serialization behavior. Predicate classes can be found in the “Class” column in the Vlabuk Xextan.

The most important alternative combining behavior to learn is that of lambda predicates, which function as auxiliary verbs. When a trailing predicate is chained to a lambda predicate in serial, the case alignment of the two predicates combines or “hinges” at the O case slot, meaning that the resulting serial inherits the O slot of the lambda predicate while the rest of the case alignment is inherited from the serialized predicate, unlike with ordinary serials. For example, given a lambda predicate **tet** (O tries to do Eu) and an ordinary action predicate **xlo** (O hits E), we obtain a complex serial predicate **tet xlo** (“O tries to hit E”).

A few of the most common lambda predicates include **ken** (Ou is possible); **tet** (O tries to do Eu); **vol** (O wants to do Eu); **txu** (O needs to do Eu); and **tse** (O intends to do Eu). The "Ou" and “Eu” in the predicate definition conveys that the serialized predicate corresponds to a **po**-clause placed in the O and E case slot, respectively.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***ken ni fol e saltik.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I can use a calculator.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***txu le zbu e lindalfuk bel.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“She needs to find a beautiful dress.”*

Lambda predicates can even serialize with other lambda predicates to form a longer chain. For instance, in the first example below, the complex serial tse **tet xen leknik** hinges three lambdas together with the ordinary predicate **leknik** (“O is a doctor”) to form a single complex predicate meaning “O intends to try to become a doctor”.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***nau nia sintep, u tse ni tet xen leknik.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“In my youth, I intended to try to become a doctor.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***vol vo ken tak xextan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“You want to be able to speak Xextan.”*

Because lambda verbs fully unite their case alignments into a single complex predicate, nouns may technically be placed before, after, or between the individual predicates without altering the meaning. However, the convention is to place the subject of the sentence immediately after the initial predicate, “sandwiching” it between the main predicate and any trailing predicates, in order to preserve the same word order as the **po**-clause variant:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***tet ni (põ) pal e ban.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I am trying to create a language.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***no fin vo (põ) dul te buk.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“You are not finished reading this book.”*

Lastly, comparisons and superlatives in Xextan are expressed using lambda verbs, namely gen (“more”) and net (“most”):

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***põ lutsna e sel xu gen fik põ galgot e xan ke net dal.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Conquering the self is harder than ascending the highest mountain.”*

Another mechanism we should cover is the ability to break up trailing serial elements from their head, which we will call split serialization. Ordinarily, serials are constructed by simply placing two predicates next to each other without an intervening operator or terminator. However, it is also possible to explicitly mark serial elements, which allows them to be moved to a later position in the sentence.

To accomplish this, all we need to do is attach a case marker to the descriptive element, just like we would otherwise do to create an ordinary noun phrase. If multiple arguments with the same case marker appear in a sentence, arguments with a repeated case marker will be treated as serial elements modifying a prior element which bears that case marker.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***don nia sat te txixo ni - o donfel.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*My friend gave this food to me - the generous one.*
 
### Lesson 11: Lambda

The term lambda as applied to logical languages is borrowed directly from Lojban, where it refers to a kind of syntactical “hole” in a clause which can be referenced in various ways. The term is also sometimes applied more broadly to a type of subordinate clause construct which defines abstract properties in terms of lambda. Despite the fancy Greek name, the concept of lambda is not terribly foreign from a natural language perspective. However, the majority of natural languages apply it in a sort of invisible or unspoken way, typically embedded directly into a grammatical construct and impossible to reference on its own.

Bane of prescriptivist English teachers the world over, you have likely grasped at this phantom grammar accident at least once purely by accident when attempting to speak a complex relative clause, as standard English conspicuously lacks a device to relocate the “target” of the relative clause from its initial position. This “target” is the very same lambda which I have just referred to… it? (Oh man, now I have to start the whole sentence over…)

Fortunately, in Xextan we are not so constrained. To refer to the target of a relative clause opened with **ke**, we can simply invoke it directly by calling its name, which in its simplest form is the lambda pronoun **xe**. This special predicate implicitly occupies the O case slot of every relative clause – in both short and long scope varieties – unless specifically placed elsewhere.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***pen ni e dan kẽ vol ni sun e xe.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I am thinking about the house in which I want to live.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***godqik o xallun e dallun kẽ spe fai xe o sollit e go.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“The moon orbits a planet toward which sunlight reflects off of it.”*

When **xe** is invoked in a **po**-clause instead of a relative clause, it creates a proposition focused on the lambda “hole” rather than the clause itself:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***val põ vet o len e xe.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“What a person believes is important.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***no dun o sik põ zal ni sot za xe.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“The seeker does not know where I am hiding.”*

As you can see, in Xextan, lambda serves the function played by indirect questions in English and other Indo-European languages. Most indirect questions, including “where”, “why”, and “who”/”what”/”which” can be expressed by introducing a subordinate clause containing **xe** in combination with the appropriate preposition. However, indirect yes-or-no questions, which in English are expressed with the conjunction “whether”, cannot be constructed in the same way. Instead, a distinct but related construction is used, by introducing the irrealis tense to the subordinate clause, indicated by the tense marker **xa**:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***dun ni põ xa lup vo ni.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I know whether [or not] you love me.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***san po sna põ xa tet fi-sil.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Success depends on whether one tries hard.”*

The irrealis tense has another important function, in constructing “if” statements. To achieve this, we need the conditional preposition **xau**, which corresponds to **xa** in the same way that the tenses **pa**, **na**, and **fa** correspond to their prepositional variants **pau**, **nau**, and **fau**. In formal logic terms, **xau** marks the antecedent (if X…) while xa marks the consequent (...then Y) of an if-then statement. In Xextan, while the two elements of the hypothetical may occur in any order, take care to apply the correct marker to each.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***xa zalxen vo e kiltun xãu got vo fai tu xte.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“You will reach the forest if you follow this path."*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***xãu dun vo e ban Loqban, u xa kol pe vo o ban Xextan.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“If you already know Lojban, then Xextan will be easy for you."*

Finally, we can also make use of the long scope variants of case markers using the lambda pronoun. When applied to a case marker or a determiner other than **po** itself, the lambda construction takes on a “that which does…” or “that which is…” meaning.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***fip vo ẽ no sendun vo e xe.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“You are afraid of something which you do not understand.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***fa qip nau tep dal õ zgitak o xe fi-dalson qe pio xin tut.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Those who sing loudly and with their whole heart will live long.”*

### Lesson 12: Transmogrification

The core principle of the design and philosophy of Xextan is “doing more with less”, and this is also apparent in the way the language handles types. Some logical languages such as Lojban (and, to a lesser extent, Loglan) maintain strict systems of type correctness, preferring to create new words or constructions to apply to different kinds of sentence elements rather than extrapolating existing devices to apply to multiple different circumstances.

This does have certain advantages, particularly at the parser level, but it also comes at the expense of ease of learning for the human user. Since Xextan values accessibility and practicality over engineered perfection, it takes a radically different approach to types from its predecessors. It is actually more difficult than you might expect to commit a syntax error when speaking Xextan; rather, you are much more likely to stumble your way into something perfectly grammatical but semantically nonsensical.

This is primarily because most parts of speech in Xextan which accept an argument (operators) are designed to be able to accept other kinds of arguments than their typical “input”. When an operator which expects an argument of a certain type instead encounters a sentence element which it does not normally expect, rather than throwing an error, it simply “pretends” that the mismatched element belongs to the correct type. This behavior is not merely intended as a fallback for type errors and edge cases: in fact, it is a powerful tool which can be employed intentionally in various ways.

A sentence element to which this effect has been applied does not actually change its underlying behavior or relationship to other elements. Thus I have nicknamed this peculiar feature transmogrification, in reference to the famous Calvin & Hobbes comic strip wherein young Calvin “invents” a device to allow him to magically transform into a tiger like his buddy Hobbes. (The reader knows, of course, that Calvin has not really turned into a tiger and that this is all just pretend – but in Calvin’s imagination, it is as real as can be.)

The most common use case for transmogrification involves the verb marker **u**. Recall that the word or phrase that follows **u** is always the main verb of the clause in which it appears. Typically, the word that follows **u** will be a predicate of some sort, as this is the type which **u** expects as its input. However, there is nothing stopping us from feeding it other kinds of words, including pronouns, determiners, and even tags. As you can see from the following examples, this is one of the situations in which it is appropriate (indeed, even recommended) to break the default verb-subject-object word order in order to shift the emphasis of the sentence.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***o pal de tu buk u ni.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“The creator of this book is me.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***la Din u tie, je la Din u ne.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“God is three, and God is one.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***o zgi u ke kok de põ qat ni vol qip.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Music is what keeps me going.”*

One might say that this basic copula-esque behavior of **u** forms the foundation of the transmogrification behavior of most other operators. (However, note that on the syntax level, **u** is actually a preposition, and functions identically to case markers or other prepositions.)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***dun ni e kẽ no dun vo e xe.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“I know something that you don’t know.”*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***ten sua ni e búbal na; i xne o vua, ju slu o nia.***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Everybody’s got a water buffalo; yours is fast but mine is slow.”*

Formally speaking, the argument version of transmogrification employs a trick involving the special null predicate **bo**. Similar to **ka**, **bo** is a particle which behaves as a predicate in all ways, even forming serials with adjacent predicates. In the above examples, it is as though an invisible **bo** were inserted between the case marker and the tag, or following the determiner.  On its own, the meaning of **bo** is entirely undefined, and left up to context. It is primarily useful to refer anaphorically to an entity or action which has been previously stated, and is therefore known to the listener.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;***jo bo!***
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*“Do the thing!”*