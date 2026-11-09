# AAM 데일리 트렌드 브리핑

매일 아침 Claude 예약 작업이 AI·마케팅 트렌드를 검색해 `data/YYYY-MM-DD.json`을 만들고
`data/index.json`의 `dates` 맨 앞(최신순)에 날짜를 추가한 뒤 push 합니다. Vercel이 자동 배포합니다.

## 브리핑 JSON 형식
```json
{
  "date": "2026-11-10",
  "updated": "07:30 KST",
  "headline": "오늘 한 줄 요약",
  "sections": [
    {"title": "AI 뉴스", "items": [{"title": "", "summary": "", "source": "", "url": ""}]},
    {"title": "신규 툴·모델", "items": []},
    {"title": "오늘의 경제 한 줄", "items": []},
    {"title": "소상공인·마케팅 활용 포인트", "items": [{"title": "", "summary": "", "tip": "소상공인에게 이렇게 써먹기"}]}
  ]
}
```
