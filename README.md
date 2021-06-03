
# Exercise Counter 
  
Count the repetitions of exercise using pose estimation implemented in Pytorch and trained on **HRNet** ([Link](https://arxiv.org/pdf/1902.09212.pdf)) .Model is also scalable to multiple person using YOLOv3. This repo is built on the top of this repo ([Link](https://github.com/stefanopini/simple-HRNet)).


[Demo Videos](https://drive.google.com/drive/folders/1145dMy3WfEOOWInNj9WI23lcoUJaET_L?usp=sharing)

## Steps to run   

 1. Clone this repository  

```
git clone https://github.com/Garvit-32/exercise-counter.git  
```    

 2. Install all the dependencies  

```  
pip install -r requirements.txt   
```  

3. Download weights from [here](https://drive.google.com/file/d/1---z6T5BDPvwfYF0xHfLrmVGOp6jY4qO/view?usp=sharing) and put in folder named weights

4. Run inference   
```  
python main.py --filename <path to exercise video> --exercise_type <exercise number> --weights <path to weights>  
```
| Exercise Name | Exercise Number |
|--|--|
| PushUps | 1 |
| Squats or Situps | 2 |
| Pullups | 3 |
| Dumbell Curl | 4 |
| Dumbell Side Lateral | 5 |
It can be extended to other exercise as well. 

Example  
```  
python main.py --filename 'demo_videos/squat.mp4' --exercise_type 2 
```  

## DEMO  
    

<table>
 <tr>
  <td align="center"><img src="gifs/pushups.gif" width="80%" height="auto" /></td>
  <td align="center"><img src="gifs/squat.gif" width="100%" height="auto" /></td>
  
 </tr>
  <tr>
  <td align="center"> <img src="gifs/dumbell.gif" width="70%" height="auto" /></td>
  <td align="center"><img src="gifs/pullups.gif" width="100%" height="auto" /></td>
 </tr>
</table>
  
    
  

## References
1. https://github.com/stefanopini/simple-HRNet
2. https://github.com/duc-tran/infant