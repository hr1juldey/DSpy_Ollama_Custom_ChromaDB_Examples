# DSpy Ollama Custom Examples with Custom Ollama based Retriever for ChromaDB 

## Anchknowledgements and premise of writng this code

The methods and ways mentionned in most of the `DSPy` examples that uses `ChromadbRM` ,`ColBERTv2`, `MilvusRM`, `QdrantRM`, `WeaviateRM`  etc fails 
to consider these points mentionned below:

1. Everybody is Not a seasoned progrmmaer who can easily spin-up local databases, web servers on a whim!
2. LLM != `GPT-4` or `GPT-3.5` or `Grok` or `Claude` or any other bigshot expensive money burning exernal api keys that makes a big hole in a `Dev`'s Pocket and Morale
3. I Whole heartedly respect and love all those investors and Scientists who made it possible to develop and use all these Greate LLms, But Being a  Biologist to turned himself from coding Dna to Coding LLMs, I believe  
> **Life** (and a pair of `Kanjoose Bengali Engineers` 😉 ) always finds a way! (To get away with doing things easy and for free 😝)
4. Sorry for diverting into the cavernous side alleys of insomniac thoughts.
5. And another issue is that everyone is not a guy who uses pthon with *OOPs*, and this can be a big OOps!! for a lot of newcommers =`nc`


## What did I do

Well well, being a subset of `nc` myself (with a history of making complex programms in [Blender's](https://www.blender.org/)  Geometry node) and having blessed with Guides, friends and Youtubers  Like [Arnav Singhvi](https://www.linkedin.com/in/arnav-singhvi-1323a7189/) & [Herumb Shandilya](https://www.linkedin.com/in/herumb-shandilya/) from [`DSPy`](https://dspy-docs.vercel.app/)
[Connor Shorten](https://www.linkedin.com/in/connor-shorten-34923a178/) from [`Weaviate`](https://www.linkedin.com/company/weaviate-io/) and [Tamoghna Das](https://www.linkedin.com/in/tamoghnadas12/), My College senior who brought me into this world of LLms in November 2022. And The last but Not the least [`Perplexity`](https://www.perplexity.ai/) for enabling millions like me who are a subset of `nc` to code without fear of syntaxes. 

1. Studied the Ollama Library in python that is given by [ollama](https://ollama.com/) and make an embedder:retiever  function pair
2. made a local server of Ollama and Chromadb run from a given directory from urls `http://localhost:11434/` and `http://localhost:8000/` respectively.
3. Used NLTK's `Sent_tokenize` for chunking the text into sentences that will be fed to the ChromaDB 
4. Made a Ollama based LLM run in DSPy
5. Created the default `GenerateAnswer` and `GenerateSearchQuery` `Signature`s for Rag (Never used the `GenerateSearchQuery` for being a noob myself 😝)
6. Created a `markdown` file that has the data I am doing `RAG` on (in a later example I will show you how to do rag on web search data)


## So let's jump into the project!!!
