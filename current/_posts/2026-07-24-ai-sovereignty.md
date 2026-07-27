---
layout: post
title: "What Do I Get to Own? (The Real Meaning of AI Sovereignty)"
date: 2026-07-24
categories: [ai, strategy, policy]
excerpt: "AI sovereignty is being used to mean six different things simultaneously. But strip them back and they all reduce to the same question."
draft: true
---

<lead>The phrase "AI sovereignty" is everywhere right now. To a European commissioner it means one thing. To a CISO it means something different. A graphic designer in Galway asking whether her livelihood is safe interprets something different again. A government minister in Paris, watching Washington pull the plug on a frontier model overnight, says "sovereignty" in a different way entirely. But they are all asking the same basic question: *what part of this future do I get to own?*</lead>

That question has five answers, one for each level at which AI is reshaping power. The same conversation, playing out at different scales.

---

## The personal: meaning, agency, dignity

If AI does the writing, the designing, the coding, the analysis, what is left? The Star Trek version is liberation from drudgery and freedom for more meaningful work. The honest answer is that we do not know yet, and the benefits may not be fairly distributed.

The wealth question is embedded in the dignity question. When intelligence gets industrialised and the returns flow to whoever owns the infrastructure, the rest of us are not merely inconvenienced, but are cut out. A small number of people are privatising intelligence itself (the one thing that has always been distributed roughly equally among humans) and building business models that rent it back to everyone else.

This is the defining political question of the next decade. Will ordinary people get to participate in the upside of AI, or merely have it happen to them? It likely depends on decisions being made right now, or perhaps on the decisions that aren't being made.

---

## The cultural: who writes the story?

Ireland is an interesting case study. Small, with a living but fragile minority language, and a long experience of its identity being flattened by a dominant anglophone culture. John Wayne in the Quiet Man still stings. No one likes someone else telling their story badly.

AI accelerates this risk in ways that are easy to overlook.

The Irish language problem starts with data quality. Academic research confirms that LLMs degrade low-resource languages not just through absence of training data but through poor quality training data: literal translations, beginner-level text, early machine translation output that encodes errors as norms. What gets baked into the model becomes the baseline. Generations of Irish speakers could end up learning from an AI that speaks a subtly wrong version of their own language, and never know it.

Then there is the archive question. Ireland has fifty years of broadcasting in the RTÉ archives, painstakingly digitized in an epic project at great taxpayer expense. It is an underused asset of enormous cultural value in the custody of a distressed semi-state. If it gets licensed to a foreign AI company for a one-time fee (the typical deal) it would become a perpetual source of "Irish" content under non-Irish control that pays no dividends to Ireland. Bloomsbury has already done a version of this with academic publishing. The BBC negotiated new frameworks under government pressure. The question of who owns the right to generate Irish cultural content is not rhetorical. The Irish government's AI Advisory Council (of which I was a member) [flagged this directly in its published recommendations](https://assets.gov.ie/static/documents/Irelands_AI_Advisory_Council_Recommendations_-_Helping_to_Shape_Irelands_AI_Future.pdf), calling for publicly-funded data to be treated as a protected national asset rather than a one-time licensing opportunity.

One obvious policy response is preferential licensing of public data to AI firms indigenous to, or conducting significant R&D within, Ireland or the EU. The UK's National Data Strategy implements a similar policy , but in the EU it runs straight into a legal wall. The EU's Open Data Directive came into effect shortly before generative AI broke out in 2022, effectively prohibiting member states from discriminating in favour of domestic firms when making public data available. European public data must be made freely available to any foreign AI company that wants it, on equal terms with domestic firms that don't yet exist at scale. The regulation meant to democratise data access is, in practice, preventing Ireland and Europe from using its own data strategically.

[Údarás na Gaeltachta](https://en.wikipedia.org/wiki/%C3%9Adar%C3%A1s_na_Gaeltachta) (roughly, the Irish state agency tasked with the defense of Irish language, regions and culture) takes this seriously, launching Ireland's first AI language benchmark leaderboard and a €1.2m initiative with TG4 to fund Irish-language digital media development. More than most low-resource language countries have managed, but unlikely to be enough.

This generalises beyond Ireland. Every small country, every minority culture, every low-resource language faces the same structural risk: the hegemony of AI-generated media regressing it to the mean of the training data, with the cost falls on the culture being erased.

---

## The corporate: you pay twice

This is where the stakes are most immediately tangible for anyone running a business.

Satya Nadella framed it clearly in July 2026 with what he called the [Reverse Information Paradox](https://snscratchpad.com/posts/reverse-information-paradox/). To make a foundation model genuinely useful, an enterprise must feed it their proprietary context, workflows, institutional knowledge, and continuous human corrections. He calls the byproduct "intelligence exhaust." Every prompt, every tool call, every corrected output subtly trains and refines the vendor's model. The enterprise pays for the service twice: first with money, and second with the institutional know-how that constitutes its competitive moat.

Alex Karp put it more bluntly on CNBC in July 2026:

> *"I am paying for tokens that create no value. These people are stealing the weights and alpha of my business, and they're creating a wealth tax that does not help the poor, it just punishes."*

Security researchers at OriginHQ demonstrated in 2026 that AI models can even reconstruct highly classified, unwritten internal corporate rules purely from the AI exhaust left behind by employees using a system over just a few weeks. The institutional intelligence of a business is visble to the LLM, reading between the lines of the prompts.

Imagine an insurance company automates its underwriting and claims processing using a rented AI. The AI learns the risk models, the edge cases, the pricing logic, the fraud patterns. At what point does the AI vendor have everything it needs to run an insurance company? At what point does the customer's continued subscription amount to funding the development of their own competitor? It's worth noting that Sequoia [identified insurance as their #1 target sector](https://sequoiacap.com/article/services-the-new-software/) for AI disruption.

This is called [platform envelopment](https://www.hbs.edu/faculty/Pages/item.aspx?num=38631), coined by Eisenmann, Parker and Van Alstyne in the *Strategic Management Journal* in 2011. A platform watches third parties prove demand in adjacent markets, then ships a native version and eliminates them. Microsoft did it to Netscape. Apple does it routinely to App Store developers. The third party funds the R&D; the platform holds the option.

At Demonware, we built multiplayer middleware for Xbox and PlayStation. When PlayStation Network launched, game studios had a free but inferior alternative built into the platform. Every feature we shipped from that point was effectively free R&D for Microsoft and Sony. Any breakthrough would be duplicated. That weighed on us, and it factored into our decision to sell to Activision when we did (where Demonware still runs Call of Duty online platform).

Salesforce launched [Agentforce for Financial Services](https://www.salesforce.com/news/stories/agentforce-for-financial-services-announcement/) in 2025, absorbing workflows that fintech companies had built on top of its own CRM platform. Alex Karp called out Anthropic by name, already moving into design, code, law, finance and life sciences. This isn't a future risk.

What was opportunistic in the 1990s is now deliberate. The major AI labs are under enormous pressure to justify their valuations, AI erodes the technical moats that previously made verticals defensible, and agent platforms can deploy skills at a scale no previous platform could match. Envelopment is no longer opportunistic, it's the intentional strategy. The lucrative verticals, insurance above all, should be paying attention.

And then there is the continuity question, which the corporate and national layers share.

---

## The national and continental: the kill switch

On 12 June 2026, the Trump administration issued an immediate export control directive restricting use of Anthropic's Fable and Mythos frontier model by non-US citizens. Anthropic disabled them globally for all customers within hours.

The models were eventually restored on 30 June after Anthropic agreed to a new pre-release government evaluation framework. Meanwhile OpenAI has offered to [sell a 5% stake to the US government](https://www.theguardian.com/technology/2026/jul/02/openai-stake-us-government-ai-sam-altman) if Anthropic, Google and Meta would do the same. The US government now appears to have defacto approval rights over commercial AI, may be on a path to partially nationalising its AI industry, and either way has demonstrated a willingness to abruptly foreign terminate access.

The [reaction was not calm](https://www.euronews.com/2026/06/13/wake-up-call-europe-reacts-to-anthropic-halting-access-to-its-fable-5-and-mythos-5-ai-mode). Bruno Retailleau, a senior French political figure:
> *"In the race for artificial intelligence, a nation that depends on others for its technology is a nation that can be unplugged overnight."*

The majority of Europe's effort is led from regulation lens, with the continental policy apparatus focused on the EU AI Act, which has nothing to say about protecting access to AI infrastructure or developing our own. The AI Act gives us an illusion of control. I was a member of Ireland's AI Advisory Council, and we had already identified this exposure in its [published recommendations](https://assets.gov.ie/static/documents/Irelands_AI_Advisory_Council_Recommendations_-_Helping_to_Shape_Irelands_AI_Future.pdf), explicitly flagging "*vulnerability to geopolitical risks, such as trade restrictions on US-based AI technologies*" as a core economic sovereignty concern. This risk was clearly telegraphed, but I think everyone was surprised by how quickly the US demonstrated its power.

The scale of Europe's economic dependency is massive. The [Draghi report](https://commission.europa.eu/topics/eu-competitiveness/draghi-report_en) discusses Europe effectively failed to embrace innovation during the last major disruption:
> "Europe largely missed out on the digital revolution led by the internet and the productivity gains it brought: in fact, the productivity gap between the EU and the US is largely explained by the tech sector."

Whatever European successes did emerge were quickly acquired by those US companies (for example, Deepmind is one of the top three global AI labs, and was founded and runs in the UK but was acquired by Google). As a result, Europe now substantially imports its digital infrastructure from US companies. The economic analysis firm [Asterès published a report](https://www.cigref.fr/from-technological-dependency-to-economic-capture-the-cost-of-cloud-software-services-inflation-to-europe) that find that Europe spends €330 billion on US cloud and software providers each year. This may soar as AI embeds itself in business across the continent.

Infrastructure is something you should build, not rent. Europe needs to find a way to redirect this spending into its own innovation, digital and AI infrastructure.

Europe has domestic AI companies that are leaning into this situation. Mistral AI has reached a $23 billion valuation and $400 million in Annual Recurring Revenue on the pitch "[you don't want anyone to turn off your systems](https://www.startupriders.com/p/mistral-growth-playbook)" and a [clearly stated mission of AI sovereignty](https://europe.mistral.ai/). Germany's Aleph Alpha [was acquired](https://cohere.com/blog/cohere-alephalpha-join-forces) by Canada's Cohere with funding from the Schwarz Group (owners of * Lidl*) who will provide cloud infrastructure to the combined entity, with the goal of providing sovereign alternative to US AI. This deal happened months after the announcement of the [Canada-Germany joint AI declaration and launch of their sovereign technology alliance](https://www.canada.ca/en/innovation-science-economic-development/news/2026/02/canada-and-germany-sign-ai-joint-declaration-and-launch-sovereign-technology-alliance.html), with both companies viewing "advanced technologies are central to economic security, competitiveness and democratic resilience".

The other dependency axis that Europe is only beginning to process is China. Mark Zuckerberg open-sourced the Llama model so that Meta wouldn't become a tenant on someone else's AI platform, openly citing tough lessons learned trying to run Facebook as an app in Apple's ecosystem. Meta couldn't win the AI race, so he changed the game so no one could win, so "[power isn't concentrated in the hands of a small number of companies](https://about.fb.com/news/2024/07/open-source-ai-is-the-path-forward/)" (thanks Mark!). For similar reasons, Chinese companies have picked up the baton, collectively continuing to pull the rug out from under proprietary AI with their open source models (most notably DeepSeek, Qwen, Kimi and Z.ai's GLM). These have now nearly closed the gap with closed-source AI, often with much better energy and cost efficiency.  Chinese AI now accounts for 30% of all global AI downloads, against 15.7% for US models. For now, this is a gift to every country that wants the option of running its own frontier-level AI.

However, there are strategic downsides to becoming dependent on continued gifts from China. Broad adoption of Chinese open-source LLMs has been described as "[infrastructure colonisation](https://www.cigionline.org/articles/chinese-ai-models-and-the-high-stakes-fight-for-ai-neutrality/)": distributing free AI that carries the ideological alignment with the Chinese Communist Party. An [Australian Strategic Policy Institute report](https://www.aspi.org.au/report/the-partys-ai-how-chinas-new-ai-systems-are-reshaping-human-rights/) found that Chinese AI "strengthen the CCP's ability to shape information, behaviour and economic outcomes at home and overseas". An LLM, it turns out, is an excellent way to productise political censorship and propaganda. There may be more subtle ways that LLMs might be trained to produce results in the context of hybrid warfare, producing specific output in response to specific triggers - an AI-era equivalent of "The Manchurian Candidate".

Even if you accept or mitigate the political bias in the training of the Chinese models, it would be foolish to expect continued access to the best of China's R&D spend. [Reuters reported](https://www.reuters.com/world/beijing-is-looking-curbing-overseas-access-chinas-top-ai-models-sources-say-2026-07-07/) that in early July the CCP called in its major AI labs to discuss placing tough export controls on advanced Chinese AI, due to angst about advanced AI like Anthropic's Mythos as a strategic cyberweapon, and the need for China to develop its own countermeasures in response. In a future where the most intelligent AI is restricted due to its offensive capabilities, then all counties that don't have their own are doubly disadvantaged: they remain strategically vulnerable to cyberattack from both sides, and structurally unable to even rent access the level of intelligence that will drive the future of the world's innovation across all sciences and engineering.

Europe, in short, will be cut out.

---

## The economic: who owns the supply chain?
Karl Marx argued that those who own the means of production control the economy. In an AI era, those who own the intelligence control both the economy and all future innovation. If AI replaces human knowledge work, power inevitably shifts to AI infrastructure. Wealth redistribution through middle-class wages slows down, more capital aggregates to the shareholders in the AI industry, and wealth inequality becomes more extreme.

Even Sam Altman acknowledges the danger. In 2025, he warned that "[*the balance of power between capital and labor could easily get messed up*](https://blog.samaltman.com/three-observations)." He has suggested giving all humans a personal compute budget, floated partially nationalising OpenAI, and [previously proposed](https://moores.samaltman.com/) an American public wealth fund to share the proceeds among US citizens.

The problem is that if the companies that own the AI aren't based in your economy, then you can't even tax them. The automation is purely extractive, replacing wealth redistribution through wages within your economy with AI fees that flow straight out of your economy. Unlike previous automation waves, AI doesn't primarily threaten low-wage routine work. It threatens the educated professional class — the very people who assumed they were safe. Programming, finance, law, analysis: the knowledge work that commands a premium. An [Anthropic study](https://www.anthropic.com/research/labor-market-impacts) found that workers in the most exposed occupations earn 47% more than those in unexposed jobs and are substantially more educated. Perhaps people will upskill, or perhaps they'll find that they can't outrun the rate that AI is improving at.

Governments could face a double blow: declining tax income from the highest-paid earners, at precisely the moment that job displacement drives demand for welfare, retraining and other public support.

In 2025, Eric Schmidt (former CEO/chairman of Google) answered a Stanford student's question about what countries not at the AI frontier should do. His answer ([clip on YouTube](https://youtu.be/bnRfQNqP37s?si=w0epntBMW4tf2ZM8&t=2429)):
>  "They'll have to face the fact that this is a rich country's game. Huge capital, lots of technically strong people, strong government support, right? There are two examples. There are lots of other countries that have all sorts of problems. They don't have those resources. They'll have to find a partner. They'll have to join with somebody else. "

Every country will have a unique set of mitigation strategies they can employ, but the time to start is now. For example, in Ireland:

- **Hosting AI.** Ireland already hosts the European operations of major cloud companies, has a supply chain capable of building and running data centers, with extensive transatlantic data connectivity.
- **Renewables.** Ireland has abundant potential for cheap renewable wind energy. AI is energy intensive, and AI data centers will be developed where cheap and abundant energy is available.
- **Climate.** Ireland's cool stable climate reduces cooling requirements in data centers.
- **Regulation.** Ireland sits within the EU regulatory framework, providing access to 450 million EU citizens, while remaining culturally and commercially close to the US, with traditionally commercially pragmatic approaches to regulatory enforcement.

Ireland's key challenge is developing its energy. Already, data centers consumed [23% of metered electricity in 2025](https://www.cso.ie/en/releasesandpublications/ep/p-dcmec/datacentresmeteredelectricityconsumption2025/keyfindings/), and Amazon abandoned a [€300M AI facility](https://www.irishtimes.com/ireland/2025/07/25/amazon-scraps-plan-for-dublin-plant-and-hundreds-of-jobs-over-failure-to-secure-power-supply/) adjacent to the M50 in north-west Dublin that same year for lack of power supply. When the planning decisions comes down to homes or data centers, home should always win. But a better answer is to develop the underlying energy infrastructure on all fronts, seizing the commercial opportunity to drive investment in renewable infrastructure, and secure a fundamental part of the AI supply chain within our economy (and to tax it!).

Physical hosting is the foundation, not the ceiling. Ireland needs to climb the stack: cloud operations, model deployment, security and compliance, liquid cooling, power electronics, grid optimisation, enterprise AI services - the parts of the supply chain that generate real margin and keep skilled jobs in the economy.

---

## participation not protectionism

Sovereignty is not about stopping AI. Any instinct to protect by closing it off is misguided. Ireland learned that before 1959 and has not forgotten it. The way forward is to insist on participation.

At every level (personal, cultural, corporate, national, continental, economic) the question is the same: what part of this are you building for yourself, and what part are you renting from someone who has a different set of interests? The people, companies, and countries that answer that question early, and make deliberate architectural choices rather than drifting into dependency, will be in a fundamentally different position in ten years.

Sovereignty is not granted. It is built. The only real question is whether you start before or after you needed it.

---

*I served on the Irish Government's AI Advisory Council. The Council's published recommendations, [Helping to Shape Ireland's AI Future](https://assets.gov.ie/static/documents/Irelands_AI_Advisory_Council_Recommendations_-_Helping_to_Shape_Irelands_AI_Future.pdf), are cited in this article. Several arguments here - particularly on data sovereignty, the RTÉ archive, and the EU Open Data Directive - draw on a working draft I co-authored that informed the Council's AI sovereignty section. That paper was never independently published; its more specific policy recommendations ran into the political constraints described above. The views expressed in this article are my own.*
