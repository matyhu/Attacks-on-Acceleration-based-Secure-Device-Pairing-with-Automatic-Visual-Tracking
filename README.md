# Attacks-on-Acceleration-based-Secure-Device-Pairing-with-Automatic-Visual-Tracking
## 1. We gathered 10 volunteers with 10 mobile phones for the experiment.
**The details of the 10 volunteers and their mobile phones are as follows:**

|  Characteristics   | Volunteer1  | Volunteer2   | Volunteer3  | Volunteer4   | Volunteer5  | Volunteer6   | Volunteer7  | Volunteer8   | Volunteer9  |  Volunteer10  |
|  :----:  | :----:  |  :----:  | :----:  | :----:  | :----:  |:----:  | :----:  |:----:  | :----:  |:----:  |
| **Sex**| male | male | male | male | male |female|female|female|female|female|
| **Age**  | 27 | 25|26|23|25|25|25|26|26|24|
|**Phone Brand**| Yijia ACE2|iPhone7|Huawei nova9|iPhone13Pro|Redmi k50u|JianguoPro2|iPhone7|Vivo iQQneo5|iphone13 mini|Xiaomi 12S|
|**Operating System**|Android13|iOS15.2.1|HarmonyOS3.0.0|iOS16.1|Android12|Anroid7.1.1|iOS11|Android11|iOS16.4.1|Android12|

## 2.Experiments include complex real-world scenarios: indoors and outdoors.
**The shaking time of each volunteer is roughly 30s.**
<div align=center>

![Alt](./10Hz/Indoor/Huawei%20nova9_HarmonyOS3.0.0/Rotation/Indoor_10Hz_Huaweinova9_rotation.gif)
<center><p> The indoor scenario  <center><p>

![Alt](./10Hz/Outdoor/Huawei%20nova9_HarmonyOS3.0.0/Rotation/Outdoor_10Hz_Huaweinova9_rotation.gif)
<center><p> The outdoor scenario   <center><p>
</div>

## 3. The motion of each volunteer includes two movement modes: shaking and rotation.
* **Shaking Mode: in this mode, the volunteers hold the mobile phone tightly and move at the fastest speed. The movement of the wrist was not given much thought.**
* **Rotation Mode: in this mode, the volunteers shake the phone as much as possible using the force of the wrist. In this exercise mode, the speed of the volunteer is slow, but the range of motion is large.**

<div align=center>

![Alt](./10Hz/Indoor/Huawei%20nova9_HarmonyOS3.0.0/Shaking/Indoor_10Hz_Huaweinova9_shaking.gif)
<center><p> The shaking mode   <center><p>

![Alt](./10Hz/Indoor/Huawei%20nova9_HarmonyOS3.0.0/Rotation/Indoor_10Hz_Huaweinova9_rotation.gif)
<center><p> The rotation mode   <center><p>

</div>

## 4.The display content of each experiment result includes 2 videos, 3 figures and the final coherence.

**Let's take the results in the "./10Hz/Indoor/Huawei nova9_harmonyOS3.0.0/Shaking/" subfolder as an example to show the results of each experiment:**

**Videos**
* **Color video: it is displayed as a .gif, playing the shaking process recorded by the camera.**
<div align=center>

 ![Alt](./10Hz/Indoor/Huawei%20nova9_HarmonyOS3.0.0/Shaking/Indoor_10Hz_Huaweinova9_shaking.gif) 
<center><p> The color video of the shaking   <center><p>

</div>

* **Depth video: it is displayed as a gif, playing the depth information of shaking. Note: The depth video of the indoor scene is composed of the picture set of the depth map, but the picture set of the depth video of the composite outdoor scene is rendered by aligning the depth with the color point cloud.**

<div align=center> 

 ![Alt](./10Hz/Indoor/Huawei%20nova9_HarmonyOS3.0.0/Shaking/Indoor_10Hz_Huaweinova9_shaking_depth.gif) 
<center><p> The depth video of the shaking   <center><p>

</div>

**Figures** 
* **The acceleration estimation by HSTD: two curves in the figure are the seneor measured acceleration and the estimated acceleration curve respectively. The plot intuitively represents the similarity of the estimated acceleration to the sensor measured acceleration.**
  
<div align=center> 

 ![Alt](./10Hz/Indoor/Huawei%20nova9_HarmonyOS3.0.0/Shaking/The%20acceleration%20estimation%20by%20HSTD.png) 

</div>

* **The frequency domain of the acceleration: the abscissa corresponding to the peak in the figure represents the volunteer's exercise frequency (ie, how many times per second it can shake). The more coincident the two curves in this figure, the higher the similarity of the two acceleration sequences.**

<div align=center> 

 ![Alt](./10Hz/Indoor/Huawei%20nova9_HarmonyOS3.0.0/Rotation/The%20frequency%20domain%20of%20the%20acceleration.png) 

</div>

* **The magnitude squared cohenrence of two accelerations: The correlation of the two acceleration series is finally calculated from the partial integral values in this curve. The region with larger values in the figure corresponds to the frequency band where the two acceleration sequences are most similar in the amplitude-frequency domain.**

<div align=center> 

 ![Alt](./10Hz/Indoor/Huawei%20nova9_HarmonyOS3.0.0/Shaking/The%20magnitude%20squared%20cohenrence%20of%20two%20accelerations.png) 

</div>

**Final coherence：**
* **For the calculation process of final coherence, please refer to Section III-B of the paper.**
* **Here we directly give the value of final coherence 0.8103, which exceeds the threshold of 0.55. Therefore, it shows that the mobile phone using this model and system can successfully carry out the attack.**


# 5.We conduct experiments with sampling frequencies of 60Hz and 100Hz.
**To justify that the camera and accelerometer sampling frequency is 10 Hz because the maximum frequency at which a person shakes the phone is within 5 Hz (ie, shake the phone 5 times per second). We selected the youngest and most powerful volunteer and made him shake the phone as fast as possible to complete two sets of experiments:**

**1. Set the sampling frequency of both the camera and the acceleration sensor to 60Hz:**
* **Shaking Mode**:
<div align=center> 

   ![Alt](./60Hz/Shaking/60Hz_shaking.gif)
   ![Alt](./60Hz/Shaking/60Hz_shaking_depth.gif)
   ![Alt](./60Hz/Shaking/The%20frequency%20domain%20of%20the%20acceleration.png)

</div>

* **Rotation Mode:**
<div align=center> 

   ![Alt](./60Hz/Rotation/60Hz_rotation.gif)
   ![Alt](./60Hz/Rotation/60Hz_rotation_depth.gif)
   ![Alt](./60Hz/Rotation/The%20frequency%20domain%20of%20the%20acceleration.png)
</div>

**2. Set the sampling frequency of both the camera and the acceleration sensor to 100Hz:**
* **Shaking Mode:**
<div align=center> 

   ![Alt](./100Hz/Shaking/100Hz_shaking.gif)
   ![Alt](./100Hz/Shaking/100Hz_shaking_depth.gif)
   ![Alt](./100Hz/Shaking/The%20frequency%20domain%20of%20the%20acceleration.png)

</div>

* **Rotation mode:**
<div align=center> 

   ![Alt](./100Hz/Rotation/100Hz_rotation.gif)
   ![Alt](./100Hz/Rotation/100Hz_rotation_depth.gif)
   ![Alt](./100Hz/Rotation/The%20frequency%20domain%20of%20the%20acceleration.png)
</div>

# 6.Directory Tree:
**We have done 44 experiments in total, and this directory tree shows the storage structure of all experimental results. According to the name of the folder, click to enter the last level folder, and you can see the results of the corresponding experiment.**
```
Attacks-on-Acceleration-based-Secure-Device-Pairing-with-Automatic-Visual-Tracking
    ├─10Hz
    │  ├─Indoor
    │  │  ├─Huawei nova9_HarmonyOS3.0.0
    │  │  │  ├─Rotation
    │  │  │  └─Shaking
    │  │  ├─iPhone13Pro_iOS16.1
    │  │  │  ├─Rotation
    │  │  │  └─Shaking
    │  │  ├─iphone13_iOS16.4.1
    │  │  │  ├─Rotation
    │  │  │  └─Shaking
    │  │  ├─iPhone7_iOs11
    │  │  │  ├─Rotation
    │  │  │  └─Shaking
    │  │  ├─iPhone7_iOS15.2.1
    │  │  │  ├─Rotation
    │  │  │  └─Shaking
    │  │  ├─JianguoPro2_Anroid7.1.1
    │  │  │  ├─Rotation
    │  │  │  └─Shaking
    │  │  ├─Redmi k50u_Android12
    │  │  │  ├─Rotation
    │  │  │  └─Shaking
    │  │  ├─Vivo iQQneo5_Android11
    │  │  │  ├─Rotation
    │  │  │  └─Shaking
    │  │  ├─Xiaomi 12S_Android12
    │  │  │  ├─Rotation
    │  │  │  └─Shaking
    │  │  └─Yijia ACE2_Android13
    │  │      ├─Rotation
    │  │      └─Shaking
    │  └─Outdoor
    │      ├─Huawei nova9_HarmonyOS3.0.0
    │      │  ├─Rotation
    │      │  └─Shaking
    │      ├─iPhone13Pro_iOS16.1
    │      │  ├─Rotation
    │      │  └─Shaking
    │      ├─iphone13_iOS16.4.1
    │      │  ├─Rotation
    │      │  └─Shaking
    │      ├─iPhone7_iOS11
    │      │  ├─Rotation
    │      │  └─Shaking
    │      ├─iPhone7_iOS15.2.1
    │      │  ├─Rotation
    │      │  └─Shaking
    │      ├─JianguoPro2_Anroid7.1.1
    │      │  ├─Rotation
    │      │  └─Shaking
    │      ├─Redmi k50u_Android12
    │      │  ├─Rotation
    │      │  └─Shaking
    │      ├─Vivo iQQneo5_Android11
    │      │  ├─Rotation
    │      │  └─Shaking
    │      ├─Xiaomi 12S_Android12
    │      │  ├─Rotation
    │      │  └─Shaking
    │      └─Yijia ACE2_Android13
    │          ├─Rotation
    │          └─Shaking
    |─60Hz
    |    ├─Rotation
    |    └─Shaking
    ├─100Hz
    │    ├─Rotation
    │    └─Shaking


```
**The final coherence for all experiments is shown as fellow:**

<escape>

<table style="undefined;table-layout: fixed; width: 1184px">
<colgroup>
<col style="width: 109px">
<col style="width: 112px">
<col style="width: 86px">
<col style="width: 86px">
<col style="width: 125px">
<col style="width: 96px">
<col style="width: 90px">
<col style="width: 94px">
<col style="width: 86px">
<col style="width: 103px">
<col style="width: 103px">
<col style="width: 94px">
</colgroup>
<thead>
  <tr>
    <th colspan="2">Characteristic</th>
    <th>Volunteer1</th>
    <th>Volunteer2</th>
    <th>Volunteer3</th>
    <th>Volunteer4</th>
    <th>Volunteer5</th>
    <th>Volunteer6</th>
    <th>Volunteer7</th>
    <th>Volunteer8</th>
    <th>Volunteer9</th>
    <th>Volunteer10</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td colspan="2">Sex</td>
    <td>male</td>
    <td>male</td>
    <td>male</td>
    <td>male</td>
    <td>male</td>
    <td>female</td>
    <td>female</td>
    <td>female</td>
    <td>female</td>
    <td>female</td>
  </tr>
  <tr>
    <td colspan="2">Age</td>
    <td>27</td>
    <td>25</td>
    <td>26</td>
    <td>23</td>
    <td>25</td>
    <td>25</td>
    <td>25</td>
    <td>26</td>
    <td>26</td>
    <td>24</td>
  </tr>
  <tr>
    <td colspan="2">Phone Brand</td>
    <td>Yijia ACE2</td>
    <td>iPhone7</td>
    <td>Huawei nova9</td>
    <td>iPhone13Pro</td>
    <td>Redmi k50u</td>
    <td>JianguoPro2</td>
    <td>iPhone7</td>
    <td>Vivo iQQneo5</td>
    <td>iphone13 mini</td>
    <td>Xiaomi 12S</td>
  </tr>
  <tr>
    <td colspan="2">Operating System<br></td>
    <td>Android13</td>
    <td>iOS15.2.1</td>
    <td>HarmonyOS3.0.0</td>
    <td>iOS16.1</td>
    <td>Android12</td>
    <td>Anroid7.1.1</td>
    <td>iOS11</td>
    <td>Android11</td>
    <td>iOS16.4.1</td>
    <td>Android12</td>
  </tr>
  <tr>
    <td rowspan="2">10Hz Indoor <br>experiments' final coherence</td>
    <td>Rotation Mode</td>
    <td>0.8599</td>
    <td>0.8642</td>
    <td>0.8745</td>
    <td>0.8189</td>
    <td>0.9623</td>
    <td>0.8192</td>
    <td>0.8947</td>
    <td>0.8471</td>
    <td>0.8383</td>
    <td>0.8721</td>
  </tr>
  <tr>
    <td>Shaking Mode</td>
    <td>0.7601</td>
    <td>0.8318</td>
    <td>0..8103</td>
    <td>0.8004</td>
    <td>0.8125</td>
    <td>0.8154</td>
    <td>0.7861</td>
    <td>0.7103</td>
    <td>0.7624</td>
    <td>0.7457</td>
  </tr>
  <tr>
    <td rowspan="2">10Hz Outdoor<br>experiments' final coherence</td>
    <td>Rotation Mode</td>
    <td>0.8596</td>
    <td>0.8423</td>
    <td>0.8575</td>
    <td>0.8056</td>
    <td>0.8301</td>
    <td>0.8427</td>
    <td>0.8475</td>
    <td>0.8611</td>
    <td>0.8629</td>
    <td>0.8293</td>
  </tr>
  <tr>
    <td>Shaking Mode</td>
    <td>0.7180</td>
    <td>0.7121</td>
    <td>0.6293</td>
    <td>0.6733</td>
    <td>0.5989</td>
    <td>0.7791</td>
    <td>0.6126</td>
    <td>0.7432</td>
    <td>0.6255</td>
    <td>0.7949</td>
  </tr>
  <tr>
    <td rowspan="2">60Hz experiments' final coherence</td>
    <td>Rotation Mode</td>
    <td>0.7581</td>
    <td colspan="9" rowspan="4"></td>
  </tr>
  <tr>
    <td>Shaking Mode</td>
    <td>0.5728</td>
  </tr>
  <tr>
    <td rowspan="2">100Hz experiments' final coherence</td>
    <td>Rotation Mode</td>
    <td>0.7629</td>
  </tr>
  <tr>
    <td>Shaking Mode</td>
    <td>0.7840</td>
  </tr>
</tbody>
</table>
</escape>
