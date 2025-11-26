FROM eclipse-temurin:17-jdk
WORKDIR /app
COPY . .
# make mvnw executable and build
RUN chmod +x mvnw && ./mvnw clean package -DskipTests
EXPOSE 8080
CMD ["sh", "-c", "java -jar target/*.jar"]
