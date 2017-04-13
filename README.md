# Clojure를 여행하는 히치하이커를 위한 안내서
* Clojure라는 언어 자체가 정말 강력한 도구이고, 그나마 대중적인 편에 속한 Lisp 계열언어입니다. 하지만, 국내에는 인지도가 많지도 않고, 리소스가 그렇게 많지도 않으며, 초보자가 입문하기에도 진입장벽이 있습니다. ~(이 글을 처음 쓴 사람도 역시 초보자입니다.)~
  * Clojure라는 프로그래밍 언어를 배우는데 있어서 생태계에 적응하는 것 역시 어려울 뿐만 아니라, 타 프로그래밍 언어 커뮤니티처럼 `따라해보면서 직접 뭔가를 만들어보는` 방식의 예제도 빈약합니다.
  * Clojure 프로젝트를 빌드할 때 볼 수 있는 `uberjar`, `classpath`, `gradle` 등 자바를 모르는 사람이 봤을때 토가 나오는 키워드들, 한번 에러가 발생할때마다 stacktrace가 어렵게끔 출력되는 최소 10개 이상의 에러 로그들, 신경쓰이는 것들이 한두가지가 아닙니다.   
* Clojure로 프로그래밍을 처음 해보는 사람들, 호기심에 Clojure를 접해봤지만 어떻게 써야할 지 몰라 헤매는 사람들, Clojure를 본격적으로 배우기도 전에 헤매는 사람들을 위한 가이드를 만들어보고자 거창하게 `Clojure를 여행하는 히치하이커를 위한 안내서`라는 제목으로 가이드를 작성하고 있습니다.
* 이 가이드는 실용적인 목적으로 쓰이는 것을 지향하고 있습니다. `함수형 프로그래밍이 왜 좋은지`보다는 좀 더 실전에서 직접 활용해볼 수 있는 방향으로 가는 것을 추구합니다. 


# 시작하기
## 로드맵
TODO

## 분야별로 입문하기
TODO

## Clojure 커뮤니티 참여하기
Clojure 커뮤니티에 참여하는 것만으로도 충분히 도움이 됩니다! 다른 개발자 분들과의 인맥을 쌓을수도 있고, 알지 못했던 정보를 알아가기도 하겠죠. 여러분의 조그마한 기여가 저희 Clojure 커뮤니티에 큰 도움이 될 수도 있어요!
* [Clojure Korea Slack](https://clojure-korea.slack.com/)
* [Clojure Korea Facebook](https://www.facebook.com/groups/defnclojure/)

### 유명 개발자들 팔로우하기
Clojure 커뮤니티의 유명한 개발자를 팔로하는 것도 역시 여러분에게 도움이 될 수 있어요! Clojure 관련된 소식을 빠르게 접해볼 수도 있고, Clojure 개발자로서 안목을 키우게 될 수도 있어요!  

#### Twitter
Twitter는 개발자들이 많이 이용하는 SNS 중 하나입니다. 라이브러리 업데이트 소식, Clojure 버전 갱신 소식, 혹은 신기술 동향 등 많은 정보들이 실시간으로 올라옵니다. 관심있는 계정들을 팔로해서 RSS 서비스처럼 이용할 수 있습니다.

##### 한국
* [@dalzony](https://twitter.com/dalzony) : Clojure Bridge Seoul을 주최하신 분입니다.

##### 해외
* [@weavejester](https://twitter.com/weavejester) : Clojure 관련 오픈소스 라이브러리를 많이 만드시는 분입니다. compojure, codox, environ 등 Github 레포지토리의 절반 이상이 Clojure로 짜여져 있습니다.
* [@fogus](https://twitter.com/fogus) : `Joy of Clojure` 저자입니다.

##### 기타
* [@oss_clj](https://twitter.com/oss_clj) : Clojure 관련된 오픈소스 라이브러리 소식이 올라오는 계정입니다.
* [@planetclojure](https://twitter.com/planetclojure) : Clojure와 관련된 아티클들이 실시간으로 올라옵니다.

## 개발환경, 툴

### 편집기
* [VS Code](https://code.visualstudio.com/)
* [Cursive](https://cursive-ide.com/)
* [Emacs](https://www.gnu.org/software/emacs/)
* [Vim](http://www.vim.org/)
* [Atom](https://atom.io/)

### Leiningen
TODO

# 참고자료
## 라이브러리

### Mathematics
* [cats](https://github.com/funcool/cats) : 카테고리 이론을 이용한 FP 구현체입니다.

### Cryptography
* [buddy](https://github.com/funcool/buddy) : Luminus에서 쓰이는 보안 모듈입니다.

### Data Analysis
* [neanderthal](https://github.com/uncomplicate/neanderthal) : 행렬 연산에 쓰이는 라이브러리입니다.
* [gorilla-repl](https://github.com/JonyEpsilon/gorilla-repl) : Python의 Jupyter notebook처럼 입력에 따른 결과를 시각화시켜서 표시해주는 프레임워크입니다.

#### Natural Language Processing
* [postagga](https://github.com/fekr/postagga) : 자연어 처리 라이브러리 입니다.


### Web Scraping
* [enlive](https://github.com/cgrand/enlive) : Python의 beautiful-soup처럼 HTML 의 특정 id, class에 해당되는 문서의 내용을 추출하는데 쓰이는 라이브러리 입니다.

### Web Development

#### Web Framework
* [arachne](http://arachne-framework.org/) : Clojure로 짜인 MVC 웹프레임워크입니다. 
* [Luminus](http://www.luminusweb.net/) : Clojure로 짜인 마이크로 웹프레임워크 입니다.

#### Template engine
* [Selmer](https://github.com/yogthos/Selmer) : Django에서 영감을 얻어서 만들어진 템플릿 엔진입니다.

#### Clojure Script : Clojure와 같은 문법으로 작성하는 프로그래밍 언어이며, 자바스크립트로 트랜스파일됩니다.
* [re-frame](https://github.com/reagent-project/reagent) : Clojure Script로 React 컴포넌트를 사용할 수 있습니다.
* [datascript](https://github.com/tonsky/datascript)


### Documentation
* [codox](https://github.com/weavejester/codox)
  * 함수의 description에 작성한 내용을 토대로 HTML 포맷으로 문서를 생성해줍니다.
  * Markdown 포맷으로 문서를 작성할 수도 있습니다.

### Database
* [Toucan](https://github.com/metabase/toucan) : Clojure용 ORM
* [HoneySQL](https://github.com/jkk/honeysql)
* [Monger](https://github.com/michaelklishin/monger) : Mongo DB Client입니다

#### Database Migration
* [ragtime](https://github.com/weavejester/ragtime)
* [migratus](https://github.com/yogthos/migratus) : Luminus 공식 문서에서 권정하는 라이브러리입니다.

### Environment
* [environ](https://github.com/weavejester/environ) : 환경변수를 관리할때 쓰이는 라이브러리입니다.

### Infra
* [chazel](https://github.com/tolitius/chazel) : Hazelcast 클라이언트입니다.
* [langohr](https://github.com/michaelklishin/langohr) : RabbitMQ 클라이언트입니다.
* [carmine](https://github.com/ptaoussanis/carmine) : Redis 클라이언트입니다.

### API
* [graphql-clj](https://github.com/tendant/graphql-clj) : GraphQL 구현체 입니다.

### For fun
* [yetibot](https://github.com/devth/yetibot) : 챗봇 라이브러리 입니다.


## 책

### 국내에 출판된 책들
* [Brave Clojure](http://www.kyobobook.co.kr/product/detailViewKor.laf?ejkGb=KOR&mallGb=KOR&barcode=9791186697221&orderClick=LAH&Kc=) : 이해하기 쉽게, 수많은 예제코드와 일러스트를 이용해서 설명한 것이 특징입니다.
  * 웹상에서도 무료로 볼 수 있습니다. [Web Version](http://www.braveclojure.com/introduction/)
* [Living Clojure](http://www.kyobobook.co.kr/product/detailViewKor.laf?ejkGb=KOR&mallGb=KOR&barcode=9788966261802&orderClick=LAH&Kc=) : 초보자가 입문하기 괜찮은 책입니다.
* [Joy of Clojure](http://www.kyobobook.co.kr/product/detailViewKor.laf?mallGb=KOR&ejkGb=KOR&barcode=9791186697122) : 어느 정도 Clojure 프로그래밍 경험을 쌓고 나서 보는 것을 추천합니다.

### 해외에 출판된 책들
* [Clojure for Data Science](https://www.amazon.com/Clojure-Data-Science-Henry-Garner/dp/1784397180)
* [Web Development with Clojure](https://pragprog.com/book/dswdcloj/web-development-with-clojure) : Luminus를 이용해서 웹개발하는 방법을 소개합니다.

## 웹사이트
* [Clojure Docs](https://clojuredocs.org/) : Clojure의 Core 라이브러리에 정의된 함수에 대한 친절한 문서와 예제들이 있습니다. 커뮤니티가 주도해서 문서화하는 것이기 때문에, 여러분도 문서화에 참여할 수 있습니다.

### 문제풀이 사이트
* [Project Euler](https://projecteuler.net/) : 수학문제 풀이 중심입니다.
* [4clojure](http://www.4clojure.com/) : Clojure 문제풀이 사이트라면 항상 언급되는 사이트 중 하나입니다. 문제를 풀고나면 다른 사람들이 어떻게 풀이했는지 확인할 수 있습니다.
* [Codewars](https://www.codewars.com/) : 4clojure와 비슷하지만, Ruby/Python/Elixir/C#/Java 등 다양한 언어로 문제풀이를 할 수 있도록 지원합니다. 4clojure와 달리, 새로운 문제가 여러번 갱신된다는 것이 특징입니다.   
* [Exercism](http://exercism.io/)
* [Hackerrank](https://www.hackerrank.com/) : 프로그래밍 문제를 알고리즘, 자료구조, 함수형 프로그래밍, 기타 다양한 분야별로 풀어볼 수 있다는 것이 특징입니다. 여러 기업에서 코딩인터뷰 목적으로 이용하는 사이트이기도 합니다. 

## 아티클
* [Clojure Design Pattern](http://clojure.or.kr/docs/clojure-and-gof-design-patterns.html) : Java와 비교했을 때, Clojure를 이용한 함수형 프로그래밍이 얼마나 강력한지 소개하는 글입니다. 
  * [원문보기](http://mishadoff.com/blog/clojure-design-patterns/)

## 동영상
* [Parallel Programming, Fork Join, and Reducers - Daniel Higginbotham (with slides)](https://www.youtube.com/watch?v=eRq5UBx6cbA) : Clojure를 이용한 병렬 프로그래밍을 다루고 있습니다.

## 슬라이드

* [Clojure - An Introduction for Java Programmers](https://www.slideshare.net/adorepump/clojure-an-introduction-for-java-programmers)

## Best Practices

TODO

## Clojure를 사용하는 기업들
* [Amazon]()
* [Atlassian]()
* [Ebay]()
* [Facebook]()
* [Puppet Labs]()
* [Salesforce]()
* [Soundcloud]()
* [Spotify]()
* [Thought Works]()
* [Walmart Labs]()