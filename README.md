# Word录入简谱 + Python转MusicXML格式

## Step1：在Word中安装新的字体
将DiziFont.ttf下载至本地后，在Word中进行安装，就可以和Word中普通的字体（eg: 宋体，黑体）一样使用了。

## Step2：在Word中进行简谱录入
开始进行简谱的录入。首先，第一行为乐曲标题，第二行为调号和节拍。然后，在Word中将字体调至DiziFont，并使用如下的规则进行具体音符的录入：

- 1 2 3 4 5 6 7：基本音符
- 8：高音
- *：低音
- z：八分音符
- x：十六分音符
- c：三十二分音符
- b：十六分音符低音
- n：三十二分音符低音
- \：小节线

一个示例如下所示：

![image](https://github.com/hrsoup/A-Method-to-Collect-Jianpu/blob/main/files/jianpuex.png)

## Step3：将简谱显示的Word文档转成MusicXML/MIDI格式

使用Word2XML.ipynb可将Word文档转换成MusicXML文件。

在MuseScore中可对MusicXML格式文件进行五线谱式的显示，一个例子如下，之后也可以通过MuseScore导出MIDI格式文件：

![image](https://github.com/hrsoup/A-Method-to-Collect-Jianpu/blob/main/files/staff.png)

-----------------

### 环境
- Windows系统
- Microsoft Word
- Python 3
    - Music21
    - Docx
