# Spring Boot + VueJS Template

This is a template for anyone looking to use Spring Boot + Vue.JS in the same project. 

## Development

- Run the Spring Boot application which will run on port 8080
- Run the Vue application (/src/frontend)  which will run on port 3000
- All calls to `/api/**` are proxied to 8080 thanks to `vue.config.js`

## Packaging 

When you run `mvn clean package` the frontend Vue application will build in the `dist` directory. 
The Maven plugin `maven-resources-plugin` will copy the contents of the build directory into `/target/static/classes`

## Deployment

The `system.properties` is a file I used for Heroku to set the Java version and deploy the application. 

https://spring-boot-vue-template.herokuapp.com/



