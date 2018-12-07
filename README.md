HAN은 구조도 더 복잡하고, ATTENTION 까지사용, 그리고 GLOVE를 이용해 단어임베딩도 사용했는데도 95
그냥 LSTM은 임베딩부터 학습하고 ATTENTION도 안썼는데, 그냥 문단을 LSTM 사용하니 성능이 99

같은 데이타인데 왜그럴까?


HAN 



An aexample of HAN from paper: http://www.cs.cmu.edu/~./hovy/papers/16HLT-hierarchical-attention-networks.pdf. ,  NAACL-HLT, 16'

Code was combined from two publickly available sources:
https://gist.github.com/cbaziotis/7ef97ccf71cbc14366835198c09809d2

https://github.com/richliao/textClassifier

https://richliao.github.io/supervised/classification/2016/12/26/textclassifier-HATN/

https://hist0134.blog.me/221179965199

https://m.blog.naver.com/PostView.nhn?blogId=hist0134&logNo=221386940063&navType=tl

설명 : http://hugrypiggykim.com/2018/05/31/han-hierarchical-attention-networks-for-document-classification/


1) data 폴더에 labeledTrainData.tsv 필요
   - wget https://www.kaggle.com/c/word2vec-nlp-tutorial/download/labeledTrainData.tsv
   - 이름바꾸고 unzip
2) glove 폴더에 glove.6B.100d or glove.6B.200d, (단어, 임베딩)쌍으로 
   - http://nlp.stanford.edu/data/glove.6B.zip

![han attention visualization](https://user-images.githubusercontent.com/38748880/49410835-f95dae00-f7a9-11e8-93a6-596e66140033.PNG)
<img width="551" alt="feedforwardattention" src="https://user-images.githubusercontent.com/38748880/49410883-1e522100-f7aa-11e8-960a-c31ca51d5e28.png">




<img width="298" alt="hierachicalattention" src="https://user-images.githubusercontent.com/38748880/49410897-24e09880-f7aa-11e8-81bc-5c551b6ef812.png">





![image](https://user-images.githubusercontent.com/38748880/49410969-696c3400-f7aa-11e8-87c9-ac8edc84ba73.png)



