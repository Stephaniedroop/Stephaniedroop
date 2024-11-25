Hi, I’m @Stephaniedroop (Steph)

I'm a PhD student at University of Edinburgh in computational cognitive modelling. This is 'doing psychology with the tools of computer science' and my main project is about how people suggest new explanations to explain the surprising behaviour of others.

What I mean by that is: say you see your mate Pete running across campus to the pizza van. Why? That's easy to explain if you know Pete likes pizza, and it's lunch time. Easy! Everyone knows a liking for pizza tends to promote pizza-eating behaviour! But a love of pizza doesn't mean you eat pizza every minute of every day. Besides, what if you know Pete's on a diet, doesn't like pizza, and it isn't even lunchtime? It seems toally normal that we humans would start to hypothesise and brainstorm: maybe he knows the person who works there and he's dropping off his keys, maybe he saw his kid run into the road behind the van... any number of reasons. It seems we integrate what else we know about the world.

Current systems can't do this, so it seems a good place to start to formalise what it is about human minds is special, and how we might make systems later that can do it.

I made a start on this with a project called `gw`, which stands for `gridworld` (little square depictions of worlds that characters can move about in, like a cartoon urban environment).

It's my main PhD project, so is not finished yet. The latest, most exciting and most user-friendly bit is the `Collider` project. Here I scale down the whole model to a small easy environment, to make sure it works and we understand its implications. A collider is when two causes can both cause an effect. It can either be disjunctive (either cause on its own can cause the effect) or conjunctive (both are needed).

The world is inherently stochastic: often noise prevents things happening reliably 100% of the time. However, if we knew the whole story, we could determine the cause. We model this as deterministic links in the structural equation model, but with an exogenous noise variable. Effectively, this has to be on at the same time as its twin node but importantly, it is unobserved (latent). The Collider project is a behavioural experiment where people select from causal explanations for the outcomes of situations. I implement Quillien's 2020 popular model of causal selection (Counterfactual Effect Size Model; CESM) which successfully produces the same pattern of data as the behavioural experiment, except for in a few key situations. These situations are where people cite unobserved causes, which the model makes no difference for. The is an important area to tweak the model for, which is work in progress at November 2024.

My main programming language is R. I use that for data analysis and visualisation, (see TuringToM project repo for examples), and for programming models using probability distributions, simulation and logic (`gw`). 

You can read more details on the README for each project.

## Other

At November 2024 I am developing a business idea and through this trying to find a realworld application for my causal models. Even developing the idea is helping me implement machine learning models, for example, I'm gauging customer engagement with my different ads by modelling the ads as a multi-armed bandit problem with beta-bernoulli distributions, where ones that are successful with clicks get shown more ('win-stay') and if they are not so good they sometimes get shown again but mostly a different one wil be shown ('lose-Thompson-sample'). More on how that goes later.


<!---
Stephaniedroop/Stephaniedroop is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
