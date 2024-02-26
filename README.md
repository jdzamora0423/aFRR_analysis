This project is about analysis and forecasting of activated volume of secondary balancing power in the German grid, focusing on the behavior of trend breaks, or spikes in activated volume.

### Discussion

The activated energies, both positive and negative, have distributions highly skewed to the right. Most of the time the activated energies are relatively low, averaging around 26MWh with the 75th percentile only at 30 MWh. The differences for different intervals were also averaging at zero with a standard deviation of around 36 MWh.

Data using the 15-min interval was most helpful in analyzing changes in the activated energies where larger spikes mostly occur on the hour of almost every hour of the day. The box plot of the 120-minute interval showed that relatively higher changes in activated energies happen at the middle of the day and during the night.

Forecasting changes in activated energy for aFRR is difficult since spikes occur during different times on different days. Both ARIMA and RNN (LSTM) models had difficulty in predicting the spikes in the data. LSTM model performed slightly better than the ARIMA model. The ARIMA model only predicted a few values and predicted the rest to be zero, while the LSTM model was predicting values all throughout.

Upward spikes in activated volume difference for positive energy means that there was more demand than the power generated, while upward spikes with the negative energy means there was more supply. The analysis from this paper can help guide the TSOs in procuring the adequate amount of capacity for certain time frames. The generating units can also target certain time frames where spikes are high so their bids will have higher chance of activation.

For future studies, it is recommended that more data is to be used for analysis of larger time frames, such as daily, weekly, and monthly. It is also recommended that more forecasting models are tested to see if there would be a model that can more accurately predict the larger spikes. Advanced decomposition methods can also be used for better understanding the behavior of the changes in activated energies.
