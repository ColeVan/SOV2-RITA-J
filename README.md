# SOV2-RITA-J
This project is for finding a solution to use Security Onion Elastic data with Jupyter Notebooks. 

The goal is to successfully use this notebook project below with Security Onion for beacon detection capabilities. 

https://github.com/Cyb3r-Monk/RITA-J/blob/main/C2%20Detection%20-%20HTTP.ipynb 

So far I am able to pull back data from Security Onion using the elastic API. Please see Zeek-Network-Hunting.ipynb above. I am not able to pull back the correct data to use it in conjunction with RITA-J notebook.



Jupyter Notebooks with Security Onion

Cuurently trying to find method to query SOv2 elastic data and retrieve the fields below.

'ts'

'id.orig_h'

'id.resp_h'

'host'

'id.resp_p'

'method'


![image](https://user-images.githubusercontent.com/70167373/146839611-e793d651-9e41-4544-a31c-ec83d913b348.png)


Unfortunately, I cannot accomplish this with the query string below using jupyter notebooks.

message:"ts" AND 'id.orig_h' AND 'id.resp_h' AND 'host' AND 'id.resp_p' AND 'method'

The big problem! 

To use this notebook, “link below”, I need to parse the fields above in order to set variable for them in the fields below.

https://github.com/Cyb3r-Monk/RITA-J/blob/main/C2%20Detection%20-%20HTTP.ipynb

![image](https://user-images.githubusercontent.com/70167373/146839670-30a92416-c4c8-4c73-a98d-a3d23199dd25.png)

So far, this setup is successful. The additional imports are for further use elsewhere so please disregard.

The query search string below allows me to pull data back from SOv2 Elastic. Unfortunately, this is not the parsed data needed in order to set columns to use RITA-J notebook 
above.


![image](https://user-images.githubusercontent.com/70167373/146839716-48fa7b07-1c35-450b-b71b-4904cc8f9869.png)

As you can see the fields needed below are not present. This is the issue!

'ts'

'id.orig_h'

'id.resp_h'

'host'

'id.resp_p'

'method'

![image](https://user-images.githubusercontent.com/70167373/146839745-8bc58746-5eac-4f1f-b899-00b0411be553.png)





