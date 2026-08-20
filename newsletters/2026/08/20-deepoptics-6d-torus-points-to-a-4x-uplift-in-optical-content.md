# Deep|Optics: 6D Torus Points to a 4x Uplift in Optical Content per TPU

**来源：** FUNDA <fundaai@substack.com>  
**日期：** 2026-08-20  
**查看原邮件：** <https://mail.google.com/mail/u/1/#search/subject%3A%22Deep%7COptics%3A%206D%20Torus%20Points%20to%20a%204x%20Uplift%20in%20Optical%20Content%20per%20TPU%22>

---

Key takeaway

Supply-chain rumors suggest Google’s training-oriented TPU 9t might raise the torus dimensionality to 6D while retaining the torus architecture, with deployment targeted for 2027–2028. If realized, wrap-around optical ports per TPU on the scale-up side would rise from 1.5 (3D) to 6, a fourfold increase in OCS ports and optical module content per TPU; combined with the 800G→2.4T Coherent Lite speed and modulation upgrade, the value uplift would exceed 4x. This direction aligns with the two evolution paths we laid out in our earlier report.

> **译文：** 供应链传闻表明，谷歌面向训练的 TPU 9t 可能会在保留环面架构的同时，将环面维度提升至 6D，并计划于 2027-2028 年部署。如果实现，从规模化角度来看，每个 TPU 的环绕式光端口数量将从 1.5 个（3D）增加到 6 个，OCS 端口数量和每个 TPU 的光模块数量将增加四倍；结合 800G→2.4T 相干 Lite 的速度和调制升级，价值提升将超过 4 倍。这一方向与我们在之前的报告中提出的两条演进路径相符。

I. The Two Evolution Paths from Our Earlier Report

> **译文：** 一、我们之前报告中提到的两条演化路径

In Deep|AI Infra 2026, we argued that, in the agent era, the system bottleneck is shifting from single-chip compute to system-wide communication efficiency. MoE shifts the communication pattern from All-Reduce toward bisection-bandwidth-hungry All-to-All. Per the GShard paper, as experts scale from 128 to 2,048, All-to-All time for MoE dispatch/combine rises from 16% to 36% of MoE + Transformer layer execution time. On that basis, we expected Google to push along two lines:

> **译文：** 在 Deep|AI Infra 2026 大会上，我们指出，在智能体时代，系统瓶颈正从单芯片计算转向系统级通信效率。MoE 将通信模式从 All-Reduce 转向对带宽要求更高的 All-to-All。根据 GShard 的论文，随着专家数量从 128 个增加到 2048 个，MoE 调度/合并的 All-to-All 时间占 MoE + Transformer 层执行时间的比例从 16% 上升到 36%。基于此，我们预期谷歌会沿着以下两个方向发展：

Scale-out expansion: the number of in-rack TH6 switches rises from one to four–six per rack, DCN bandwidth up 4–6x, the scale-out OCS port ratio moves from 0.2:1 to 1:1, and the optical module ratio increases from 1:1–1:2 to 1:3–1:4;

> **译文：** 横向扩展：机架内 TH6 交换机的数量从每机架 1 台增加到 4 至 6 台，DCN 带宽提高 4 至 6 倍，横向扩展 OCS 端口比率从 0.2:1 提高到 1:1，光模块比率从 1:1 至 1:2 提高到 1:3 至 1:4；

Scale-up dimensionality: a 3D torus’s bisection bandwidth grows only as N^(2/3); assuming the torus architecture is retained, adding dimensions is the main practical route to higher bisection bandwidth, with the OCS Port-to-xPU ratio rising from 1.5:1 toward 2:1–10:1.

> **译文：** 扩展维度：3D 环面的二分带宽仅随 N^(2/3) 增长；假设保留环面架构，增加维度是提高二分带宽的主要实用途径，OCS 端口与 xPU 的比率从 1.5:1 上升到 2:1–10:1。

II. TPU 8t/8i and Virgo: How the Thesis Is Playing Out, Layer by Layer

> **译文：** 二、TPU 8t/8i 和 Virgo：论文逐层展开

Unsubscribe