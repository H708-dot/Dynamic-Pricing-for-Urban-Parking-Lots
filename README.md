# Dynamic-Pricing-for-Urban-Parking-Lots
Capstone Project of Summer Analytics 2025 hosted by Consulting &amp; Analytics Club × Pathway

## Background and Motivation

Urban parking spaces are a limited and highly demanded resource. Prices that remain static throughout the day can lead to inefficiencies, either overcrowding or underutilization. To improve utilization, dynamic pricing based on demand, competition, and real-time conditions is crucial. 

This project simulates such a system: participants will create an intelligent, data-driven pricing engine for 14 parking spaces using real-time data streams, basic economic theory, and ML models built from scratch, using only NumPy, Pandas libraries.

## Data Description

Data collected from 14 urban parking spaces over 73 days, sampled at 18 time points per day with 30 minutes of time difference (from 8:00 AM to 4:30 PM the same day).

### Each record includes the following:

#### Location Information:

- Latitude and longitude of each parking space (to calculate proximity to competitors).

#### Parking Lot Features:

- Capacity (maximum number of vehicles that can be parked)
- Occupancy (current number of parked vehicles)
- Queue length (vehicles waiting for entry)

#### Vehicle Information:

- Type of incoming vehicle: car, bike, or truck

#### Environmental Conditions:

- Nearby traffic congestion level
- Special day indicator (e.g., holidays, events)

Each time step reflects the state of each parking lot, and demand will fluctuate throughout the day based on these features.

## Project Objective

Your goal is to build a dynamic pricing model for each parking space such that:

- The price is realistically updated in real-time based on:
    - Historical occupancy patterns
    - Queue length
    - Nearby traffic
    - Special events
    - Vehicle type
    - Competitor parking prices
- It starts from a base price of$ 10
- The price variation is smooth and explainable, not erratic
- Optional: The system suggests rerouting vehicles to nearby lots if the current lot is overburdened.
