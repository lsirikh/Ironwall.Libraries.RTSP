# Ironwall RTSP and ONVIF Library

WPF에서 RTSP 영상을 표시하고 ONVIF 탐색·PTZ·프리셋을 연결하는 .NET Framework 라이브러리입니다. 카메라와 프리셋 정보를 저장하는 데이터베이스 서비스도 포함합니다.

## 구성

- [Services](Services): 장치 탐색, PTZ, 카메라·프리셋 저장
- [RawFramesReceiving](RawFramesReceiving), [RawFramesDecoding](RawFramesDecoding): 영상 프레임 처리
- [ViewModels](ViewModels), [Views](Views): 영상과 카메라 UI
- [DataProviders](DataProviders), [Models](Models): 카메라 데이터 관리

## 개발 환경

Windows / .NET Framework 4.8 / WPF, Caliburn.Micro, Dapper와 SQLite를 사용합니다. 프로젝트는 외부 ONVIF·Ironwall 소스에 의존하므로 참조 경로를 먼저 맞춰야 합니다. 디코더의 네이티브 라이브러리도 실행 환경에 필요합니다.

독립 실행 앱이 아니라 관제 앱에 포함하는 모듈입니다. 외부 RTSP·ONVIF 구현의 출처와 라이선스는 유지합니다.
