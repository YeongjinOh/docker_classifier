## SW Maestro BackEnd 과제

#### Score
	<p>  0.7165 (Name : 오영진2) </p>

#### IP address
	<p>  제가 건물에서 할당받는 외부 IP가 인터넷에 연결할 때 마다 바뀌어, 최고 점수를 받는 시점의 IP 주소를 모르겠습니다. </p>
	<p> 가장 최근에 보낸 IP주소는 210.57.238.3입니다. </p>
#### 소스 코드 설명
	<p> 기본적으로 주어진 classify_server.ipynb와 soma_classifier.ipynb를 뼈대로 코드를 작성하였으나, 
	상황을 바꿔가며 테스트 하기 위해 비슷한 코드를 여러개 만들었습니다. </p>
	<p> 최고 점수를 받은 시점의 commitd은 <a href="https://github.com/YeongjinOh/docker_classifier/commit/22ee58062a28c1c1eadb2190c18495784b79323f"> "split morph" </a> 입니다.
	training.ipynb 코드 내에서 training을 진행하며 학습 프로세스는 아래와 같습니다.  </p>
	<ol>
		<li>stop words 제거 </li>
		<li>konply를 이용한 형태소 단위 쪼개기</li>
		<li>caffe를 이용하여 이미지 데이터 활용 (캐싱해놓은 json 결과 파일을 이용)</li>
		<li> 10000개중 9000개의 data로 training </li>
		<li> 나머지 1000개의 data로 validation </li>
	</ol>
