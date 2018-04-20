![程序媛的if](https://github.com/fabiokilling/Git/blob/master/Files/%E7%9B%B8%E4%BA%B2%E5%9B%BE.jpg)

# # -*- coding: utf-8 -*-

"""

Created on Fri Apr 20 09:06:25 2018

@author: ArcherX

"""

import easygui

easygui.msgbox('这是一个相亲APP')

try:
    
    age = easygui.integerbox('输入年龄')

    颜值 = float(easygui.enterbox('颜值评分0-99.9，此处调用百度AIP人脸识别打分接口，请运行另一段代码得出分数'))

    年薪 = int(easygui.enterbox('年薪单位为k，请输入税前年薪'))

    公务员 = int(easygui.enterbox('是否为公务员，是输入1，否输入0'))

    王思聪 = int(easygui.enterbox('是否是王思聪本人，是输入1，否输入0'))

    print(age,颜值,年薪)

    if 王思聪 == 1:
    
        easygui.msgbox("老公！")
    
    elif age > 30:

        easygui.msgbox('太老!')

    elif age <= 30:

        #easygui.msgbox('颜值打分?')

        if 颜值 < 50:
        
            easygui.msgbox('太丑!')
        
        elif 颜值 >= 50:
    
            #easygui.msgbox('年薪?')
        
            if 年薪 < 120:
            
                easygui.msgbox('太穷!')
            
            elif 120 <= 年薪 < 150:
            
                if 公务员 == 0:
                
                    easygui.msgbox('不安稳还穷!')
                
                elif 公务员 == 1:
                
                    easygui.msgbox('你拥有了见我的权力，我的手机号是131xxxxxxxx')
                
            elif 年薪 >= 150:
            
                easygui.msgbox('我很满意，我的手机号是1316xxxxxx')
            
except:
    
    easygui.msgbox('滚(ノ｀Д)ノ!')
        
#MarkDown格式不能直接复制=。=
