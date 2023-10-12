# RLbot_crypto_trading

There are 5 RL agents. Each of these uses different algorithms to produce maximum profit on initial investment. There are 3 actions – buy, sell and hold- to choose from. The first RL agent, ‘random_game’, as the name suggests performs these actions at random. The second agent, ‘reward_based _games’ takes into account the history of rewards garnered per action for the first two step of that train episode only. The third agent, ‘policy_based_game’ only looks at the ‘ti_score’ for that time step. The ’ti_score’ is the technical indicator score that is a measure of how profitable a buy will be. The fourth agent, ‘reward_based _games2’ takes into account the history of rewards garnered per action for the previous 2 steps only. If the reward for the latest step is more than that of the previous step, the action is repeated, else, a random action is performed. The fifth agent, ‘policy_based_game2’ repeats a profitable action just the same as in ‘reward_based_games2’ but instead of performing a random action in case of decrease in rewards, this agent decides an appropriate action based on the ‘ti_score’. 

For different use cases, different agents may be employed. There is a comparison function that could be used to compare performances of all agents for a given set of data.  

The code was run on bitcoin price data and ‘poilcy_based_games2’ yielded a simulated profit of 15-20% profit on an average for a trial period of 30 days.  
