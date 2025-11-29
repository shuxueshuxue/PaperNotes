#paper #llm

[Context_Cascade_Compression_Exploring_the_Upper_Limits_of_Text_Compression_692926b2e931079b65d68b94_main](Context_Cascade_Compression_Exploring_the_Upper_Limits_of_Text_Compression_692926b2e931079b65d68b94_main.pdf)

![|600](paper%20note%201.png)

It's interesting that it uses an extra LLM to compress information.

Qwen2.5 1.5B and Qwen2.5 3B. While initialized with pre-trained weights, both the encoder and decoder are trained.

My question is, is it really new?

> For the scope of this paper, our investigation is **focused exclusively on the fundamental task of text reconstruction**. This task serves as a direct and rigorous benchmark for evaluating the information fidelity of our C3 compression architecture. By tasking the model with perfectly recreating the original input text from its compressed representation, we can quantitatively measure the degree of information preserved throughout the compression-decompression cycle. This setup provides a clear, objective measure of the compression’s "lossiness" and establishes a baseline for the model’s capabilities.

Since it doesn't demonstrate its performance for tasks besides text reconstruction, it doesn't convince that it's useful compression.
