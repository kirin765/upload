## 서블릿과 파일 업로드1
* multiparts로 전송시 구분선에 따라 다양한 parts가 넘어온다.
* request.getParts()

## 서블릿과 파일 업로드2
* 서블릿을 통한 part를 통해 헤드, 이름등을 가져올 수 있다.
* part.getSubmittedFileName(), part.getInputStream(), part.write(...)