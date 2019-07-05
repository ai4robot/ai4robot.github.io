1. 데이터 추가방법

데이터를 추가하려면 yml파일을 수정하거나, md파일에서 yml 문법을 사용합니다. 요소를 추가할 때 들여쓰기가 중요합니다.

이미지는 "/assets/~ "에 적당한 폴더에 넣고, yml의 링크도 동일하게 "/assets/~.jpg" 형식으로 하시면 됩니다.


- codes, datasets
    _data/codes.yml
    _data/datasets.yml 을 통해서 데이터 관리가 가능합니다.
    
    main 자식의 변수
    
    title : 제목
    body : 내용
    image : 관련 이미지
    link : 관련 링크
    
    여러 link를 가질 수 있어 link는 리스트 형식으로 작성했습니다.
    link:
        - name: "repository"
          url: "exam.ple"
        - name: "repository2"
          url: "exam2.ple"
        
    위 형식처럼 여러요소를 넣을 수 있습니다.


- publications
    publications는 _data/publications.yml을 통해서 데이터 관리가 가능합니다.


    main변수 내에 title(국제/국내학회), journal이 있습니다.
    현재는 국제학회/국내학회로 나누었고 journal에는 각 논문들을 리스트형식으로 만들었습니다.
    
    journal의 변수 
    title : 논문이름
    author : 저자
    academy : 학회 이름
    image : 관련 이미지
    link : 관련 링크

    형식으로 되어있고, 여러 링크가 필요할 수 있어, 리스트형식으로 작성했습니다.

    link:
        - name: "repository"
          url: "exam.ple"
        - name: "repository2"
          url: "exam2.ple"
    
    위와 같은 형식으로 사용할 수 있습니다.

- people
    people은 _data/people.yml을 통해서 데이터 관리가 가능합니다.
    
    - main 변수 내에
    department : 그룹이름
    child : 연구진 리스트

    - child 내에
    name : 이름
    position : 직책
    image : 프로필 사진
    description : 자기소개
    link : 관련 링크

    형식으로 되어있고, 여러 링크가 필요할 수 있어, 리스트형식으로 작성했습니다.

    link:
        - name: "repository"
          url: "exam.ple"
        - name: "repository2"
          url: "exam2.ple"
    
    위와 같은 형식으로 사용할 수 있습니다.


- blog
 블로그의 각 게시글은 _posts/ 경로에 저장할 수 있습니다.
 저장형식은 yyyy-mm-dd-제목.md로 작성하시면 되고,
 상단에 yml형식으로 추가하셔야합니다.
 * 추가적으로 제목/카테고리로 url이 형식됨으로 겹치는 제목과 카테고리를 생성하면 접근이 어렵습니다.


 ---
 title: "Post: Link"        # * 제목 (필수)

 categories:                # * 카테고리 (필수)
   - Post Formats

 header:                    # 게시글 상단에 이미지 혹은 비디오를 삽입가능
  image: /assets/~.jpg      # 이미지를 넣을 시 경로
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"  # 이미지를 넣을 시 캡션
  video:                   # 비디오를 넣을 시
   id: value               # 비디오 값
   provider: youtube       # 프로바이저 입력

 tags:                     # 게시글 하단에 태
   - link
   - Post Formats

 toc: true                 # 우측의 네비게이션 바를 넣을 시
 toc_label: "Getting Started"

  link: https://github.com   # 게시글의 링크를 넣을 시 

  excerpt: "exam"           # 부제, 미작성시 본문내용이 들어감

  last_modified_at: 2018-01-03T09:45:06-05:00  # 수정일자

  sidebar:                         # 좌측 사이드바 (기본형)
   title: "Sample Title"
   nav: sidebar-sample

   sidebar:                        # 좌측 사이드바 커스텀
  - title: "Title"
    image: http://placehold.it/350x250
    image_alt: "image"
    text: "Some text here."
  - title: "Another Title"
    text: "More text here."
    nav: sidebar-sample
 ---

위와 같이 --- --- 중간부분에 yml에 필요한 데이터들을 작성 후 하단에 .md양식으로 게시글을 포스팅하시면 됩니다.


2. 레이아웃 수정하기

blog > _layout/posts.html
blog 게시글 > _layout/single.html
codes > _layout/codes.html
datasets > _layout/datasets.html
profile > _layout/profile.html
소개, index > _layout/splash.html



를 변경하시면 됩니다.
해당 레이아웃이 문서의 전부가 아니라 html안의 상속이나 include 부분이 있습니다.

3. 페이지 추가하기
3.1 _data/navigation.yml에 title과 url 추가
3.2 _pages/에 .md파일 생성
3.3 상단에 
---

--- 를 추가 후(yml 형식) permalink, layout, title 항목 작성