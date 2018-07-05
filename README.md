
by Gregory Urman

www.linkedin.com/in/gregoryurman  

_scroll to the bottom to see a list of reference links, please_


# Monte Carlo Method as applied to GridWorld #

In this blog, we will discuss the Monte Carlo Method (a fundamental concept in Reinforcement Learning) as it relates to our program, GridWorld. It would be helpful for the reader to look at the following links to provide better context:

- https://user-images.githubusercontent.com/22970879/42120041-d7145168-7bd1-11e8-8f11-42546269f56e.png

- https://user-images.githubusercontent.com/22970879/42313209-65c09134-7fff-11e8-9e06-2b0f66338aa4.png

- https://github.com/gurman24/What-are-States-and-State-to-State-Transitions-


Now that we are caught up, "Monte Carlo methods are a broad class of computational algorithms that rely on repeated random sampling to obtain numerical results. Their essential idea is using randomness to solve problems that might be deterministic in principle." [1] It might also interest the reader to know that Monte Carlo methods can also be applied to "what if" scenarios, computer graphics, Artificial intelligence for games, and even Finance and Business!!! [same source] 

In terms of GridWorld, Monte Carlo methods are also useful for finding optimal solutions similarly to Value Iteration, see below:

![07-05-18 monte carlo rewards and decimals](https://user-images.githubusercontent.com/22970879/42337126-fa95520c-8042-11e8-8fe2-c8fc421fd139.PNG)



To borrow from another source:

- Monte carlo records info from running the entire simulation
- involves episodic interaction with the system/environment
- Each episode involves "playing the game"
- Learn from repeated simulated experience
- Policy evaluation uses
 - State-value pairs, which is the estimate of the value of State S (the current State)
- Policy update will use
  - State, action, and value triples (s; a; G), which is an estimate of the Q-value state-action pairs
-  Eeffective Monte Carlo algorithms need to ensure that all state-action pairs are sampled, and maybe even repeatedly 
- Exploring using Monte Carlo methods may involve using Epsilon-Greedy algorithms similar to Multi-Armed Bandit [2] 

-------------------------------------------------------------------------------------------------------------------------------

# Conclusion: #

- Monte Carlo Methods was a revolutionary concept that applies to Reinforcement Learning, many concepts that involve randomness and problem solving, as mentioned above.

- Monte Carlo involves running through the entire episode of calculations, using state-action pairs, averaging episodes, and  continuously updating policy [3]

- Monte Carlo methods also apply to  TD (temporal differences) for calculating values:
 - In Monte Carlo, the G function is the TOTAL REWARD for everything
 -	So Monte Carlo is about whatever rewards ACTUALLY HAPPENED
 -	The TD is about the estimated rewards for that episode/epoch [also, reference #3]

-------------------------------------------------------------------------------------------------------------------------------


[1] = https://en.wikipedia.org/wiki/Monte_Carlo_method

[2] = Dr. Hart slides, Regis University 2018

[3] = paraphrase of something Dr. Hart said.
