layout	title	date	blurb	og_image
post
Post example
2021-03-26 10:00:40 -0700
A look at an example post using Bay Jekyll theme.
/assets/img/content/post-example/Banner.jpg
<img src="{{ "/assets/img/content/post-example/Banner.jpg" | absolute_url }}" alt="bay" class="post-pic"/>

### - JVM이란 무엇인가

> JVM(Java Virtual Machine), JAVA 개발환경에서 JAVA Compiler는 {*}.java파일을 {*}.class라는 Java Byte Code로 변환한다.
> 여기서, Byte Code는 Machine Langueage가 아니기 때문에 OS에서 바로 실행되지 않는다.
> 이에, OS에서 바로 JAVA를 컴파일하고 실행하기위해 JVM이 Byte Code를 해석하여 실행해주는 역할을 수행한다.
> **따라서, JVM을 사용하게 되면 특정 OS에 종속되지 않는다는 특징을 가지게 된다.**

### - 컴파일 하는 방법

> {*}.java 파일을 컴파일하여 Byte Code인 {*}.class 파일로 만든다.
> => $javac {*}.java
> => {*}.class 파일이 생성되어있는지 확인

### - 실행하는 방법

> {*}.java를 컴파일한 {*}.class Byte Code파일을 실행한다.
> => $java {*}

### - 바이트 코드란 무엇인가

> 바이트 코드란, JVM이 해독할 수 있는 JAVA compiler에 의해 컴파일된 자바 소스 코드이다.

> {*}.java 파일을 JAVA compiler에 의해 compile을 수행하면, {*}.class 파일이 생성되며 이 파일이 바이트 코드이다.

> 이렇게 생성된 {*}.class 바이트 코드를 JVM에서 해독하여 프로그램 구동을 수행한다.


### - JIT컴파일러란 무엇이며 어떻게 동작하는지

> JIT(Just-In-Time) compiler는 바이트 코드를 CPU로 직접 전달할 수 있는 명령어로 바꾸는 컴파일러이다.

> 즉, JIT 컴파일러란 바이트코드({*}.class)를 CPU에서 구동할 수 있는 명령어로 바꾸어 전달하는 JVM에 해당한다.


### - JVM 구성 요소

> _인터프리터_ : 인터프리터란, JAVA compiler로 컴파일된 {*}.class 파일을 각 하드웨어 및 OS에 종속적이지 않도록 특성에 맞게 변환해주는 역할을 수행한다. 이를 통해 JAVA는 OS 및 하드웨어에 종속적이지 않을 수 있게된다.

> _클래스 로더_ : 클래스 로더란, 말그대로 클래스 파일 ({*}.class)을 읽어들이는 역할을 수행한다.

> _Runtime Data Area_ : JVM의 메모리 영역으로 JAVA Application을 실행할때 사용되는 데이터들을 적재하는 영역이다. 클래스 로더에 의해 로딩되는 클래스 파일들은 Runtime Data Area에 적재된다.

> _실행 엔진_ : 클래스 로더에 의해 Runtime Data Area에 적재된 클래스 파일을 기계어로 변환하고 실행하는 역할을 수행한다.

> _가비지 콜렉터_ : 가비지 콜렉터는 Heap영역에서 생성된 객채들 중에 참조되지 않아 사용하지 않는 객체들을 찾아서 제거하는 역할을 수행한다.


### - JDK와 JRE의 차이

__> JDK(Java Development Kit) : JVM, JAVA API, JAVA Tool, JAVA Compiler 등, JRE에서 제공하는 환경들과 개발에 필요한 명령어, JAVA 컴파일러까지 포함된 kit._
_> JRE(Java Runtime Environment) : JVM, JAVA API와 같이 JAVA Application을 실행하기 위한 최소의 실행환경을 제공.__

> JDK와 JRE의 차이 : 위에서 설명했듯이, JRE는 JAVA Application을 실행하기 위한 최소한의 실행환경을 포함하고 있으며, JDK는 JRE에서 제공하는 실행환경뿐만아니라, JAVA 개발에 필요한 명령어들과 JAVA Compler를 포함한 kit라는 차이점을 가지고 있다.
