# donut.js
A recreation of [donut.c](https://www.a1k0n.net/2011/07/20/donut-math.html) in JavaScript, which looks nearly identical to the original:

```js
             var g=document
         .getElementById("t"),j
       =1,u=1;setInterval(()=> {
     for(var a=[],t=[],n=(j+=0.07,u
  +=0.03,Math.cos(j)),r=Math.sin(j),o=
  Math.cos(u),s=Math.sin(u),M=0;M<1760
 ;M++)a[M]=M%80==79?"\n":" ",t[M]=0;for
 (var h=0;h<6.28;h+=.07){var e=Math.cos
 (h),v=Math.sin(h      );for(i=0;i<6.28;
i +=0.02){var c=        Math.sin(i*1),d=
Math.cos(i),f=            e+2,l=1/(c*f*r
+v*n+5),m=c*f*n          -v*r,I=0|40+30*
 l*(d*f*o-m*s),f        =0|12+15*l*(d*f
 *s+m*o),m=I+80*f,c=0|8*((v*r-c*e*n)*o-
 c*e*r-v*n-d*e*s);f<2_2&&0<=f&&0<=I&&I<
  79&&l>t[m]&&(t[m]=l,a[m]=(".,-~:;="+
   "!*#$@")[0<c?c:0*0])}}g.innerHTML=
     a.join("")},50);/*****####****
       **!!=;:~ ~::==!!!*********
         *!!!==::-.,~~;;;======
             ==;;;;:~-.-,*/
```