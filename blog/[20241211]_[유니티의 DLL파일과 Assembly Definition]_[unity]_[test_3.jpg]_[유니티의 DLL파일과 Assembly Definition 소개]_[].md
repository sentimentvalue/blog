### DLL(Dynamic-Link Library) & PDB(Program Database)
- Library: 컴퓨터 프로그램이 사용하는 비휘발성 자원(함수, 데이터, 타입 등)의 모임
- DLL: 여러 프로그램에서 동시에 사용할 수 있는 코드와 데이터를 포함하는 라이브러리
- 유저 작성 스크립트는 dll로 생성되어 Unity Editor에서 사용됨
- pdf 파일에는 앱의 디버그 구성에 대한 링크를 허용하는 디버깅 및 프로젝트 상태 정보가 저장

### Assembly Definition
이전에는 모든 라이브러리를 한번에 컴파일했지만, Assembly Definition을 사용하면 연관되어있는 라이브러리만 컴파일하여 시간을 단축시킴
+프로젝트를 잘개나누어서 바뀐 부분만 적용시킴. VSCode에서 확인시 프로젝트가 나뉘어져있는것을 확인할수있음

사용법:
스크립트 우클릭->Assembly Definition 클릭=asmdef 파일이 생성됨(스크립트 이름과 동일한 이름으로 설정하는게 좋음)
filename에 어떤 dll에 속해있는지 알려줌

주의사항:
별도의 라이브러리 또는 스크립트는 다른 dll에 있는 스크립트를 참조하지 못함.
- 가장 기본 라이브러리인 Assembly-CSharp은 모든 라이브러리 참조 가능
- 스크립트를 참조당할 스크립트 Assembly Definition 폴더(하위폴더 포함)내로 이동시 참조 가능
참조하는 방법:
참조할 스크립트 우클릭->Assembly Definition 생성 -> 이전 스크립트 Assembly Definition으로 이동->Assembly Definition References에 참조할 어셈블리데피니션 추가
- VSCode Explorer에 프로젝트에 참조 스크립트를 추가한 라이브러리 하위폴더(Depencies/Projects)에 참조한 내역 존재
- Assembly Definition을 통해 스파이더 구조로 마구잡이로 참조시 오류가 뜰수 있음.ㅌ