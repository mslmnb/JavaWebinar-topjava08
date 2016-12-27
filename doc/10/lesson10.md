# Онлайн проекта <a href="https://github.com/JavaWebinar/topjava08">Topjava</a>

### <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFfk43cG91Yk9pM3JxUHVhNFVVdHlxSlJtZm5oY3A4YXRtNk1KWEZxRlFNeW8">Материалы занятия (скачать все патчи можно через Download папки patch)</a>


## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Разбор домашнего задания HW9

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 1. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFZnQ2dDZsT0dvYjQ">HW9</a>
#### Apply 1_HW9_binding_ajax.patch

> - JavaScript `i18n[]` локализацию перенес в `footer.jsp`
> - Other validation solution: <a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/html/mvc.html#mvc-ann-initbinder">customizing data binding with @InitBinder</a>
  
#### Apply 2_HW9_test.patch
#### Apply 3_HW9_datetimepicker.patch

> Изменил формат ввода dateTime в форме без 'T': при биндинге значений к полям формы в `datatablesUtil.updateRow` для поля `dateTime` делаю `replace('T', ' ')`. 

- <a href="http://xdsoft.net/jqplugins/datetimepicker/">DateTimePicker jQuery plugin</a>
- <a href="https://github.com/xdan/datetimepicker/issues/216">Datetimepicker and ISO-8601</a>

## Занятие 10:

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 2. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFTVZyQnBlYUtkNms">Spring Security Taglib. Method Security Expressions.</a>
#### Apply 04_secure_tag_annotation.patch
-  <a href="http://docs.spring.io/spring-security/site/docs/current/reference/htmlsingle/#declaring-the-taglib">Spring Security Taglib.</a>
-  <a href="http://docs.spring.io/spring-security/site/docs/current/reference/htmlsingle/#jc-method">Method Security</a> и <a href="http://docs.spring.io/spring-security/site/docs/current/reference/htmlsingle/#method-security-expressions">Method Security Expressions</a>. Зависимость от контекста mvc/parent.

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 3.  <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFc1JMTE4xVG0zN0U">Interceptors. Редактирование профиля. JSP tag files.</a>
#### Apply 05_interceptor.patch
-  Добавляем профиль. <a href="http://www.mkyong.com/spring-mvc/spring-mvc-handler-interceptors-example/">Spring interceptors</a>.
#### Apply 06_profile_jsptag.patch

> - ProfileRestController.update(user) изменился на userTo (нельзя, например, изменять себе роли).
> - Добавил локализацию

-  <a href="http://www.techrepublic.com/article/an-introduction-to-jsp-20s-tag-files/">Делаем jsp tag для ввода поля формы</a>.
-  <a href="http://www.codejava.net/frameworks/spring/spring-mvc-form-validation-example-with-bean-validation-api">Spring MVC Form Validation</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 4. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNWpUNktMeGJURmM">Форма регистрации.</a>
#### Apply 07_registration.patch

> Добавил локализацию

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 5. <a href="https://drive.google.com/file/d/0B9Ye2auQ_NsFZ19lU29VVDRfNXM">Обработка исключений в Spring.</a>
                                                                                                                                
#### Apply 08_not_found_404.patch
-  <a href="http://spring.io/blog/2013/11/01/exception-handling-in-spring-mvc#using-http-status-codes">Используем HTTP status code</a>
-  <a href="http://stackoverflow.com/questions/2195639/restful-resource-not-found-404-or-204-jersey-returns-204-on-null-being-returne">RESTful resource not found</a>
-  <a href="http://stackoverflow.com/questions/9930695/rest-api-404-bad-uri-or-missing-resource">REST API 404</a>
#### Apply 9_global_exception.patch
-  <a href="http://spring.io/blog/2013/11/01/exception-handling-in-spring-mvc#global-exception-handling">Global Exception Handling</a>
#### Apply 10_controller_based_exception.patch
- <a href="http://spring.io/blog/2013/11/01/exception-handling-in-spring-mvc#errors-and-rest">Сериализация Exception в JSON</a>
- <a href="http://spring.io/blog/2013/11/01/exception-handling-in-spring-mvc#controller-based-exception-handling">Exception Handling на уровне контроллера</a>
- <a href="https://www.javacodegeeks.com/2013/11/controlleradvice-improvements-in-spring-4.html">@ControllerAdvice improvements in Spring 4</a>
- <a href="https://dzone.com/articles/spring-31-valid-requestbody">@Valid @RequestBody + Error handling</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 6. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFUHNiYzNMbkF6ajQ">Encoding password</a>
#### Apply 11_password_encoding.patch

> Перенес вызовы `UserUtil.prepareToSave` из `AbstractUserController` в `UserServiceImpl`.

- <a href="http://docs.spring.io/spring-security/site/docs/current/reference/htmlsingle/#core-services-password-encoding">Password Encoding</a>

### ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 7. <a href="https://drive.google.com/open?id=0B9Ye2auQ_NsFNDlPZGdUNThzNUU">Межсайтовая подделка запроса (CSRF).</a>
#### Apply 12_csrf.patch
-  <a class="anchor" id="csrf"></a><a href="https://ru.wikipedia.org/wiki/Межсайтовая_подделка_запроса">Межсайтовая подделка запроса (CSRF)</a>
-  <a href="http://docs.spring.io/spring-security/site/docs/current/reference/html/csrf.html#csrf-using/">Using Spring Security CSRF Protection</a>
-  <a href="http://docs.spring.io/spring-security/site/docs/current/reference/html/csrf.html#csrf-include-csrf-token-ajax">Ajax and JSON Requests</a>
-  <a href="http://blog.jdriven.com/2014/10/stateless-spring-security-part-1-stateless-csrf-protection/">Stateless CSRF protection</a>
-  Ресурсы:
    -  <a href="http://habrahabr.ru/post/264641/">Spring Security 4 + CSRF</a>
    -  <a href="http://stackoverflow.com/questions/11008469/are-json-web-services-vulnerable-to-csrf-attacks">Are JSON web services vulnerable to CSRF attacks</a>
    -  <a href="https://ru.wikipedia.org/wiki/Правило_ограничения_домена">Правило ограничения домена (SOP)</a>
    -  <a href="https://ru.wikipedia.org/wiki/Cross-origin_resource_sharing">Cross-origin resource sharing (CORS)</a>

## ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Домашнее задание HW10
- Сделать валидацию в AdminAjaxController/MealAjaxController через `ExceptionInfoHandler` (вернуть клиенту `ErrorInfo` и статус `HttpStatus.BAD_REQUEST`. Тип методов контроллеров можно вернуть обратно на `void`).
- Сделать валидацию принимаемых json объектов в REST контроллерах через `ExceptionInfoHandler`
  - <a href="https://dzone.com/articles/spring-31-valid-requestbody">@Valid @RequestBody + Error handling</a>
- Сделать обработку ошибки при дублирования email ("User with this email already present in application") для: 
  - регистрации / редактирования профиля пользователя
  - добавления / редактирования пользователя в списке
    
#### Optional

- Починить UTF-8 в редактировании профиля и регистрации (если windows). Подумайте, почему они поломались.
- Сделать в приложении выбор локали (см. http://topjava.herokuapp.com/)
  -  <a href="http://www.mkyong.com/spring-mvc/spring-mvc-internationalization-example">Spring MVC internationalization sample</a>
  -  <a href="http://www.concretepage.com/spring-4/spring-4-mvc-internationalization-i18n-and-localization-l10n-annotation-example">Spring 4 MVC Internationalization</a>
  
## ![question](https://cloud.githubusercontent.com/assets/13649199/13672858/9cd58692-e6e7-11e5-905d-c295d2a456f1.png) Ваши вопросы

> В чем отличие между аннотоацией `@PreAuthorize("hasRole('ROLE_ADMIN')")` и конфигурацией в jsp: `<sec:authorize access="isAuthenticated()">`, `<sec:authorize access="hasRole('ROLE_ADMIN')">` ?

Анотация `@PreAuthorize` обрабатывается Spring анологично `@Transactional`, `@Cacheable` - класс проксируется и до-после вызова метода добавляется функциональность.
В данном случае перед вызовом метода проверяются роль залогиненного юзера. JSTL тэг `authorize` выполняет проверку условия в залогиненном юзере внутри jsp.

> Какой из `SessionLocaleResolver` и `CookieLocaleResolver` а какой лучше использовать для локализации?

Я взял `CookieLocaleResolver`. Он хранит информацию в куках, которые хранятся долго у клиента на компьютере. Локаль в сессии проподает вместе с логаутом.
