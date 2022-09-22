FROM tomcat:8.5.72-jdk8
WORKDIR /usr/local/tomcat/webapps
# 워킹 디렉터리가 잘 바꼈는지 확인하기 위해 명령어 수행
RUN pwd
# 작업 디렉터리에 ROOT 디렉터리를 생성하는 명령
RUN mkdir ./ROOT
ADD index.jsp ./ROOT
ENV TZ=Asia/Seoul
EXPOSE 8080
CMD [ "catalina.sh", "run" ]