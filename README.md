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

<img width="580" height="635" align="center" alt="image" src="https://github.com/user-attachments/assets/27d1110d-d4ef-4645-99bc-6a5472346e9e" />
 

## License:
  
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
