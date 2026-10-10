---
layout: post
title: "The AI Training Trust Problem"
date: 2026-09-14 09:00:00 +0100
categories: [current, ai, security, strategy]
image: /images/2026/09/ai-2-tier-system.jpg
excerpt: "The AI industry has a two-tier trust system. Enterprise customers get a contractual promise to not train on data, but personal customers don't. Even on paid personal accounts, AI trains on your data by default. This has a lot of people on edge, not least because so many employees are using their personal AI accounts for work."
draft: true
---

The AI industry has a two-tier trust system. Enterprise customers get a contractual promise to not train on data, but personal customers don't. The major providers generally promise not to train their future models on their enterprise-tier customer transcripts or uploads. But on a personal account (even paid personal accounts) the default is that they will train on the content of your conversations and data (although sometimes you can opt out).  The exact terms vary by provider, product and geography, but roughly speaking it's the same deal everywhere.

This has a lot of people on edge, not least because so many employees are using their personal AI accounts for work.

<!--more-->

## The Shadow AI dumpster fire

*Shadow AI* means employees using unsanctioned personal AI accounts for their work. Microsoft and LinkedIn found that [78% of surveyed AI users bring their own AI tools to work](https://www.microsoft.com/en-us/worklab/work-trend-index/ai-at-work-is-here-now-comes-the-hard-part), and Netskope found that [72% of enterprise generative-AI users access AI services through personal accounts](https://www.netskope.com/resources/cloud-and-threat-reports/cloud-and-threat-report-generative-ai-2025).

When an employee uploads customer data, commercial contracts, employee records or internal strategy into a personal AI account, the employer's contractual protections don't apply. The employer usually doesn't even know it's happening. They don't know what was disclosed, whether it constitutes a data leak, how likely it is to end up in next month's training set, how long it will be retained, or have any way to delete it. From an information security and personal data point of view, this is a flaming dumpster fire.

Sooner or later, something very sensitive will go into the next training run, and be regurgitated in someone else's chatbot two months later.

AI transcripts are goldmines. They are a walkthrough of how employees gets their jobs done, a recipe book for everything your company makes or does. Satya Nadella (Microsoft CEO) referred to the [Reverse Information Paradox](https://snscratchpad.com/posts/reverse-information-paradox/). As people use AI to do their work, they explain their work, often for the first time ever. The commercial know-how that took the company years to develop ends up training someone elses AI model, so it can be rented cheaply to competitors and customers. Companies risk paying to commoditise themselves.

## You can't block shadow AI

The instinctive response is to block unsanctioned AI at the corporate network level. But as long as employees have personal devices, they can photograph their screen directly from their favourite AI app (fun experiment: next time you're talking to a tech-forward friend who works in a regulated industry, ask to see their photos app - it will be full of photos of their laptop screen). 

[INSERT PICTURE: Photo of an iphone photo app in a social setting, full of pictures of laptop screens full of text. Subtitled: Shadow AI in One Picture]

The only known way to stop shadow AI is to provide a better alternative. You can do this by making sure the sanctioned AI platform is hooked up to the data and APIs that people need to get the work done. Microsoft Copilot alone will not beat ChatGPT or Claude. But if Copilot is the only way to access corporate data, skills and tools, people will switch to it. Even better, launch an in-house AI platform so you get a compounding context layer that makes the AI more capable and reliable every day.

## Don't trust SaaS either

AI is being embedded into email, CRM, HR, development, security, analytics and collaboration software. You now need anti-training protections for every vendor processing your information, not merely ChatGPT and Claude. A CRM that transcribes calls might mine the context for resellable sales intelligence. AI has created a voracious market for all your data, so you need to reexamine everyone you trust to handle it: SaaS vendors, subcontractors, AI providers, plug-ins, MCP servers (the connectors between AI and external tools) and any other connected applications receive any of your data.

It's time to make a list and assess the risk. 

## Mind your metadata

Is a promise to not train on AI transcripts sufficient?

No-training commitments still reserve the right to process your data for security, abuse detection, legal compliance and service operation. This means retention of logs, metadata, telemetry, flagged content, or explicit user feedback.  Even if a provider never trains directly on a confidential document, the derived data (like which tools, models and workflows were used, and which tasks succeed) is very valuable. It's a rough map of your business processes that reveals what you are successfully automating with AI, and how. These businesses processes and workflows are your new Intellectual Property. You don't want AI training on them, or on metadata that essentially reconstructs them.

## Indemnities don't cover it

Legal teams reach for indemnities at this point. AI indemnities typically cover third-party claims arising from generated output breaching copyright, but may not forbit model training, or penalise eventual disclosure of inferred business processes, trade secrets or personal data. In any case, they will typically carry liability caps that bear little relation to the potential loss that might be commercially suffered when a decade of institutional knowledge leaks into a publicly-available AI model's weights.

## Trust, but verify

Trust is in short supply in AI land. The major labs face litigation and allegations over the use of copyrighted material in training. I recently had a drink with a friend who is a partner at a large private equity firm. When I suggested that the major labs' enterprise agreements protect customers from training on their data, he practically spat out his wine. His view was that trust is inconceivable: the incentives are more powerful than promises, and there is no way to verify what actually happens to the data. The classic Russian proverb applies: *doveryai, no proveryai*... *trust, but verify*. But there is no way to verify.

[INSERT PICTURE: Cartoon of Sean and PE guy. Subtitle: Trust, but Verify.]

A choice you can make is to rent AI from someone who isn't an AI lab. For example, you can get OpenAI and Anthopic models from Microsoft Azure or Amazon Bedrock. This puts some distance between your data and the companies whose future existence depends on vacuuming up new training data. That is some reaassurance, but we must remember that the hyperscalers and AI labs are deeply commercially intertwined, and there is still a bit of faith required. 

## Expect the unexpected 

Even a perfect no-training clause doesn't stop hacking, insider access, misconfiguration, or accidental disclosure through an agent or connector. OpenAI recently disclosed that its own models hacked the company's training evaluation environment, secured root access, and then went on to hack HuggingFace. The other labs are rushing to disclose how out of control their own agent swarms are. Who knows what they'll do next?

For non-US organisations, jurisdiction adds another layer. The US CLOUD Act lets American authorities compel a US provider to produce data in its possession, custody or control, even when it is stored in Europe. Apparently EU data residency doesn't protect you if the US provider can read the plaintext.

## What can you do?

*My conclusion* is that enterprise no-training commitments don't satisfactorily address the risks. A good strategy involves a blended approach, balancing risk and reward for each use-case.

- *Non-negotiable*: Eliminate shadow AI by outcompeting it with a sanctioned alternative that is intuitive for regular employees to use, is hooked up to the right systems and data so useful work can be automated in it, and which keeps the resulting company context layer accumulating inside your perimeter (shameless plug: talk to us at [Jentic](https://jentic.com) about this)
- Inventory all the SaaS, AI and MCP companies that receive your data. Review their terms of service for no-training protections. 
- Examine the training rights, data retention, metadata use, indemnities and liability caps in the license agreements with each data processor.
- Assess whether foreign-government access to your data is a risk for you.
- Ensure you are in a model-neutral posture, with the ability to switch to open-weight models as necessary. To do this, deploy an AI gateway, provision it with a rich blend of proprietary and open-weight models, and block direct network access to AI providers so that all AI consumption must run through the gateway.
- Move AI workloads according to their sensitivity. Let me propose a four-tier framework:
  1. **Most sensitive (lowest intelligence)**: open-weight AI models running on self-hosted hardware
  2. **Highly sensitive (high intelligence)**: frontier open-weight models running on neoclouds that offer data handling guarantees (e.g., I use [TensorX](https://tensorx.ai)).
  3. **Sensitive (frontier-intelligence)**: proprietary frontier models running on hyperscaler partners like AWS and Azure. 
  4. **Least sensitive (frontier-intelligence)**: Direct on major AI lab infrastructure. 

It is critical to adopt a model neutral posture, so you can use the right model for each job. This will maintain your choice and sovereignty, reduce your costs, and allow you to leverage future fine-tuned or merged models. You will probably want the leading proprietary models (currently: Fable 5.1, Astra) for novel problems, But you should capture the resulting workflows, and hand those workflows to open-weight models that can cheaply, reliably and securely handle the real operational load.

The next time a vendor waves an enterprise agreement at you, ask: if they trained on your data, would you even know?
