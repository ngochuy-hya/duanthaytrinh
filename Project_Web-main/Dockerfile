# Sử dụng Tomcat chính thức + JDK 21
FROM tomcat:9.0.104-jdk21

# Xoá ứng dụng mặc định của Tomcat (tùy chọn)
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy WAR file vào thư mục webapps của Tomcat
COPY target/FurnitureShop_11_11_14h-1.0.war /usr/local/tomcat/webapps/ROOT.war

# Mở port 8080 cho Tomcat
EXPOSE 8080

# Không cần ENTRYPOINT vì Tomcat tự start khi container chạy
