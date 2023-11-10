# 고려대학교 디지털 인문학 입문 06분반

06 분반 프로젝트 데이터 업로드 저장소입니다.

# 동아시아 신비한 동물 사전(Fantastic Beasts in East Asia)

고려대학교 문과대학 디지털인문학입문II 06분반 프로젝트 데이터 업로드 저장소입니다.

## 개요

- 본 프로젝트는 고려대학교 문과대학 디지털인문학입문II 06분반 수업의 일환으로 진행됩니다.
- 디지털 인문학의 도구 사용법을 학습하고 해당 분야에 대한 이해를 심화시키는 것이 목적입니다.
- 동아시아의 **환상의 동물들**을 역사 기록에서 발굴하고 생성 AI를 통해 시각적으로 구현해 보고자 합니다.
- 이 프로젝트는 동아시아의 환상의 동물들 안에 숨어 있는 동아시아인들의 자연에 대한 인식과 상상력을 살펴보고자 하는 것이 목적입니다.
- 가을 학기 동안 우리가 수집할 환상의 동물들이 주로 나타날 것으로 예상되는 목록은 아래와 같습니다.
  - 산해경(山海經)
  - 용재총화(慵齋叢話)
  - 용재총화(慵齋叢話)
- 환상의 동물에 대한 기록들은 대단히 파편적이기 때문에 과거 역사 기록 보다는 현대에 정리한 인터넷 자료를 참고하는 것이 좋을 것 같습니다. 참고할 만한 웹사이트 및 웹페이지는 다음과 같습니다. 저작권에 관한 문제가 발생할 경우, 아래 [저작권](#저작권) 섹션을 참조하여 주세요.

  - [산해경 원문](https://zh.wikisource.org/wiki/%E5%B1%B1%E6%B5%B7%E7%B6%93)
  - 곽재식 작가의 [괴물 백과 사전 전체 목록](https://oldstory.postype.com/post/1477014)
  - 윤규의 [한국요괴도감](https://blog.naver.com/gkrbdbsgk2)
  - 월도마왕의 [한국, 동서방 전설 링크 일람](https://blog.naver.com/ichigeki1028/220931551383)

## 프로젝트 기여 방법

기여를 원하시는 모든 분들은 프로젝트 데이터에 기여할 수 있으며, 가을학기 종강 후에 기여를 시작해 주시면 감사하겠습니다.

이 프로젝트는 학생들의 Git/Github 사용 능력 향상을 목적으로 하기 때문에, 아래의 방법으로 기여해 주세요:

- Git 또는 Github에 익숙하지 않은 경우, [이 가이드](https://git-scm.com/book/ko/v2)를 참고하여 기본적인 사용법을 익히실 수 있습니다.
- Github에서 기여하실 때는 Pull Request를 통해 기여하실 수 있으며, [Pull Request 가이드](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests)를 참조하세요.

### 데이터 기여 방법

1. `template.json` 파일을 다운로드하고, 각 필드에 대한 설명을 충분히 읽어주세요. 파일의 예시는 아래와 같습니다.

   ```json
   {
     "student_id": "학번, 이름, 닉네임 (일관되게 사용해 주세요)",
     "name": "환상의 동물 이름. 인간을 기반으로 한 요괴들은 지양해 주세요.",
     "image": "images/your_image_name.png (이미지 파일은 images 폴더에 저장해 주세요. jpg 형식도 가능합니다.)",
     "image_prompt": "AI 이미지 생성에 사용한 프롬프트",
     "animals": ["영감동물1", "영감동물2", "영감동물3"],
     "original": "원문을 여기에 입력합니다.",
     "translated": "기록 번역본을 여기에 입력합니다.",
     "source": "원문의 출처를 여기에 입력합니다.",
     "comment": "이 환상의 동물에 대한 개인적인 생각이나 타인에게 알리고 싶은 정보를 여기에 입력합니다."
   }
   ```

#### 데이터 기여 방법 상세 안내

- **학번 (`student_id`)**: 문자열로만 구성해주세요. 파일 업로드 시 이를 파일명으로 활용합니다. 이미 존재하는 ID가 있을 경우 연번을 부여합니다.
- **환상의 동물명 (`name`)**: 개인 이름이 아닌 동물의 이름을 기입해야 합니다.
- **이미지 (`image`)**: 생성형 AI로 제작한 동물 이미지를 `images` 폴더에 업로드하고, 파일명은 `images/`로 시작해야 합니다.
- **프롬프트 (`image_prompt`)**: AI 생성 이미지에 사용한 프롬프트를 기재합니다. 완벽한 재현은 불가능하지만 유사한 결과를 얻는 데 도움이 됩니다.
- **영감동물 (`animals`)**: 리스트로 작성해야 하며, 되도록 사람이 아닌 존재들로 작업해 주세요.
- **원문 (`original`)**: 기록 원문을 여기에 기입합니다. 이는 데이터 수정 및 검증 시 사용됩니다.
- **번역 (`translated`)**: 한문이나 옛 한글인 경우, 번역문을 기재합니다. 이 프로젝트는 주로 영감동물 사용을 확인하는 것을 목적으로 하므로 완벽한 번역은 필요하지 않습니다.
- **출처 (`source`)**: 출처가 되는 책 이름을 기재합니다. 한글로만 적되, 한자 병기는 허용하지 않습니다.
- **메모 (`comment`)**: 기타 참고할 만한 특이사항을 기재합니다.

#### 기여 절차

1. `template.json`을 `data` 폴더에 복사하고 원하는 이름으로 변경합니다.
2. `images` 폴더에 AI로 생성된 이미지를 업로드합니다. 파일명은 중복을 피해주세요.
3. Commit을 하고 자유롭게 메시지를 작성합니다.
4. Pull Request(PR)를 생성하고, 제목은 "학번 - 환상의동물명"으로 합니다.
5. PR 승인을 기다립니다. 자동 스크립트로 형식을 검증합니다. 거절 시, 메시지를 확인하고 수정 후 재시도합니다.

## 데이터 시각화

결과물은 실시간으로 확인 가능합니다:

**[데이터 시각화 사이트 바로 가기](https://fantastic-beasts.cola172.store)**

### 주의사항:

- **서버 유지 관리로 인한 중단**: 프로젝트 초기 단계인 현재에는 서버 유지 관리를 위해 종종 서비스 접근이 불가능할 수 있습니다.

- **저장소 비공개**: 시각화 사이트의 코드 저장소는 공개되지 않습니다.

## 향후 계획

- 의미 있는 데이터셋이 구축될 때까지 데이터 작업을 계속할 예정입니다.
- 최종 목표는 네트워크 및 통계 분석을 통해 학술 저작물로 출간하는 것입니다.

## 저작권 안내

### 소유권

- 본 프로젝트의 소유자는 KAIST 문화기술대학원 최동혁입니다.
- 소유자는 이 프로젝트에 대한 모든 법적 책임을 지며, 권리를 보유합니다.

### 사용 조건

- 본 프로젝트는 **교육 및 학술 목적**으로만 사용할 수 있습니다.
- 상업적 이용은 엄격히 금지되어 있습니다.
- 교육 및 학술 목적으로 활용하시려는 경우, 소유자와 저장소 링크를 반드시 첨부해야 합니다.

### 데이터 기여

- 수업의 수강생은 최소 10개, 최대 13개의 데이터 작업을 해야 합니다.
- 추가 기여를 원할 경우, 소유자에게 논의하세요.
- 기여도에 대한 문의는 소유자 이메일([dhchoi.lazy@gmail.com](mailto:dhchoi.lazy@gmail.com))로 연락 바랍니다.
- 기여도가 인정될 경우, 학술 논문에 차등 인용 예정입니다.
