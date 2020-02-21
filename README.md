# Android-Architecture-Components.

Android Architecture Components를 이해하기 위해 스스로 공부한 것을 정리하고 직접 프로젝트로 만들어보며 이해하기 위한 레퍼지토리입니다.

- [모바일 앱 사용자 환경](https://github.com/Jaesungchi/Android-Architecture-Components#모바일 앱 사용자 환경)

## 모바일 앱 사용자 환경

데스크톱 앱과 안드로이드의 다른점은 데스크톱 앱의 경우는 단일 진입점이 있고 하나의 모놀리식 프로세스로 실행됩니다. 하지만 안드로이드는 액티비티, 프래그먼트, 서비스, Content Provider, Broadcast Receiver등의 여러 앱 구성요소가 포함됩니다.

안드로이드에서는 짧은 시간내에 여러 앱과 상호작용할때가 많아 앱이 사용자 중심의 다양한 워크플로 와 작업에 맞게 조정이 되어야합니다. 왜냐하면 다양한 과정에서 다른 앱을 들어갔다가 돌아온다던지, 화면이 회전된다던지 , 전화가 온다던지 등의 다양한 과정에서 사용환경이 중단 될 수 있습니다. 이러한 환경에서 중단이 된 후 다시 돌아가도 하던 작업들이 남아있어야 합니다. 또한, 운영체제에서 새로운 앱을 위한 공간을 확보하기 위해 언제든지 앱의 프로세스를 종료할 수 있습니다.

이러한 환경을 고려해보면 운영체제나 사용자가 앱의 구성요소를 언제든지 제거 할 수 있기 때문에 앱 구성요소에 앱 데이터나 상태를 저장해서는 안되며 앱 구성요소가 서로 종속되면 안됩니다.



---

# 출처

[앱 아키텍처 가이드](https://developer.android.com/jetpack/docs/guide)