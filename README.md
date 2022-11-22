# proxy-revealer
> the idea behind the proxy revealer is to get the real ip and the one the proxy parsed and changed .... 
>  if we use window.location it will return the real href -> the one of the proxy and after the parse it will warp it function that will change it to the real ip 
> and every instance of the uri will be changed to the "fake addr " of the address and not of the proxy 
# demo : 
jct proxy : https://lev.jct.ac.il/dana/home/index.cgi

<img width="1013" alt="image" src="https://user-images.githubusercontent.com/90776557/203329062-63ae1fb4-59f3-4674-a274-b2fe182c7592.png">

let's connect to our website : https://proxyfinder-production.up.railway.app/
it will look like that : 
<img width="655" alt="image" src="https://user-images.githubusercontent.com/90776557/203329782-5cc36a16-c6a7-4d51-bbd8-a9fb65fff6b9.png">
# in the console of the jct proxy : 
## parsed windows location : 
 <img width="375" alt="image" src="https://user-images.githubusercontent.com/90776557/203330115-89d07792-5a67-4922-83a3-8fd8e8bdaa94.png">

## non parsed : 
<img width="541" alt="image" src="https://user-images.githubusercontent.com/90776557/203330230-6a15ded5-3059-4611-ba0e-b6aa1d87e7cd.png">


so to sturggle with parse we used : http://www.jsfuck.com/ 
and then the code of window.location.href cant be changed and to avoid of cahnge of the addr we encoded it in base64 and decoded in the server side 
and this is how we cracked it 
## parsed code to jsfuck code : 

<img width="757" alt="image" src="https://user-images.githubusercontent.com/90776557/203332214-078d8a84-bd56-41fd-9925-b70c4e663cc9.png">

# use without proxy : 

<img width="661" alt="image" src="https://user-images.githubusercontent.com/90776557/203330879-1e42458f-e0e7-4887-aabf-955c388674b4.png">

# use with jct proxy : 

<img width="611" alt="image" src="https://user-images.githubusercontent.com/90776557/203330946-b630e741-5edf-495f-bd5e-c5b514ac16b4.png">


<img width="775" alt="image" src="https://user-images.githubusercontent.com/90776557/203331062-d5d9386f-228d-4268-825a-6c79380fee01.png">


