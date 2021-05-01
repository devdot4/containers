FROM java
RUN echo "Using Java."
COPY . /app
RUN echo "Copying contents to /app"
WORKDIR /app
RUN echo "Work directory updated to /app"
RUN ./mvnw package
RUN echo "Running Maven package manager."
EXPOSE 8080
RUN echo "Port 8080 is exposed."
CMD ["java", "-jar", "target/spring-petclinic-2.4.5.jar"]
RUN echo "Running target/spring-petclinic-2.4.5.py"