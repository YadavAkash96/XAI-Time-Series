# XAI Implementation on Time Series Tool Tracking Data

Find the data source link here: https://cmutschler.de/datasets/tool-tracking-dataset 

## This repository has implementation of Attention based LSTM:AT-LSTM and XAI analysis on the trained model

1. To get same tool tracking data and base setup follow below repo

```
git clone https://github.com/crispchris/tool-tracking.git

wget https://christofferloeffler.com/tooltracking/tool-tracking-data.zip -O tool-tracking-data.zip

unzip tool-tracking-data.zip && rm tool-tracking-data.zip

```

2. Setup a python env:
```
conda create --name tool_tracking_env python>=3.10
conda activate tool_tracking_env
pip install -r requirements.txt
```

3. Follow data loading notebook to load and visualize data
```
how-to-load-the-data.ipynb
```

4. Finally, Run AT_LSTM.ipynb

### Architecture of AT-LTSM

The Attention-based LSTM (AT-LSTM) architecture leverages both temporal dependencies and attention mechanisms to effectively model tool usage patterns in time-series data.

<p align="center">
  <img width="580" height="635" align="center" alt="image" src="https://github.com/user-attachments/assets/27d1110d-d4ef-4645-99bc-6a5472346e9e" />
</p>


### XAI Results:

XAI using Attention Activation visualizes the decision-making process of AT-LSTM on Electric and Pneumatic Screwdrivers over a sample size of 32.

<p align="center">
  <img width="1915" height="861" alt="XAI: Attention Activation" src="https://github.com/user-attachments/assets/bab92846-3470-4192-9ae7-d377f69dc1d1" />
</p>


#### Tool: Electric Screwdriver

Visualization combining Attention Activation and Integrated Gradients highlights the most influential temporal segments contributing to model predictions.

<p align="center">
  <img width="1918" height="858" alt="Electric Screwdriver XAI" src="https://github.com/user-attachments/assets/ea403a8f-51e2-4613-ae44-4e502c63bb3d" />
</p>


#### Tool: Pneumatic Rivet Gun

Both techniques reveal distinct temporal focus areas, enabling interpretability of model predictions for complex tool behavior.

<p align="center">
  <img width="1984" height="868" alt="Pneumatic Rivet Gun XAI" src="https://github.com/user-attachments/assets/7ead73f7-0578-4426-a2d1-722f333127e0" />
</p>

### Model Performance:

The performance table shows a comprehensive comparison of deep learning models across tools, loss functions, and XAI strategies, with AT-LSTM showing strong results.

<p align="center">
  <img width="1054" height="283" alt="image" src="https://github.com/user-attachments/assets/57431f16-9e5c-4935-8355-7a1f4a322f19" />
</p>

### Conclusion:

AT-LSTM, empowered by attention mechanisms and interpretable via XAI techniques, demonstrates high performance and strong generalization across tool recognition tasks.

<p align="center">
  <img width="1049" height="242" alt="Conclusion" src="https://github.com/user-attachments/assets/5ec8d967-63c5-4cc2-be04-f31fdf7b8b75" />
</p>


## License:
  
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
