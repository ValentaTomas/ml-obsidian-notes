For a given word the n-gram outputs a list of all sequences in the word that have the length bigger or equal that the n-gram's `minn` and lesser or equal than the n-gram's `maxn`. The start and end of the word is also considered a character.

For a word `apple` an n-gram with `maxn = 3` and `minn = 3` is `['<ap', 'app', 'ppl', 'ple', 'le>']`. The `<` and `>` represents the start and the end of the word.