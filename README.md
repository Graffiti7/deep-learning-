# Deep Learning

## 模型示意图

<p align="center"><img  src="https://github.com/Graffiti7/deep-learning-/blob/master/mutli-head.png?raw=true" width="85%" height="85%"></p>


## 实验环境

pytorch 1.9
python 3.8
ubuntu 16.04

## 数据集下载

实验使用 Imagenet-1k 数据集 <a href ='https://image-net.org/'>下载链接</a>

## 运行方式

运行脚本在src/train下的train.sh
根据需要模型设置，在脚本进行修改即可
实验模型在src/models目录中，其中多头模型在resnet50.py中定义
同时根据结果输出与参数打印可对于src目录下的main.py文件进行修改（打开注释即可）

## 实验结果

<table>
<tr>                                      
    <td rowspan="2" align='center'>Network</td>
    <td rowspan="2" align='center'>Dataset</td>
    <td colspan="2" align='center'>Norm</a></td>
    <td colspan="2" align='center'>Mutil-head</td>
    <td colspan="2" align='center'>Adaptive-Mutil-head</td>
</tr>
<tr>
    <td align='center'>top1-acc</td>
    <td align='center'>top5-acc</td>
    <td align='center'>top1-acc</td>
    <td align='center'>top5-acc</td>
    <td align='center'>top1-acc</td>
    <td align='center'>top5-acc</td>
</tr>
<tr>
    <td>Resnet50 (no-shortcut)</td>
    <td rowspan="4"> Imagenet-1k</td>
    <td align='center'>65.83</td>
    <td align='center'>86.63</td>
    <td align='center'>69.03</td>
    <td align='center'>89.02</td>
    <td align='center'><strong>70.52</strong></td>
    <td align='center'><strong>89.38</strong></td>
</tr>
<tr>
    <td>ResNet50</td>
    <td align='center'>76.31</td>
    <td align='center'>92.98</td>
    <td align='center'>72.51</td>
    <td align='center'>91.09</td>
</tr>
<tr>
    <td>ResNet50_svpn (no-shortcut)</td>
    <td align='center'>71.00</td>
    <td align='center'>89.39</td>
    <td align='center'>73.03</td>
    <td align='center'>91.10</td>

</tr>
<tr>
    <td>ResNet50_svpn</td>
    <td align='center'>77.24</td>
    <td align='center'>93.24</td>
    <td align='center'>76.16</td>
    <td align='center'>92.68</td>

</tr>
</table>