# Reinforcement Learning-Based Stock Trading Agent

This project implements a Reinforcement Learning (RL) agent using **Proximal Policy Optimization (PPO)** to trade AAPL stock. The agent learns to buy, sell, or hold based on historical price patterns and technical indicators — aiming to maximize long-term portfolio value.

---

## Problem Statement

Design an autonomous agent that can trade a stock using only past price data. The goal is to **outperform a simple buy-and-hold strategy** using Reinforcement Learning.

---

## Technologies Used

- Python
- Pandas, NumPy
- Matplotlib
- Stable-Baselines3 (PPO)
- OpenAI Gym (custom environment)

---

## Features Engineered

- **Daily Return**  
- **5-day & 20-day Moving Averages**

The agent's observation at each time step is:
[cash, shares_held, price, MA5, MA20, daily_return]

---

## Actions

- `0`: Hold  
- `1`: Buy 1 share  
- `2`: Sell 1 share  

---

## Reward

Reward is defined as the **change in total portfolio value** after each action.

---

## Results

The PPO agent learned to:
- Buy near dips
- Sell after upward trends
- Avoid overtrading

## Files

- `AAPL_Dummy.csv`: Historical stock data
- `RL_Trading_Agent.ipynb`: Full training + evaluation notebook
- `README.md`: Project documentation
