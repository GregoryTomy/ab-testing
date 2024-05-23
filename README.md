# What is A/B Testing

> A/B testing (also known as split testing) is a process of showing two variants of the same web page to different segments of website visitors at the same time and comparing which variant drives more conversions.

# Business Problem Statement
Cookie Cats, a popular mobile puzzle game developed by Tactile Entertainment, is designed to captivate and engage players through its entertaining gameplay and strategic challenges. One critical aspect of the game’s design is the placement of gates, which are points in the game where players must wait or make in-app purchases to progress. The placement of these gates can significantly influence player retention and overall game engagement.
 
Recently, the game develowpment team at Cookie Cats has hypothesized that relocating the initial gate from level 30 to level 40 may improve player retention and engagement. To test this hypothesis, an A/B test was conducted where new players were randomly assigned to one of two groups: 

1. The control group with the gate at level 30 (gate_30)
2. The experimental group with the gate moved to level 40 (gate_40).

The primary objective of this analysis is to determine whether moving the gate to level 40 has a positive impact on player behavior, specifically focusing on key metrics such as the number of game rounds played within the first 14 days (sum_gamerounds) and retention rates at one day (retention_1) and seven days (retention_7) after installation.

# Data

The data we have is from **90,189 players** that installed the game while the AB-test was running. The variables are:

1. *userid*: A unique number that identifies each player.
2. *version*: Whether the player was put in the control group (gate_30 - a gate at level 30) or the group with the moved gate (gate_40 - a gate at level 40).
3. *sum_gamerounds*: the number of game rounds played by the player during the first 14 days after install.
4. *retention_1*: Did the player come back and play 1 day after installing?
5. *retention_7*: Did the player come back and play 7 days after installing?