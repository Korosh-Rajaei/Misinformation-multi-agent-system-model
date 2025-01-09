# Misinformation-multi-agent-system-model  
a NetLogo model which mimics how false information spreads across a network of individuals. Five distinct agents in total interact with one another by circling our NetLogo environment at random. When individuals come into physical contact with one another, they spread false information by altering one other's "opinion". 5 Distinct agents are used each with different behavioral patterns and effects on the other agents: Source of Misinformation, Experts, Influencers, Supporters, and Individuals.  

# Agents  
The source of misinformation is a stationary agent represented as a cube. It has a radius of influence of 3 units, affecting any agent that enters this range, except Experts. When affected, an agent’s opinion decreases by -25 multiplied by their susceptibility. The source of misinformation has a fixed and immutable opinion value of -100.  
  
Experts are moving agents designed to counter misinformation. Upon contact, they positively influence opinions: increasing Individuals' opinions by +25, Influencers' by +7, and Supporters' by +5 multiplied by their susceptibility. Experts themselves have a fixed opinion of 100, which does not change regardless of interaction. They move at a speed of 2 units per tick, allowing them to reach and influence agents effectively.
  
Influencers are fast-moving agents, traveling at 3 units per tick, the fastest of all agents. They start misinformed with an initial opinion of -5. When interacting with other agents, they alter opinions as follows: Individuals by +/-10, Supporters by +3 or -5, and other Influencers by +/-1. Influencers can become informed when they come into contact with Experts, transitioning from spreading misinformation to combating it.  
  
Supporters are moving agents who start with a misinformed opinion of -10. They rarely become informed due to their unique susceptibility value, which influences their responsiveness to Experts. Upon interaction, Supporters modify opinions as follows: Individuals by +/-5, Influencers by +/-1, and other Supporters by +/-2. They move at a speed of 1 unit per tick, making them slower than Influencers and Experts but equivalent to Individuals.  
  
Individuals are moving agents with an initial neutral opinion of 0, but their opinions can change dynamically based on interactions. They are influenced by other agents as follows: Supporters by +/-2, Influencers by +/-1, and other Individuals by +/-3. Susceptibility plays a significant role in determining how much misinformation affects them, but they are not misinformed if they interact with informed agents. Individuals move at a speed of 1 unit per tick, similar to Supporters.  

# Credits  
This project was made for the course Multi-Agent Systems. I was responsible for coding of the NetLogo model and data extraction from the model. Amirhossein Shahsavari and Emre Uysal also helped me with the logic and programming of the MAS model. Princewill Ayuk, Andrei Donea, and Mattia Sferrazza aided with the initial project idea and data analysis. 
