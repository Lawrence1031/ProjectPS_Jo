Project PS (1점4조)
----
<img width="300" alt="001" src="https://github.com/Lawrence1031/ProjectPS_Jo/assets/144416099/5b9c6af0-1fd2-4bbd-86a9-bb6249b860b7">

3D 퍼즐 방탈출 게임
----
 <details>
    <summary>Sample Image</summary>

   <img width="696" alt="001" src="https://github.com/Lawrence1031/ProjectPS_Jo/assets/144416099/9e9d295a-e6e1-45dc-bda5-6a45d96a249f">

   <img width="696" alt="001" src="https://github.com/Lawrence1031/ProjectPS_Jo/assets/144416099/a80ece64-4512-49e4-869a-7d0383b2eede">

 </details>

프로젝트 정보
----
- 제작기간 2023.12.18 ~ 2023.12.20
- 참여인원 5명
- 맡은 역할 - 상호작용 시스템, 스크립터블 오브젝트(SO), 사운드

사용 기술
-----
- Unity(2022.3.2f1)
- Figma

Structure
----
<details>
<summary>Structure</summary>
<div markdown="1">
   
![ProjectPS02](https://github.com/Lawrence1031/ProjectPS_Jo/assets/144416099/06339fa9-4046-476f-a03d-60d08c74c51f)

</div>
</details>

핵심 기능
----
### 1. 문 오브젝트
> 방 탈출 퍼즐 게임의 기본 사이클에서 플레이어의 승리를 의미하는 다음 단계로의 진행을 책임지는 문을 구현하였습니다.
>
> 플레이어의 상태(아이템이나 조건을 만족했는지)에 따라서 문이 열리거나 열리지 않거나를 조절하며
>
> 열리지 않는 상태라면 플레이어에게 힌트를 제공하는 식으로 게임을 풀어나갈 수 있게 하였습니다.
> 
> [코드](https://github.com/Lawrence1031/ProjectPS_Jo/blob/main/Assets/02.Scripts/Objects/DoorObjects/DoorObejct.cs)

</br>

### 2. 스크립터블 오브젝트(SO)
> 게임에서 사용되는 아이템(열쇠)과 오브젝트(문 등)의 데이터를 저장하는데 SO를 사용하였습니다.
>
> 인벤토리가 있는 게임으로 아이템의 이미지를 직관적으로 연결시키기 위해서,
>
> 문과 열쇠의 연결관계를 확실히 하기 위해서 SO를 사용했습니다.
>
> 또, 문의 잠금이 해제되었는지를 저장하기 위해 SO를 이용하였습니다.
>
> 아래의 코드는 아이템 SO와 문 SO입니다.
> 
> [아이템 SO](https://github.com/Lawrence1031/ProjectPS_Jo/blob/main/Assets/03.SO/ItemData.cs)
>
> [문 SO](https://github.com/Lawrence1031/ProjectPS_Jo/blob/main/Assets/03.SO/DoorData.cs)

</br>

### 3. 사운드 시스템
> 싱글톤화 시킨 사운드 매니저를 도입하여 사운드를 관리했습니다.
> 
> 필요한 사운드들을 배열로 관리하여 필요한 지점에서 매니저를 호출하여 작동시켰습니다.
> 
> 아래의 코드는 사운드 매니저와 그를 호출하는 코드의 예시입니다.
> 
> [사운드 매니저](https://github.com/Lawrence1031/ProjectPS_Jo/blob/main/Assets/02.Scripts/Manager/SoundManager.cs)
> 
> [예시](https://github.com/Lawrence1031/ProjectPS_Jo/blob/main/Assets/02.Scripts/Items/DeskInteraction.cs#L48)

</br>

참고 문서
----
<details>

[개인 노션](https://scythe-sesame-8dc.notion.site/Project-PS-52afc65ec8ff42dda27ec4dff6c28abe?pvs=4)

[팀 노션](https://teamsparta.notion.site/1-4-38c84c4ca03c4d8b8236f10f7b90ce28)

[피그마](https://www.figma.com/file/VA1X4x5hwlYSh98eRGRdmt/Unity4_14-(Copy)?type=whiteboard&t=Kvl4Ckfkp0vMHypF-6)

[팀 깃허브](https://github.com/Lawrence1031/ProjectPS)

</details>
