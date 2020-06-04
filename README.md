# idshwk7
准备好两张图片，分别是原图片ori.png和水印图片watermark.png。
下载盲水印工具blind-watermark，放到虚拟机里，将准备好的两张图片放到该文件夹里。
打开终端，进入该文件夹，输入encode.py --image ori.png --watermark watermark.png --result test.png将水印图片放入到原图片中，生成隐藏后的图片test.png，即完成了信息隐藏。
输入decode.py --image test.png --orig ori.png --result mark.png提取隐藏的水印，生成了提取后的隐藏图片mark.png，即完成了信息提取。
另外，在下载盲水印工具时，由于没有注意虚拟机所用python版本为python3，一开始无法编译，然后对python2所写代码进行修改后才能在虚拟机上编译
