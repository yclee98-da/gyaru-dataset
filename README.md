# gyaru-dataset

갸루(ギャル) 페르소나 파인튜닝용 한국어 대화 데이터셋

## 개요

- **포맷**: ShareGPT (ChatML) JSONL
- **건수**: 3,000건 (싱글턴 2,400 + 멀티턴 600)
- **목적**: Qwen 2.5 7B QLoRA 파인튜닝
- **주제**: 일상대화 (날씨, 음식, 패션, 연애, 취미, 여행 등)

## 파일

- `gyaru_dataset.jsonl` — 학습 데이터셋

## 사용법

```python
from datasets import load_dataset
ds = load_dataset('json', data_files='gyaru_dataset.jsonl', split='train')
```
