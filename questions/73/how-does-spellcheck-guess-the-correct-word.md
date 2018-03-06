## How does spellcheck guess the correct word?

- posted by: [ursa_arcadius](https://stackexchange.com/users/-1/68-ursa-arcadius) on 2011-04-18
- tagged: `computers`, `programming`, `word-processing`
- score: 4

Sometimes I have had some words that are pretty far off but are still corrected.  Other times I have had long words that are off by only one letter that it can not find a suggestion for.  What methods does it use for suggesting words that are sometimes not even close to the desired word?


## Answer 85

- posted by: [Tangurena](https://stackexchange.com/users/-1/74-tangurena) on 2011-04-18
- score: 3

<p>Generally, there are 4 steps to a <a href="http://en.wikipedia.org/wiki/Spell_checker" rel="nofollow">spell checker</a>'s operation:  </p>

<ol>
<li>Scan the text and break things up into words and word-stems.  </li>
<li>Compare the words and word-stems against some dictionary.   </li>
<li>Compare the words against a model of grammar. </li>
<li>If not found, suggest alternative via closest matches.  </li>
</ol>

<p><a href="http://en.wikipedia.org/wiki/Stemming" rel="nofollow">Word-stemming</a> is the technique of finding the basic root portion of a word. <code>stand</code> is the stem of <code>standing</code>.</p>

<p>Step 3 is usually called "grammar checking" but is frequently done as part of spell-checking because it is the way to catch correctly spelled words that are the wrong word for the sentence they are in; such as effect/affect and its/it's.  </p>

<p>When words are found in your document that are not in the dictionary, the spell checker is going to suggest the most likely candidates by using measurements like <a href="http://en.wikipedia.org/wiki/Levenshtein_distance" rel="nofollow">Levenshtein distance</a>. These <a href="http://en.wikipedia.org/wiki/Approximate_string_matching" rel="nofollow">algorithms</a> try to guess what the smallest number of changes need to be made to turn one word into another.  </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
