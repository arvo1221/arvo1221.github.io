# Studying Adaptive Cruise Control

## 개요
 차량동역학 스터디에서 발표한 자료를 업로드 하였습니다.
 교재는 Rajesh Rajamani 박사님의 Vehicle Dynamics and Control Second Edition을 사용하였으며 Chapter 6의 5,6절 내용을 다루고 있습니다.
 
 
 <img src="https://user-images.githubusercontent.com/54099930/109526758-44380e80-7af6-11eb-9f09-fc79f7b0a025.jpg" width="690">
 
### Autonomous Control with Constant Spacing
 
 <img src="https://user-images.githubusercontent.com/54099930/109527989-9a598180-7af7-11eb-805d-333eb0ecc1fe.jpg" width="690">
 
 <img src="https://user-images.githubusercontent.com/54099930/109528152-bc530400-7af7-11eb-9e0e-878892066e49.jpg" width="690">

 Kp = 1 Kv = 0.3 일 때 String Stability를 만족하지 못함을 bode plot을 통해 알 수 있습니다.
 앞선 4절에서 String Stability를 만족하기 위한 두 가지 조건을 제시합니다.

 <img src="https://user-images.githubusercontent.com/54099930/109531497-4fda0400-7afb-11eb-959b-30a922a32710.jpg" width="480">
 
 <img src="https://user-images.githubusercontent.com/54099930/109528160-bf4df480-7af7-11eb-8217-9aaa242a3ad2.jpg" width="690">

 차량간 거리를 상수로 제어하고자 한다면 어떠한 gain을 사용하더라도 String Stability를 만족하지 못함을 확인하였습니다.

### Autonomous Control with The Constant Time-Gap Policy

 <img src="https://user-images.githubusercontent.com/54099930/109528535-1f449b00-7af8-11eb-8537-934bbb93cfaa.jpg" width="690">

 차량간 거리를 상수가 아닌 i번째 차량의 속도에 비례하게 제어하는 것으로 변경합니다.
 
 <img src="https://user-images.githubusercontent.com/54099930/109528539-210e5e80-7af8-11eb-927d-07602e00343e.jpg" width="690">

 ddot x_i = ddot x_i_desired 를 만족하지 못하므로 tau*dddot x_i + ddot x_i = ddot x_i_desired 으로 수정합니다.
 
 <img src="https://user-images.githubusercontent.com/54099930/109528546-223f8b80-7af8-11eb-8826-528bee9b3dfd.jpg" width="690">
 
 <img src="https://user-images.githubusercontent.com/54099930/109528624-3be0d300-7af8-11eb-97b7-f358e7891ef0.jpg" width="690">
 
 <img src="https://user-images.githubusercontent.com/54099930/109528629-3d120000-7af8-11eb-86ca-b6832eeb7e3c.jpg" width="690">

 필요충분조건을 증명합니다.
 
 <img src="https://user-images.githubusercontent.com/54099930/109528633-3edbc380-7af8-11eb-9f98-fcf8480136c0.jpg" width="690">

 String Stability를 만족하는 모습을 확인할 수 있습니다.

 <img src="https://user-images.githubusercontent.com/54099930/109528728-54e98400-7af8-11eb-8342-a5ce89dee748.jpg" width="690">
 
 <img src="https://user-images.githubusercontent.com/54099930/109528738-561ab100-7af8-11eb-85fe-e7dc8147c724.jpg" width="690">

 차량간 거리를 줄일 수록 같은 시간동안 더 많은 차량이 도로를 지나갈 수 있지만 h>2tau를 만족해야 하므로 한계가 있습니다. 또한 다양한 요인에 의해 한계가 있음을 설명합니다.
 
 <img src="https://user-images.githubusercontent.com/54099930/109528743-57e47480-7af8-11eb-8726-826393e51993.jpg" width="690">
 
 <img src="https://user-images.githubusercontent.com/54099930/109528816-6af74480-7af8-11eb-9b26-9caa9576b954.jpg" width="690">

 
 


