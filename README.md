# libchopshop

- NLP/text processing with automated stop word detection and stemmer-based filtering
- **input** is international language plain text (UTF-8)
- **output** is n-gram / k-mer output vectors`<uint16_t>`/`<uint32_t>`/`<uint64_t>` with optional weight vector`<float>`/`<double>`/`<int>`
  + support variable length n-grams, q-grams, skip-grams, *elasti*-grams, k-grams for arbitrary k
  + character / symbol / codepoint and word + phrase level tokens (grams)
    + "words" are discovered in the input text stream by redefinable NLP tokenizers; may be dictionary-assisted or aided otherwise.
  + attributed / augmented n-grams (POS encoding as part of the n-gram; ditto for whole-word/part-of-word/start-,end-of-word markers)
  + support weights / ranking -based filtering of the token stream ("*primus inter pares*", only the "*upper crust*" are allowed through into the output vectors)
    
  
