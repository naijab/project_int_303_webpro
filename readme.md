# MoomMim Shopping Online Store

INT303 Web Programming Project

## Tool
- Java Servlet --> controller
- JSP + JSP Custom Tag + JSTL + EL --> view
- Semantic UI --> css framework
- Apache Deltaspike Data Module --> repository
- Maven --> project manager

## Note
- Use `./mvnw` instead if not have `mvn` installed.

## Structure
```bash
├── pom.xml
├── readme.md
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── moommim
│   │   │           └── moommim_web
│   │   │               ├── config
│   │   │               │   ├── App.java
│   │   │               │   ├── CommonConstant.java
│   │   │               │   ├── Key.java
│   │   │               │   ├── ProductStatusConstant.java
│   │   │               │   ├── ServletPath.java
│   │   │               │   └── ViewPath.java
│   │   │               ├── controller
│   │   │               │   ├── base
│   │   │               │   │   └── BaseController.java
│   │   │               │   ├── CartServlet.java
│   │   │               │   ├── CheckoutServlet.java
│   │   │               │   ├── HistoryServlet.java
│   │   │               │   ├── HomeServlet.java
│   │   │               │   ├── LoginServlet.java
│   │   │               │   ├── LogoutServlet.java
│   │   │               │   ├── ProductCategoryServlet.java
│   │   │               │   ├── ProductServlet.java
│   │   │               │   ├── RegisterServlet.java
│   │   │               │   └── SearchServlet.java
│   │   │               ├── manager
│   │   │               │   └── EntityManagerProducer.java
│   │   │               ├── model
│   │   │               │   ├── Bill.java
│   │   │               │   ├── CartItem.java
│   │   │               │   ├── MailMessage.java
│   │   │               │   ├── ProductCategory.java
│   │   │               │   ├── ProductStock.java
│   │   │               │   └── UserAccount.java
│   │   │               ├── repository
│   │   │               │   ├── BillRepository.java
│   │   │               │   ├── MailRepository.java
│   │   │               │   ├── ProductCategoryRepository.java
│   │   │               │   ├── ProductStockRepository.java
│   │   │               │   └── UserRepository.java
│   │   │               ├── service
│   │   │               │   ├── AuthenticationServiceImpl.java
│   │   │               │   ├── base
│   │   │               │   │   ├── AuthenticationService.java
│   │   │               │   │   ├── BillService.java
│   │   │               │   │   ├── CartService.java
│   │   │               │   │   ├── MailService.java
│   │   │               │   │   ├── ProductCategoryService.java
│   │   │               │   │   ├── ProductService.java
│   │   │               │   │   └── UserService.java
│   │   │               │   ├── BillServiceImpl.java
│   │   │               │   ├── CartServiceImpl.java
│   │   │               │   ├── MailServiceImpl.java
│   │   │               │   ├── ProductCategoryServiceImpl.java
│   │   │               │   ├── ProductServiceImpl.java
│   │   │               │   └── UserServiceImpl.java
│   │   │               └── util
│   │   │                   ├── CacheHelper.java
│   │   │                   ├── filter
│   │   │                   │   └── DefaultWebFilter.java
│   │   │                   └── Util.java
│   │   ├── resources
│   │   │   └── META-INF
│   │   │       ├── apache-deltaspike.properties
│   │   │       ├── beans.xml
│   │   │       └── persistence.xml
│   │   └── webapp
│   │       ├── assets
│   │       │   ├── css
│   │       │   │   ├── core
│   │       │   │   │   ├── variables.css
│   │       │   │   │   └── variables.css.map
│   │       │   │   ├── module
│   │       │   │   │   ├── menu.css
│   │       │   │   │   └── menu.css.map
│   │       │   │   ├── styles.css
│   │       │   │   └── styles.css.map
│   │       │   ├── icon
│   │       │   │   ├── favicon.ico
│   │       │   │   ├── manifest.json
│   │       │   ├── images
│   │       │   │   └── logo.png
│   │       │   ├── js
│   │       │   │   └── app.js
│   │       │   └── less
│   │       │       ├── core
│   │       │       │   └── variables.less
│   │       │       ├── module
│   │       │       │   ├── global.less
│   │       │       │   └── menu.less
│   │       │       └── styles.less
│   │       ├── pages
│   │       │   ├── bill
│   │       │   │   └── show_history.jsp
│   │       │   ├── cart
│   │       │   │   └── show_cart.jsp
│   │       │   ├── checkout
│   │       │   │   ├── show_checkout_complete.jsp
│   │       │   │   └── show_checkout.jsp
│   │       │   ├── home
│   │       │   │   └── index.jsp
│   │       │   ├── login
│   │       │   │   └── login.jsp
│   │       │   ├── product
│   │       │   │   ├── show_by_category.jsp
│   │       │   │   └── show_by_product_id.jsp
│   │       │   ├── register
│   │       │   │   └── register.jsp
│   │       │   └── search
│   │       │       └── search.jsp
│   │       └── WEB-INF
│   │           ├── glassfish-resources.xml
│   │           ├── tags
│   │           │   └── master-layout.tag
│   │           └── web.xml
```
