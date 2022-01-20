code to get all color name in css formate name from https://flatuicolors.com/ of specific country

-----by row first-----
c = document.getElementsByClassName("color");
ar=[]
for(i=0;i<c.length;i++){
    ar.push("--"+c[i].innerText.toLowerCase().replaceAll(" ","-").replaceAll("'",""));
}
console.log(ar.toLocaleString().replaceAll(",","\n"))

-----by column first-----
c = document.getElementsByClassName("color");
ar=[]
for(i=0;i<5;i++){
    for (j=0;j<4;j++){
        ar.push("--"+c[i+5*j].innerText.toLowerCase().replaceAll(" ","-").replaceAll("'",""));
    }
}
console.log(ar.toLocaleString().replaceAll(",","\n"))
