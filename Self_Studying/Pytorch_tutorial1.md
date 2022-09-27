# tensor
#### 텐서는 **배열**이나 __행렬(matrix)__ 과 매우 유사한 특수한 자료구조
***In Pytorch, by using tensor, encoding(부호화) the input n output or 매개변수 of model***

텐서는 GPU나 다른 하드웨어 가속기에서 실행할 수 있다는 점만 제외하면 NumPy의 ndarray와 유사합니다. 

실제로 텐서와 NumPy배열은 종종 동일한 내부 메모리를 공유할 수 있어 데이터를 복수할 필요가 없습니다. 

텐서는 또한 자동미분에 최적화되어 있습니다. ndarray에 익숙하다면 Tensor API를 바로 사용할 수 있을 것입니다.

>  import *torch*  
import *numpy* as *np* 

##  1. Tensor 초기화 
----------------------------
텐서는 여러가지 방법으로 초기화 할 수 있습니다
 + 데이터로부터 직접 생성하기  
 > data=[[1,2],[3,4]]  
 x_data=torch.tensor(data)

+  numpy배열로부터 생성하기
> np_array=np.array(data)
x_np=torch.from_numpy(np_array)

+ 다른 텐서로부터 생성하기:
> x_ones=torch.ones_like(x_data)  
print(f"Ones Tensor:/n{x_ones}/n")  

> x_rand=torch


[출처]pytorch tutorials in Korean