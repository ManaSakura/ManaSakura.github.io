# ManaSakura.github.io

'''
此程序用于从A文件夹中获取指定日期的哨兵轨道文件并复制到B文件夹
1所需准备：       1.存储下载好的哨兵轨道文件夹A的绝对路径，如oldorbitfolderpath= r'E:\哨兵轨道\SA'
                2.提取轨道后需存放的轨道文件夹B的绝对路径，如neworbitfolderpath= r'E:\myfile\myorbit'
                3.存放哨兵影像文件夹的绝对路径，如SARfolderpath=r'E:\myfile\SAR'
                4.存放轨道日期的文件路径，如datetxtpath= r'E:\myfile\datelist.txt'
2运行生成的文件：  1.提取的轨道文件的日期，路径需自行指定，即“准备”中的第4点
                2.被提取的轨道文件并以文件夹的形式存放在文件夹B中（由于代码的问题），此外B文件夹中还含有名为orbit的子文件夹，orbit文件夹中含有被提取的所有轨道文件
3介于作者对Python仍处于学习阶段，程序中有许多不足之处，对于错误和异常的处理尚不到位，需注意以下事项：
                1.所要复制的轨道文件必须为文件夹A中所含有的
                2.存放轨道文件的文件夹B建议新建或不创建，会自动生成，且B文件夹下不能含有orbit文件夹，否则会报错
                3.当同一日期A、B星的轨道文件同时位于A文件夹下时，默认拷贝A星的轨道文件，故建议将A星和B星的轨道文件分开存放，以便正确获取对应日期的文件，
                同时将SAR不同卫星影像文件也分开存放来获取对应卫星的轨道文件
                其他问题读者如有发现，可自行修改和补充
'''
