
[Does Forcing Structured Output Degrade LLM Creativity? \| OpenReview](https://openreview.net/forum?id=vYkz5tzzjV)

An interesting paper. It says that  structured output can degrade LLM creativity. 
I think it's not limited to "creativity", but general performance, too.
There is a "cognitive load" theory to explain this.
Different models have different degree of degration.

> “Gemini-2.5-Flash, Llama-4-Maverick, and Mistral-Nemo showed approximately 4–5× greater degradation than the GPT models. This suggests that some model architectures may be more susceptible to performance loss when handling concurrent formatting and creation demands.”

This result is aligned with my observation that Gemini Flash is terrible at instruction following - so perhaps it pays more "cognitive load"!

The style of this research is similar to my this observation: [prompt trick](prompt%20trick.md)

A good blog for this: (xml is perhaps better than json)
[Why Does My LLM Structured Output Perform Poorly? \| Yanli 盐粒](https://blog.yanli.one/Why-Does-My-LLM-Structured-Output-Perform-Poorly)
