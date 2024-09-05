# <API 설계>  : url과 method의 set
  0) 전체유튜버 조회 GET /youtubers
   - req : X
   - res : map 전체 조회

  1) (개별 조회하기) GET /youtubers/:id  - id로 map 에서 객체를 찾아, 그 객체의 정보를 뿌려줌
   - req : params.id <= map에 저장된 키 값을 전달
   - res : map에서 id로 객체를 조회해서 전달

  2) (유튜버 등록하기) POST /youtubers
   - req : body <= channelTitle, sub =0, videoNum  =0 (신규 유튜버 정보를 전달)
      db에 저장까지 해줌~~~~
   - res : "channelTitle님, 유튜버 생활을 응원합니다."
