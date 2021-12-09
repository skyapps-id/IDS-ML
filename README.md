# IDS-ML

🚢[Dataset The Bot-IoT Dataset](https://research.unsw.edu.au/projects/bot-iot-dataset)

### Tools 
- Jupyter Notebook or Google Colab
- Python

### Machine Learning Method
- K-Nearest Neighbor (KNN) 


### Manual Run
1. Clone this project.
   
    ```sh
    $ git clone https://github.com/skyapps-id/IDS-ML 
    $ cd IDS-ML/
    ```

2. Download dataset place in your project
   
3. Run file ```Preprocecing Data.ipynb``` for Preprocecing Data, get file result.
    ```sh
    UNSW_2018_IoT_Botnet_V6.csv
    ```

4. Run file ```RandomOverSampler and Spliting Data.ipynb``` for Spliting Data, get file result.
    ```sh
    UNSW_2018_IoT_Botnet_V6_Train.csv
    UNSW_2018_IoT_Botnet_V6_Test.csv
    ```

5. Run file ```BOT IOT KNN FINAL V6.ipynb``` for Train Data.
   
6. Result :
    ```sh
    Confusion Matrix

    [[   196      0      0     99      0      0      0]
    [     0 292646      0      0    516      0      1]
    [     0      1 284507      0      1      3      0]
    [   101      0      0    346      0      0      2]
    [     0    349      1      2 184347      0      1]
    [     2      5      4      1      1 309289      3]
    [     0      0      0      0      0      0 310534]]

    
                  precision    recall  f1-score   support

       DDoS-HTTP     0.6555    0.6644    0.6599       295
        DDoS-TCP     0.9988    0.9982    0.9985    293163
        DDoS-UDP     1.0000    1.0000    1.0000    284512
        DoS-HTTP     0.7723    0.7706    0.7715       449
         DoS-TCP     0.9972    0.9981    0.9976    184700
         DoS-UDP     1.0000    0.9999    1.0000    309305
          Normal     1.0000    1.0000    1.0000    310534

        accuracy                         0.9992   1382958
       macro avg     0.9177    0.9188    0.9182   1382958
    weighted avg     0.9992    0.9992    0.9992   1382958
    ```

### Manual Run Simulation Real Trafic
1. Go to folder simulation.
   
2. Run file ```BOT IOT KNN FINAL V6 With 3 Class.ipynb``` for Train Data 3 Class.
   
3. Result :
   
    ```sh
    Confusion Matrix

    [[3000    0    0]
    [   0 3000    0]
    [  32   49  451]]


                  precision    recall  f1-score   support

      Attack-TCP     0.9894    1.0000    0.9947      3000
      Attack-UDP     0.9839    1.0000    0.9919      3000
          Normal     1.0000    0.8477    0.9176       532

        accuracy                         0.9876      6532
       macro avg     0.9911    0.9492    0.9681      6532
    weighted avg     0.9878    0.9876    0.9871      6532
    ```

### About Me
[Linkedin](https://www.linkedin.com/in/aji-indra-jaya-3ab6b7135)

### Licence

This work is under [MIT](LICENCE) licence.