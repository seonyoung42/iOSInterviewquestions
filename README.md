# iOSInterviewquestions

## iOS
<details> 
  <summary> Bounds 와 Frame 을 설명하시오. </summary>
  
  ```
  bounds: 자신을 기준으로 view의 위치와 크기를 표현
  frame: 슈퍼뷰를 기준으로 view의 위치와 크기를 표현
  ```
  
</details>

<details> 
  <summary> 실제 디바이스가 없을 경우 개발 환경에서 할 수 있는 것과 없는 것을 설명하시오. </summary>
  
  ```
  할 수 있는 것 : 애플페이, face id
  할 수 없는 것 : 카메라, push 알림
  ```
  
</details>

<details> 
  <summary> 앱의 콘텐츠나 데이터 자체를 저장/보관하는 특별한 객체를 무엇이라고 하는가? </summary>
  
  ```
  UserDefaults
  : 앱이 실행되는 동안(런타임) Key-Value 형태로 데이터를 저장하는 사용자의 기본 데이터베이스에 대한 인터페이스
  
  - 대용량의 데이터보다 단일 데이터(ex 사용자 기본 설정, 로그인 여부 등)를 저장하는데 더 적합
  - 싱글톤 패턴으로 설계되어 앱 전체에 단 하나의 인스턴스만 존재
  ```
 
</details>

<details> 
  <summary> 앱 화면의 콘텐츠를 표시하는 로직과 관리를 담당하는 객체를 무엇이라고 하는가? </summary>
  
  ```
  UIViewController
  : UIKit 기반 앱의 뷰 계층 구조를 관리하는 객체
  
  - 데이터의 변경에 대한 응답으로 뷰의 업데이트
  - 뷰 크기 조정 및 전체 인터페이스 레이아웃 관리
  - 뷰와의 사용자 상호 작용에 응답
  ```
</details>

<details> 
  <summary> App thinning에 대해서 설명하시오. </summary>
  
  ```
  App thinning
  : 사용자의 기기와 OS버전에 맞춰 필요한 앱 번들을 만들고 전달하는 것
  
  - App store와 OS가 사용자의 기기와 OS버전에 맞게 App의 기능을 제공하고 설치공간을 최소화하여 App 설치 최적화
  - 더 빠른 다운로드와 더 많은 공간을 제공
  - App thinning 방법 
    - Slicing : App store가 앱이 지원하는 기기 및 OS 버전에 따라 다양한 변형(App variant)를 제공하는 것
    - Bitcode : Appstore가 다운로드되기전에 디바이스에 맞게 앱을 최적화 하여 바이너리를 새로 만들어 제공하는 것
    - ODR(= Order-Demand-Resource, 주문형 리소스) : 사용자에게 해당 리소스가 필요할 때 그 리소스를 앱스토어에서 가져오는 것
  ```
</details>

<details> 
  <summary> @main에 대해서 설명하시오. </summary>
  
  <img width="436" alt="스크린샷 2023-06-17 오후 6 06 53" src="https://github.com/seonyoung42/iOSInterviewquestions/assets/77603632/c479ec91-bd4e-4876-816a-a28e26825612">

  ```
  @main
  : 프로그램 실행 시작 시 진입점을 지정하기 위한 Swift 언어의 기능
  
  @main을 선언해줌으로써 UIKit 앱의 진입점은 해당 클래스가 되고 시스템은 UIApplicationDelegate 프로토콜에 구현되어있는 정적 main() 함수를 호출하게 된다
  ```
  
</details>

<details> 
  <summary> 앱이 foreground에 있을 때와 background에 있을 때 어떤 제약사항이 있나요?  </summary>
  
  ```
  
  ```
  
</details>

<details> 
  <summary> 상태 변화에 따라 다른 동작을 처리하기 위한 앱델리게이트 메서드들을 설명하시오. </summary>
  
  ```
  
  ```
  
</details>

<details> 
  <summary> 앱이 In-Active 상태가 되는 시나리오를 설명하시오. </summary>
  
  ```
  
  ```
  
</details>

<details> 
  <summary> Scene delegate에 대해 설명하시오.  </summary>
  
  ```
  
  ```
  
</details>

<details> 
  <summary> UIApplication 객체의 컨트롤러 역할은 어디에 구현해야 하는가?  </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> App의 Not running, Inactive, Active, Background, Suspended에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> NSOperationQueue 와 GCD Queue 의 차이점을 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> GCD API 동작 방식과 필요성에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Global DispatchQueue 의 Qos 에는 어떤 종류가 있는지, 각각 어떤 의미인지 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> iOS 앱을 만들고, User Interface를 구성하는 데 필수적인 프레임워크 이름은 무엇인가? </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Foundation Kit은 무엇이고 포함되어 있는 클래스들은 어떤 것이 있는지 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Delegate란 무엇인지 설명하고, retain 되는지 안되는지 그 이유를 함께 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> NotificationCenter 동작 방식과 활용 방안에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> UIKit 클래스들을 다룰 때 꼭 처리해야하는 애플리케이션 쓰레드 이름은 무엇인가? </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> App Bundle의 구조와 역할에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>


<details> 
  <summary> 모든 View Controller 객체의 상위 클래스는 무엇이고 그 역할은 무엇인가? </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> 자신만의 Custom View를 만들려면 어떻게 해야하는지 설명하시오. </summary>
  
  ```
  ```
  
</details>


<details> 
  <summary> View 객체에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>


<details> 
  <summary> UIView 에서 Layer 객체는 무엇이고 어떤 역할을 담당하는지 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> iOS에서 뷰(View)와 레이어(Layer)의 개념과 차이점에 대해 설명해보세요.</summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> UIWindow 객체의 역할은 무엇인가? </summary>
  
  ``` 
  ```
  
</details>

<details> 
  <summary> UINavigationController 의 역할이 무엇인지 설명하시오.</summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> TableView를 동작 방식과 화면에 Cell을 출력하기 위해 최소한 구현해야 하는 DataSource 메서드를 설명하시오.</summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> 하나의 View Controller 코드에서 여러 TableView Controller 역할을 해야 할 경우 어떻게 구분해서 구현해야 하는지 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> setNeedsLayout와 setNeedsDisplay의 차이에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> stackView의 장점과 단점에 대해서 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> NSCache와 딕셔너리로 캐시를 구성했을때의 차이를 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> URLSession에 대해서 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> prepareForReuse에 대해서 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> 다크모드를 지원하는 방법에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> ViewController의 생명주기를 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> TableView와 CollectionView의 차이점을 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Dynamic Library와 Static Library의 차이점에 대해 설명해보세요. </summary>
  
  ```
  ```
  
</details>

## Autolayout
- 오토레이아웃을 코드로 작성하는 방법은 무엇인가? (3가지)
- hugging, resistance에 대해서 설명하시오.
- Intrinsic Size에 대해서 설명하시오.
- 스토리보드를 이용했을때의 장단점을 설명하시오.
- Safearea에 대해서 설명하시오.
- Left Constraint 와 Leading Constraint 의 차이점을 설명하시오.
- Auto Layout과 Frame-based Layout의 차이점은 무엇인가요?
- 성능 향상을 위해 어떤 디버깅 도구를 사용할 수 있나요? 각각의 디버깅 도구는 어떤 상황에서 사용하는 것이 좋나요?

## Swift
<details> 
  <summary> struct와 class와 enum의 차이를 설명하시오. </summary>
  
  ```
  struct : 상속(x), 값 타입 - 스택에 저장, 
  class : 상속(ㅇ), 참조 타입 - 스택에 포인터/힙에 데이터 저장,
  enum : 상속(x), 참조 타입 - 스택에 포인터/힙에 데이터 저장,
  
  셋의 공통점 : extenstion으로 기능 확장 가능, 프로토콜 채태 가능
  ```
  
</details>

<details> 
  <summary> class의 성능을 향상 시킬수 있는 방법들을 나열해보시오. </summary>
  
  ```
  class에 접근제어자(final, privete)을 사용해 Dynamic Dispatch 메커니즘으로 작동하는 Class를 Static Dispatch 방식으로 작동하게 한다.
  
  Static Dispatch : 앱이 동작하기 전인 컴파일 시점에 호출할 함수를 결정하기 때문에 성능이 좋다.
  Dynamic Dispatch : 컴파일 이후 앱을 실행하는동안인 런타임 시점에 호출하 함수를 결정하기 때문에 성능이 떨어진다.
  ```
    
</details>

<details> 
  <summary> Copy On Write는 어떤 방식으로 동작하는지 설명하시오. </summary>
  
  ```
  Copy On Write
  : Swift의 값 타입은 새로운 변수를 할당하거나 파라미터로 전달될 때 값 복사가 일어난다.
  다만, 이러한 복사 작업은 상당한 시간이 걸리므로 실제 원본이나 복사본이 수정되기 전까지는 복사를 하지 않고 원본 리소스를 공유하다가
  원본이나 복사본에서 수정이 일어날 경우, 그때 복사하는 작업을 하는 기술이다. 
  
  - Swift에선 Collection Type(Array, Dictionary, Set)을 복사해서 사용
  ```
  
</details>

<details> 
  <summary> Convenience init에 대해 설명하시오. </summary>
  
  ```
  
  ```
  
</details>

<details> 
  <summary> AnyObject에 대해 설명하시오. </summary>
  
  ```
  
  ```
  
</details>

<details> 
  <summary> Optional 이란 무엇인지 설명하시오. </summary>
  
  ```
  
  ```
  
</details>

<details> 
  <summary> Struct 가 무엇이고 어떻게 사용하는지 설명하시오. </summary>
  
  ```
  
  ```
  
</details>

<details> 
  <summary> Subscripts에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> String은 왜 subscript로 접근이 안되는지 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> instance 메서드와 class 메서드의 차이점을 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> class 메서드와 static 메서드의 차이점을 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Delegate 패턴을 활용하는 경우를 예를 들어 설명하시오. </summary>
  
  ```
  ```
  
</details>
<details> 
  <summary> Singleton 패턴을 활용하는 경우를 예를 들어 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> KVO 동작 방식에 대해 설명하시오.  </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Delegates와 Notification 방식의 차이점에 대해 설명하시오.  </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> 멀티 쓰레드로 동작하는 앱을 작성하고 싶을 때 고려할 수 있는 방식들을 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> MVC 구조에 대해 블록 그림을 그리고, 각 역할과 흐름을 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> 프로토콜이란 무엇인지 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Protocol Oriented Programming과 Object Oriented Programming의 차이점을 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Hashable이 무엇이고, Equatable을 왜 상속해야 하는지 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> mutating 키워드에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> 탈출 클로저에 대하여 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Extension에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Extension 내부에서 함수를 override할 수 있는지 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> 접근 제어자의 종류엔 어떤게 있는지 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> defer란 무엇인지 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> defer가 호출되는 순서는 어떻게 되고, defer가 호출되지 않는 경우를 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> property wrapper에 대해서 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Generic에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> some 키워드에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>


<details> 
  <summary> Result타입에 대해 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Codable에 대하여 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Closure에 대하여 설명하시오. </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Optional Chaining과 nil-coalescing operator(??)의 차이점과 사용 시 주의사항은 무엇인가요? </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> Swift에서 Async/Await 기능이 도입되기 전에, 비동기(Asynchronous) 작업을 처리하는 방법에는 어떤 것들이 있나요? </summary>
  
  ```
  ```
  
</details>

<details> 
  <summary> 타입 변환(Type Casting)과 다형성(Polymorphism)에 대해 설명해보세요. </summary>
  
  ```
  ```
  
</details>


<details> 
  <summary> Swift에서 타입 안전성(type safety)은 어떤 방식으로 보장되나요? </summary>
  
  ```
  ```
  
</details>

## ARC
- ARC란 무엇인지 설명하시오.
- Retain Count 방식에 대해 설명하시오.
- Strong 과 Weak 참조 방식에 대해 설명하시오.
- 순환 참조에 대하여 설명하시오.
- 강한 순환 참조 (Strong Reference Cycle) 는 어떤 경우에 발생하는지 설명하시오.

## Functional Programming
- 순수함수란 무엇인지 설명하시오.
- 함수형 프로그래밍이 무엇인지 설명하시오.
- 고차 함수가 무엇인지 설명하시오.
- Swift Standard Library의 map, filter, reduce, compactMap, flatMap에 대하여 설명하시오.

## Architecture
- MVVM, MVI, Ribs, VIP 등 자신이 알고있는 아키텍쳐를 설명하시오.
- 의존성 주입에 대하여 설명하시오.

## SwiftUI
- @State에 대해서 설명하시오.

## Combine
- PassthroughSubject에 대해서 설명하시오
- @Published에 대해서 설명하시오
- AnyCancellable에 대해서 설명하시오
- sink에 대해서 설명하시오
- throttle과 debounce의 차이점을 설명하시오.
- Data를 Binding 하는 방법에 대해서 설명하시오.

# Optional
아래부터는 추가로 공부를 하면 좋을 내용들입니다.

Objective-c나 rx는 회사, 팀마다 사용하는곳이 차이가있고 신입이나 주니어기준으로 필수라고 여겨지지않기에 옵셔널에 추가하였습니다.

## Rx
- Reactive Programming이 무엇인지 설명하시오.
- RxSwift를 왜 사용하는지 설명하시오.
- RxSwift의 단점을 설명하시오.
- RxSwift에서 Hot Observable과 Cold Observable의 차이를 설명하시오.
- Subject의 종류와 차이점에 대해 설명하시오.
- Subject와 Driver의 차이를 설명하시오.
- Single, Completable, Maybe의 차이점에 대해 설명하고, 언제 적용하면 좋을지 설명하시오.

## MRC
- ARC 대신 Manual Reference Count 방식으로 구현할 때 꼭 사용해야 하는 메서드들을 쓰고 역할을 설명하시오.
- retain 과 assign 의 차이점을 설명하시오.
- 특정 객체를 autorelease 하기 위해 필요한 사항과 과정을 설명하시오.
- Autorelease Pool을 사용해야 하는 상황을 두 가지 이상 예로 들어 설명하시오. 
- 다음 코드를 실행하면 어떤 일이 발생할까 추측해서 설명하시오.
Ball *ball = [[[[Ball alloc] init] autorelease] autorelease];


