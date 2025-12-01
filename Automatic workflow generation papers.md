#paper #agent 

[MetaAgent_Automatically_Constructing_MultiAgent_Systems_Based_on_Finite_State_Machines_692d15b6e931079b65d68b96_main](MetaAgent_Automatically_Constructing_MultiAgent_Systems_Based_on_Finite_State_Machines_692d15b6e931079b65d68b96_main.pdf)
[MetaAgent](https://mp.weixin.qq.com/s/fpBteFHZkwX-48PtElUS4w)
[MetaAgent: Automatically Building Multi-Agent System based on Finite State Machine \| OpenReview](https://openreview.net/forum?id=a7gfCUhwdV)
这篇论文先是被 ICLR 拒稿。几个月后被 ICML 接收。网上讨论较多，噱头比较大，贡献了一个概念，没什么方法。

拒稿理由值得一看：
The paper introduces MetaAgent, a framework for automatically constructing multi-agent systems using finite state machines (FSM). While it addresses an important problem, the paper has several critical weaknesses. The **experimental scope is narrow**, focusing on two coding tasks and one NLP task, limiting the evaluation of its generalization capabilities. Key methodological details, such as FSM implementation, test case generation, and agent design, are poorly explained, impeding reproducibility. The paper also **lacks sufficient theoretical justification** for using FSMs over alternative methods and fails to analyze the practical **trade-offs, such as computational costs**. Additionally, the writing quality, including unclear figures and inconsistencies, detracts from the paper’s overall clarity.

Strengths include addressing automation in multi-agent system design and the introduction of self-iteration and state traceback. However, these are overshadowed by the lack of detailed implementation, narrow evaluation, and limited novelty.

**Additional Comments On Reviewer Discussion:**

The rebuttal clarified some aspects, such as the FSM's role and examples of agent design, but did not sufficiently address concerns about the limited evaluation, unclear implementation details, and lack of theoretical grounding. Reviewers remained unconvinced of the framework's scalability and practical relevance. Despite efforts to provide additional explanations, the methodological and experimental limitations justify the rejection, with encouragement for substantial revisions.

## relevant works

This is a simple and elegant framework.
[GitHub - jsz-05/LLM-State-Machine: Framework for building conversational agents using a Finite State Machine (FSM) and LLMs](https://github.com/jsz-05/LLM-State-Machine?tab=Apache-2.0-1-ov-file#readme)

This one seems similar but poorly documented.
[GitHub - statelyai/agent: Create state-machine-powered LLM agents using XState](https://github.com/statelyai/agent)

In this paper, the flow is pre-defined. And not framed as multi-agent system (that is to say, the problems it's trying to solve are not complicated enough).
[StateFlow_Enhancing_LLM_TaskSolving_through_StateDriven_Workflows_692d1740e931079b65d68b97_main](StateFlow_Enhancing_LLM_TaskSolving_through_StateDriven_Workflows_692d1740e931079b65d68b97_main.pdf)
