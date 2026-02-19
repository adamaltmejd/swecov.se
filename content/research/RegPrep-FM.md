---
title: "Foundation Models on Nationwide Registers for Pandemic Preparedness"
shorttitle: "Foundation Models"
date: 2026-02-19
status: 'Ongoing'
subject: ['Artificial Intelligence', 'Education']
authors:
  - 'Thomas Eriksson'
  - 'Dominik Dietler'
  - 'Adam Altmejd'
  - 'Anders Björkelund'
  - 'Maxim Kan'
  - 'Fredrik Kahn'
  - 'Mattias Ohlsson'
  - 'Anna Mia Ekström'
  - 'Jonas Björk'
---

When a novel pathogen emerges, labeled outcome data is scarce. Foundation models pretrained on population-scale event streams could provide early predictions before supervised methods become viable. 
<!--more-->
We will train an autoregressive transformer on population-scale register event streams up to fixed calendar cutoffs, then evaluate strictly out-of-time on held-out periods to emulate deployment during a pandemic. Predictions are anchored to timestamped index events, here a positive SARS-CoV-2 test. From each index time t0, the model ingests a pre-index history, then produces autoregressive rollouts to estimate multiple outcomes over fixed horizons. The study will provide evidence of feasibility by comparing performance to supervised baselines trained on the same pre-cutoff data.
