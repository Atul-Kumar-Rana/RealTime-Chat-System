# Use Java 17
FROM eclipse-temurin:17-jdk

# Set working directory
WORKDIR /app

# Copy project files
COPY . .

# Build the Spring Boot JAR
RUN ./mvnw clean package -DskipTests

# Expose port (Spring Boot default)
EXPOSE 8080

# Run the JAR — automatically picks the created jar file
CMD ["sh", "-c", "java -jar target/*.jar"]
