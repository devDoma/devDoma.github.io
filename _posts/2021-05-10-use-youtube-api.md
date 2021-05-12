# 유튜브 API 활용하기

생성일: 2020년 12월 17일 오전 9:22
업데이트됨: 2020년 12월 17일 오후 12:58

## 왜 이 글을 쓰냐면...

안드로이드 내 자체 광고(광고가 막혀있을 경우 자사 유튜브 채널을 홍보하는 방향으로 정해짐)를 달기 위해서 유튜브 api 를 사용하게 되었다.

유튜브는 영상 재생을 지원하는 Youtube Player API와

[YouTube Android Player API | YouTube for Android | Google Developers](https://developers.google.com/youtube/android/player?hl=ko)

유튜브 컨텐츠와, 비디오 업로드, 플레이리스트 추가 제거를 지원하는 Youtube Data API를 제공한다.

[시작하기 | YouTube Data API | Google Developers](https://developers.google.com/youtube/v3/getting-started?hl=ko)

그 외에도 구독버튼, 라이브 스트리밍, 애널리틱스를 제공하니 참고하자.

## 안드로이드에 유튜브 플레이어 넣기

사실 나는 광고를 만들려고 하기 때문에 필요한 기능이 많지 않다.

내가 필요한 기능은 다음과 같다

1. 링크의 영상 재생
2. 영상을 특정 시간 동안 재생했는지 추적 후 이벤트
3. +영상 리스트의 링크들을 업데이트할 필요없이 가져오기

 1,2번은 Youtube Player  API, 3번은 Data API 이다. 3번 기능은 부가적인 것으로 만일 너무 공수가 크다면 손수 링크를 넣는 것으로 대체할 예정이다.

 먼저 익숙한 Gradle implementation 방식으로는 API를 사용할 수 없고 소스 코드를 다운받아서 라이브러리로 등록해야 한다고 한다. 유튜브가 얼마나 큰 플랫폼이고, 얼마나 핫한지를 생각해보면 이런 예전 방식을 고수하는게 놀라울 정도지만 어쩌겠는가. 구글이 갑이다.

 먼저 공식문서에서 안내하는 순서는 다음과 같다.

1. 라이브러리 코드 다운로드
2. 앱을 구글 API Console에 등록
3. 초기 설정
4. 샘플 애플리케이션

해당 문서가 굉장히 노후화되어(무려 이클립스 사용법을 안내해준다) 다른 블로그 글을 참고하였다.

[[Android Studio]Youtube(유튜브) 재생을 위한 API 사용하기 위한 준비 과정(SHA1 정보 보기)](https://xrexter.tistory.com/59)

먼저 라이브러리는 다운로드 받았고(공식문서에서) 앱을 구글 API Console에 등록 또한 안내에 따랐다. 이 떄 API는 **자격 증명**을 요구하는데, 이는 누가 해당 API를 사용했는지 추적하고 그에 따라 charge를 하기 위함이다. 상식적으로 영상 API를 공개해놨는데, 이런 과정없이 한다면 누구나 무한대로 영상을 갖다 쓸 수 있으니 반드시 필요한 과정이라 생각된다.

 이 자격증명에는 두가지 방식이 있다. Oauth 2.0 토큰으로 인증하는 방식과, API 키를 발급받아 사용하는 방식이 있는데, 나는 API 키 방식을 사용할 예정이다. Oauth 2.0은 클라이언트에 따라 토큰이 달라져 더 까다롭고, 웹과 앱을 둘다 지원해야하는 현 개발 상황과 맞지 않다.

API키를 만드는 과정은 이미 예전에 Firebase를 사용할 때 만들어놨으므로 생략한다.
비교적 쉬우니 공식문서를 보고 잘 따라가면 된다.

내가 공식문서에서 막혔던 부분이 뭐냐면 다운로드 받은 소스코드를 intelliJ 를 통해 설치하는 방법이다. 애초에 Import Project를 하면 새로운 프로젝트가 만들어지거나, 기존 프로젝트를 선택하면 덮어씌운다고 안내하기에 진행이 불가능하다.

 어쨌건 블로그 글에 따르면 다음과 같이 진행한다. 일반적인 라이브러리 생성 방법인듯 한데 처음 접해 본다.

1. 압축 푼 폴더에서 libs 폴더로 이동한 후 YouTubeAndroidPlayerApi.jar 파일을 선택한 후 복사한다.
2. 안드로이드 스튜디오에서 좌측상단에서 Project 로 변경 한 후 앱명 -> app -> libs 를 클릭 한 후 붙여 넣기를 한다. 이 때 libs폴더가 없다면 생성해준다.
3. 추가 된 jar 파일을 우클릭 한 후 아래 쪽에 Add as Libary... 를 클릭해 진행한다.
4. 제대로 되었는지 확인하기 위해 app 수준의 build.gradle 파일을 열어 implementation files('lib/YouTubeAndroidPlayerApi.jar') 이 있는지 확인한다.

### 유튜브 플레이어 준비하기

드디어 대망의 코드 작업이다. 아래 링크를 참조하였다.

[안드로이드 유튜브 플레이어 예제](https://gamjatwigim.tistory.com/39)

대략적인 흐름은 다음과 같다.

1. youtube player view의 아이디를 찾는다.
2. initialize 해준다.
3. youtube key를 호출해준다.
4. YouTubePlayer.OnInitializedListener를 상속받는다.
5. onInitialiizationSuccess에 호출할 youtubePlayer의 key를 받아서 youtubePlayer객체를 오버라이드 받은 것을 cueVideo를 해준다.

```jsx
class YoutubePlayerActivity : YouTubeBaseActivity(), YouTubePlayer.OnInitializedListener {
    override fun onInitializationFailure(p0: YouTubePlayer.Provider?, p1: YouTubeInitializationResult?) {
        TODO("not implemented") //To change body of created functions use File | Settings | File Templates.
    }
 
    override fun onInitializationSuccess(p0: YouTubePlayer.Provider?, youtubePlayer: YouTubePlayer?, isReady: Boolean) {
        if (!isReady) {
            val playKey = intent.getStringExtra("playKey")
            youtubePlayer!!.cueVideo(playKey);
        }
    }
 
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_youtube_player)
        youtube_view.initialize(getString(R.string.youtube_key), this@YoutubePlayerActivity)
    }
}
```

위의 코드대로 제대로 실행이 되었다면, 액티비티에서 재생되는 유튜브영상이 준비될 것이다.

### 유튜브 플레이어 컨트롤하기

위의 코드대로 영상은 실행이 되지만 보상형광고로서 기능하기 위해서는 시청 시간에 대한 이벤트를 받아야 한다.

## 오류사항

- 유튜브 api의 버전에 주의하자. 1.0.0 버전을 받아서 오류가 발생했다.

[Android L Youtube API - IllegalArgumentException: Service Intent must be explicit](https://stackoverflow.com/questions/27174515/android-l-youtube-api-illegalargumentexception-service-intent-must-be-explici)
