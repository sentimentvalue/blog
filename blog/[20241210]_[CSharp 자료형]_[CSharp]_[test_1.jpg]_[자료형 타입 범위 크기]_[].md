# CSharp 자료형: 타입, 범위, 크기
<br>

### 정수형: 
sbyte   <br>
   -  -128  ~  128                  
        - 8bit 1byte<br><br>

byte    <br>
   -  0  ~  255
        - 8bit 1byte<br><br>

short   <br>
   -  -32,768  ~  32,768             
        - 16bit 2byte <br><br>

ushort  <br>
   -  0  ~  65,535
        - 16bit 2byte<br><br>

int     <br>
   -  -2,147,483,648  ~  2,147,483,647
      - 32bit 4byte<br><br>

uint  
   -  0  ~  4,294,967,295
      - 32bit 4byte<br><br>

long<br>
   -  -9,223,372,036,854,775,808  ~  9,223,372,036,854,775,807
      - 64bit 8byte<br><br>

ulong<br>
   -  0  ~  18,446,744,073,709,551,615
      - 64bit 8byte<br>
<br>

### 실수형: 
float<br>
   -  32bit 4byte<br><br>

double<br>
   -  64bit 8byte<br><br>

decimal<br>
   -  128bit  16byte<br>
<br>

### 문자형:
char    <br>
   -  유니코드 16bit 문자<br><br>

string<br>
   -  유동적(입력값 크기에 따라)<br><br>
   -  값: 참조 타입

### 논리형: 
bool<br>
   -  1bit<br>
<br>

### Object: 
- 모든 타입의 값을 담을 수 있다. 인스턴스 포함<br>
- 남발할시 메모리 공간 낭비에 주요 범인<br>
<br>

### 추가: 
- 크기가 큰 자료형 변수일수록 처리가(계산) 오래걸림