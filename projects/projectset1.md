# Projects related to DOM

## project link
[Click here](https://stackblitz.com/edit/dom-project-chaiaurcode?file=index.html)

# Solution code

## project 1

```javascript
console.log("hitesh")
const buttons = document.querySelectorAll('.button');
const body = document.querySelector('body');

buttons.forEach(function (button) {
  console.log(button);
  button.addEventListener('click', function (e) {
    console.log(e);
    console.log(e.target);
    if (e.target.id === 'grey') {
      body.style.backgroundColor = e.target.id;
    }
    if (e.target.id === 'white') {
      body.style.backgroundColor = e.target.id;
    }
    if (e.target.id === 'blue') {
      body.style.backgroundColor = e.target.id;
    }
    if (e.target.id === 'yellow') {
      body.style.backgroundColor = e.target.id;
    }
    
  });
});


```
## project 2 solution
```javascript
const form=document.querySelector('form');

form.addEventListener('submit',function(e){
  e.preventDefault()

  const height=parseInt(document.querySelector('#height').value)
  const weight=parseInt(document.querySelector('#weight').value)
  const results=document.querySelector('#results')

  if(height==='' || height<0 || isNaN(height))
  {
    results.innerHTML= "Please give a valid height";
  }
  else if(weight==='' || weight<0 || isNaN(weight))
  {
    results.innerHTML= "Please give a valid weight";
  }
  else{
    const bmi=(weight / ((height*height)/10000)).toFixed(2)

    results.innerHTML=`<span>${bmi}</span>`;

    if(bmi<18.6){
      results.innerHTML=`<span>${bmi}, and you are underweight</span>`;

    }

    else if(18.6<bmi<24.9){
      results.innerHTML=`<span>${bmi}, and you are in normal range</span>`;

    }

    else if(bmi>24.9){
      results.innerHTML=`<span>${bmi}, and you are overweight</span>`;

    }

  }
})

```

#project3 solution
```javascript

```