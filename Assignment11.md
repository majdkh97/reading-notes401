# Read11

## Spring MVC
The Spring Web model-view-controller (MVC) framework is designed around a DispatcherServlet that dispatches requests to handlers, with configurable handler mappings, view resolution, locale and theme resolution as well as support for uploading files. The default handler is based on the @Controller and @RequestMapping annotations, offering a wide range of flexible handling methods. With the introduction of Spring 3.0, the @Controller mechanism also allows you to create RESTful Web sites and applications, through the @PathVariable annotation and other features.

- In Spring Web MVC you can use any object as a command or form-backing object;
- you do not need to implement a framework-specific interface or base class.
- Spring's data binding is highly flexible: for example, it treats type mismatches as validation errors that can be evaluated by the application, not as system errors.
- Thus you need not duplicate your business objects' properties as simple, untyped strings in your form objects simply to handle invalid submissions, or to convert the Strings properly.
- Instead, it is often preferable to bind directly to your business objects.

## Thymeleaf
Thymeleaf is a modern server-side Java template engine for both web and standalone environments.
Thymeleaf's main goal is to bring elegant natural templates to your development workflow — HTML that can be correctly displayed in browsers and also work as static prototypes, allowing for stronger collaboration in development teams.

- In a typical Spring MVC application, @Controller classes are responsible for preparing a model map with data and selecting a view to be rendered.
- This model map allows for the complete abstraction of the view technology and, in the case of Thymeleaf,
- it is transformed into a Thymeleaf context object (part of the Thymeleaf template execution context) that makes all the defined variables available to expressions executed in templates.