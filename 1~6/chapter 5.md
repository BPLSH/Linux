<chapter 5>  
===========  

### 접근 권한 변경 ###  
**chmod**  
* 기호모드 : chmod u+w,go-w test.c  
* 숫자모드 : chmod 755 test.c  

### 기본 접근 권한 변경 ###
**umask**  
* umask : 기본 마스크 값을 보여줌  
* -S : 마스크 값을 문자로 출력  
* umask 보수를 취한다. 텍스트 파일은 666이 최대, 디렉터리나 실행파일은 777이 최대.  
  
### 특수 접근 권한 변경 ###  
* umask의 네자리 중 맨 앞자리는 특수 접근 권한을 나타냄  
* 맨 앞자리가 0이면 기본접근 권한  
* 스티키 비트 : 1  
  디렉터리에 스티키 비트가 설명되어있으면 디렉터리 안에 누구나 파일 생성 가능(기타 사용자의 실행 권한에 'T' 표시)  
* SetGID : 2  
  해당 파일이 실행되는 동안에는 파일 소유 그룹의 권한이 적용된다.(그룹의 실행 권한이 's' 표시)  
* SetUID : 4  
  파일 소유자의 권한이 적용된다.(소유자의 실행 권한이 's' 표시)  
  

