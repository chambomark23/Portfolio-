# Presidential speech comparison

Sources: https://github.com/newtfire/introDH-Hub/tree/master/textFiles/inaugural

Early: Washington 1789, Adams 1797, Jefferson 1801.
Modern: George W. Bush 2001, Obama 2009, Trump 2017.

The six source texts were copied without edits. Texts stay outside docs; analysis screenshots and the webpage stay inside docs.

Voyant uses its automatic stop-word list. It counts 5482 words early and 5443 modern.
The initial 3-gram comparison lowercases text and uses [a-z]+(?:'[a-z]+)? tokens, keeps stop words, and counts overlapping windows separately inside each speech. Its modern count is 5439 because tokenization differs from Voyant.

Final analysis uses AntConc 3.5.9 (Linux), with each corpus loaded separately, case sensitivity off, common words retained, minimum frequency 1 and minimum range 1. N-gram experiments cover 2, 3, and a range of 4–5 words. Concordance checks include "of the people" in both groups and "we will" in the modern group. The modern Concordance Plot shows 13 matches in Bush, 12 in Obama and 26 in Trump. Actual AntConc screenshots are in docs/images. AntConc splits some punctuation differently from Voyant and the separate regex count.
