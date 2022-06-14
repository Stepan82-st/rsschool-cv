# BRYL STEPAN

## Frontend Developer

![MyPhoto](https://avatars.githubusercontent.com/u/53449161?s=400&u=562212b5eaff664f958aa78e1f3f2f49eb0efd89&v=4)

## Contact Details

* Phone: +375291611662
* Discord: Stepan#8061
* Email: bryl.step@tut.by

## About Me

My goal is to change my job.

## My skills

* HTML5, CSS3
* JavaScript
* Git, Github
* VSCode

## Code Example

**How to create a function that changes the time?**

```javascript

function addZeroHandler(param){
  if(param <= 0){
  return param = '00';
 }else{
    return param;
  }
}

function getParsedDateFormat(date){
  const year = date.getFullYear();
  const month = addZeroHandler(date.getMonth()+1);
  const day = addZeroHandler(date.getDate());
  const hour = addZeroHandler(date.getHours());
  const minutes = addZeroHandler(date.getMinutes());

  return year +'-'+ month +'-' + day +'  '+ hour + ':' + minutes;
}

function date(dateString){
  const date = new Date(dateString);

  const methodsHandler = {
    getPrefix: 'get',
    setPrefix: 'set',
    years: 'FullYear',
    months: 'Month',
    days: 'Date',
    hours: 'Hours',
    minutes: 'Minutes' 
  };
  const dateHandler = {

    value: date,

    add(amount, format){
      this._calculate(amount, format, 'add')
      this._updateValue();
    return dateHandler;
      },
      subtract(amount, format){
        this._calculate(amount, format, 'subtract');
        this._updateValue();
        return dateHandler;
      },
      _calculate(amount, format, type){
        const get = methodsHandler.getPrefix;
        const set = methodsHandler.setPrefix;
        const method = methodsHandler[format];
        switch (type){
          case 'add':
            date[set + method](date[get + method]() + amount);
            break;
            case 'subtract':
              date[set + method](date[get + method]() - amount);
              break;
        }
      },

      _updateValue(){
        this.value = getParsedDateFormat(date);
      }
  }
  return dateHandler;
}
```

## Experience

[My CV project](https://github.com/Stepan82-st/rsschool-cv/)

## Education

* IIT BGUIR
* [JavaScript Manual](https://learn.javascript.ru/) -  in progress
* RS Schools Course (JavaScript/Front-end. Stage 0) -  in progress

## Languages

* [English - A2](https://drive.google.com/file/d/1a4bSSkmIRgxVBz481DYBhMMv1zVB4L_1/view?usp=sharing)
