#### Why Kotlin
- 안드로이드 공식 언어 (2017. 5. 18 ~)
- Android Studio 3.0 부터 기본 지원
- Statically typed programming language for modern multiplatform application
	- 간결한 문법, 예외 처리(Safe), Interoperable(Java와의 상호 호환), Tool-friendly
	- Build Application For JVM. Android, Browser(JS), Native

```kotlin
var output: String
output = null				// Compilation error
```
Kotlin protects you from mistakely operating on nullable types.
```kotlin
val name = String? = null	// Nullable type
println(name.length())		// Compilation error // null pointer exception 발생 가능.
```
If you check a type is right, the compiler will auto-cast it for you
```kotlin
fun calculateTotal(obj : Any) {
	if (obj is Invoice)		// auto-cast. Invoice는 obj로 자동 형변환된다.
    	obj.calculateTotal()
}
```

#### Install
- [Kotlin 공식홈페이지](https://kotlinlang.org/) 의 Learn 탭에서 예제 코드 및 라이브 실행 가능.
- 