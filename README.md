핵심 작동 단계

0. 서버 생성
1. 교내 강의계획안 사이트로부터 크롤링으로 강의계획서 파일 저장
2. 다양한 형식의 파일을 통일된 형식으로 변환
3. tabula를 통해 자연어 추출, csv파일 생성
4-1. google vision API를 통해 자연어 추출, csv파일 생성
4-2. 추출한 문자를 koNLPY와 NLTK를 이용하여 자연어처리 및 요약
5. 강의계획서 및 csv 파일을 서버의 database에 저장

4-2, 5의 강의계획서 저장 부분은 아직 미구현인 상태입니다.

main 폴더 설명

FileScanner : 
data_1200 : 테스트를 쉽게 하기 위해 강의계획서 1200개를 수동으로 다운받아 모은 폴더입니다.
extract_file :
web : 서버 구현, 크롤링 구현과 관련된 폴더입니다.
