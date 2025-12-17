# guiyang-iot-traffic
Large-scale real-world IoT traffic dataset collected in Guiyang, China

# Guiyang Traffic Flow Dataset

This repository contains the datasets used for traffic flow analysis and forecasting in Guiyang, China.  
The data can be used for spatial-temporal modeling, graph neural networks, and intelligent transportation system research.  

Origin Data Link: https://pan.baidu.com/s/1MAVFHm-RmTfiVIC1WVvsdg?pwd=3q7h  Extraction Code: 3q7h 

---

## 📂 Dataset Files

- **`gy_link_info.txt` and `gy_link_top.txt`**  
  gy_link_info.txt and gy_link_top.txt contain the road connection information and can be used to construct the adjacency matrix of the traffic network.

- **Traffic flow data (three `.txt` files)**  
  Each file contains original traffic flow records with the following fields:  
  - `link_ID`: Road segment ID  
  - `date`: Date of observation  
  - `time_interval`: Time interval of measurement  
  - `travel_time`: Average travel time (in seconds)  

---

## 🗓️ Additional Information

- **Holiday and weekend labels**  
  These can be derived from the `date` field.  

- **Weather data**  
  Meteorological information (temperature, relative humidity, wind speed, pressure, and precipitation) can be obtained from the **China Meteorological Data Service Center (National Meteorological Science Data Center)**:  
  👉 [http://data.cma.cn/](http://data.cma.cn/)  
