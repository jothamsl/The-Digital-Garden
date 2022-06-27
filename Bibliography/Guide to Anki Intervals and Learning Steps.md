# Guide to Anki Intervals and Learning Steps

### Metadata
- Author:: Conan Liu, M.D
- Medium:: #Youtube 
- Date Created:: 2022-03-06
- - - 

## Types of Cards
There are four types of cards in Anki, they are the
**<mark style="background: #ADCCFFA6;">New</mark>**, **<mark style="background: #FF5582A6;">Learning</mark>**, **<mark style="background: #BBFABBA6;">Graduated</mark>**  and **<mark style="background: #FF5582A6;">Re-learning</mark>** cards.

![[Pasted image 20220306140810.png]]

## How Intervals are calculated

An interval is the spacing between when a card is initially shown and when it’ll be shown next. It is given as the following equation:

![[Pasted image 20220306141421.png]]

If your an initial interval of 10 days, your new interval would be equal to:$$New\ interval=10\times 2.5\times 1=25\ days$$The process continues every time you click **<mark style="background: #BBFABBA6;">good</mark>** on your card rating.

## Difference Between Ease & Interval Modifier
- Ease applies to individual cards 
- Interval modifier applies to cards within a deck

If you have a deck with an interval modifier of a 100% and a card with an ease value of 210% along with an interval of 10 days, the card’s new interval would be $10\times 2.1\times 1=21\ days$. If you later on decide to move that same card to a different deck which has an interval modifier of 70%, then the card’s new interval would become $10\times 2.1\times 0.7= \approx15\ days$. Notice how the ease value of the card remains the same even when moved to a different deck with a different interval modifier.

## How Answers Modify Ease Factor
When going through a card, the answer given alters its ease factor.

- An answer of <mark style="background: #BBFABBA6;">**Good**</mark> : *ease remains unchanged*
- An answer of <mark style="background: #FF5582A6;"> **Again**</mark> : *ease factor - 20%*
- An answer of **Hard:** *ease factor - 15%*
- An answer of <mark style="background: #ADCCFFA6;">**Easy:**</mark> *ease factor + 15%*

