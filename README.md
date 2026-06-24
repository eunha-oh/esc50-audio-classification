# Environmental Sound Classification with CNN

ESC-50 데이터셋을 활용한 Mel Spectrogram 기반 환경음 분류 프로젝트입니다.

## Overview
소리 데이터를 Mel Spectrogram 이미지로 변환하여 CNN으로 50가지 환경음을 분류하는
end-to-end 파이프라인을 직접 구현했습니다.

- 데이터셋: ESC-50 (50개 클래스, 2,000개 오디오 파일)
- 핵심 아이디어: 오디오 → Mel Spectrogram → CNN (이미지 분류로 변환)

## Pipeline
Raw Audio → Mel Spectrogram 변환 → 정규화 → CNN 학습 → 분류

## Results
| 설정 | Test Accuracy |
|------|--------------|
| Baseline | 49.25% |
| + Data Augmentation | 61.12% |

## 사용 기술
- Python, PyTorch, librosa, scikit-learn
- Google Colab (GPU)

## 실행 방법
1. `notebooks/` 폴더의 노트북을 순서대로 실행
2. ESC-50 데이터셋 자동 다운로드 포함
