## 1. TUNiB 과제설명
해당 데이터셋은 TUNiB에서 자체적으로 제작한 데이터인 DKTC(Dataset of Korean Threatening Converstations)으로 classification task 수행합니다.<br>여기서 주어진 훈련데이터의 클래스는 총4가지('협박', '갈취', '직장 내 괴롭힘', '기타 괴롭힘')이고 테스트데이터는 여기에 '일반 대화'클래스가 하나 추가 되어있습니다.
|Class|Traning|Test|
|:--:|:--:|:--:|
| 협박 대화 | 896 | 100 |
| 갈취 대화 | 981 | 100 |
| 직장 내 괴롭힘 대화 | 979 | 100 |
| 기타 괴롭힘 대화 | 1,094 | 100 |
| 일반 대화 | - | 100 |

훈련데이터에서 빠져있는 '일반 대화'는 [AI Hub](https://aihub.or.kr/?utm_source=google&utm_medium=search&utm_campaign=ga&gclid=CjwKCAjw6raYBhB7EiwABge5KnZuqLSaXjiqfgAETqQwG-_7B2r2e26nDY5cOiNSvrwEUrvIsW9GcRoCRCgQAvD_BwE)에서 내려받아 학습에 활용합니다.
## 2. 데이터 설명
### Train data
![](./reference/train.png)
- csv파일로 주어져있습니다.
- 각 conversation에 class로 라벨링되어있습니다.
- 대화내용은 '\n'으로 기준으로 나뉘어서 한줄로 이루어져있습니다.
### Test data
![](./reference/test.png)
- json파일로 주어져있습니다.
- 테스트데이터이므로 라벨은 없고 대화문만 있습니다.
- 훈련데이터와는 달리 대화내용이 '\n'으로 나뉘어져있지 않습니다.
## 3. 프로젝트 환경
- 프로그래밍 언어 : Python3
- 프레임워크 : Tensorflow, Huggingface,
- 작업 환경 : Google Colab, GCP
- 회의록 주소 : https://www.notion.so/e204ff1bd98d445e927121eaf36b59ed
## 4.
