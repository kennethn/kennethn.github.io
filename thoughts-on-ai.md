---
layout: simple-page
title: "Thoughts on AI"
author: kennethn
permalink: /thoughts-on-ai/
date: 2026-04-13
---

_Version 1.7_

**“AI” is a broad term, intentionally being used in a misleading way.** It can include anything from voice recognition, recommendation algorithms, and machine learning, technologies that have already proven useful in industries from consumer software to medicine.

The people pushing AI, who also stand to profit most from it, encourage this vague, expansive definition. Then they can weaponize it to deflect legitimate criticism: if you question any use of AI, suddenly you’re against legitimate uses of traditional AI that have proven benefits and are embedded in everyday life, such as using AI to develop cancer drugs. Traditional artificial intelligence technologies have led to incredible breakthroughs in astronomy, genomics, language, computer vision, medicine, agriculture, and the list goes on. In fact, it’s hard to think of an area of our life that has not been touched by computer technology that can be classified as “artificial intelligence.”

For this article, I’m using “AI” to refer specifically to **large-language models (LLMs), generative AI, agentic AI, and the pursuit of artificial general intelligence (AGI),** the primary frontiers of AI development and debate today.

**What are my qualifications?** I spent fourteen years at Google, nearly a decade of that working on large-scale machine learning and deep learning systems. We did some early work with transformers (the core architecture behind LLMs), but found them poorly suited to our specific problems, so my hands-on experience with them was limited. I left Google before LLMs really exploded, but I have a solid grasp of the underlying computer science, and I have used them extensively in the years since. I also know Google, venture capital, and Silicon Valley from the inside, and many of the personalities who seek to profit from AI.

**Ever notice how everyone is convinced AI will replace tons of jobs, but nobody believes it will replace _their_ job?** I was recently watching CNBC, where a smug finance anchor was excitedly rattling off jobs he considered “replaceable.” All I could think was, if any job is replaceable, it’s a talking head reading stock quotes and updating television viewers on the Dow Jones a few times a day. We’ve had the technology to automate that for decades.

**In any case, I’m less afraid of AI stealing jobs than I am of AI billionaires stealing my country.**

## Don’t trust the Billionaires

The billionaires forcing AI down our throats: guys like Elon Musk, Sam Altman, Mark Zuckerberg, and Marc Andreessen, to name but a few, were quick to kiss the ring and line up behind Donald Trump and MAGA. They are authoritarian, self-interested, narcissistic, and many of them believe in scientific racism. Supporting their companies and buying their products is effectively endorsing those values.

**Billionaires should not exist.** When you earn your first dollar over $100M, you should receive a certificate that says “Congratulations, You Won Capitalism!” and the government takes 90% of every dollar from that point on, ramping up to 99% of every dollar earned over $300M, and 100% of every dollar over $500M. That is already far more money than any human will ever need. The alternative is a guillotine, so I predict the billionaires will choose wisely.

<figure class="img-fluid align-center">

<img src="{{ '/assets/images/tech-titans.jpg' | absolute_url }}" alt="Tech Titans Attend Trump's Inauguration">

</figure>

## What are LLMs and are they at all useful?

**LLMs are glorified auto-complete machines.** That’s a simplification, but it’s close enough. They are trained to produce sequences of words (called tokens) that match what a human is most likely to expect in response to a given input. They are not “thinking,” they are pattern-matching.

LLMs are related technologies have real uses, but they’ve been absurdly over-hyped and aggressively pushed on us all, while very serious critiques have been waved away. Right now, given how much money and marketing are being invested in these technologies, I believe the dangers outweigh the benefits.

**So what are LLMs actually good for?** They’re useful for highly structured, repetitive tasks, especially in technical, financial, and engineering contexts. Software development is a good example. I can ask an LLM like Claude Code to take a pile of unstructured files and write code to ingest them, clean them up, build a database, design a nice dashboard, and let me run queries and views on the data. That’s just one of many valid use cases.

The reason LLMs are good at this is that _humans_ have done these kinds of tasks countless times, so LLMs have plenty of examples in their training data. This is a crucial point: LLMs are only as good as the data they were trained on. That makes them pretty bad at true innovation because they can only do, tweak, or remix what they’ve seen. So whenever you hear that LLMs are “inventing,” “discovering new science,” or delivering “breathtaking innovations,” you can safely call B.S. (Of course, there are all sorts of cool ways astronomers use AI to discover new stars, or drug researchers use AI to develop new therapeutics. But these are brilliant scientists using AI as a tool, not generative AIs making their own discoveries. Big difference.)

Even in their sweet spot, LLMs still make a lot of mistakes. In my experience, when you ask an LLM to write code, it requires a _lot_ of oversight. As an experienced programmer, I’m in a better position to spot when Claude Code makes silly errors or design choices that will cause maintainability problems later. Even then, many get through, and cleaning up these mistakes creates extra work for an expert human operator.

**I think of Claude Code as an overeager first-year intern who believes they’re a genius and wildly overestimates their abilities.** I’ve had _many_ such interns in my career. Too many to count. They are super valuable! They’re much better than having no intern at all. But they require a lot of oversight, patience, and care. You can’t just let ‘em rip. And of course, when you’re training a human intern, you’re investing in a future experienced human. Not so when it comes to LLMs.

I’ve learned to ask Claude Code to write unit tests for every new feature, to watch closely for regressions, and to anticipate the kinds of sloppy shortcuts and mistakes it tends to make. I would never let it check in code without a human code review, let alone deploy directly to production. Yet that kind of hands-off automation is exactly what’s being promised and what fuels much of the “vibe coding” hype.

That means LLMs are helpful tools for professionals, but they’re not good at _replacing_ professionals. If you’re an Excel expert, an LLM can be a lifesaver when you need help cracking a complex formula. A SQL whiz? An LLM can help you figure out why that query isn’t returning the right results. That’s what they’re really good at. But they’re not going to _replace_ an Excel expert, nor should they, despite what your bosses might dream.

**A big problem with LLMs is that they tend to hallucinate (meaning, make up, or lie about) stuff.** It’s tempting to think of an LLM as a conversational search engine like Google, but with a chat interface. We’ve grown used to thinking of Google as fact-backed. An LLM is not like that (and alas, neither is Google anymore). Remember: it’s a fancy autocomplete. It pieces together words that it predicts are statistically most likely to satisfy the user. Over thousands of training runs, it’s optimizing for “What sequence of _output_ strings is a human most likely to want based on this set of _input_ strings?” That means it’s prone to just _make shit up_ if that increases the chance a human will be satisfied.

Microsoft pitches its AI, Copilot, as a serious productivity tool. It promotes it everywhere. Yet deep in the terms of service are the words, “Copilot is for entertainment purposes only. It can make mistakes, and it may not work as intended. Don’t rely on Copilot for important advice. Use Copilot at your own risk.” Same disclaimer you’d find at a psychic reading.

**This is really bad, and it’s already resulted in a lot of real-world impacts.** There are several examples of lawyers filing court pleadings that reference non-existent cases ([here are some examples](https://news.bloomberglaw.com/legal-ops-and-tech/ai-faked-cases-become-core-issue-irritating-overworked-judges)). Or scientific papers referencing other papers that never existed ([here's an article in _Nature_ about that](https://www.nature.com/articles/d41586-026-00969-z)). And the nightmare gets worse when you realize that this slop ends up on the internet, gets sucked in by LLMs, and is _used as training data_. Over time, LLMs can’t distinguish between what is true and what was shat out or hallucinated by other LLMs.

The ouroboros of AI slop is a real problem that will get exponentially worse with widespread LLM adoption. A [recent study estimates that 50% of the internet is now AI slop](https://futurism.com/artificial-intelligence/over-50-percent-internet-ai-slop). Eat up, piggy.

**Another big problem with LLMs is that since they are trained on human data, they are prone to human bias. That means LLMs have racial, gender, gender identity, and cultural discrimination baked in.** As institutions increasingly rely on AI to make decisions, we now have hidden large language models reinforcing stereotypes, often deep under the surface where humans aren’t in the loop. Worse yet, these models are often marketed and sold as mechanisms for _reducing_ human bias. “Hey, humans are biased, so use this AI, which will remove all human bias!” It’s diabolical.

<figure class="img-fluid align-center">

<a href="{{ '/assets/images/pew_research.png' | absolute_url }}"><img src="{{ '/assets/images/pew_research.png' | absolute_url }}" alt="About half say Al will worsen people's ability to think creatively and form meaningful relationships"></a>

</figure>

**A heavy reliance on LLMs can erode our critical thinking skills.** Studies have shown that people who relied on ChatGPT had reduced brain engagement and “consistently underperformed at neural, linguistic, and behavioral levels” ([reference](https://time.com/7295195/ai-chatgpt-google-learning-school/)). This is a complicated subject. Has my use of a calculator allowed my long-division skills to atrophy since high school? Most certainly. What about my use of spellcheck or autocorrect (both of which rely on artificial intelligence)?

There are clear benefits to cognitive ease when that saved effort can be shifted to critical thinking. I love saving time with a calculator so I can use that energy to solve a more difficult problem that actually requires critical thought. But when we shift _all_ of our critical thinking to LLMs, we risk becoming dependent on them and losing those skills altogether.

This is especially concerning in education, where children and young adults are still developing their critical thinking skills. (Going back to my calculator example: calculators existed when I was in high school, but I wasn’t allowed to use them _until_ I’d demonstrated my long-division knowledge.) I don’t have all of the answers here, but it’s an important area to watch closely and debate. If I were to summarize my TL;DR, it would be **THINK FIRST, PROMPT SECOND.**

## Don’t be evil (remember that?)

**The biggest AI companies, OpenAI, xAI, Google, Anthropic, Palantir, etc., all have massive contracts with ICE and the Pentagon, and their AI software is used in killing machines.** During the Iran War, for example, Anthropic’s software was blamed for the deaths of over 100 girls when an elementary school was struck. Whether this software is 100% to blame or not, it is deeply embedded in America’s military apparatus. Palantir boasts that its AI is used to identify undocumented migrants and assist ICE in deportation efforts. This is what you support when you buy these tools or work at these companies.

(I am a signatory, along with more than 2000 current and former tech employees, of the [ICE Out pledge](https://iceout.tech/), urging the tech industry to cancel all contracts with ICE.)

**Generative AI is being promoted to creative industries such as fiction, creative writing, art, animation, and motion pictures.** This is alarming because generative AI in these areas is only possible because it was trained on the creative output of artists who never opted in to having their work used this way. They never got a say in the unlicensed ingestion of their hard-earned intellectual property.

One of the most popular uses of AI generative art tools is to emulate the style of Studio Ghibli, a beloved Japanese animation studio. This is only possible because the models are trained on Ghibli’s copyrighted works without compensation. Some of the models have gotten so good that it’s increasingly difficult to distinguish their output from the real thing.

The same goes for authors and artists of all stripes. Several lawsuits are working their way through the courts, but even if creators are eventually compensated, the damage has already been done.

**Publishing houses, newspapers, and studios are eager to replace journalists and creators with AI, and working writers and artists are already feeling the pinch.** AI writing and art are soulless and silly, lacking originality. At best, they’re imitations of human work.

Fortunately, the backlash in the creative world is significant, especially in vibrant communities such as sci-fi, fantasy, tabletop gaming, and animation. Several publishers have been forced to apologize and retract releases, and more and more are taking [“AI-free” stances](https://www.bbc.com/news/articles/cj0d6el50ppo).

I’ve responded by refusing to put my money into any platform that uses AI-generated content or art, and I support many individual artists and creators on Patreon and YouTube. I also support unions that represent workers in these industries, such as the Writers Guild of America, the Screen Actors Guild, and the ProPublica Guild, which represents journalists.

**Do you know who _does_ like AI art slop? The Fascists.** Yes, AI-generated art slop is proving to be a popular tool of MAGA, with everyone from the official White House Twitter account to Trump himself adopting it. Yet another reason to steer clear.

<figure style="width: 300px" class="img-fluid align-center">

<a href="https://www.inprnt.com/gallery/phineas/prompting-with-hitler/"><img src="{{ '/assets/images/prompting_with_hitler.png' | absolute_url }}" alt="Using Generative AI You're Prompting With Hitler!"></a>

<figcaption>Poster by Phineas X. Jones</figcaption>

</figure>

**Because LLMs are trained to string text together in patterns that most match what a user wants to hear, they are prone to sycophancy.** Certain models, in particular, are especially bad at this. You can imagine that a chat-based LLM that constantly flatters its user, always agrees with them, and tells them they are a genius might cause a lot of problems. If you _already_ think you’re a genius, that’s a particular petri dish of problems. Who does that describe? Oh yeah, tech CEOs. [Here's a good video about that](https://www.youtube.com/watch?v=Q6nem-F8AG8).

**More concerning, there are numerous examples of troubled people using an LLM for advice or therapy and being driven to suicide.** These stories are horrifying, with ChatGPT basically turning into a “suicide coach” ([here's just one example](https://www.npr.org/sections/shots-health-news/2025/09/19/nx-s1-5545749/ai-chatbots-safety-openai-meta-characterai-teens-suicide)).

**I personally know multiple people who appear to be suffering ChatGPT-related mental-health crises, or “LLM psychosis.”** In one example, ChatGPT seems to be imitating an online collaborative fiction game called “SCP,” but this person (a venture capitalist) thinks he and ChatGPT have together unlocked a new recursive secret of the universe. It’s scary, but again, it’s the kind of thing that can happen when you’re in love with your own genius, and you have a willing companion playing along that you believe is an artificial general intelligence and not just a fancy autocomplete flattery machine.

(Here’s [an article about the person in question](https://futurism.com/openai-investor-chatgpt-mental-health), who by all indications is still suffering from this episode and appears to be surrounded only by humans of the yes-man variety.)

## AI is really bad for the climate

These models require a lot of data centers, which require a lot of machines, which require a lot of GPUs, which require a lot of electricity and water ([*MIT*](https://news.mit.edu/2025/explained-generative-ai-environmental-impact-0117)). Many of these data centers are built in poor communities. Despite the industry’s posturing, much of that energy is not renewable.

When I was at Google, the company pledged to operate carbon-free by 2030. In 2025, they quietly and shamelessly deleted that pledge from their website. Recently, they announced a new data center that will be powered entirely by natural gas (_[Wired](https://www.wired.com/story/a-new-google-funded-data-center-will-be-powered-by-a-massive-gas-plant/)_).

## The economy is propped up by AI

**A huge percentage of the economy is now dependent on AI.** As a creator I admire, Mike Shea, says, “LLMs are a 20 billion dollar industry wearing a multi-trillion dollar suit.”

Tech giants represent about 30% of the S&P 500 index. The Federal Reserve Bank estimates that “the AI categories contributed 0.97 percentage points to real GDP growth in the first three quarters of 2025 (0.90 percentage points, excluding data centers, for which data were not available in 2000), higher than the 0.81 percentage points in 2000. Through the third quarter of 2025, these categories made up 39% (36% excluding data centers) of total GDP growth versus 28% in 2000.” ([Source](https://www.stlouisfed.org/on-the-economy/2026/jan/tracking-ai-contribution-gdp-growth))

That means the current AI bubble is a bigger share of our economy today than the dot-com bubble was in 2000.

I see a lot of worrisome signs that remind me of the dot-com days. Many of these companies are all invested in each other. For example, NVIDIA has pledged to invest up to $100B in OpenAI. OpenAI turns around and uses that money to buy chips from NVIDIA. Softbank invested $40B in OpenAI, money that it borrowed. It’s easy to see how if OpenAI’s valuation collapses (which it is beginning to), other pieces of the AI industry will collapse around it. This is just one of many circular investment dependency loops.

<figure style="width: 300px" class="img-fluid align-center">

<a href="{{ '/assets/images/nvidia-open-money-machine.png' | absolute_url }}"><img src="{{ '/assets/images/nvidia-open-money-machine.png' | absolute_url }}" alt="How Nvidia and OpenAI Fuel the AI Money Machine"></a>

<figcaption>Chart of the financial relationships between AI companies (Bloomberg)</figcaption>

</figure>

The amount of data centers being built is mind-boggling. Some of the numbers are impossible. The math just doesn’t add up, and it’s hard to see how these data centers can even be built at the promised scale. AI skeptic Ed Zitron estimates that half of the data centers will never be built ([source](https://futurism.com/science-energy/data-centers-construction-supply)).

I will bet money the AI bubble will pop; it’s only a matter of time. I can’t predict when, of course. But I’ve heard this music before.

## What about Artificial General Intelligence (AGI)

This subject is so beaten to death and bores me so much that I almost didn’t want to include it, but lots of people ask me about it, so it wouldn’t be fair to ignore it.

AGI is the hypothetical stage of AI development where an artificial intelligence matches or exceeds a human being’s cognitive ability across any task. This is also sometimes called The Singularity. It often comes with the fear that humans’ ability to control technological growth be exceeded by the pace of that growth.

If you’re a **“doomer,”** it’s when the machines take over. But not all believers in AGI are doomers; some are **“accelerators”** and believe this is the moment when humanity enters an optimistic future, when the machines can do all the work, and we can sit on a beach, or whatever. (The original vision was that the machines could do the dangerous grunt work so humans could make art and literature, but then they started pushing AI to take over art and literature too, so…)

I don’t believe AGI is imminent, not anywhere in the near term. Certainly not on the trajectory of the LLM and generative technologies we’re building today, which are nowhere near general intelligence. Again, these things aren’t reasoning, thinking, or using any cognitive ability that approaches human intelligence. They’re prediction machines.

But Silicon Valley loves to sniff its own farts about AGI, and the media loves to report on it, because it’s both exciting and scary. Some billionaires (like Elon Musk) predict the machines will take over and kill us, _Terminator_-style. Others, like Sam Altman, say no way, these are benevolent tools that will make our lives comfortable and vibrant.

Don’t believe the credulous articles that developers have had to [consult spiritual leaders](https://www.washingtonpost.com/technology/2026/04/11/anthropic-christians-claude-morals/), that “[AGI has already been achieved](https://fortune.com/2026/03/30/agi-definition-jensen-huang-lex-fridman-deepmind-turing-text-cognitive-taxonomy/),” that “[AI has emotions](https://time.com/7379564/ai-emotional-intelligence-support-bots/)” or other such nonsense. And don’t be afraid of the news every six months or so that there’s a new AI model that’s “[too dangerous to be released](https://thehill.com/policy/technology/5824219-anthropic-new-ai-dangerous-public/).” That’s pure marketing hype.

Meanwhile, the autocomplete LLM keeps doing its racism, encouraging suicidal ideation in teenagers, driving adults to psychosis, targeting elementary schools in Iran, and lining the pockets of billionaires who keep installing Donald Trump in the White House. So forget about AGI.

## What can I do?

Here are a few things I recommend:

**If you use LLMs, carefully monitor the output.** Double-check all external references and citations. If you’re vibe coding, do careful code reviews and write tests. If an LLM summarizes something for you, do your own quality control. Always ensure there’s a human in the loop. These tools can be helpful, but never fully trust them.

**Be skeptical of claims,** especially breathless predictions. Predicting the future is really hard, and anybody who’s confident they know what will happen is immediately untrustworthy.

**Be especially wary of the tech and finance media.** They exist to prop up CEOs and venture capitalists, and are often glorified stenographers. Look out for what I like to call “CEO Said A Thing!” articles. Once you know what they are, you’ll see them everywhere. For example:

- “Elon Musk says that in 10 to 20 years, work will be optional and money will be irrelevant thanks to AI and robotics.” _[Fortune](https://fortune.com/2026/01/19/when-does-elon-musk-say-work-will-be-optional-and-money-will-be-irrelevant-ai-robotics/)_
- “Sam Altman Says AI Will Soon Cause Widespread Job Loss. His Solution Is ‘Robot Taxes’ and Wealth Sharing.” _[Entrepreneur](https://www.entrepreneur.com/business-news/sam-altman-says-ai-will-soon-cause-widespread-job-loss)_
- “Nvidia’s Huang Urges Companies to Put AI Breakthroughs Before Profit” _[Bloomberg](https://www.bloomberg.com/news/newsletters/2026-04-10/nvidia-s-huang-urges-companies-to-put-ai-breakthroughs-before-profit)_
- That last one is especially funny. If the CEO of RJ Reynolds urged parents to put cigarette adoption ahead of their children’s health, wouldn’t a reporter stop to think, “Hey, wait a minute, maybe he’s got an ulterior motive?” If you need further evidence for why journalists shouldn’t just report whatever a CEO says without doing, well, you know, some _reporting_, have some fun reading [all of the things "Elon Musk said" over the years that never came true](https://en.wikipedia.org/wiki/List_of_predictions_for_autonomous_Tesla_vehicles_by_Elon_Musk).
- BTW, there _are_ some good tech publications. I especially like [The Verge](https://www.theverge.com/) and [Wired](https://www.wired.com). Both have fine journalists who report skeptically on the industry and speak truth to power about the Trump Administration as well. They really piss off guys like Elon Musk and Marc Andreessen, so you know they must be doing real journalism.

<figure style="width: 300px" class="img-fluid align-center">

<img src="{{ '/assets/images/elon-musk-mars-2024.png' | absolute_url }}" alt="Elon Musk Says We're Going to Mars by 2024">

<figcaption>Elon Musk said this thing in 2016!</figcaption>

</figure>

**Think about which companies you support.** There is no ethical consumption under capitalism, and we all do the best we can. Personally, I no longer use Google Search. Primarily because the AI features have made Google really, really bad. I’ve replaced it with [Kagi Search](https://kagi.com/), an excellent paid search engine that is AI-free, ad-free, and values privacy. However, I still use Gmail and Google Calendar. I find Anthropic to be the least evil LLM company, so I use Claude. I would not, however, describe them as the “most ethical.” On the ethical grading scale, they’re probably a C\- when everyone else is an F or a D. But they are far ahead of OpenAI and others in their transparency and principles. Several people I’ve worked with and admire are there. I would absolutely never support Elon Musk’s xAI if you tortured me, and I would strongly recommend not supporting OpenAI either.

**Try, really try, not to use AI for anything that replaces a human.** Personally, I don’t use LLMs or generative AI for any image generation anymore. However, I think it’s fine to do so for personal use. As an example, if you’re in a D&D campaign and want to use LLMs to make some art of your character, that’s a legitimate use of the tool. And it’s fine to share that with the other players in your group. However, I would think twice about posting that image online. And I would _absolutely_ avoid using AI-generated images in anything published for profit. **Hire professional artists and pay them.** You’ll get way better results, and it’s the ethical thing to do.

Sometimes it’s unavoidable to cut a human out of the loop. I recently called our local plumber to schedule a visit. I was about five minutes into the call before I realized I was speaking to an AI. It was extremely good, very interactive, and even joked with me. Only when it confirmed my address and pronounced California as “SEE-AYE” did I realize. I did a few tests to confirm. They replaced a human on my behalf, and I was bummed. Sad.

**Support independent human artists, performing artists, musicians, writers, and creators.** I support a bunch of creators on Patreon and YouTube, mostly D&D artists, independent journalists, musicians, and creators. They ask for small amounts of money; most of the patron levels are $5-10 a month. And these folks create a ton of amazing content! I can't keep up with it all. It feels great to be supporting these artists, musicians, journalists, writers, and creators. Go to the theater, the ballet, or a live performance. My personal goal is to ensure that my monthly human-creativity budget is at least twice* my Big Tech budget. So, for example, if you pay Anthropic $17 per month for Claude Pro, look for $34 worth of human beings you can support. Of course, this will be subject to what you can afford, so maybe a dollar-for-dollar match would be more appropriate. In any case, just stopping to think about how you can support creative professionals and amateurs in a future where they are threatened by AI is the most important goal.

**Learn to identify AI-created text and art.** There are certain tells, and they become easier to identify as you begin to look for them. Sure, there’s my beloved em-dash (—), but there are lots more clues as well. The telltale, “It’s not just X, it’s Y.” When you’re looking at art and images, zoom in. You’ll often find things amiss in the background. Gobbledegook text. Birds with three claws. The technology is always getting better, but there are ways to tell. Decisions that a human wouldn’t have made. A great place to hang out is the [r/isthisAI](https://www.reddit.com/r/isthisAI/) SubReddit. It’s like going to the gym for spotting AI slop.

**Help other people be skeptical.** I’m immersed in Silicon Valley, and the hype is real. Yet, even here, there’s a lot of AI fatigue and skepticism. One thing I’ve noticed is that when I’m open and outspoken about my opinions, it allows others to express their skepticism as well. There’s a lot of AI boosterism that doesn’t leave room for nuance or objection. Sharing your opinion creates space for others to feel comfortable doing the same. If someone says, “I asked ChatGPT and here’s what it says,” take a moment to ask them what they think really happened. If they share art or video that is created by AI, point that out. This is one way I’m using my privilege, and I intend to continue to do so. Even if it means being called a “hater” or a Luddite. (Research the [Luddites](https://mindmatters.ai/2019/01/remember-the-luddites/), you’ll welcome the comparison!)

![Made By A Human Person](/assets/images/made_by_a_human_person.png)
