사이클이 없는 무방향 연결 그래프를 *트리*라고 합니다. 트리에서 차수가 1인 노드는 *리프 노드*라고 합니다.

트리를 생각해 봅시다. 모든 두 리프 노드의 쌍에 대해 우리는 이 노드들 사이의 거리를 결정할 수 있습니다. 한 리프 노드에서 다른 리프 노드로 이동하기 위해 거쳐야 하는 간선의 수가 되겠죠. 모든 리프 노드에 대해 이러한 거리들이 주어질 때, 여러분은 트리를 재구성해야 합니다.

### 입력 형식

첫 번째 줄에 트리에 있는 리프 노드의 수 $l$ ($1 \le l \le 200$)이 주어집니다. 다음 $l$개 줄에는 리프들 사이의 거리를 나타내는 $l$개의 정수가 주어집니다. 거리가 200보다 큰 경우는 주어지지 않고, 모든 거리는 음이 아니며, 자기 자신과의 거리는 0이고, 리프 $i$와 $j$의 거리는 리프 $j$와 $i$의 거리와 같습니다.

### 출력 형식

만약 주어진 조건대로 트리를 재구성하는 것이 불가능하다면 첫 번째 줄에 `-1`을 출력합니다.

그렇지 않다면 트리의 정점의 수 $n$을 출력합니다. 다음 $n-1$개의 줄에 트리의 각 간선이 연결하는 두 정점의 번호를 공백을 사이로 두고 출력합니다. 가능한 경우가 여러가지라면, 아무거나 출력해도 좋습니다. 번호 순으로 처음 $l$개 정점 ($1, 2, \cdots, l$번 정점)은 모두 리프 노드로 입력에서 주어진 순서대로 번호가 붙어 있어야 하며, 나머지 노드는 번호를 임의로 붙여도 좋습니다.

### 예제

<table class='table table-bordered table-condensed'>
 <thead>
  <tr>
   <th style="width: 50%;">입력</th>
   <th style="width: 50%;">출력</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td class="code-font">3<br/>
0 2 3<br/>
2 0 3<br/>
3 3 0</td>
   <td class="code-font">5<br/>
1 4<br/>
2 4<br/>
3 5<br/>
4 5</td>
  </tr>
 </tbody>
</table>