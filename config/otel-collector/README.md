# OpenTelemetry Collector Configuration

## 개요
이 설정 파일(`otelcol-config.yml`)은 Kafka로 Trace 데이터를 전송하기 위해 수정된 버전입니다.

## 원본 위치 (Reference)
- Repository: opentelemetry-demo
- Path: `src/otelcollector/otelcol-config.yml`

## 변경 사항
- `exporters`에 `kafka` 추가 (Port: 9092)
- `service.pipelines.traces`에 `kafka` exporter 연결

## 사용법 (How to Apply)
이 파일을 데모 프로젝트의 원본 위치에 덮어쓰거나, Docker Volume으로 마운트해서 사용합니다.