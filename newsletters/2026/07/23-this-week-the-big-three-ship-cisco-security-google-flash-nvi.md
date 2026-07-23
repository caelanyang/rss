# 📡 This Week: The Big Three Ship — Cisco Security, Google Flash, NVIDIA Cosmos 3 Edge

**来源：** Marktechpost AI  
**日期：** 2026-07-23  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22%F0%9F%93%A1%20This%20Week%3A%20The%20Big%20Three%20Ship%20%E2%80%94%20Cisco%20Security%2C%20Google%20Flash%2C%20NVIDIA%20Cosmos%203%20Edge%22>

---

View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/46f3d4ca-8206-4c67-8da1-0aefb52e5b1f/600x100.png?t=1782465050)
Follow image link: (https://pxllnk.co/q6nz845)
Caption: _**Together with Mistral AI**_

==Cisco releases security small language models that hunt bugs, Poolside ships an agentic-coding MoE, Google's Flash tier gets cheaper and a Cyber variant, and NVIDIA puts a world model on a robot.== ==Meet ==**[Voxtral: Mistral's full audio stack, built for voice agents](https://pxllnk.co/q6nz845)**


> **译文：** ==思科发布用于查找漏洞的安全小型语言模型，Poolside推出代理编码MoE，谷歌Flash层降价并推出网络安全版本，NVIDIA将世界模型应用于机器人。== ==介绍 ==**[Voxtral：Mistral为语音代理构建的完整音频堆栈](https://pxllnk.co/q6nz845)**


View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/50004ce3-2956-47e2-acdb-438c1620b1da/600x50.png?t=1782465583)
Caption: 

### **[Cisco Foundation AI Releases Antares-350M & 1B: Open Models That Localize Code Vulnerabilities](https://www.marktechpost.com/2026/07/21/cisco-foundation-ai-releases-antares-350m-and-1b-open-weight-models-that-localize-known-vulnerabilities-inside-real-codebases/)**


> **译文：** ### **[思科基金会人工智能发布 Antares-350M 和 1B：可定位代码漏洞的开放模型](https://www.marktechpost.com/2026/07/21/cisco-foundation-ai-releases-antares-350m-and-1b-open-weight-models-that-localize-known-vulnerabilities-inside-real-codebases/)**


Cisco Foundation AI open-sourced **[Antares-1B](https://huggingface.co/fdtn-ai/antares-1b)** and **[Antares-350M](https://huggingface.co/fdtn-ai/antares-350m)** — models that **pinpoint known vulnerabilities inside real codebases**, connecting CVE/advisory data to the exact vulnerable lines. They **run locally** and cut cost **up to 172x versus GPT-5.5** on a new localization benchmark. (**[Cisco blog](https://blogs.cisco.com/ai/introducing-antares-the-most-efficient-open-weight-ai-models-for-vulnerability-localization)**)


> **译文：** 思科基金会人工智能开源了 **[Antares-1B](https://huggingface.co/fdtn-ai/antares-1b)** 和 **[Antares-350M](https://huggingface.co/fdtn-ai/antares-350m)** 模型，这些模型能够**精确定位真实代码库中的已知漏洞**，并将 CVE/安全公告数据与具体的漏洞代码行关联起来。它们**可在本地运行**，并且在新的本地化基准测试中，与 GPT-5.5 相比，成本**最多可降低 172 倍**。（**[思科博客](https://blogs.cisco.com/ai/introducing-antares-the-most-efficient-open-weight-ai-models-for-vulnerability-localization)**）


**So what:** Vulnerability triage is high-volume, repetitive, and expensive on frontier APIs. A 350M model that localizes bugs locally at 1/172nd the cost makes continuous in-repo scanning the default — and open weights mean it runs where the code already lives.


> **译文：** **所以呢：**对于前沿 API 而言，漏洞分类工作量巨大、重复性高且成本昂贵。一个成本仅为 1/172 的 3.5 亿模型可以将漏洞本地化，从而使持续的仓库内扫描成为默认选项——而且开放权重意味着它可以在代码已存在的地方运行。


----------

----------View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/158fe355-f64c-4090-bc08-158edfbf4c27/600x50.png?t=1782465836)
Caption: 

----------
### **[Build an Agentic Event-Venue Operator with MongoDB Atlas, Voyage & LangGraph](https://pxllnk.co/twdn5)**


> **译文：** ----------

### **[使用 MongoDB Atlas、Voyage 和 LangGraph 构建智能活动场地运营商](https://pxllnk.co/twdn5)**


A hands-on [build: a stateful agent that runs a venue-operations workflow end to end. ](https://pxllnk.co/twdn5)**[MongoDB Atlas](https://pxllnk.co/twdn5)**[ for data + vector search, ](https://pxllnk.co/twdn5)**[Voyage](https://pxllnk.co/twdn5)**[ embeddings for retrieval, and ](https://pxllnk.co/twdn5)**[LangGraph](https://pxllnk.co/twdn5)** to orchestrate the planning / tool-calling loop into a durable graph.


> **译文：** 一个动手实践的[构建：一个有状态的代理，可以端到端地运行场地运营工作流。](https://pxllnk.co/twdn5)**[MongoDB Atlas](https://pxllnk.co/twdn5)**[用于数据和向量搜索，](https://pxllnk.co/twdn5)**[Voyage](https://pxllnk.co/twdn5)**[用于检索的嵌入，以及](https://pxllnk.co/twdn5)**[LangGraph](https://pxllnk.co/twdn5)**将规划/工具调用循环编排成一个持久图。


**So what:** A clean reference for the emerging ["database + embeddings + graph orchestration" agent stack](https://pxllnk.co/twdn5) — the pattern most production agents are quietly converging on.


> **译文：** **所以呢：** 一个清晰的参考资料，用于新兴的[“数据库+嵌入+图编排”代理堆栈](https://pxllnk.co/twdn5)——大多数生产代理正在悄悄地向这种模式靠拢。


----------~_sponsored_~

View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/047d8087-e0c1-4c81-8602-8f902e183899/600x50.png?t=1782465964)
Caption: 

----------
### **[Voxtral: Mistral's full audio stack, built for voice agents](https://pxllnk.co/q6nz845)**


> **译文：** ----------

### **[Voxtral：Mistral 为语音代理构建的完整音频堆栈](https://pxllnk.co/q6nz845)**


[Voxtral Transcribe](https://pxllnk.co/q6nz845) delivers the lowest word error rate of any transcription API. Speaker diarization, word-level timestamps, and context biasing across 13 languages, with recordings up to 3 hours per request. Need live audio? Voxtral Realtime streams sub-200ms, open-weights under Apache 2.0 and deployable on edge.


> **译文：** Voxtral Transcribe 拥有所有转录 API 中最低的词错误率。它支持 13 种语言的说话人分割、词级时间戳和上下文偏好，每次请求最多可处理 3 小时的录音。需要实时音频？Voxtral Realtime 提供低于 200 毫秒的流传输，采用 Apache 2.0 开源协议，并可部署在边缘设备上。


[Try Voxtral now](https://pxllnk.co/q6nz845)

----------~_sponsored_~

View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/8b8d904f-8ec2-4efe-b3f8-cca0cfbc1844/600x50.png?t=1782466130)
Caption: 

### **[Poolside Releases Laguna S 2.1: A 118B Agentic-Coding MoE](https://www.marktechpost.com/2026/07/21/poolside-releases-laguna-s-2-1/)**

Poolside shipped **[Laguna S 2.1](https://poolside.ai/blog/introducing-laguna-s-2-1)**, a **118B-total-parameter MoE** with **8B activated per token** and a long context window, built for **agentic coding**. It joins the lighter **[Laguna XS 2.1](https://huggingface.co/poolside/Laguna-XS-2.1)** (33B/3B), both available via Poolside's API and on **OpenRouter**.


> **译文：** Poolside 发布了 **[Laguna S 2.1](https://poolside.ai/blog/introducing-laguna-s-2-1)**，这是一个 **总参数量为 1180 亿的 MoE**，**每个 token 可激活 80 亿个参数**，并具有较长的上下文窗口，专为 **代理编码** 而构建。它与更轻量级的 **[Laguna XS 2.1](https://huggingface.co/poolside/Laguna-XS-2.1)**（330 亿/30 亿）一起，可通过 Poolside 的 API 和 **OpenRouter** 获取。


**So what:** The coding-model field is splitting into a purpose-built agentic tier — sparse MoEs tuned for the plan/edit/test loop, not one-shot completion. 8B active from 118B total is the efficiency bet: frontier coding behavior at mid-tier serving cost.


> **译文：** **所以呢：**编码模型领域正在分裂成一个专门构建的代理层——稀疏的模型单元（MoE），针对计划/编辑/测试循环进行优化，而非一次性完成。1180亿总数中活跃的80亿是效率的体现：以中等服务成本实现前沿编码行为。


View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/9ccc034c-4793-412d-94f7-407d198dc1b7/600x50.png?t=1782766338)
Caption: 

### **[Google Releases Gemini 3.6 Flash, 3.5 Flash-Lite & 3.5 Flash-Cyber](https://www.marktechpost.com/2026/07/21/google-releases-gemini-3-6-flash-3-5-flash-lite-and-3-5-flash-cyber-a-cheaper-more-token-efficient-flash-tier-built-for-agentic-workloads/)**


> **译文：** ### **[谷歌发布 Gemini 3.6 Flash、3.5 Flash-Lite 和 3.5 Flash-Cyber](https://www.marktechpost.com/2026/07/21/google-releases-gemini-3-6-flash-3-5-flash-lite-and-3-5-flash-cyber-a-cheaper-more-token-efficient-flash-tier-built-for-agentic-workloads/)**


Google refreshed the Flash tier for agentic workloads. [**Gemini 3.6 Flash**](https://deepmind.google/models/gemini/flash/) cuts **output token usage ~17% vs 3.5 Flash** (up to **65% on some benchmarks**) at lower cost, alongside a lighter **3.5 Flash-Lite** and a security-focused **3.5 Flash-Cyber**. ([**Google blog**](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5/))


> **译文：** Google 更新了用于智能体工作负载的 Flash 层。[**Gemini 3.6 Flash**](https://deepmind.google/models/gemini/flash/) 相比 3.5 Flash，**输出令牌使用量减少了约 17%**（在某些基准测试中甚至减少了高达 65%），且成本更低。此外，Google 还推出了更轻量级的 **3.5 Flash-Lite** 和专注于安全的 **3.5 Flash-Cyber*。（[**Google 博客**](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5/)）


**So what:** For agents, token efficiency is the cost curve — a 17–65% cut in output tokens compounds across every multi-step run. A dedicated Cyber variant also signals security is becoming its own model track, not a fine-tune afterthought.


> **译文：** **所以呢：**对于代理而言，代币效率就是成本曲线——每次多步骤运行中，输出代币减少 17% 到 65% 都会累积影响。专门的网络安全变体也表明，安全性正在成为其自身的模型方向，而不是事后微调的附属品。


View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/d61eb9e0-4977-4070-a150-19090a258559/600x50.png?t=1784188854)
Caption: 

### **[NVIDIA Releases Cosmos 3 Edge: A 4B Open World Model That Runs Robot Actions On-Device](https://www.marktechpost.com/2026/07/21/nvidia-releases-cosmos-3-edge-a-4b-parameter-open-world-model-that-reasons-and-generates-robot-actions-on-device/)**


> **译文：** ### **[NVIDIA 发布 Cosmos 3 Edge：一款可在设备端运行机器人动作的 4B 开放世界模型](https://www.marktechpost.com/2026/07/21/nvidia-releases-cosmos-3-edge-a-4b-parameter-open-world-model-that-reasons-and-generates-robot-actions-on-device/)**


A **4B-parameter open world-action model (WAM)** that **reasons over a scene and generates robot actions on-device**, in real time. It runs at **robot-control resolution (640×360)**, ships on **ROS 2**, with [**weights on Hugging Face**](https://huggingface.co/nvidia/Cosmos3-Edge) and a full [**technical report**](https://research.nvidia.com/labs/cosmos-lab/cosmos3/technical-report.pdf). ([**launch blog**](https://huggingface.co/blog/nvidia/cosmos3edge))


> **译文：** 这是一个**4B参数开放世界动作模型（WAM）**，能够**对场景进行推理并在设备上实时生成机器人动作**。它以**机器人控制分辨率 (640×360)**运行，基于**ROS 2**，并附有[**Hugging Face上的权重**](https://huggingface.co/nvidia/Cosmos3-Edge)和完整的[**技术报告**](https://research.nvidia.com/labs/cosmos-lab/cosmos3/technical-report.pdf)。（[**发布博客**](https://huggingface.co/blog/nvidia/cosmos3edge)）


**So what:** Physical AI's bottleneck is latency — a robot can't wait on a cloud round-trip to decide its next move. A 4B world model that reasons and acts locally at control resolution is the shape of edge robotics: perception-to-action in one on-device model.


> **译文：** **所以呢？**物理人工智能的瓶颈在于延迟——机器人无法等待云端往返数据来决定下一步行动。边缘机器人技术的核心在于构建一个能够以控制分辨率进行本地推理和行动的4B世界模型：在单一设备端模型中实现从感知到行动的整个过程。


View image: (https://media.beehiiv.com/cdn-cgi/image/fit=scale-down,format=auto,onerror=redirect,quality=80/uploads/asset/file/297b22c5-4b74-487d-be79-cf21211895e5/600x50.png?t=1783125675)
Caption: 

----------
### **$ ./partner --with us **

**# ****Reach 1M+ AI developers, researchers & builders.**
**# ****Sponsor a future issue of the Intelligence Brief.**
**>**** apply: **_[**forms.gle/CY1eqZzuWFQBp7dH9**](https://forms.gle/CY1eqZzuWFQBp7dH9)_

----------

----------
## **How was today’s email?**

### **[Awesome](mailto:asif@marktechpost.com?subject=Liked%20today%27s%20picks%3F&body=A%20lot%20%F0%9F%98%8D%0D%0A-%0D%0A*Have%2030%20seconds%3F%20Please%20Help%20us%20improve%3A*%0D%0A%0D%0A1.%20My%20favorite%20section%20of%20the%20email%20is%3A%0D%0A%0D%0A2.%20I%20would%20like%20to%20see%20more%20of%3A%0D%0A%0D%0A3.%20I%20would%20like%20to%20see%20less%20of%3A%0D%0A%0D%0A4.%20Is%20this%20your%20favorite%20newsletter%3F%0D%0A%0D%0A5.%20If%20not%2C%20who%20is%20and%20why%3F)****    |   ****[Decent](mailto:asif@marktechpost.com?subject=Liked%20today%27s%20picks%3F&body=Yes%20%F0%9F%99%82%0D%0A-%0D%0A*Have%2030%20seconds%3F%20Please%20Help%20us%20improve%3A*%0D%0A%0D%0A1.%20My%20favorite%20section%20of%20the%20email%20is%3A%0D%0A%0D%0A2.%20I%20would%20like%20to%20see%20more%20of%3A%0D%0A%0D%0A3.%20I%20would%20like%20to%20see%20less%20of%3A%0D%0A%0D%0A4.%20Is%20this%20your%20favorite%20newsletter%3F%0D%0A%0D%0A5.%20If%20not%2C%20who%20is%20and%20why%3F)****     |   ****[Not Great](mailto:asif@marktechpost.com?subject=Liked%20today%27s%20picks%3F&body=Not%20much%20%F0%9F%98%95%0D%0A-%0D%0A*Have%2030%20seconds%3F%20Please%20Help%20us%20improve%3A*%0D%0A%0D%0A1.%20My%20favorite%20section%20of%20the%20email%20is%3A%0D%0A%0D%0A2.%20I%20would%20like%20to%20see%20more%20of%3A%0D%0A%0D%0A3.%20I%20would%20like%20to%20see%20less%20of%3A%0D%0A%0D%0A4.%20Is%20this%20your%20favorite%20newsletter%3F%0D%0A%0D%0A5.%20If%20not%2C%20who%20is%20and%20why%3F)**

----------

———

You are reading a plain text version of this post. For the best experience, copy and paste this link in your browser to view the post online:
https://www.aidevsignals.com/p/this-week-the-big-three-ship-cisco-security-google-flash-nvidia-cosmos-3-edge


> **译文：** 您正在阅读此文章的纯文本版本。为了获得最佳阅读体验，请复制此链接并粘贴到浏览器中以在线查看文章：

https://www.aidevsignals.com/p/this-week-the-big-three-ship-cisco-security-google-flash-nvidia-cosmos-3-edge
