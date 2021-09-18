# Synthetic-Dataset-Navigation-Ground Robot


## Information
Dataset for paper ->  "Synthetic dataset for navigation tasks of autonomous systems and ground robots".

Conference -> http://itnt-conf.org/index.php


## Citing
If you find this repository useful for your research please use the following bibtex citations

```
@article{ ,
  title={Synthetic dataset for navigation tasks of autonomous systems and ground robots},
  author={Larisa Zherdeva, Evgeniy Minaev, Denis Zherdev, Vladimir Fursov},
  journal={ },
  volume={ },
  number={ },
  pages={ -- },
  year={2021},
  publisher={IEEE}
}
```

# Dataset structure
<!--ts-->

   0. [Trajectory File](#Trajectory-file)
   1. [Directory Tree](#Directory-Tree)
   2. [Relief Surface](#Relief-Surface)
   3. [Flat Surface](#Flat-Surface)
      * [Type a wood](#Type-a)
      * [Type b gravel](#Type-b)
      * [Type c grass](#Type-c)
      * [Type d sand](#Type-d)
      * [Type e mud](#Type-e)
      * [Type f street](#Type-f)
      * [Type g concrete](#Type-g)
      * [Type h metal](#Type-h)
  
   4. [Motion Blur](#Motion-Blur)
      * [Type b gravel](#MB-Type-b)
      * [Type f street](#MB-Type-f)

5. [Credits](#Credits)
      
<!--te-->
<br/>

# Trajectory File
*.csv file decryption*
<br/>
| time, sec | x axis, cm | y axis, cm | z axis, cm | roll, ° | pitch, ° | yaw, ° | distance to surface<br/>(*experimental for relief*), cm | speed, km/h |
|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
| ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 7.925049 | 336.818604 | 100.622841 | 19.972425 | -0.027649 | 0.039745 | 51.9977 | 19.972424 | 1.789359 |
| ... | ... | ... | ... | ... | ... | ... | ... | ... |
        
[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>
      
# Directory Tree

**You can download FULL dataset in one click:  ![DOWNLOAD DATASET](https://storage-liav.ipsiras.ru/index.php/s/smK9yMfEdwdPFeQ)**
<br/>

```
├───FlatSurface_MotionBlurOFF/
│   │
│   ├───a_wood/
│   │   │
│   │   ├───01_line/
│   │   │   └───01_material/
│   │   │       ├───speed_2/
│   │   │       │   ├─── img_001.png
│   │   │       │   ├─── ...
│   │   │       │   └─── file.csv
│   │   │       ├───speed_8/
│   │   │       │   └─── ...
│   │   │       └───speed_15/
│   │   │           └─── ...
│   │   │
│   │   ├───02_circle/
│   │   │   └───.../
│   │   │       └───.../
│   │   │           └───...
│   │   │
│   │   └───.../
│   │
│   ├───b_stone/
│   │   └───.../
│   │
│   └───.../
│
├───FlatSurface_MotionBlurON/
│   │
│   ├───b_stone/
│   │   │
│   │   └───04_figure eight_motionblur/
│   │       └───01_material/
│   │           ├───speed_2/
│   │           │   ├─── img_001.png
│   │           │   ├─── ...
│   │           │   └─── file.csv
│   │           ├───speed_8/
│   │           │   └─── ...
│   │           └───speed_15/
│   │               └─── ...
│   │
│   └───f_street/
│       └───.../
│
└───Relief_MotionBlurOFF/
    │
    ├───b_stone/
    │   └───.../
    └───.../
```
[:arrow_up:Dataset structure](#Dataset-structure)
<br/>


# Relief Surface
**..or you can download only specific data**
<br/>
*Motion Blur OFF*
<br/>
TRAJECTORY TYPE: **FIGURE EIGHT**
<br/>
<img src="/img_table/relief_gif.gif" width="250">
<br/>
| Surface Type | b - *gravel / stones* | d - *sand* | f - *street  /  bricks* |
|:---------:|:---------:|:---------:|:---------:|
| Img |![](/img_table/relief_b.png)<br/> [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/APKMTkqnrPygaRF) | ![](/img_table/relief_d.png)<br/> [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/y9BAbQqt7JHag6B) | ![](/img_table/relief_f.png)<br/> [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/KJ74cQKgfGbn3CA) |

[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>
___


# Flat Surface
**..or you can download only specific data**
<br/>
## Type a
*wood  /  parquet  /  laminate*
<br/>
*Motion Blur OFF*
| Surface<br/> Image | LINE TRAJECTORY | CIRCLE TRAJECTORY<br/> ![](/img_table/circle.png) | RECTANGLE TRAJECTORY<br/> ![](/img_table/req.png) | FIG. EIGHT TRAJECTORY<br/> ![](/img_table/fig.png) | NON-INTER. TRAJECTORY<br/> ![](/img_table/nonIntersect.png) | INTER. TRAJECTORY<br/> ![](/img_table/Intersect.png) |
|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
| ![](/img_table/a_01.png) 01_material | :x: | ![](/img_table/circle_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/fiDz5DJE8bqbn5X)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/zfBa2BQsn3ad6bA)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/6dSicdW5ZLWHWwy) | ![](/img_table/req_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/AKf5tDFWFzMrXaH)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/6Bg2HTbkAYtmsmC)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/y6Q5etcC5HEmWWD) | ![](/img_table/fig_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/HjeoXkjJRkL9sDM)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/DjxyAimoQZNgXSW)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/9ykqbzT2kKCEooM) | ![](/img_table/nonIntersect_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/yXTCR9PwKogxo6F)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/tL7DiTaT74LrSTJ)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/YaKqF2t3MXDyHG7) | ![](/img_table/Intersect_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/sRbyd5FfT8gXJW7)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/SWzqPJqW5TAkePd)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/EWCfJMe6oxStGDt) |
| ![](/img_table/a_02.png) 02_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/qyjSaSTHdH89MJC) | :x: | :x: |
| ![](/img_table/a_03.png) 03_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/rKc4xi5MoZibCba) | :x: | :x: |
| ![](/img_table/a_04.png) 04_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/WCC7L3K37sErfye) | :x: | :x: |
| ![](/img_table/a_05.png) 05_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/MFpqBLQnD6Di9cZ) | :x: | :x: |
| ![](/img_table/a_06.png) 06_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/kt8zeqaySZr2Nn7) | :x: | :x: |
| ![](/img_table/a_07.png) 07_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/ebxwkYFAYsfSk9Q) | :x: | :x: |
| ![](/img_table/a_08.png) 08_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/FDXaEq9Rn2o7C2D) | :x: | :x: |

[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>

## Type b
*gravel  /  stones*
<br/>
*Motion Blur OFF*
| Surface<br/> Image | LINE TRAJECTORY | CIRCLE TRAJECTORY<br/> ![](/img_table/circle.png) | RECTANGLE TRAJECTORY<br/> ![](/img_table/req.png) | FIG. EIGHT TRAJECTORY<br/> ![](/img_table/fig.png) | NON-INTER. TRAJECTORY<br/> ![](/img_table/nonIntersect.png) | INTER. TRAJECTORY<br/> ![](/img_table/Intersect.png) |
|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
| ![](/img_table/b_01.png) 01_material | :x: | ![](/img_table/circle_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/4axzScSne64bK2Z)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/gZNk5xKfB4a44Pd)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/QzJe3p8D2t3endE) | ![](/img_table/req_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/zcc7PDEKBgKLbai)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/WHHG5Z4t5JHiGjz)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/dZLySEoDXS66RRK) | ![](/img_table/fig_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/idCdNFXQdxBfEp4)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/2P9N8zzBmnawSLt)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/LwCCLkQpwJL9nF9) | ![](/img_table/nonIntersect_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/4PZnyBXj56Bxz37)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/w54wExqAN6NjtAb)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/qDNx9qckidPTB9x) | :x: |
| ![](/img_table/b_02.png) 02_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/zT6Mq5bSnEz82ik) | :x: | :x: |
| ![](/img_table/b_03.png) 03_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/rfoiian3cH5R2W4) | :x: | :x: |
| ![](/img_table/b_04.png) 04_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/qCbwsQsEpwmrXDW) | :x: | :x: |

[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>

## Type c
*grass  /  leaves*
<br/>
*Motion Blur OFF*
| Surface<br/> Image | LINE TRAJECTORY | CIRCLE TRAJECTORY<br/> ![](/img_table/circle.png) | RECTANGLE TRAJECTORY<br/> ![](/img_table/req.png) | FIG. EIGHT TRAJECTORY<br/> ![](/img_table/fig.png) | NON-INTER. TRAJECTORY<br/> ![](/img_table/nonIntersect.png) | INTER. TRAJECTORY<br/> ![](/img_table/Intersect.png) |
|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
| ![](/img_table/c_01.png) 01_material | :x: | ![](/img_table/circle_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/XdCcPRnokCA9CTp)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/DjHTS5DLcbqAqNY)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/TqiNPDE6bS3fNic) | ![](/img_table/req_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/362TYYEXHGw3CjT)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/2watNXsYjiY49PH)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/irjADBaJ2spPGEk) | ![](/img_table/fig_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/ojcodfiRKmd3NHt)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/4qy87zrNW99kS9G)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/8dsey4y6rM6M7nY) | ![](/img_table/nonIntersect_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/MdPSQp9JMNjQM2J)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/FbPYLpizb78oLEw)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/fGF5nwZBKKgtsmJ) | ![](/img_table/Intersect_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/aS3fCmzKaBEzz9Q)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/TKFxT8jzCtMDF8i)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/cANR8PnBXaRCXjn) |
| ![](/img_table/c_02.png) 02_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/3L8tZCcAMyae2oe) | :x: | :x: |
| ![](/img_table/c_03.png) 03_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/cKkyi7WrH9P48ZE) | :x: | :x: |
| ![](/img_table/c_04.png) 04_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/YGDma5Zaw6TKnAw) | :x: | :x: |

[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>

## Type d
*sand*
<br/>
*Motion Blur OFF*
| Surface<br/> Image | LINE TRAJECTORY | CIRCLE TRAJECTORY<br/> ![](/img_table/circle.png) | RECTANGLE TRAJECTORY<br/> ![](/img_table/req.png) | FIG. EIGHT TRAJECTORY<br/> ![](/img_table/fig.png) | NON-INTER. TRAJECTORY<br/> ![](/img_table/nonIntersect.png) | INTER. TRAJECTORY<br/> ![](/img_table/Intersect.png) |
|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
| ![](/img_table/d_01.png) 01_material | :x: | ![](/img_table/circle_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/t7TfJzTLZpEGHRp)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/EtZGBdY3t6YByQJ)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/K5q6Tkmrxa9yBQM) | ![](/img_table/req_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/TMHP7dnafesMZLq)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/Fef8Efxyjn5eNd9)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/GgWs2ZRyGAqBQfB) | ![](/img_table/fig_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/KbCtKtWSkcYCNJG)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/WKYkKs2Xk6ztfjz)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/JxqnXYQF4STXg8E) | ![](/img_table/nonIntersect_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/CYL5xdsEZKHpwGR)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/sFoz6tFYJ5Mw73t)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/kc4o4koYWjL7EM9) | :x: |
| ![](/img_table/d_02.png) 02_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/wg5fsiN7B293CMx) | :x: | :x: |
| ![](/img_table/d_03.png) 03_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/KTAYfFqsGRTCAra) | :x: | :x: |

[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>

## Type e
*mud*
<br/>
*Motion Blur OFF*
| Surface<br/> Image | LINE TRAJECTORY | CIRCLE TRAJECTORY<br/> ![](/img_table/circle.png) | RECTANGLE TRAJECTORY<br/> ![](/img_table/req.png) | FIG. EIGHT TRAJECTORY<br/> ![](/img_table/fig.png) | NON-INTER. TRAJECTORY<br/> ![](/img_table/nonIntersect.png) | INTER. TRAJECTORY<br/> ![](/img_table/Intersect.png) |
|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
| ![](/img_table/e_01.png) 01_material | :x: | ![](/img_table/circle_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/KqDMZd5a6cWEtek)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/gEt4y3yn2JZbmBx)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/29jZGD2YmSL6PnA) | ![](/img_table/req_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/BzyrtxnDSbWcQP6)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/wbCHTkwLTKq3xog)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/GYtxnCzBAxn4S63) | ![](/img_table/fig_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/WjfzYWZWwC5Sndx)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/FbRjxQDcZ25soXZ)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/qMeZ5fpJFra3zrx) | ![](/img_table/nonIntersect_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/J7bXkEjTy9rpwCd)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/gY5r7s65kKmeBxz)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/5KXepwZ4r8CRqat) | :x: |
| ![](/img_table/e_02.png) 02_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/jGrgYoLCGBpM98p) | :x: | :x: |
| ![](/img_table/e_03.png) 03_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/W3gWoTf3JTorc2k) | :x: | :x: |

[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>

## Type f
*street  /  bricks*
<br/>
*Motion Blur OFF*
| Surface<br/> Image | LINE TRAJECTORY | CIRCLE TRAJECTORY<br/> ![](/img_table/circle.png) | RECTANGLE TRAJECTORY<br/> ![](/img_table/req.png) | FIG. EIGHT TRAJECTORY<br/> ![](/img_table/fig.png) | NON-INTER. TRAJECTORY<br/> ![](/img_table/nonIntersect.png) | INTER. TRAJECTORY<br/> ![](/img_table/Intersect.png) |
|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
| ![](/img_table/f_01.png) 01_material | :x: | ![](/img_table/circle_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/wmsP8QJHckgw5XG)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/MzbfQLX6xCPEPdx)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/8zDqd4AX2XnsXH4) | ![](/img_table/req_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/x3GsiqHt3Ydjxey)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/fKE7r4dZYGYScLy)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/DHdwbEnsZXDETSB) | ![](/img_table/fig_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/ANnsAZGjJXyqGMf)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/9aGXQKptENc7G7T)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/QGQyf4CraHnApbN) | ![](/img_table/nonIntersect_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/XpoCygTcYFpinrn)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/WQqtT8zSFRokBp9)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/8DdsHRfrp7cywEE) | ![](/img_table/Intersect_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/G95zyEBXwo93n7S)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/BFDWJ7qZRjeHEN9)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/BBYegz6cs9dF2XY) |
| ![](/img_table/f_02.png) 02_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/CnCZwPMFZ5dkeYK) | :x: | :x: |
| ![](/img_table/f_03.png) 03_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/yBTRBFK3Rptjpf8) | :x: | :x: |
| ![](/img_table/f_04.png) 04_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/afZH2qtJkEGRoKp) | :x: | :x: |

[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>

## Type g
*asphalt  /  concrete*
<br/>
*Motion Blur OFF*
| Surface<br/> Image | LINE TRAJECTORY | CIRCLE TRAJECTORY<br/> ![](/img_table/circle.png) | RECTANGLE TRAJECTORY<br/> ![](/img_table/req.png) | FIG. EIGHT TRAJECTORY<br/> ![](/img_table/fig.png) | NON-INTER. TRAJECTORY<br/> ![](/img_table/nonIntersect.png) | INTER. TRAJECTORY<br/> ![](/img_table/Intersect.png) |
|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
| ![](/img_table/g_01.png) 01_material | :x: | ![](/img_table/circle_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/dMQLZT67Gg9Zot3)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/itDP7EDPLA6864g)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/fbQt3GWpDG8Lsns) | ![](/img_table/req_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/mP7bwiq89wCY7sk)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/qJBxPJESsZzpqtp)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/fNNE83TZYtY8Mif) | ![](/img_table/fig_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/8yeB6GGDfFTnqBP)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/6bJtDZ2AnWrYbP8)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/fTofWTBsXqobGot) | ![](/img_table/nonIntersect_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/6Sbrk7Ybn6beSBd)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/yWLYtCri48L7aBb)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/7nsW3xwtLkYfcXm) | :x: |
| ![](/img_table/g_02.png) 02_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/q23Hk2Xb9MpABq7) | :x: | :x: |
| ![](/img_table/g_03.png) 03_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/wcoFPF4iTSHWKip) | :x: | :x: |
| ![](/img_table/g_04.png) 04_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/xSWzJAg8Nr7GZir) | :x: | :x: |

[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>

## Type h
*metal*
<br/>
*Motion Blur OFF*
| Surface<br/> Image | LINE TRAJECTORY | CIRCLE TRAJECTORY<br/> ![](/img_table/circle.png) | RECTANGLE TRAJECTORY<br/> ![](/img_table/req.png) | FIG. EIGHT TRAJECTORY<br/> ![](/img_table/fig.png) | NON-INTER. TRAJECTORY<br/> ![](/img_table/nonIntersect.png) | INTER. TRAJECTORY<br/> ![](/img_table/Intersect.png) |
|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
| ![](/img_table/h_01.png) 01_material | :x: | ![](/img_table/circle_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/Esy3iYsPQ7tExJt)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/SFezLfJCcQC4A68)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/WGL8B7ZBDo4wdrd) | ![](/img_table/req_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/dr7mJRP4cDiTeSs)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/ZnZKDRW52sfiA3z)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/4oNpSx5RLeHXwdy) | ![](/img_table/fig_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/b4RHa9w4eFJR4oS)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/gnbdZZdS5EjdRky)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/Mkj3mY6k8m228if) | ![](/img_table/nonIntersect_speeds.png)<br/> :large_blue_circle: [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/KFKL9xgMnZtr8S6)<br/> :red_circle: [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/qiMKNE53z47TJR5)<br/> :green_circle: [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/AQdHxHo5ymkfDcT) | :x: |
| ![](/img_table/h_02.png) 02_material | :x: | :x: | :x: | [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/rWKXabmEWSnWgKR) | :x: | :x: |

[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>
___


# Motion Blur
## MB Type b
*gravel  /  stones*
<br/>
TRAJECTORY TYPE: **FIGURE EIGHT**

| | Speed max = 2 km/h | Speed max = 8 km/h | Speed max = 15 km/h |
|:---------:|:---------:|:---------:|:---------:|
| Motion Blur Amount=0.1 Max=1 | ![](/img_table/mb_b_m1_s2.png)<br/> [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/6GBmER8BpqRkAo9) | ![](/img_table/mb_b_m1_s8.png)<br/> [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/2S5pqZ96JyoGFwt) | ![](/img_table/mb_b_m1_s15.png)<br/> [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/5mSqWM6gpZnpZ3t) |
| Motion Blur Amount=0.1 Max=2 | ![](/img_table/mb_b_m2_s2.png)<br/> [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/FYaxdNPw6B8ogCZ) | ![](/img_table/mb_b_m2_s8.png)<br/> [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/5cWX4QfNZKnx5nd) | ![](/img_table/mb_b_m2_s15.png)<br/> [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/CFzxJgFw9qbdKMF) |

[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>

## MB Type f
*street  /  bricks*
<br/>
TRAJECTORY TYPE: **FIGURE EIGHT**

| | Speed max = 2 km/h | Speed max = 8 km/h | Speed max = 15 km/h |
|:---------:|:---------:|:---------:|:---------:|
| Motion Blur Amount=0.1 Max=1 | ![](/img_table/mb_f_m1_s2.png)<br/> [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/B3nNWHMtZ97HM4K) | ![](/img_table/mb_f_m1_s8.png)<br/> [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/c6QbR8EctJsmowj) | ![](/img_table/mb_f_m1_s15.png)<br/> [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/4YXGSTMRZJd59ed) |
| Motion Blur Amount=0.1 Max=2 | ![](/img_table/mb_f_m2_s2.png)<br/> [2_km/h](https://storage-liav.ipsiras.ru/index.php/s/28NDGrybmMbJmRD) | ![](/img_table/mb_f_m2_s8.png)<br/> [8_km/h](https://storage-liav.ipsiras.ru/index.php/s/Cx4KzSDbJMqEqgp) | ![](/img_table/mb_f_m2_s15.png)<br/> [15_km/h](https://storage-liav.ipsiras.ru/index.php/s/5yM4oc5RTG98L2H) |

[:arrow_up:Dataset structure](#Dataset-structure)
<br/>
<br/>
___


# Credits
Unreal Engine 4:
https://www.unrealengine.com/en-US/

Twinmotion Materials for Unreal Engine:
https://www.unrealengine.com/marketplace/en-US/product/twinmotion-materials
<br/>

# License
This project is licensed under the MIT License
<br/>
