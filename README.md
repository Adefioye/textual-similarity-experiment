## AI similarity feature

Just a plaground for testing semantic models on how they can help solve 2 major issues in an AI-driven educational app
- How similar students' responses are in terms of near copy-and-pastinf
- How similar students' responses are in terms of paraphrasing

Essentially create a solution that can spot 2 issue:
- copy-and-paste response
- paraphrased response

## Current findings
- For STSB, openai doing great with a correlation of 0.88 relative to gold label
- For MRPC, the data essentially fall in 2 categories `paraphrased sentence` and `near-copy sentence` and openai embedding model doing great as the mean similarity score for both are `0.93` and `0.87` respectively. This suggests semantic models are kind of great at spotting `paraphrased` and `near-copy` sentence.
- For Clough-Stevenson plagiarism dataset, it can be seen that `non-plagiarised` data has lower similarity relative to near-copy and paraphrased data. The only issue here now is that the `non-plagiarized` data has similarity score as high as `0.88`.
- For spin-bot paraphrased paragraphs and documents, the mean similarity scores are `0.93` and `0.92` respectively. Most of the similarity score distributions are over `90%`, suggesting semantic search works effectively in identifying machine-generated paraphrased texts.

## TODO 
- [ ] Inspect non-plagiarized data in Clough-Stevenson data to observe how similar the no-plagiarized text is relative to original text.

Really not well handled in git