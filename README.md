### app
app is first object making
~~~
script(src="https://gnjo.github.io/app/app.js" onload="window.app('q')"
//window.q={}
~~~
~~~
window.app('a,b,c')
//window.a={},window.b={},window.c={}
~~~
~~~
;function(root){
 
 function entry(str){
  for(const k of (str||'').split(',').filter(d=>d))
   root[k]={}
 }
 root.app=entry;
}(this);
~~~
