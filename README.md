## 프로젝트 생성 

▶ `npx expo init REACT-DATASTORAGE-BASIC`<br>

## AsyncStorage

▶key값으로 String을 저장 (유저에 대한 정보, 마지막 접속시간, 임시정보 저장) -> cookie와 비숫한 사용 용도<br>
▶ setItem -> key와 value값을 넘겨 값을 저장하는 것 value는 string으로만 저장 <br>
▶ remove -> key값에 해당하는 value 값을 삭제<br>
▶ clear -> 모든 값을 삭제<br>
▶ mergeItem -> object안에서 같은 key 값이 있는 경우 한가지로 합쳐주는 것 <br>
▶ 최대 저장 사이즈가 정해져 있다.<br>

## Fetch API 

▶ RemoteURL에 있는 리소스를 가져올떄 사용 <br>
▶ HTTP-> server에 데이터 저장, 업데이트 등을 요청하고 결과를 되받는것 <br>
▶ Request Method -> 어떤 동작을 위한 요청인지를 미리 나타내는 것 -> GET,POST,PUT,PATCH,DELETE<br>
▶ GET-> 특정 리소스를 가져와야 할때 사용 <br>
▶ POST -> 어떤 데이터의 저장해야 할때 사용 <br>
▶ PUT -> 특정 리소스를 업데이트 할때 사용 (전체)<br>
▶ PATCH -> 특정 리소스 중 특정 정보만 변경할때 사용 <br>
▶ DELETE -> 리소스를 아예 삭제<br>

## Request 데이터 전달

▶ 데이터를 서버로 전달하는 방법 ex- Path Parameter, Query Parameter, Request Body<br>
▶ Path Parameter -> URL Path내부에 값을 함께 넘기는 것 ex- 특정 유저 ID를 통해 정보 가져올때<br>
▶Query Parameter -> URL 뒷부분에 ? 를 붙이고 그 뒤에 key값과 value값을 넘겨주는 것 ex- 이름 성별로 검색해서 가져올때<br>
▶Request Body -> URL에 데이터가 보이지 않고 Body에 작성해서 넘기게 된다 데이터가 긴경우 Request Body 사용이 적합하다 (URL 길이제한) ex- 회원가입 게시글 등록 할때<br>

## Response status code

▶ 200: 정상적으로 처리 <br>
▶ 500: 서버에서 처리 중 에러가 발생 <br>
▶ 400: Client에서 값을 잘못 전달함<br>
▶ 403: 유저정보는 식별되나 해당 URL로의 접근이 거부 <br>
▶ 404: URL이 존재하지 않음 <br>

## Redux-persist

▶ 저장소에 마지막 Redux상태를 저장하였다가 이어서 사용 할 수 있도록 하는 것 React-Native에서는 AsyncStorage에 저장 <br>
▶ PersistGate -> Component형태로 작성되어있음 Storage로부터 데이터를 로드해 Redux를 업데이트 로딩하는 동안에 Loading 컴포넌트 추가 가능 <br>
▶ BlackList = 유지하지 않아도 되는 Redux Key값들, WhiteList = 유지를 해야 하는 key값<br>





