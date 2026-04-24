# Peer Robotics - CV Intern Assignment

## Task:
Scenario: You have to develop an application for a customer in which the Peer 3000 AMR with forks moves around the facility as a pallet material mover using its onboard cameras to recognize if a pallet is ready to be moved. For context, this is a reference video of the Peer 3000 AMR running live trailer unloading operations. Please refer to the three sample photos provided below from our actual deployment sites to answer the following questions.

## Questions:
1.	Look closely at the differences between the three images. In Image 1 and Image 2, the pallets are staged within blue tape lines. In Image 3, there are no blue lines. Define the exact visual heuristics your pipeline would use to confidently conclude "readiness to move" across all three distinct scenarios. **[View Solution](./Q1.md)**

2.	Beyond readiness, the AMR must physically engage the pallet. How would your pipeline confirm that the fork pockets (the dark voids at the base) are structurally clear of debris before driving into them? **[View Solution](./Q2.md)**

3.	Write a step-by-step solution flow diagram from raw input image -> your solution -> output: "is the pallet ready to be moved?" **[View Solution](./Q3.md)**

4.	Select an open-source VLM (e.g., PaliGemma, LLaVA, Moondream). Write the specific prompt you would use for this task, run the provided images through your chosen model, and attach the raw results/outputs. **[View Solution](./Q4.md)**

5.	Say the Jetson AGX Orin has only 5GB of available VRAM and 20% GPU, and you cannot run this modern VLM at an input of 1080p/30fps under these constraints. How will you architect and optimize your solution to achieve the task without crashing the system? Think of an innovative pipeline design that achieves the result without compromising the robot's real-time navigation. **[View Solution](./Q5.md)**

6.	Plastic wrap glare and harsh, varying warehouse lighting frequently break purely vision-based models. Look at the intense reflections in Image 2. If your VLM pipeline fails to reliably detect the pallet's boundaries or "readiness" due to this glare, what specific traditional CV technique (e.g., contour detection, specific filtering) or alternative sensor data would you fuse into your stack to prevent a failure or collision? **[View Solution](./Q6.md)**

7.	Your pipeline works perfectly for this specific warehouse. Next month, we deploy a fleet of 5 robots to a new facility that uses yellow lines, entirely different payloads on top of the pallets, and different lighting. How will you scale your solution beyond the initial facility without starting from scratch? **[View Solution](./Q7.md)**

8.	Before deploying this scaled solution to the live robots, how would you quantitatively evaluate your pipeline's performance? Define the specific metrics you would use to prove it is ready. **[View Solution](./Q8.md)**
