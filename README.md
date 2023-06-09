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


<table class="tg" style="undefined;table-layout: fixed; width: 1184px">
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
    <th class="tg-c3ow" colspan="2"><span style="font-weight:bold">Characteristic</span></th>
    <th class="tg-7btt">Volunteer1</th>
    <th class="tg-7btt">Volunteer2</th>
    <th class="tg-7btt">Volunteer3</th>
    <th class="tg-7btt">Volunteer4</th>
    <th class="tg-7btt">Volunteer5</th>
    <th class="tg-7btt">Volunteer6</th>
    <th class="tg-7btt">Volunteer7</th>
    <th class="tg-7btt">Volunteer8</th>
    <th class="tg-7btt">Volunteer9</th>
    <th class="tg-7btt">Volunteer10</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-7btt" colspan="2"><span style="font-weight:bold">Sex</span></td>
    <td class="tg-c3ow">male</td>
    <td class="tg-c3ow">male</td>
    <td class="tg-c3ow">male</td>
    <td class="tg-c3ow">male</td>
    <td class="tg-c3ow">male</td>
    <td class="tg-c3ow">female</td>
    <td class="tg-c3ow">female</td>
    <td class="tg-c3ow">female</td>
    <td class="tg-c3ow">female</td>
    <td class="tg-c3ow">female</td>
  </tr>
  <tr>
    <td class="tg-7btt" colspan="2">Age</td>
    <td class="tg-c3ow">27</td>
    <td class="tg-c3ow">25</td>
    <td class="tg-c3ow">26</td>
    <td class="tg-c3ow">23</td>
    <td class="tg-c3ow">25</td>
    <td class="tg-c3ow">25</td>
    <td class="tg-c3ow">25</td>
    <td class="tg-c3ow">26</td>
    <td class="tg-c3ow">26</td>
    <td class="tg-c3ow">24</td>
  </tr>
  <tr>
    <td class="tg-7btt" colspan="2">Phone Brand</td>
    <td class="tg-c3ow">Yijia ACE2</td>
    <td class="tg-c3ow">iPhone7</td>
    <td class="tg-c3ow">Huawei nova9</td>
    <td class="tg-c3ow">iPhone13Pro</td>
    <td class="tg-c3ow">Redmi k50u</td>
    <td class="tg-c3ow">JianguoPro2</td>
    <td class="tg-c3ow">iPhone7</td>
    <td class="tg-c3ow">Vivo iQQneo5</td>
    <td class="tg-c3ow">iphone13 mini</td>
    <td class="tg-c3ow">Xiaomi 12S</td>
  </tr>
  <tr>
    <td class="tg-7btt" colspan="2">Operating System<br></td>
    <td class="tg-c3ow">Android13</td>
    <td class="tg-c3ow">iOS15.2.1</td>
    <td class="tg-c3ow">HarmonyOS3.0.0</td>
    <td class="tg-c3ow">iOS16.1</td>
    <td class="tg-c3ow">Android12</td>
    <td class="tg-c3ow">Anroid7.1.1</td>
    <td class="tg-c3ow">iOS11</td>
    <td class="tg-c3ow">Android11</td>
    <td class="tg-c3ow">iOS16.4.1</td>
    <td class="tg-c3ow">Android12</td>
  </tr>
  <tr>
    <td class="tg-7btt" rowspan="2">10Hz Indoor <br>experiments' final coherence</td>
    <td class="tg-7btt">Rotation Mode</td>
    <td class="tg-c3ow">0.8599</td>
    <td class="tg-c3ow">0.8642</td>
    <td class="tg-c3ow">0.8745</td>
    <td class="tg-c3ow">0.8189</td>
    <td class="tg-c3ow">0.9623</td>
    <td class="tg-c3ow">0.8192</td>
    <td class="tg-c3ow">0.8947</td>
    <td class="tg-c3ow">0.8471</td>
    <td class="tg-c3ow">0.8383</td>
    <td class="tg-c3ow">0.8721</td>
  </tr>
  <tr>
    <td class="tg-amwm">Shaking Mode</td>
    <td class="tg-baqh">0.7601</td>
    <td class="tg-baqh">0.8318</td>
    <td class="tg-baqh">0..8103</td>
    <td class="tg-baqh">0.8004</td>
    <td class="tg-baqh">0.8125</td>
    <td class="tg-baqh">0.8154</td>
    <td class="tg-baqh">0.7861</td>
    <td class="tg-baqh">0.7103</td>
    <td class="tg-baqh">0.7624</td>
    <td class="tg-baqh">0.7457</td>
  </tr>
  <tr>
    <td class="tg-7btt" rowspan="2">10Hz Outdoor<br>experiments' final coherence</td>
    <td class="tg-7btt">Rotation Mode</td>
    <td class="tg-c3ow">0.8596</td>
    <td class="tg-c3ow">0.8423</td>
    <td class="tg-c3ow">0.8575</td>
    <td class="tg-c3ow">0.8056</td>
    <td class="tg-c3ow">0.8301</td>
    <td class="tg-c3ow">0.8427</td>
    <td class="tg-c3ow">0.8475</td>
    <td class="tg-c3ow">0.8611</td>
    <td class="tg-c3ow">0.8629</td>
    <td class="tg-c3ow">0.8293</td>
  </tr>
  <tr>
    <td class="tg-amwm">Shaking Mode</td>
    <td class="tg-baqh">0.7180</td>
    <td class="tg-baqh">0.7121</td>
    <td class="tg-baqh">0.6293</td>
    <td class="tg-baqh">0.6733</td>
    <td class="tg-baqh">0.5989</td>
    <td class="tg-baqh">0.7791</td>
    <td class="tg-baqh">0.6126</td>
    <td class="tg-baqh">0.7432</td>
    <td class="tg-baqh">0.6255</td>
    <td class="tg-baqh">0.7949</td>
  </tr>
  <tr>
    <td class="tg-7btt" rowspan="2">60Hz experiments' final coherence</td>
    <td class="tg-7btt">Rotation Mode</td>
    <td class="tg-c3ow">0.7581</td>
    <td class="tg-hafo" colspan="9" rowspan="4"></td>
  </tr>
  <tr>
    <td class="tg-amwm">Shaking Mode</td>
    <td class="tg-baqh">0.5728</td>
  </tr>
  <tr>
    <td class="tg-7btt" rowspan="2">100Hz experiments' final coherence</td>
    <td class="tg-7btt">Rotation Mode</td>
    <td class="tg-c3ow">0.7629</td>
  </tr>
  <tr>
    <td class="tg-7btt">Shaking Mode</td>
    <td class="tg-c3ow">0.7840</td>
  </tr>
</tbody>
</table>
</escape>

##  6.The final coherence comparison of two legal devices and the attacker

**10 volunteers shake two legal devices together, and we use a camera to randomly record the trajectory of one of the devices and estimate the acceleration. Man-in-the-middle attacker using estimated acceleration to attack legal devices. We conducted a total of 45*3=135 experiments, and the experimental results are stored in the "./Two legal devices&Attacker" folder. All the final coherence of the two mobile phones and the attacker at 10Hz, 60Hz and 100Hz are stored in the "./Two legal devices&Attacker/The final coherence comparison of two legal devices and the attacker.xlsx".**

* **1. Take the results in the path "Two_legal_devices&Attacker/1-Yijia ACE2 Android13/2-iPhone7 iOS15.2.1" as an example. The attacker randomly attacks the device indicated in the first legend, and the acceleration curve of the attacked device is red.**

**10Hz:**
  
<div align=center> 

 ![Alt](./Two_legal_devices&Attacker/1-Yijia%20ACE2%20Android13/2-iPhone7%20iOS15.2.1/1%262_10Hz.gif) 
  <center><p> Shaking volunteer1 and volunteer2's devices in one hand<center><p>

  ![Alt](./Two_legal_devices&Attacker/1-Yijia%20ACE2%20Android13/2-iPhone7%20iOS15.2.1/Acc%20comparison_10Hz.jpg)
  <center><p> The acceleration comparison of two legal devices and the attacker <center><p>

</div>

**The final coherence of device1 and device2 shaking in one hand is 0.723.
The attacker selects device2, and the final coherence of attacker's estimated acceleration and device2's measures acceleraion is 0.876.**

**60Hz:**

<div align=center>

![Alt](./Two_legal_devices&Attacker/1-Yijia%20ACE2%20Android13/2-iPhone7%20iOS15.2.1/1%262_60Hz.gif)
<center><p> Shaking volunteer1 and volunteer2's devices in one hand  <center><p>

![Alt](./Two_legal_devices&Attacker/1-Yijia%20ACE2%20Android13/2-iPhone7%20iOS15.2.1/Acc%20comparison_60Hz.jpg)
<center><p> The acceleration comparison of two legal devices and the attacker   <center><p>
</div>

**The final coherence of device1 and device2 shaking in one hand is 0.641.
The attacker selects device2, and the final coherence of attacker's estimated acceleration and device2's measures acceleraion is 0.792.**

**100Hz:**

<div align=center>

![Alt](./Two_legal_devices&Attacker/1-Yijia%20ACE2%20Android13/2-iPhone7%20iOS15.2.1/1%262_100Hz.gif)
<center><p> Shaking volunteer1 and volunteer2's devices in one hand  <center><p>

![Alt](./Two_legal_devices&Attacker/1-Yijia%20ACE2%20Android13/2-iPhone7%20iOS15.2.1/Acc%20comparison_100Hz.jpg)
<center><p> The acceleration comparison of two legal devices and the attacker   <center><p>
</div>

**The final coherence of device1 and device2 shaking in one hand is 0.853.
The attacker selects device2, and the final coherence of attacker's estimated acceleration and device2's measures acceleraion is 0.874.**

 * **2. We draw the results as follow:** 
  
**The final coherence comparison of two legal devices and the attacker in 10Hz**
<div align=center> 

 ![Alt](./Two_legal_devices%26Attacker/Comparison%20of%20final%20coherence_10Hz.png ) 

</div>

**The final coherence comparison of two legal devices and the attacker in 60Hz**

<div align=center> 

 ![Alt](./Two_legal_devices%26Attacker/Comparison%20of%20final%20coherence_60Hz.png ) 

</div>

**The final coherence comparison of two legal devices and the attacker in 100Hz**

<div align=center> 

 ![Alt](./Two_legal_devices%26Attacker/Comparison%20of%20final%20coherence_100Hz.png ) 

</div>

##  7. In indoor and outdoor real environments, three wirst rotaiton modes (pitch, roll, yaw) in 10Hz, 60Hz, 100Hz are performed.

**10 volunteers conducted experiments in three kinds of wirst rotation modes (pitch, roll, yaw) in indoor and outdoor real environments, and each mode collected accelerations at three frequencies of 10Hz, 60Hz and 100H. A total of 10*2*3*3=180 experiments were performed. Experimental results are stored in the "./Wrist_rotation" folder.**

<div align=center>

![Alt](./Wrist_rotation/Three%20modes%20of%20the%20device.jpg) 

</div>

* **We take the results of the volunteer1 as an example to show.**

   **1.1 Indoor Pitch Mode**
<div align=center>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/1-pitch/1-Yijia%20ACE2%20Android13_pitch_10Hz.gif)
<center><p> 10Hz   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/1-pitch/Acc%20comparison_10Hz.jpg)
<center><p> The final coherence of two accelerations is 0.872   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/1-pitch/1-Yijia%20ACE2%20Android13_pitch_60Hz.gif)
<center><p> 60Hz   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/1-pitch/Acc%20comparison_60Hz.jpg)
<center><p> The final coherence of two accelerations is 0.945   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/1-pitch/1-Yijia%20ACE2%20Android13_pitch_100Hz.gif)
<center><p> 100Hz   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/1-pitch/Acc%20comparison_100Hz.jpg)
<center><p> The final coherence of two accelerations is 0.844   <center><p>

</div>

   **1.2 Indoor Roll Mode**
<div align=center>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/2-roll/1-Yijia%20ACE2%20Android13_roll_10Hz.gif)
<center><p> 10Hz   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/2-roll/Acc%20comparison_10Hz.jpg)
<center><p> The final coherence of two accelerations is 0.823   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/2-roll/1-Yijia%20ACE2%20Android13_roll_60Hz.gif)
<center><p> 60Hz   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/2-roll/Acc%20comparison_60Hz.jpg)
<center><p> The final coherence of two accelerations is 0.835   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/2-roll/1-Yijia%20ACE2%20Android13_roll_100Hz.gif)
<center><p> 100Hz   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/3-yaw/Acc%20comparison_100Hz.jpg)
<center><p> The final coherence of two accelerations is 0.774   <center><p>

</div>

   **1.3 Indoor Yaw Mode**
<div align=center>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/3-yaw/1-Yijia%20ACE2%20Android13_yaw_10Hz.gif)
<center><p> 10Hz   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/3-yaw/Acc%20comparison_10Hz.jpg)
<center><p> The final coherence of two accelerations is 0.697   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/3-yaw/1-Yijia%20ACE2%20Android13_yaw_60Hz.gif)
<center><p> 60Hz   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/3-yaw/Acc%20comparison_60Hz.jpg)
<center><p> The final coherence of two accelerations is 0.658   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/3-yaw/1-Yijia%20ACE2%20Android13_yaw_100Hz.gif)
<center><p> 100Hz   <center><p>

![Alt](./Wrist_rotation/Indoor/1-Yijia%20ACE2%20Android13/3-yaw/Acc%20comparison_100Hz.jpg)
<center><p> The final coherence of two accelerations is 0.698   <center><p>

</div>


**2.1 Outdoor Pitch Mode**
<div align=center>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/1-pitch/1-Yijia%20ACE2%20Android13_pitch_10Hz.gif)
<center><p> 10Hz   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/1-pitch/Acc%20comparison_10Hz.jpg)
<center><p> The final coherence of two accelerations is 0.773   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/1-pitch/1-Yijia%20ACE2%20Android13_pitch_60Hz.gif)
<center><p> 60Hz   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/1-pitch/Acc%20comparison_60Hz.jpg)
<center><p> The final coherence of two accelerations is 0.896   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/1-pitch/1-Yijia%20ACE2%20Android13_pitch_100Hz.gif)
<center><p> 100Hz   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/1-pitch/Acc%20comparison_100Hz.jpg)
<center><p> The final coherence of two accelerations is 0.902   <center><p>



</div>


**2.2 Outdoor Roll Mode**
<div align=center>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/2-roll/1-Yijia%20ACE2%20Android13_roll_10Hz.gif)
<center><p> 10Hz   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/2-roll/Acc%20comparison_10Hz.jpg)
<center><p> The final coherence of two accelerations is 0.611   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/2-roll/1-Yijia%20ACE2%20Android13_roll_60Hz.gif)
<center><p> 10Hz   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/2-roll/Acc%20comparison_60Hz.jpg)
<center><p> The final coherence of two accelerations is 0.857   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/2-roll/1-Yijia%20ACE2%20Android13_roll_100Hz.gif)
<center><p> 10Hz   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/2-roll/Acc%20comparison_100Hz.jpg)
<center><p> The final coherence of two accelerations is 0.866   <center><p>

</div>


**2.3 Outdoor Yaw Mode**
<div align=center>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/3-yaw/1-Yijia%20ACE2%20Android13_yaw_10Hz.gif)
<center><p> 10Hz   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/3-yaw/Acc%20comparison_10Hz.jpg)
<center><p> The final coherence of two accelerations is 0.611   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/3-yaw/1-Yijia%20ACE2%20Android13_yaw_60Hz.gif)
<center><p> 10Hz   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/3-yaw/Acc%20comparison_60Hz.jpg)
<center><p> The final coherence of two accelerations is 0.611   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/3-yaw/1-Yijia%20ACE2%20Android13_yaw_100Hz.gif)
<center><p> 10Hz   <center><p>

![Alt](./Wrist_rotation/Outdoor/1-Yijia%20ACE2%20Android13/3-yaw/Acc%20comparison_100Hz.jpg)
<center><p> The final coherence of two accelerations is 0.611   <center><p>

</div>

* **We save all the results in "./Wirst_rotation/Results of the final coherence.xlsx", and draw the results as follows:**
  
  **Indoor comparison of final coherence in pitch mode:**
<div align=center>


![Alt](./Wrist_rotation/Indoor/Final%20coherence%20of%20pitch%20mode.png)

</div>

  **Indoor comparison of final coherence in roll mode:**
<div align=center>


![Alt](./Wrist_rotation/Indoor/Final%20coherence%20of%20roll%20mode.png)

</div>

  **Indoor comparison of final coherence in yaw mode:**
<div align=center>


![Alt](./Wrist_rotation/Indoor/Final%20coherence%20of%20yaw%20mode.png)

</div>

  **Outdoor comparison of final coherence in pitch mode:**
<div align=center>


![Alt](./Wrist_rotation/Outdoor/Final%20coherence%20of%20pitch%20mode.png)

</div>

  **Outdoor comparison of final coherence in roll mode:**
<div align=center>


![Alt](./Wrist_rotation/Outdoor/Final%20coherence%20of%20roll%20mode.png)

</div>

**Outdoor comparison of final coherence in yaw mode:**
<div align=center>


![Alt](./Wrist_rotation/Outdoor/Final%20coherence%20of%20yaw%20mode.png)

</div>