모해라는 앱을 팀 git에서 개발 중입니다.
오늘 모해'라는 앱을 개발하고 있습니다. 오늘 모해는 개인 혹은 여러명이 모였을 때, 놀고 싶은데 뭘 해야할지 모를 때 몇번의 버튼 클릭으로 가볍게 뭐하고 놀지 추천받을 수 있는 앱입니다. 저희는 쉬운 접근성과 정확한 결과 도출에 초점을 두고 개발하고 있습니다.

앱 개발 파트 : 로그인 및 회원 가입, 성격 파악 조사, 상세 조사, 추천 리스트 표시 및 지도 표시

인원 별 개발 파트 : 
이주영 – 상세 조사
김도윤 – 로그인 및 회원 가입
권혁준 – 추천 리스트 표시 및 지도 표시
박유진 – 성격파악조사

사용한 프레임워크 : googleplace, googlemaps, swiftyjson, firebase, snapkit, facebooksdk, kakaosdk, googlesdk

사용한 api : google place api

진행사항:
현재 ‘로그인’, ‘성격 파악 조사’, ‘상세 조사’, ‘추천리스트’ 화면으로 네명이 각자 나누어 진행중에 있습니다.

처음 들어가면 보이는 로그인 화면은 구글, 페이스북, 카카오로 로그인이 가능하도록 기능을 추가 하였으며, 추후에 애플 로그인도 추가할 예정입니다.
그리고 사용자가 최초 로그인 시 사용자의 성격을 파악할 수 있는 40개의 질문지 화면을 제공받게됩니다.
최초 로그인이 아닐때는 로그인 사 바로 상황 파악 질문지 5개가 나오게됩니다. 
두 설문지를 통한 현재 사용자의 상태 파악이 완료 하면 알고리즘에 의하여 놀거리가 추천되고 사용자가 재추천을 원할시 다시 추천받을 수 있는 버튼을 구현합니다. 
추천을 받는 것을 원하면 아래에 추천 키워드와 관련된 리스트가 뜨게 되고 리스트에서 원하는 매장이나 놀거리를 누르면 사용자 위치를 기반으로 지도에서 검색되어 핀이 뜨게 됩니다.
https://github.com/team-mohae/MoHae/ 
여기서 자료를 볼 수 있습니다.

추천을 해줄 놀 수 있는 곳 리스트

- 불꽃 놀이
- EDM 페스티벌
- 계절별 꽃 축제
- 먹거리 축제
- 북 페스티벌
- 가구 만들기 클래스
- 바리스타 클래스
- amusement_park - 놀이공원
- aquarium - 수족관
- art_gallery - 미술관
- bakery - 빵집
- bar - 술집
- beauty_salon - 미용실 네일
- bicycle_store - 자전거
- book_store - 서점
- bowling_alley - 볼링
- cafe - 카페
- campground- 캠핑장
- church - 교회
- florist - 꽃집
- gym - 요가 스포츠클럽
- library - 도서관
- lodging - 하숙 모텔 호텔
- movie_rental - dvd
- movie_theater - 영화관
- museum - 박물관
- night_club - 클럽 노래방
- park - 공원
- pet_store - 펫샵
- restaurant -음식점
등등


platform :ios, '11.0'
use_frameworks!

target 'Mohae' do
    pod 'Firebase/Core'
    pod 'Firebase/Database'
    pod 'SnapKit', '~> 5.0.0'
    pod 'Firebase/Auth'
    pod 'GoogleMaps'
    pod 'GooglePlaces'
    pod 'Alamofire'
    pod 'SwiftyJSON'
    pod 'Firebase'
end
