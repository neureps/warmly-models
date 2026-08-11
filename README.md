# warmly-models

온기(Warmly) 온디바이스 모델 **서빙 미러** — 릴리스 에셋 전용 리포.

- 원본 레지스트리: Hugging Face neureps/warmly-qwen35-{2b,08b}-enko-gguf (버전·제조법은 ondevice-models 리포 MODEL-REGISTRY/RELEASE 문서)
- 미러 이유: 셀룰러망에서 HF CDN 다운로드가 ~100KB/s로 저속 (실기기 실측 2026-08-11)
- 에셋은 업로드 시 sha256(HF LFS oid) 일치 검증. 앱(src/infra/engine/models.ts)이 이 릴리스 URL을 가리킨다.
- 스페이셜 ONNX 2종 출처: onnx-community/depth-anything-v2-small rev 4472b73(Apache-2.0), andraniksargsyan/migan rev 1538c13(MIT)
