# 實作8: 零基礎Python快速入門與實作

## 暖身: 請同學先參考Lab8-3的程式, 並將老虎的圖像在Colab中Show出來

<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/141663909-675e94e0-6cc4-445d-b207-4eac2833b6ed.png" 
      width="30%" height="30%">
    </div>
    
## Lab 8-1 零基礎Python快速入門與實作, 1/2, W13

### 實作體驗用Python Code, [link](https://github.com/Grace-TA/ES-Fall2021/blob/main/Lab8_Python/python1.py)

### 實作1175a + Final Result

<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/141648771-c537c6e3-5dbe-432a-8d4e-df2b0158b3b4.png" 
      width="60%" height="60%">
    </div>

---

## Lab 8-2 零基礎Python快速入門與實作, 2/2, W14

### 實作體驗用Python Code, [link](https://github.com/Grace-TA/ES-Fall2021/blob/main/Lab8_Python/python2.py)

### 實作1185 + Final Result

<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/141650308-c39531f4-adec-4b35-9a4a-928d1c92f9a4.png" 
      width="60%" height="60%">
    </div>
   
---

## Lab 8-3 建立我們的Colab Notebook (e.g., Filename: ShowPhoto.ipynb), 用Python來看一下有哪些圖像可進行分類 (Image Classification)

### 實作體驗用Python Code, [link](https://github.com/Grace-TA/ES-Fall2021/blob/main/Lab8_Python/show-image.py)

### 實作: Show teapot

<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/141649607-1f654dab-f4f0-49bf-bf94-5f71fbca7107.png" 
      width="30%" height="30%">
    </div>
    


### 實作: Show turtle

<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/141649609-636c620b-62c2-4072-90f9-354752fc7616.png" 
      width="30%" height="30%">
    </div>
    


實作: 請自選一個來試試

<div align="center">
     <img 
      src="https://user-images.githubusercontent.com/89304181/141649613-5026711d-f772-4b3a-8523-4eb29d188dff.png" 
      width="30%" height="30%">
    </div>
    


Exp: Show Dog

````python
"""## 2. 選擇圖像 
您可以選擇以下圖像之一，或使用您自己的圖像。 請記住，模型的輸入大小各不相同，其中一些使用動態輸入大小（啟用對未縮放圖像的推斷）。 鑑於此，方法 load_image 已經將圖像重新縮放為預期格式。

選項: ['老虎'，'公共汽車'，'汽車'，'貓'，'狗'，'蘋果'，'烏龜'，'火烈鳥'，'鋼琴'，'蜂窩'，'茶壺']

param ['tiger', 'bus', 'car', 'cat', 'dog', 'apple', 'turtle', 'flamingo', 'piano', 'honeycomb', 'teapot']
"""

print('*** Done by %s at ' % ts3,today, type(today))
## Demo: Show tiger

image_name = 'dog' 

images_for_test_map = {
    "tiger": "https://upload.wikimedia.org/wikipedia/commons/b/b0/Bengal_tiger_%28Panthera_tigris_tigris%29_female_3_crop.jpg",
    "bus": "https://upload.wikimedia.org/wikipedia/commons/6/63/LT_471_%28LTZ_1471%29_Arriva_London_New_Routemaster_%2819522859218%29.jpg",
    "car": "https://upload.wikimedia.org/wikipedia/commons/4/49/2013-2016_Toyota_Corolla_%28ZRE172R%29_SX_sedan_%282018-09-17%29_01.jpg",
    "cat": "https://upload.wikimedia.org/wikipedia/commons/4/4d/Cat_November_2010-1a.jpg",
    "dog": "https://upload.wikimedia.org/wikipedia/commons/archive/a/a9/20090914031557%21Saluki_dog_breed.jpg",
    "apple": "https://upload.wikimedia.org/wikipedia/commons/1/15/Red_Apple.jpg",
    "turtle": "https://upload.wikimedia.org/wikipedia/commons/8/80/Turtle_golfina_escobilla_oaxaca_mexico_claudio_giovenzana_2010.jpg",
    "flamingo": "https://upload.wikimedia.org/wikipedia/commons/b/b8/James_Flamingos_MC.jpg",
    "piano": "https://upload.wikimedia.org/wikipedia/commons/d/da/Steinway_%26_Sons_upright_piano%2C_model_K-132%2C_manufactured_at_Steinway%27s_factory_in_Hamburg%2C_Germany.png",
    "honeycomb": "https://upload.wikimedia.org/wikipedia/commons/f/f7/Honey_comb.jpg",
    "teapot": "https://upload.wikimedia.org/wikipedia/commons/4/44/Black_tea_pot_cropped.jpg",
}

img_url = images_for_test_map[image_name]
image, original_image = load_image(img_url, image_size, dynamic_size, max_dynamic_size)
show_image(image, 'Scaled image')

````

![image](https://user-images.githubusercontent.com/89304181/142746689-074c1278-2690-4542-8554-74c1783f2d19.png)

### Reference Code:

![image](https://user-images.githubusercontent.com/89304181/142749427-c22c154d-f2ac-40cc-ba63-2deccfeb88eb.png)
