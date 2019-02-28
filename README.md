### 다음 TV의 메타정보를 이용하여 이름, 회차정보, 날짜로 파일 이름 변경 해준다.
## 가능한 형식
**변경전**  
이름.E01.190101.720p-AAA  
이름 1-2회 합본.E01.190101.1080p.ETC-BBB  
**변경후**  
검색된이름.E01.190101.720p-AAA  
검색된이름.E01-E02.190101.1080p.ETC-BBB  

**사용 환경 : 파이썬 2.7**  
**renamefile.json 설정항목** 

DOWNLOADDIR - 파일명이 변경될 파일이 있는 디렉토리
TARGETDIR    - 이름이 변경된 파일이 저장될 디렉토로  
DUPEDIR     - 중복된 파일 있을 때 저장되는 디렉토리  
IS_GENRE     - 장르명과 제목으로 파일이 저장될 경로 생성  
선택항목 : 'Y, y, N, n'  
ex)DOWNLOADDIR/장르명/제목/제목.E01.1801010.ETC.mp4  
기본값 : N  
IS_ETC                     - 파일명에 릴정보 등 추가 여부 선택  
                                    선택항목 : 'Y, y, N, n'  
                                    ex) 제목.E01.1801010.ETC.mp4  
                                    기본값 : Y  
IS_SEASON              - 파일명에 시즌 번호  추가 여부 선택  
                                      에피소드 번호가 1000이 넘어가는 경우 자동으로 추가  
                                    선택항목 : 'Y, y, N, n'  
                                    ex) 제목.S01E01.1801010.ETC.mp4  
                                    기본값 : N  

ZEROFILL                  - 에피소드번호 앞에 0추가  
                                      기본 값은 2  
                                      ex) 2일때 01,02, 03, 09, 10, 100  
                                             3일때 001, 002, 100, 1000  
DELIMITER                - 파일명의 구분자  
                           기본값은 .
