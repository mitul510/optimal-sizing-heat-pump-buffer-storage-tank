# The Influence of Dynamic Electricity Prices on the Sizing of Heat Pumps and Buffer Storage Tanks

This repository contains the Python-based optimization model developed for my master's thesis at Hochschule Ansbach. The model analyzes residential heating demand and evaluates cost-optimal sizing and operation strategies for heat pumps and buffer storage systems under dynamic electricity tariffs.

## Thesis Information

- Program: M.Eng. Smart Energy Systems  
- Author: Mitulkumar Ghanshyambhai Makwana  
- Year: 2025  
- University: Hochschule Ansbach  
- Supervisor: Prof. Dr. Mathias Moog  

## Overview of the Model

The model performs the following steps:

- Loads hourly heat demand and electricity spot market prices
- Interpolates Coefficient of Performance (CoP) based on flow temperature
- Simulates heat pump and buffer tank behavior over a one-year period
- Optimizes the daily operation to minimize energy cost using the SLSQP method from the SciPy library
- Calculates final cost, energy consumption, and penalty cost

## Repository Contents

- `thesis_model_3kW_750L.ipynb` – Main simulation and optimization notebook
- `.gitignore` – Ignores unnecessary cache and system files
- `LICENSE` – MIT License

## Results Summary

- Total Initial Guess Cost: €555.39  
- Optimized Cost: €542.17  
- Cost Reduction: €13.22  
- Real Electricity Cost: €532.11  
- Penalty Cost: €10.05  
- Total Heat Consumed: 7400.60 kWh  
- Total Heat Produced: 7611.18 kWh

## Conclusion

The simulation results indicate that oversizing the heat pump and buffer tank system is not economically beneficial. When higher investment costs are considered, the additional operational savings from larger systems are too small to justify the cost. This conclusion is based on structured simulations using real dynamic electricity price data and aligns with modern cost-optimization strategies for decentralized heating systems.

## Technologies and Libraries Used

- Python 3  
- Jupyter Notebook  
- NumPy  
- Pandas  
- Matplotlib  
- SciPy (SLSQP solver for constrained optimization)

## Contact

For questions, collaboration, or reference, feel free to reach out:

Email: mitulmakwana5257@gmail.com  
LinkedIn: https://linkedin.com/in/mitulmak

## License

This project is licensed under the MIT License.
