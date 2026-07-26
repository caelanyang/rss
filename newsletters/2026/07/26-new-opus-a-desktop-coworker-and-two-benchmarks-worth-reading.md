# 📡  New Opus, a Desktop Coworker, and Two Benchmarks Worth Reading

**来源：** Marktechpost AI  
**日期：** 2026-07-26  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22%F0%9F%93%A1%20%20New%20Opus%2C%20a%20Desktop%20Coworker%2C%20and%20Two%20Benchmarks%20Worth%20Reading%22>

---

From: Marktechpost AI <marktechpost-newsletter@mail.beehiiv.com>
To: news.hodor@gmail.com <news.hodor@gmail.com>
Subject: 📡  New Opus, a Desktop Coworker, and Two Benchmarks Worth Reading


> 🌐 **译文：**
> 发件人：Marktechpost AI <marktechpost-newsletter@mail.beehiiv.com>

收件人：news.hodor@gmail.com <news.hodor@gmail.com>

主题：📡 新 Opus、桌面协作软件以及两项值得关注的基准测试

View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/46f3d4ca-8206-4c67-8da1-0aefb52e5b1f/600x100.png?t=1782465050)
Follow image link: (https://pxllnk.co/c1pzvpb)
Caption: _**Together with Datalab **_

==Anthropic ships Opus 5 at unchanged pricing, Andrew Ng releases a desktop coworker that hands you finished work, and a Rust tokenizer hits 24.53 GB/s. And the open OCR and ASR fields get honest benchmarks.== **[Datalab's Marker 2 vs MinerU, Docling & LiteParse: The Doc-Parsing Benchmark](https://www.marktechpost.com/2026/07/24/datalab-marker-v2-vs-mineru-docling-and-liteparse-benchmark-breakdown/)**


> 🌐 **译文：**
> ==Anthropic 以不变的价格发布了 Opus 5，吴恩达发布了一款桌面协作工具，可以帮你处理完成的工作，Rust 分词器达到了 24.53 GB/s 的速度。此外，开源 OCR 和 ASR 领域也获得了客观的基准测试结果。== **[Datalab 的 Marker 2 对比 MinerU、Docling 和 LiteParse：文档解析基准测试](https://www.marktechpost.com/2026/07/24/datalab-marker-v2-vs-mineru-docling-and-liteparse-benchmark-breakdown/)**

View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/50004ce3-2956-47e2-acdb-438c1620b1da/600x50.png?t=1782465583)
Caption: 

### **[Meet GigaToken: A Rust BPE Tokenizer at 24.53 GB/s, Up to 989x Faster](https://www.marktechpost.com/2026/07/23/meet-gigatoken-a-rust-bpe-tokenizer-that-encodes-text-at-24-53-gb-s-up-to-989x-faster-than-huggingface-tokenizers/)**


> 🌐 **译文：**
> ### **[隆重推出 GigaToken：一款 Rust BPE 分词器，速度高达 24.53 GB/s，比 Huggingface Tokenizers 快 989 倍](https://www.marktechpost.com/2026/07/23/meet-gigatoken-a-rust-bpe-tokenizer-that-encodes-text-at-24-53-gb-s-up-to-989x-faster-than-huggingface-tokenizers/)**

Marcel Røed released **[GigaToken](https://github.com/huggingface/tokenizers)**, an open-source **Rust BPE tokenizer** that encodes text at **24.53 GB/s** on a 144-core AMD EPYC 9565 — vs 24.8 MB/s for HuggingFace tokenizers, a claimed **up to 989x speedup** (and ~681x over tiktoken). It's a **drop-in replacement**, 66% Rust / 33% Python.


> 🌐 **译文：**
> Marcel Røed 发布了开源的 Rust BPE 分词器 GigaToken，在 144 核 AMD EPYC 9565 处理器上，其文本编码速度高达 24.53 GB/s，而 HuggingFace 分词器的速度仅为 24.8 MB/s，据称速度提升高达 989 倍（比 tiktoken 快约 681 倍）。GigaToken 可直接替代 HuggingFace 分词器，代码构成中 66% 为 Rust，33% 为 Python。

**So what:** Tokenization is invisible until it's your bottleneck — at data-prep and high-throughput inference scale, it absolutely is. A drop-in that turns MB/s into GB/s reclaims real wall-clock time from every pipeline that touches text.


> 🌐 **译文：**
> **所以呢？** 分词在成为瓶颈之前是隐形的——但在数据准备和高吞吐量推理规模下，它绝对是瓶颈。一个能将 MB/s 的性能提升到 GB/s 的即插即用组件，就能为所有涉及文本处理的流程节省实际运行时间。

----------

----------View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/158fe355-f64c-4090-bc08-158edfbf4c27/600x50.png?t=1782465836)
Caption: 


> 🌐 **译文：**
> ----------查看图片：(https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/158fe355-f64c-4090-bc08-158edfbf4c27/600x50.png?t=1782465836)

图片说明：

----------
### **[Datalab's Marker 2 vs MinerU, Docling & LiteParse: The Doc-Parsing Benchmark](https://www.marktechpost.com/2026/07/24/datalab-marker-v2-vs-mineru-docling-and-liteparse-benchmark-breakdown/)**


> 🌐 **译文：**
> ----------

### **[Datalab Marker 2 对比 MinerU、Docling 和 LiteParse：文档解析基准测试](https://www.marktechpost.com/2026/07/24/datalab-marker-v2-vs-mineru-docling-and-liteparse-benchmark-breakdown/)**

A head-to-head of open PDF-to-markdown parsers. **[Marker 2](https://pxllnk.co/c1pzvpb)** scores **76.0 on olmOCR-bench at 2.9 pages/sec** — matching Gemini/MinerU quality while running **~5x faster**, beating MinerU and Docling on **score and throughput at once**.


> 🌐 **译文：**
> 开源 PDF 转 Markdown 解析器的正面交锋。**[Marker 2](https://pxllnk.co/c1pzvpb)** 在 olmOCR-bench 测试中获得 **76.0 分，速度为 2.9 页/秒**，与 Gemini/MinerU 的质量相当，运行速度**快约 5 倍**，在**得分和吞吐量**方面均胜过 MinerU 和 Docling。

**So what:** [Document parsing](https://pxllnk.co/c1pzvpb) is the silent failure point of most RAG stacks — bad extraction poisons everything downstream. Winning quality and speed simultaneously makes Marker 2 the new default front door for turning PDFs into clean model input.


> 🌐 **译文：**
> **所以呢：** [文档解析](https://pxllnk.co/c1pzvpb)是大多数RAG堆栈的隐形故障点——糟糕的提取会影响下游的所有环节。Marker 2兼顾质量和速度，使其成为将PDF转换为干净模型输入的全新首选方案。

----------~_sponsored_~

View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/047d8087-e0c1-4c81-8602-8f902e183899/600x50.png?t=1782465964)
Caption: 

----------
### **[Andrew Ng Releases OpenWorker: A Local-First Desktop AI Coworker](https://www.marktechpost.com/2026/07/23/andrew-ng-just-released-openworker-an-open-source-local-first-desktop-ai-coworker-that-returns-finished-deliverables-instead-of-chat/)**


> 🌐 **译文：**
> ----------

### **[吴恩达发布 OpenWorker：一款本地优先的桌面 AI 协作工具](https://www.marktechpost.com/2026/07/23/andrew-ng-just-released-openworker-an-open-source-local-first-desktop-ai-coworker-that-returns-finished-deliverables-instead-of-chat/)**

Andrew Ng released **[OpenWorker](https://github.com/andrewyng)**, an **MIT-licensed, local-first** desktop agent that **returns finished deliverables instead of chat** — a polished doc, a filled spreadsheet — working across **35 app connectors** while keeping data on your machine.


> 🌐 **译文：**
> Andrew Ng 发布了 **[OpenWorker](https://github.com/andrewyng)**，这是一个 **MIT 许可、本地优先** 的桌面代理，它**返回完成的交付物而不是聊天记录**——例如，一份完善的文档、一个填好的电子表格——它支持 **35 个应用程序连接器**，同时将数据保留在您的计算机上。

**So what:** The "chat with your AI" paradigm is giving way to "hand me the output." A local-first agent that produces deliverables — not turns — is a real bet on privacy plus autonomy, and open-sourcing it sets the template everyone else copies.


> 🌐 **译文：**
> 所以呢？“与AI对话”的模式正在被“把输出结果给我”的模式所取代。一个以本地为先、能够产出成果（而非回合）的智能体，是对隐私和自主性的真正押注，而将其开源则为其他人树立了效仿的模板。

----------

View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/8b8d904f-8ec2-4efe-b3f8-cca0cfbc1844/600x50.png?t=1782466130)
Caption: 

### **[Anthropic Ships Claude Opus 5: Frontier Agentic Coding at Unchanged Opus Pricing](https://www.marktechpost.com/2026/07/24/meet-the-new-claude-opus-5-frontier-class-agentic-coding-and-computer-use-at-unchanged-opus-pricing/)**


> 🌐 **译文：**
> ### **[Anthropic 推出 Claude Opus 5：前沿智能编码，Opus 定价不变](https://www.marktechpost.com/2026/07/24/meet-the-new-claude-opus-5-frontier-class-agentic-coding-and-computer-use-at-unchanged-opus-pricing/)**

Anthropic released **[Claude Opus 5](https://www.anthropic.com/news/claude-sonnet-5)**, its new frontier model tuned for **agentic coding and computer use** — and it holds **Opus pricing at $5 / $25 per million tokens**. It tops **[SWE-bench Verified](https://www.swebench.com/)**, extending Anthropic's lead on real terminal-based coding tasks.


> 🌐 **译文：**
> Anthropic 发布了其全新前沿模型 **[Claude Opus 5](https://www.anthropic.com/news/claude-sonnet-5)**，该模型专为**智能体编码和计算机应用**而设计，并将 **Opus 定价为每百万代币 5 美元/25 美元**。它超越了 **[SWE-bench 验证](https://www.swebench.com/)**，进一步巩固了 Anthropic 在基于真实终端的编码任务方面的领先地位。

**So what:** Frontier capability jumps while price holds flat — that's the whole story of this cycle. When each Opus generation gets meaningfully better at agentic coding without raising the meter, the economics of shipping software with an agent in the loop keep improving.


> 🌐 **译文：**
> 所以呢？前沿功能大幅提升，价格却保持不变——这就是本轮周期的全部意义所在。每一代 Opus 都能在不提高价格的情况下显著提升智能体编码能力，因此，采用智能体进行软件开发的经济效益会持续提升。

View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/9ccc034c-4793-412d-94f7-407d198dc1b7/600x50.png?t=1782766338)
Caption: 

### **[Build an Agentic Event-Venue Operator with MongoDB Atlas, Voyage & LangGraph](https://pxllnk.co/twdn5)**


> 🌐 **译文：**
> ### **[使用 MongoDB Atlas、Voyage 和 LangGraph 构建智能活动场地运营商](https://pxllnk.co/twdn5)**

A hands-on [build: a stateful agent that runs a venue-operations workflow end to end. ](https://pxllnk.co/twdn5)**[MongoDB Atlas](https://pxllnk.co/twdn5)**[ for data + vector search, ](https://pxllnk.co/twdn5)**[Voyage](https://pxllnk.co/twdn5)**[ embeddings for retrieval, and ](https://pxllnk.co/twdn5)**[LangGraph](https://pxllnk.co/twdn5)** to orchestrate the planning / tool-calling loop into a durable graph.


> 🌐 **译文：**
> 一个动手实践的[构建：一个有状态的代理，可以端到端地运行场地运营工作流。](https://pxllnk.co/twdn5)**[MongoDB Atlas](https://pxllnk.co/twdn5)**[用于数据和向量搜索，](https://pxllnk.co/twdn5)**[Voyage](https://pxllnk.co/twdn5)**[用于检索的嵌入，以及](https://pxllnk.co/twdn5)**[LangGraph](https://pxllnk.co/twdn5)**将规划/工具调用循环编排成一个持久图。

**So what:** A clean reference for the emerging ["database + embeddings + graph orchestration" agent stack](https://pxllnk.co/twdn5) — the pattern most production agents are quietly converging on.


> 🌐 **译文：**
> **所以呢：** 一个清晰的参考资料，用于新兴的[“数据库+嵌入+图编排”代理堆栈](https://pxllnk.co/twdn5)——大多数生产代理正在悄悄地向这种模式靠拢。

~_sponsored_~

View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/d61eb9e0-4977-4070-a150-19090a258559/600x50.png?t=1784188854)
Caption: 

### **[Best Open Speech-Recognition (ASR) Models in 2026: WER, Latency & License Compared](https://www.marktechpost.com/2026/07/23/best-open-speech-recognition-asr-models-in-2026-wer-languages-latency-and-license-compared/)**


> 🌐 **译文：**
> ### **[2026 年最佳开源语音识别 (ASR) 模型：词错误率、延迟和许可对比](https://www.marktechpost.com/2026/07/23/best-open-speech-recognition-asr-models-in-2026-wer-languages-latency-and-license-compared/)**

A practical roundup of the top open ASR models on **WER, languages, latency, and license**. NVIDIA's [**Parakeet RNNT 1.1B**](https://huggingface.co/nvidia/parakeet-rnnt-1.1b) tops the [**Open ASR Leaderboard**](https://huggingface.co/spaces/hf-audio/open_asr_leaderboard), beating Whisper large-v3 on average WER, with [**Canary 1B**](https://huggingface.co/nvidia/canary-1b) leading multilingual transcription + translation.


> 🌐 **译文：**
> 本文对各大开源ASR模型进行了实用性汇总，重点关注**WER、语言、延迟和许可**。NVIDIA的Parakeet RNNT 1.1B在Open ASR排行榜上名列榜首，平均WER优于Whisper large-v3，而Canary 1B在多语言转录和翻译方面领先。

**So what:** Open ASR has quietly caught and passed Whisper. If you're building voice agents, the right pick now hinges on the tradeoff table — WER vs latency vs language coverage vs license — not on "just use Whisper."


> 🌐 **译文：**
> 所以呢？Open ASR 已经悄然赶超 Whisper。如果你正在构建语音代理，现在正确的选择取决于权衡利弊——词错误率 (WER)、延迟、语言覆盖范围和许可协议——而不是“直接用 Whisper”。

View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/297b22c5-4b74-487d-be79-cf21211895e5/600x50.png?t=1783125675)
Caption: 

----------
### **$ ./partner --with us **

**# ****Reach 1M+ AI developers, researchers & builders.**
**# ****Sponsor a future issue of the Intelligence Brief.**
**>**** apply: **_**[forms.gle/CY1eqZzuWFQBp7dH9](https://forms.gle/CY1eqZzuWFQBp7dH9)**_


> 🌐 **译文：**
> **# ****触达超过 100 万 AI 开发者、研究人员和构建者。**

**# ****赞助未来一期的《智能简报》。**

**>****申请：**_**[forms.gle/CY1eqZzuWFQBp7dH9](https://forms.gle/CY1eqZzuWFQBp7dH9)**_

----------

----------
## **How was today’s email?**

### **[Awesome](mailto:asif@marktechpost.com?subject=Liked%20today%27s%20picks%3F&body=A%20lot%20%F0%9F%98%8D%0D%0A-%0D%0A*Have%2030%20seconds%3F%20Please%20Help%20us%20improve%3A*%0D%0A%0D%0A1.%20My%20favorite%20section%20of%20the%20email%20is%3A%0D%0A%0D%0A2.%20I%20would%20like%20to%20see%20more%20of%3A%0D%0A%0D%0A3.%20I%20would%20like%20to%20see%20less%20of%3A%0D%0A%0D%0A4.%20Is%20this%20your%20favorite%20newsletter%3F%0D%0A%0D%0A5.%20If%20not%2C%20who%20is%20and%20why%3F)****    |   ****[Decent](mailto:asif@marktechpost.com?subject=Liked%20today%27s%20picks%3F&body=Yes%20%F0%9F%99%82%0D%0A-%0D%0A*Have%2030%20seconds%3F%20Please%20Help%20us%20improve%3A*%0D%0A%0D%0A1.%20My%20favorite%20section%20of%20the%20email%20is%3A%0D%0A%0D%0A2.%20I%20would%20like%20to%20see%20more%20of%3A%0D%0A%0D%0A3.%20I%20would%20like%20to%20see%20less%20of%3A%0D%0A%0D%0A4.%20Is%20this%20your%20favorite%20newsletter%3F%0D%0A%0D%0A5.%20If%20not%2C%20who%20is%20and%20why%3F)****     |   ****[Not Great](mailto:asif@marktechpost.com?subject=Liked%20today%27s%20picks%3F&body=Not%20much%20%F0%9F%98%95%0D%0A-%0D%0A*Have%2030%20seconds%3F%20Please%20Help%20us%20improve%3A*%0D%0A%0D%0A1.%20My%20favorite%20section%20of%20the%20email%20is%3A%0D%0A%0D%0A2.%20I%20would%20like%20to%20see%20more%20of%3A%0D%0A%0D%0A3.%20I%20would%20like%20to%20see%20less%20of%3A%0D%0A%0D%0A4.%20Is%20this%20your%20favorite%20newsletter%3F%0D%0A%0D%0A5.%20If%20not%2C%20who%20is%20and%20why%3F)**


> 🌐 **译文：**
> ### **[Awesome](mailto:asif@marktechpost.com?subject=Liked%20today%27s%20picks%3F&body=A%20lot%20%F0%9F%98%8D%0D%0A-%0D%0A*Have%2030%20seconds%3F%20Please%20Help%20us%20improve%3A*%0D%0A%0D%0A1.%20My%20favorite%20section%20of%20the%20email%20is 2. 我希望看到更多 ADA 的内容。3. 我希望看到更少 ADA 的内容。4. 这是你最喜欢的电子报吗？5. 如果不是，你是谁？为什么？**** ****[Decent](mailto:asif@marktechpost.com?subject=Liked%20today%27s%20picks%3F&body=Yes%20%F0%9F%99%82%0D%0A-%0D%0A*Have%2030%20seconds%3F%20Please%20Help%20us%20improve%3A*%0D%0A%0D%0A1.%20My%20favorite%20section%20of%20the%20email%20is%3 A%0D%0A%0D%0A2.%20我希望看到更多%20A%0D%0A%0D%0A3.%20我希望看到更少%20A%0D%0A%0D%0A4.%20这是您最喜欢的简报吗？5.%20如果不是，请问您是谁？为什么？****    |   ****[不是太棒了](mailto:asif@marktechpost.com?subject=Liked%20today%27s%20picks%3F&body=Not%20much%20%F0%9F%98%95%0D%0A-%0D%0A*Have%2030%20seconds%3F%20Please%20Help%20us%20improve%3A*%0D%0A%0D%0A1.%20My%20favorite%20section%20of%20the%20email%20is 2. 我希望看到更多 A 的内容。3. 我希望看到更少 A 的内容。4. 这是你最喜欢的电子报吗？5. 如果不是，你是谁？为什么？

----------

———

You are reading a plain text version of this post. For the best experience, copy and paste this link in your browser to view the post online:
https://www.aidevsignals.com/p/this-week-the-big-three-ship-cisco-security-google-flash-nvidia-cosmos-3-edge-2


> 🌐 **译文：**
> 您正在阅读此文章的纯文本版本。为了获得最佳阅读体验，请复制此链接并粘贴到浏览器中以在线查看文章：

https://www.aidevsignals.com/p/this-week-the-big-three-ship-cisco-security-google-flash-nvidia-cosmos-3-edge-2