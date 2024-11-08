- **DI**
    - Dependency Injection으로 의존관계 주입이라고 한다.
    - 체는 자신이 필요로 하는 의존성(다른 객체)을 직접 생성하지 않고, 외부에서 전달받아 사용 → 프로그램의 결합도를 낮추고, 테스트와 유지 보수를 용이
    - 의존한다 라는것 → ex) A가 B를 의존한다. B가 변하면 A에 영향을 미친다.
    - Spring Framework에서 @Autowired와 같은 애노테이션으로 DI를 구현합니다.
- **IoC**
    - IOC는 제어의 역전으로 인스턴스의 생성부터 소멸까지 개발자가 아닌 컨테이너가 대신 관리해주는 것을 말한다. (프레임워크)
    - IOC 컨테이너는 DI를 통해 주입시킨다.
    - 인스턴스의 생성의 제어를 서블릿과 같은 bean을 관리해주는 컨테이너가 관리합니다.
- **프레임워크와 API의 차이**
    - 프레임워크는 애플리케이션 개발을 위한 구조와 필요한 기능을 미리 제공하는 큰 틀
    - 프레임워크는 개발자가 직접 호출하는 것이 아니라, 프레임워크가 개발자의 코드를 호출하며, 개발자는 프레임워크가 제공하는 규칙에 맞춰 코드를 작성
    - API는 특정 기능을 수행하는 함수와 그에 대한 설명을 제공하는 인터페이스입니다. →개발자는 API를 호출하여 필요한 기능을 구현
    - API는 일반적으로 라이브러리 형태로 제공되며, 개발자가 직접 메서드를 호출하여 사용
    - 프레임워크는 애플리케이션의 구조와 실행 흐름을 제어하는 반면, API는 특정 기능을 수행하는 데 필요한 도구와 인터페이스만 제공
- **AOP**
    - AOP는 관점 지향 프로그래밍
    - 핵심 로직과 공통 기능을 분리하여 코드의 중복을 줄이고 유지보수를 쉽게 하는 프로그래밍 방식

      → 모든 서비스 메서드에 로그를 기록하는 기능이 필요할 때, 각 메서드마다 로그 코드를 넣는 대신, AOP를 사용하여 특정 지점(예: 메서드 시작 전후)에 자동으로 로그가 기록되도록 설정할 수 있습니다.

    - Advice: 특정 시점에 실행될 코드 (예: Before, After, Around)
    - Join Point: Advice가 적용될 수 있는 지점 (메서드 호출, 객체 생성 등)
    - Pointcut: Advice를 적용할 실제 대상 지점의 정의
- **서블릿**

  Java를 사용해 웹 애플리케이션의 요청과 응답을 처리하는 서버 사이드 프로그래밍 기술입니다. 웹 서버에서 실행되며, 클라이언트(웹 브라우저)의 요청을 받아 데이터를 처리하고, 결과를 HTML 형태로 클라이언트에 응답합니다.

    - 동작과정
    1. 클라이언트가 HTTP 요청을 보냄.
    2. 서블릿 컨테이너가 서블릿을 호출하여 요청을 전달함.
    3. 서블릿이 요청을 처리하고 응답을 생성하여 컨테이너에 전달함.
    4. 컨테이너가 응답을 클라이언트로 전송함.

  ###