# LinkedList

Linked List 는 Node 라는 구조체가 연결되는 형식으로 데이터를 저장하는 자료구조

node는 데이터 값과 next node 의 주소값을 저장한다.

하지만 linked list는 메모리상에서는 비연속적으로 저장이 되어 있지만 각각의 node가 next node의 메모리 주소값을 가리킴으로써 논리적인 연속성을 가지게 된다.

Array 와 linkedList의 차이 

![image](https://github.com/gusdn0108/linkedlist/assets/96761523/f236bca2-35ce-4c98-a403-be1a429ffd56)

array 구조상 데이터 저장은 그림처럼 1,2,3,4 이런식으로 순서대로 저장이 된다 이렇게 함으로써 어느 인덱스를 가든 랜덤 액세스 

즉 시간복잡도 O(1) 접근이 가능하다

LinkedList는 어떻게 저장을할까 ?

![image](https://github.com/gusdn0108/linkedlist/assets/96761523/0a8b6242-8d2f-460b-9ede-e7d6f75c05b1)

요 그림처럼 순서대로 저장되어 있는것이 아닌 뒤죽박죽으로 되어있기 때문에 각각의 노드의 첫 주소값 얘네들을 가리키는 next address 를 저장함으로써 논리적인 연속성을 가지게 된다..!


![image](https://github.com/gusdn0108/linkedlist/assets/96761523/8c831190-58a5-49a9-97a3-fc209c972bbb)

이렇게보면 논리적으로 1 2 3 4 연속적으로 순차적으로 연결되어 있구나 싶겠지만 하지만 실직적 물리적으로는 연속적으로 저장이 되어 있지 않으구나 를 메모리를 통하여 알수있다.

그림을 다시 퀄리티있게 그려보자면

![image](https://github.com/gusdn0108/linkedlist/assets/96761523/c424fcf0-2661-40e0-9253-d99ad8af89db)


(1) 1이라는 데이터를 저장을 하였고 여기 주소값을 따라 가보니깐 (2)가 나온다 이후 (2)에 적혀있는 주소값으로 갔더니 (3) 노드가 나오게된다 이때 이 값이 필요하다면 이 값을 접근하면 되는거고 아니면 다음 노드로 가면되는 방식인 것이다.

이렇게 LinkedList는 물리적으로는 `비연속` 적으로 되어 있지만 논리적으로는 연속적인것이다. 

각 node들은 데이터 저장만 할 뿐만이 아니라 next node의 address 값도 가지고 있어야 하기 때문에 논리적으로 연속성을 유지하면서 연결 될 수 있는것이다 

다만 Array의 경우 연속성을 쥬이하기 위하여 메모리 상에서 순차적으로 데이터를 저장하는 방식을 사용하였지만 Linked List에는 메모리상에서 연속성을 유지하지 않아도 되기 때문에 메모리 사용이 조금 더 자유롭다 다만 next node 의 address 도 추가적으로 저장해야 하기 때문에 데이터 하나당 차지하는 메모리가 더 커지게 된다 .

![image](https://github.com/gusdn0108/linkedlist/assets/96761523/bcdc0c38-5794-4bb3-be4e-df3883b99d93)







