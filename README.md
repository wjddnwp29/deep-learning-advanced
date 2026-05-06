# Deep Learning Advanced

딥러닝심화 강의 과제 모음.

## 과제 목록

| # | 주제 | 내용 |
|---|------|------|
| HW01 | RNN 실습 | LSTM 직접 구현 vs `nn.LSTM` 성능 비교 |
| HW02 | RNN 응용 - 혐오표현 분류 | 모델 아키텍처 탐색 → 개선 → 하이퍼파라미터 튜닝 |
| HW03 | Transformer 실습 | Transformer 구현 + Cross-Attention / ViT 시각화 |
| HW04 | GPT 기반 커스텀 챗봇 | GPT-2 파인튜닝 + Gradio 인터페이스 |
| HW05 | CycleGAN 실습 및 개선 | Transform·하이퍼파라미터·구조·Normalization·Albumentations 등 6개 실험 |
| HW06 | DDPM 실습 | DDPM 구현, 학습량·EMA 실험 (CIFAR-10) |
| HW07 | 기말과제 제안서 | Consistency Models 활용 반도체 웨이퍼 결함 패턴 생성 (제안) |
| HW08 | 기말 과제 | DDPM·DDIM·CM 구현, FID 평가, 클래스별 비교 (WM-811K) |

## 데이터셋

용량 문제로 일부 데이터셋은 제외됨.

- HW02: `data/*.parquet`
- HW05: `ukiyoe2photo` (Kaggle에서 별도 다운로드)
- HW08: WM-811K — 노트북에서 `kagglehub`로 자동 다운로드

## 노트북 출력

HW06은 원본이 GitHub 단일 파일 제한(100MB)을 초과해 출력만 제거함. 시각화 결과는 `HW06/experiment_*` 폴더에 별도 보존.
