# (2012) Guided Image Filtering
`Hyperparameters: r=60, eps=0.00001`<br>
- guided gilter ， opencv的boxfilter運算時間: 0.0040 秒
- guided gilter ， 自定義boxfilter的運算時間: 7.8414 秒
- guided gilter ， opencv內建的GF運算時間: 0.0030 秒
![7c984509-6464-4064-b17f-b7e6a7f979c9](https://github.com/user-attachments/assets/90be0fc0-5e05-4de1-ae46-9641ab099a6f)
-



Reference : HE, Kaiming; SUN, Jian; TANG, Xiaoou. Guided image filtering. IEEE transactions on pattern analysis and machine intelligence, 2012, 35.6: 1397-1409.<br><br>
引導圖像濾波文章復現<br>
使用python<br><br>
- 原文PDF &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;：[點擊此連結](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6319316)
- 原文DOI &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;：[點擊此連結](https://doi.org/10.1109/TPAMI.2012.213)
- 原作者matlab code &nbsp;：[點擊此連結](https://kaiminghe.github.io/eccv10/index.html)<br><br>


操作說明 
---
把圖片放進 `my dataset` 資料夾，打開 `my_CAP_main.py` 檔案執行即可<br>
結果圖將儲存在 `my result` 資料夾中。<br><br>


result檔案名稱說明
---
- 原圖名稱
- d &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : 深度圖
- local_min_d &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : 深度圖取local_min
- GF_d &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : 取 guide filter(引導圖=原圖, 輸入圖=local_min_d, r=15, eps=1e-3)
- t &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : GF_d 還原的 transmission, &beta; = 1
- clip_t &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; : 截斷(t, 0.1, 0.9)
- my_CAP beta=1.0 &nbsp; : 最終去霧結果圖<br><br>

---
關於
---

- 復現 : 蕭晉杰
- 時間 : 2024.09.12
