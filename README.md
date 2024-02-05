[![logo](https://raw.githubusercontent.com/naver/lucy-xss-filter/master/docs/images/logo/LUCYXSS_792x269px_white.jpg)](https://github.com/naver/lucy-xss-filter)

아래는 Java 17과의 호환성 문제를 해결하기 위해 수정된 Lucy 라이브러리의 새로운 `README.md` 파일 예시입니다. 이 파일은 기존의 내용을 바탕으로 하되, Java 17과의 호환성 문제를 해결한 부분을 강조하여 작성되었습니다.

---

## Overview
이 라이브러리는 기존의 [lucy-xss-filter](https://github.com/naver/lucy-xss-filter)의 기능을 기반으로 하여 Java 17 호환성 문제를 해결한 버전입니다. Java 17에서 `java.persistence` 패키지가 `java.jakarta`로 이동함에 따라 발생한 호환성 문제를 해결하여, 최신 Java 버전에서도 안정적으로 사용할 수 있습니다.

Lucy-Xss-Servlet-Filter는 웹 어플리케이션으로 들어오는 모든 요청 파라메터에 대해 기본적으로 XSS 방어 필터링을 수행합니다. 이 라이브러리를 사용하면 다음과 같은 이점을 얻을 수 있습니다:

- 설정 파일만으로 간편하게 XSS 방어 구성 가능
- 비즈니스 로직 변경 없이 XSS 방어 적용
- 개발자가 XSS 방어를 신경 쓸 필요가 없음
- 파라메터명 관리를 통한 보다 세밀한 필터링 규칙 적용 가능

## Compatibility Update for Java 17
이 버전은 Java 17 호환성을 위해 특별히 수정되었습니다. `java.persistence`에서 `java.jakarta`로의 이동과 관련된 문제를 해결하여, Java 17 이상에서도 라이브러리가 문제없이 작동하도록 했습니다.

## Release Information

```XML
<dependency>
	<groupId>com.yourdomain</groupId>
	<artifactId>lucy-xss-servlet-java17</artifactId>
	<version>1.0.0</version>
</dependency>
```

## Getting Started
기본적인 설정은 원본 라이브러리와 동일합니다. `web.xml`과 `lucy-xss-servlet-filter-rule.xml`에 대한 설정 예제는 기존 문서를 참조하십시오.

**중요 변경 사항:** Java 17 환경에서 라이브러리를 사용할 경우, 관련된 호환성 문제를 해결하기 위해 추가적인 설정이 필요할 수 있습니다. 이러한 설정은 [Java 17 호환성 가이드](https://example.com/java-17-compatibility-guide)에서 확인할 수 있습니다.

## Contributing
Java 17과의 호환성 개선을 포함하여 Lucy-XSS에 기여하고 싶으신 분은 환영합니다! 기여 방법에 대한 지침은 [여기](https://github.com/yourfork/lucy-xss-servlet-filter-java17/contributing)에서 확인하실 수 있습니다.

## Licensing
이 프로젝트는 Apache License, Version 2.0에 따라 라이선스가 부여됩니다. 전체 라이선스 텍스트는 LICENSE 파일에서 확인할 수 있습니다.

---