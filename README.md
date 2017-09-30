# react-native-datePicker
##  1.
##  npm install  react-native-datepicker-yf --save
##  2.
##  react-native link react-native-datepicker-yf
##  3.
##  import DatePicker from 'react-native-datepicker-yf'

![image](https://github.com/AbelHuai/react-native-datePicker/blob/master/04052A13-367F-4497-93F1-A6775FC40CC9.png)

##  DatePicker是个dialog所以 this.datePicker.showDialog()是展示DatePicker
>  <DatePicker \
      ref={(dialog) => { \
         this.datePicker = dialog \
     }} \
     yearData={this.yearGroup} \
     selectData={new Date} \
     onChange={this.onChange} \
     keepShowModal={false} \
     formatCharacter="-" \
     cancleText="取消" \
     finishText="确定" \
     title="出生年月日" \
     modalColor="#0000" \
     itemStyle={{color: 'black', fontSize: 18}} \
     buttonStyle={{color: 'red', fontSize: 18}} \
     titleStyle={{color: 'black', fontSize: 18}} \
  /> \
 //创建数据（年份） \
  createData = () => { \
         for (let i = 1900; i < 2050; i++) { \
             this.yearGroup.push(i.toString()) \
         } \
     } 

yearData //年份数据 \
selectData // 默认选中的日期\
keepShowModal // 点击控件外是否收起日期选择\
formatCharacter // 返回日期数据的分隔符\
onChange // 选择完成回调\
cancleText // 取消文字\
finishText // 确定文字\
title // 提示标题\
modalColor // Model背景色\
itemStyle // 日期数据样式\
buttonStyle // 左右文字样式\
titleStyle // 中间标题样式\
