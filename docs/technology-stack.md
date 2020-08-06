## Back end
  * Windows 10 
  * Apache HTTP server configured as reverse proxy
  * JRE 8
  * Apache Tomcat Java application server
  * Web service application, incorporating:
      *Data model
          * Embedded Apache Derby database
          * Hibernate ORM
          * Custom entity classes
          * Spring Boot Data
          * Custom data repository interfaces
       * Service controllers
          * Spring MVC
          * Custom controller classes
       * View composition & serialization
          * Jackson JSON
          * Custom view classes & interfaces
       * Authentication
          * Spring Security
          * Google Sign In (external service; see https://developers.google.com/identity
          * Custom authentication verification class
## Front end

   * Emulator Pixel 2 API 28 
   * Data model
       * SQLite
       * Custom entity and other model classes
       * Custom type converters
       * Data access object (DAO) interfaces
    * Remote service interfaces
       * Retrofit
       * ReactiveX
       * Gson
       * Custom serializer/deserializers
   * View Model components
       * Android Lifecycle framework (ViewModel & LiveData)
       * Custom view model classes
   * View
       * Custom RecyclerView.Adapter and RecyclerView.Holder classes
       * Custom layouts
   * Controller
       * Custom activity and fragment classes
   * Authentication
       * Google Sign In (external service; see https://developers.google.com/identity
       * Custom sign in service class