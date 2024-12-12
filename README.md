# InfernoTamer

**InfernoTamer** is a Multi-Agent Reinforcement Learning (MARL) framework designed to coordinate firefighting planes in a dynamic grid environment. The agents collaborate to extinguish fires of varying intensities, manage limited water stacks, and efficiently navigate a randomized environment.

---

## 🌟 Key Features

- **Dynamic Environment:**
  - Fires have randomized locations and intensities.
  - Planes have randomized starting positions and water stack levels.
- **Multi-Agent Collaboration:**
  - Planes work together to minimize fire spread and optimize resource allocation.
- **COMA (Counterfactual Multi-Agent Policy Gradient):**
  - Utilized for effective credit assignment and coordination among agents.
- **Action Masking:**
  - Ensures agents only take valid actions based on their local observations.

---

## 🎯 Problem Statement

The goal of **InfernoTamer** is to simulate and solve a disaster management problem where:

- **Fires:** Randomly placed on the grid with intensities ranging from 1 (low) to 3 (high).
- **Planes:** Equipped with limited water stacks, they must:
  - Move to refill stations to replenish their stacks.
  - Navigate towards fires to extinguish them.

The simulation ends when all fires are extinguished or the maximum episode length is reached.

---

## 🚀 Methodology

### 1. **Environment:**
- **Grid Setup:**
  - A 2D grid represents the environment.
  - Fires, planes, stack refill stations, and empty cells are placed randomly at the start of each episode.
- **Randomization:**
  - Fires: Randomized in terms of location and intensity.
  - Planes: Randomized in terms of starting location and initial water stack levels.

### 2. **Multi-Agent Collaboration:**
- Agents (planes) must cooperate to:
  - Prioritize extinguishing high-intensity fires.
  - Refill water stacks efficiently.
  - Avoid unnecessary movement or resource wastage.

### 3. **COMA (Counterfactual Multi-Agent Policy Gradient):**
- **Why COMA?**
  - Efficient credit assignment by comparing an agent’s action to counterfactual baselines.
  - Ensures coordinated decision-making in a shared reward setting.

### 4. **Action Masking:**
- Validates and restricts agent actions based on local observations:
  - Move towards fires, empty cells, or refill stations.
  - Extinguish fires if adjacent.
  - Perform a "no-op" if no valid actions are available.

---

## 🧪 Example

Here’s what an episode might look like:

- Fires with intensities of 1, 2, or 3 spread across the grid.
- Planes strategically move to extinguish fires while managing their stack levels.
- The episode ends when all fires are extinguished or the time limit is reached.
- [Watch Now]()
---

## 📊 Performance Metrics

- **Reward:**
  - Based on the intensity of fires extinguished and resource efficiency.
- **Steps:**
  - The total number of steps taken by all agents.

---

## 🌐 Contact

For questions or collaboration:
- **Email:** highcsavci@gmail.com.com
- **GitHub:** [Your GitHub Profile](https://github.com/highcansavci)
