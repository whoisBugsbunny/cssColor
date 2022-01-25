Code to get all color name in css formate name from https://flatuicolors.com/ of specific country

<h1>-----by Row First-----</h1>

```
c = document.getElementsByClassName("color");
ar=[]
for(i=0;i<c.length;i++){
    ar.push("--"+c[i].innerText.toLowerCase().replaceAll(" ","-").replaceAll("'",""));
}
console.log(ar.toLocaleString().replaceAll(",","\n"))
```
<h1>-----by Column First-----</h1>

```
c = document.getElementsByClassName("color");
ar=[]
for(i=0;i<5;i++){
    for (j=0;j<4;j++){
        ar.push("--"+c[i+5*j].innerText.toLowerCase().replaceAll(" ","-").replaceAll("'",""));
    }
}
console.log(ar.toLocaleString().replaceAll(",","\n"))
```

bootstrap 4 https://getbootstrap.com/docs/4.0/getting-started/download/

bootstrap 5 https://getbootstrap.com/docs/5.0/getting-started/download/
