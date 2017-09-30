# react-native-datePicker

1.
npm install  react-native-datepicker-yf --save
2.
react-native link react-native-datepicker-yf

3.import DatePicker from 'react-native-datepicker-yf'

DatePicker是个dialog所以 this.datePicker.showDialog()是展示DatePicker
<DatePicker
    ref={(dialog) => {
        this.datePicker = dialog
    }}
    yearData={this.yearGroup}
    selectData={moment(new Date).format('YYYY-MM-DD')}
    onChange={this.onChange}
    keepShowModal={false}
    cancleText="取消"
    finishText="确定"
    title="出生年月日"
    modalColor="#0000"
    itemStyle={{color: 'black', fontSize: 18}}
    buttonStyle={{color: 'red', fontSize: 18}}
    titleStyle={{color: 'black', fontSize: 18}}
/>

 createData = () => {
        for (let i = 1900; i < 2050; i++) {
            this.yearGroup.push(i.toString())
        }
    }
