# (2012) Guided Image Filtering
`image shape = (512, 384)`<br>
`Hyperparameters: r=60, eps=0.00001`<br>
- guided gilter ， opencv的boxfilter運算時間 : 0.0040 秒
- guided gilter ， 自定義boxfilter的運算時間 : 7.8414 秒
- guided gilter ， opencv內建的GF運算時間 : 0.0030 秒<br><br>
![7c984509-6464-4064-b17f-b7e6a7f979c9](https://github.com/user-attachments/assets/90be0fc0-5e05-4de1-ae46-9641ab099a6f)
#

`image shape = (750, 916)`<br>
`Hyperparameters: r=9, eps=0.01`<br>
- guided gilter ， opencv的boxfilter運算時間 : 0.0140 秒
- guided gilter ， 自定義boxfilter的運算時間 : 12.7071 秒
- guided gilter ， opencv內建的GF運算時間 : 0.0105 秒<br><br>
![fbb711ad-bbbf-4ef4-9890-b9a6fa1f26b3](https://github.com/user-attachments/assets/7ba6d4be-e36d-401d-b4c3-401fa1074903)
#

`image shape = (353, 800)`<br>
`Hyperparameters: r=9, eps=0.01`<br>
- guided gilter ， opencv的boxfilter運算時間 : 0.0100 秒
- guided gilter ， 自定義boxfilter的運算時間 : 7.8759 秒
- guided gilter ， opencv內建的GF運算時間 : 0.0060 秒<br><br>
![33649b05-dfc5-4793-a9af-4178b414f288](https://github.com/user-attachments/assets/35a58c1c-b862-449f-bc36-d97645568bd0)
#





Reference : HE, Kaiming; SUN, Jian; TANG, Xiaoou. Guided image filtering. IEEE transactions on pattern analysis and machine intelligence, 2012, 35.6: 1397-1409.<br><br>
引導圖像濾波文章復現<br>
使用python<br><br>
- 原文PDF &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;：[點擊此連結](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6319316)
- 原文DOI &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;：[點擊此連結](https://doi.org/10.1109/TPAMI.2012.213)
- 原作者matlab code &nbsp;：[點擊此連結](https://kaiminghe.github.io/eccv10/index.html)<br><br>


操作說明 
---
打開 `guided filter.ipynb` , 修改圖片名稱並執行即可<br><br>



result名稱說明
---
- image &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : 原圖
- image_gray &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : 原圖轉灰階
- d &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : 深度圖
- guided_filter (opencv_boxFilter) : 使用opencv的boxfilter運算的guided filter
- guided_filter (defboxFilter)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : 使用自定義boxfilter運算的guided filter
- guided_filter (opencv)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : 使用opencv內建的guided filter<br><br>


---
關於
---

- 聯繫 : jayabc321@gmail.com
- 復現 : 蕭晉杰
- 時間 : 2024.09.12
