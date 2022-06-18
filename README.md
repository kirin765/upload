## 서블릿과 파일 업로드1
* multiparts로 전송시 구분선에 따라 다양한 parts가 넘어온다.
* request.getParts()

## 서블릿과 파일 업로드2
* 서블릿을 통한 part를 통해 헤드, 이름등을 가져올 수 있다.
* part.getSubmittedFileName(), part.getInputStream(), part.write(...)

## 스프링과 파일 업로드
* 스프링에서 제공하는 MultipartFile으로 데이터 확인 가능
* file.getOriginalFilename(), file.transferTo()

## 예제로 구현하는 파일 업로드, 다운로드
* UrlResource를 통해 파일을 가져올 수 있다.
* List<UploadFile>와 같이 여러파일을 한번에 리스트로 받을 수 있다.
* CONTENT_DISPOSITION 헤더를 통해 파일 다운로드 가능