# config-server
Spring Cloud Configuration Server là một ứng dụng tập trung quản lý tất cả các cấu hình liên quan tới ứng dụng. 

Đầu tiên sẽ tạo project hoặc có sẵn rồi thì chỉ thêm thư viện là Config Server:

<dependency>
   <groupId>org.springframework.cloud</groupId>
   <artifactId>spring-cloud-config-server</artifactId>
</dependency>

Ở hàm Main thì thêm @EnableConfigServer
Ở file application.properties ta cấu hình port và uri...
Ex:
server.port=8888

spring.cloud.config.server.git.uri=https://github.com/o7planning/spring-cloud-config-git-repo-example.git

# For File System:
# spring.profiles.active=native
# spring.cloud.config.server.native.searchLocations=C:/Users/tran/Desktop/config
