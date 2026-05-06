# 딥러닝심화 (2025-2) 과제 모음

금오공과대학교 컴퓨터공학부 인공지능공학과 20231049 정우제

2025년 2학기 딥러닝심화 강의의 1~8주차 과제 보고서 및 실험 결과를 정리한 저장소.

## 과제 목록

| # | 과제명 | 주요 내용 | 마감일 | 배점 |
|---|--------|-----------|--------|------|
| HW01 | 과제1. RNN 실습 | LSTM 직접 구현 vs `nn.LSTM` 성능 비교, 한글 char/unit 데이터셋 | 2025.09.14 | 20 |
| HW02 | 과제2. RNN 응용 - 혐오표현 분류 | 모델 아키텍처 탐색 → 개선 → 하이퍼파라미터 튜닝 (3실험) | 2025.09.21 | 20 |
| HW03 | 과제3. Transformer 실습 | Transformer 구현 방식별 성능 비교 + Cross-Attention/ViT 시각화 | 2025.10.12 | 20 |
| HW04 | 과제4. GPT 기반 커스텀 챗봇 만들기 | GPT-2 파인튜닝(학습 노트북) + Gradio 인터페이스(추론 노트북) | 2025.10.29 | 20 |
| HW05 | 과제5. CycleGAN 실습 및 개선 | Transform·하이퍼파라미터·G/D 구조·Normalization·Albumentations·논문 기법 등 6개 실험 | 2025.11.16 | 20 |
| HW06 | 과제6. DDPM 실습 | DDPM 구현, 학습량 변화·EMA 적용 등 3개 실험 (CIFAR-10) | 2025.12.03 | 20 |
| HW07 | 과제7. 기말과제 제안서(발표) | Consistency Models 활용 반도체 웨이퍼 결함 패턴 생성 제안 | 2025.12.10 | 20 |
| HW08 | 과제8. 기말 과제 결과 보고서(발표) | DDPM·DDIM·CM 구현, FID 정량 평가, 클래스별 정성 비교 (WM-811K) | 2025.12.21 | 60 |

## 폴더 구조

```
deep-learning-advanced/
├── HW01/  # LSTM 한글 데이터 처리
├── HW02/  # 혐오표현 분류 (data/ 제외)
├── HW03/  # Transformer + 어텐션 시각화
├── HW04/  # GPT-2 챗봇 (학습 + Gradio)
├── HW05/  # CycleGAN 실험 결과 (ukiyoe2photo 데이터셋 제외)
├── HW06/  # DDPM (실험별 .pt, .gif, png 결과 포함)
├── HW07/  # 기말 제안서
└── HW08/  # 기말 결과 - Consistency Models
```

## 데이터셋 관련 안내

용량 문제로 일부 데이터셋은 저장소에서 제외함.

- **HW02**: `data/*.parquet` 제외
- **HW05**: `ukiyoe2photo` 데이터셋 제외 (Kaggle에서 별도 다운로드 필요)
- **HW08**: WM-811K wafer map 데이터셋은 노트북 내 `kagglehub.dataset_download("qingyi/wm811k-wafer-map")`로 자동 다운로드

## 노트북 출력 관련 안내

- **HW06** 노트북은 원본이 347MB로 GitHub 단일 파일 제한(100MB)을 초과해, 코드/마크다운은 그대로 두고 출력만 제거. 시각화 결과는 `HW06/experiment_1`, `experiment_2`, `experiment_3`, `HW06_experiment_result/` 폴더에 별도 저장됨.
- 그 외 과제 노트북은 출력 포함 상태로 보존.

## 실행 환경

- Python 3.x
- PyTorch
- Jupyter Notebook
- 사용 라이브러리는 각 노트북 상단 import 셀 참고

## 학기 정보

2025년 2학기 (2025-2) — 딥러닝심화
