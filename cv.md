---
layout: page
title: Curriculum vitae
permalink: /cv/
---

{% if site.cv_pdf and site.cv_pdf != '' %}
[Download CV (PDF)]({{ site.cv_pdf | relative_url }})
{% else %}
My curriculum vitae will be added here.
{% endif %}

<!--
PDF 사용 방법:
1. assets/files/cv.pdf에 실제 CV 파일을 업로드합니다.
2. _config.yml에서 cv_pdf: "/assets/files/cv.pdf"로 변경합니다.
3. 저장하면 위 안내 문장이 PDF 다운로드 링크로 바뀝니다.

이 페이지에 직접 이력을 적어도 됩니다. 아래 예시를 복사하세요.

## Appointments

- **Year–present.** Position, institution.

## Education

- **Year.** Degree, institution. Advisor: Name.
-->
