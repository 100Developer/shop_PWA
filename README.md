# shop_PWA

## PWA MP 2021 10 12

### ✅ 새롭고 강력한 소프트웨어 앱을 만드는 방식

HTML, CSS, JavaScript를 이용해서 만든 웹앱을 모던한 웹브라우저 APIs와 결합해서 크로스플랫폼에서 동작하는 어플리케이션을 손쉽게 만드는 것

이미 만든 웹사이트나 웹어플리케이션에 몇가지만 추가하면 손쉽게 데스크탑에서 동작하는 모바일에서 동작하는 어플리케이션을 만들 수 있다.

네이티브앱은 플랫폼에서 지원하는 다양한 API를 사용하여 다양한 기능을 사용하지만, 플랫폼에서만 사용할 수 있다는 단점이 있다.
반대로 브라우저에서 동작하는 웹앱은 플랫폼에 상관없이 브라우저만 있으면 사용가능하므로 사람들이 쉽게 접근해서 사용할 수 있는 장점이 있지만 네이티브앱처럼 플랫폼 자체의 API를 사용할 수 없다는 단점이 있다.

그래서 PWA는 접근성이 높은 웹앱의 장점과 플랫폼 API를 사용할 수 있는 네이티브 앱의 장점이 결합되어진 형태임

웹어플리케이션 > 아이폰이 나오면서 등장하게됨

---

#### alex russell + frances berriman > PWA (2015)

- responsive web design
- service workers
- app manifest
- push notification
- native app-like capabilities

---

#### PWA를 위한 4가지 조건

1. 웹앱 또는 웹페이지

2. HTTPs

3. application manifest

4. service worker

---

#### HEAD 상단 추가 코딩

```html
<link rel="manifest" href="manifest.json" />
```

#### HEAD 하단 추가 코딩

```html
<script type="module">
  import 'https://cdn.jsdelivr.net/npm/@pwabuilder/pwaupdate';
  const el = document.createElement('pwa-update');
  document.body.appendChild(el);
</script>
```
