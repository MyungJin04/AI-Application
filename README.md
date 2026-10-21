# 인공지능응용 (AI Application)

202312312 송명진

| 과제 | 파일 | 현재 검증 상태 |
| --- | --- | --- |
| 과제 1: Python 데이터 처리 | [과제1_202312312_송명진.ipynb](assignment1/과제1_202312312_송명진.ipynb) | 기본 1~5와 심화 6~7 모두 실행 및 자동채점 통과 |
| 과제 2: 데이터 정제 | [과제2_202312312_송명진.ipynb](assignment2/과제2_202312312_송명진.ipynb) | 6개 함수 구현 완료. 수업 스타터 `tinytrack.py` 확보 후 전체 실행 필요 |
| 과제 3: 미세조정 · ONNX 배포 · 폐루프 평가 | [과제3_202312312_송명진.ipynb](assignment3/과제3_202312312_송명진.ipynb)<br>[my_policy_v1.onnx](assignment3/my_policy_v1.onnx)<br>[compare_v1.csv](assignment3/compare_v1.csv)<br>[my_policy_v1_result.json](assignment3/my_policy_v1_result.json) | 문제 1~6 자동채점 통과 출력 및 저장된 오류 없음 확인. 심화 결과표·근거 3줄 확인. ONNX 평가 결과와 CSV·JSON 일치 검증 완료 |
| 7주차 리더보드 v2: DAgger | [my_policy_v2.onnx](week07/my_policy_v2.onnx)<br>[실험 기록과 실행 노트북](week07/README.md) | DAgger 2회전 완료. 선택 v1. ONNX 계약·배치 1/8 출력 검증 완료. 공개 세 시드 평균 1.0× 86.43 / 1.2× 69.58 |
| 8주차 비교 리포트: 모듈형 vs E2E | [비교 리포트](week08/비교리포트_202312312_송명진.md)<br>[실행 노트북·결과](week08/README.md) | 전체 실험 실행 완료. 정책×조건 점수표·그래프·해석 5문장 및 CSV 일치 검증 완료 |

자동채점 셀의 소스는 배포본과 동일하게 보존했습니다.

과제 2는 수업 저장소 `mhahn0106/ku-sm-aiapp`의 `e2e_starter/tinytrack.py`가 필요합니다. 수업 데이터로 전체 실행한 후 선택 gain 실험의 실제 결과와 `my_dataset_v1.json`을 추가해야 합니다.

과제 3의 미세조정 모델은 공개 트랙 평가에서 점수 86.723, 완주율 1.0, 이탈률 0.0을 기록했습니다. 심화 시드 0/1/2 평가의 평균·표준편차는 전체 미세조정 86.43·0.20, 동결 학습 28.32·9.90입니다.

`.npz` 데이터와 학습 체크포인트(`.pt`, `.pth`)는 제출 대상에서 제외하며, 과제 3의 ONNX 배포 모델은 제출물에 포함합니다.
