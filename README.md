# Keyshot渲染器极简入门教程
## 第一步 : 安装keyshot
### 1.下载安装包和破解文件：
链接：https://pan.baidu.com/s/1rWfBoKXqiJniyA_pmtaapw 提取码：h9q8 

### 2.WIN10系统的话，按下图操作，关闭实时防护
![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/1.png)
![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/2.png)

### 3. 按照这个网页的描述进行安装和破解：http://www.xue51.com/soft/34154.html

### 4. keyshot 9 resources文件夹介绍
修改以下内容需要重启软件才能生效，从网上找到的非官方资源，下载后放到对应文件夹内：

文件夹名称|内容
---|:--:
Environment|环境(灯光)
Materials|材质库
Renderings|渲染完成后的文件默认在这里
Texture|贴图、纹理

![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/8.png)

## 第二步：打开工程开始修改模型
### 1.硬件工程师会制作好模型雏形（.bip 或者 .ksp 文件），收到之后直接打开
示例keyshot工程：GO_Game_Pad : 链接：https://pan.baidu.com/s/16NS7Oex_RKoLJCpKvxYygA 提取码：9a52 
![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/1%20%5B1%5D.png)

### 2.按照顺序，可以做以下几点调整：
#### A.模型：
当需要对模型进行修改的时候，挪动位置和缩放可以在Keyshot里操作，如果需要更加复杂的操作就点击文件->另存为->选择step格式文件，然后用Rhino/Fusion360打开进行修改（也可以找硬件工程师修改）
例子：给屏幕添加显示画面：
![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/11.png)

#### B.材质：
点击左上角的库栏目的《材质》，选中想要的材质直接拖到模型里就行。
Keyshot中文材质库：链接：https://pan.baidu.com/s/1-cWnJklN_R395nGzVNuFmA 提取码：xf5v 
材质安装方式：放在keyshot8 资源文件下的Materials目录下

   I.材质绑定：如果给多个物体赋予相同的材质，系统会进行绑定，之后在右侧材质一栏修改材质的时候，已绑定的多个物体会一起修改，方便批量修改，如果不想绑定，可以右键模型选择解绑，解绑后再赋予材质
   
   II.对材质的编辑（B站搜索《Keyshot 材质》看教程）
   
   ![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/7.png)
#### C.环境：
在左侧的库栏目里的《环境》里找出合适的环境，拖动到主图上，然后在右侧的《环境》里可以进行二次修改（B站搜索《keyshot环境》或者《keyshot灯光》）
![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/2%20%5B1%5D.png)

#### D.照明：
这里选择《基本》选项就行，也可以试下选其他选项看看效果


#### E.相机：
这里可以保存多个镜头并锁定，这样调整视角之后可以快速回到选定的视角；主要设置《视角/焦距》，跟单反相机里的135mm焦距一样，比如50mm的话近大远小很明显，200mm接近正交，近大远小现象不明显，能较为客观地展现尺寸
![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/4.png)

#### F.图像：
这里的分辨率是预览框的分辨率，适配自己的显示器就行，但是横宽比例要与最终出图的比例一致；另外有一些调节选项，不重要，可以在这里调也可以导到PS里面再调
![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/5.png)

### 3.渲染静态图
点击最上面的菜单栏的《渲染》->渲染，在弹出的界面定好出图的最终分辨率，必须把《选项》一栏的抗锯齿级别和阴影拉满，然后点击渲染，等待完成就行。也可以《添加到Monitor》等同于任务序列，可以累积多个任务之后再一起渲染，适合晚上离开电脑前设置好队列一起渲染多张图，通宵渲染
![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/Image%20%5B1%5D.png)
![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/Image.png)

### 4.渲染动画
一个简单的动画是在时间轴里看到：整体效果是由一个运动的相机和多个不同运动动作的模型组成的
B站搜索《keyshot 动画》自学，建议在开始制作动画前，写好脚本，跟负责人取得同意之后再制作，因为这个阶段的修改和导出视频会花巨大的时间；渲染动画需要把上述说到的分辨率、抗锯齿级别和阴影进行一定的下调，否则渲染视频会花费连续几天的时间
![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/9.png)
![avatar](https://raw.githubusercontent.com/JayceWork/Keyshot_Picture/main/10.png)
