<p align="center">
  <a href="https://dawnilove.github.io/Kinema/"><img src="docs/banner.svg" alt="Kinema — 로봇을 조립하고, 학습시키고, 달성시키는 샌드박스"></a>
</p>

<h3 align="center">부품을 이어 붙여 로봇을 만들고, 강화학습으로 과제를 달성시키세요.</h3>

<p align="center">
  <b>조립 · 과제 · 학습 · 실험 노트</b> — 네 단계가 한 앱에.<br>
  파이썬도, 개발 도구도, GPU도 필요 없어요. 설치파일 하나로 Windows에서 바로 돌아가요.
</p>

<p align="center">
  <a href="https://dawnilove.github.io/Kinema/"><img src="https://img.shields.io/github/v/release/Dawnilove/Kinema?label=%EC%B5%9C%EC%8B%A0%20%EB%B2%84%EC%A0%84&labelColor=121417&color=FF5A1F&style=for-the-badge" alt="최신 버전"></a>
  <img src="https://img.shields.io/badge/Windows-10%20%7C%2011-2C323B?labelColor=121417&style=for-the-badge" alt="Windows 10, 11">
  <img src="https://img.shields.io/badge/GPU-%EB%B6%88%ED%95%84%EC%9A%94-2C323B?labelColor=121417&style=for-the-badge" alt="GPU 불필요">
</p>

<p align="center">
  <a href="https://github.com/Dawnilove/Kinema/releases/latest/download/Kinema-Setup.exe"><b>⬇ Kinema-Setup.exe 내려받기</b></a> ·
  <a href="https://dawnilove.github.io/Kinema/">소개 사이트</a>
</p>

> 이 저장소는 **배포용**이에요. 설치파일과 사용 설명만 있고, 소스 코드는 공개하지 않아요.

<p align="center">
  <img src="images/train.png" alt="학습 화면: 지금 정책이 한 판 하는 3D 재생, 성공률 곡선, 지표 카드">
</p>

<table>
  <tr>
    <td width="50%"><img src="images/project.png" alt="시작 화면"><br><sub><b>시작</b> · 틀 카드로 바로 시작하는 첫 화면</sub></td>
    <td width="50%"><img src="images/assembly.png" alt="조립 화면"><br><sub><b>조립</b> · 부품 카드로 붙이고, 3D에서 작업 부위와 목표를 확인해요</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="images/scene.png" alt="과제 화면"><br><sub><b>과제</b> · 과제를 고르고 목표가 나올 범위를 상자로 정해요</sub></td>
    <td width="50%"><img src="images/monitor.png" alt="실험 노트"><br><sub><b>실험 노트</b> · 실험을 비교하고 메모와 AI 조언을 받아요</sub></td>
  </tr>
</table>

## ✨ 이렇게 이어져요

| 단계 | 하는 일 |
|---|---|
| **1 조립** | 링크·관절·바퀴·다리·그리퍼를 카드로 이어 붙이고 3D에서 바로 확인해요. 잘못 붙이면 이유를 알려 줘요. URDF·MJCF 파일도 불러와요. |
| **2 과제** | 팔 뻗기 · 이동 · 균형 · 걷기 · 집어서 옮기기 중에서 고르고, 목표가 나올 범위를 상자로 정해요. |
| **3 학습** | 시작 버튼 하나로 강화학습(SAC·PPO·TD3)을 돌려요. 진행 띠·곡선·**정책 재생**이 실시간으로 움직이고, 일시정지도 되고, 창을 닫아도 학습은 계속돼요. |
| **4 실험 노트** | 실험을 시간순으로 보고, 두 개를 골라 곡선과 바뀐 설정을 비교해요. 메모와 AI 조언도 한 장에 있어요. |

- 🎬 **정책 재생** — 학습하는 동안 지금 정책이 한 판 하는 모습을 3D로 봐요. 손이 지난 길과 지나온 자세 잔상, 지난 판 겹쳐 보기도 돼요. 학습 결과에는 영향이 없어요.
- 🩺 **자동 진단** — 학습이 막히면 원인 후보를 알려 주고, 안전한 것은 스스로 고쳐요.
- 🤖 **AI 조언 (선택)** — 분석가 2명이 따로 기록을 보고, **의견이 같은 것만** 설정 제안으로 보여 줘요. 적용은 새 설정 파일로만 되고, 학습은 자동으로 시작하지 않아요.
- 💾 **내 데이터는 내 PC에** — 모든 기록은 `문서\Kinema`에 저장돼요.

## ⬇ 설치

1. **Releases**에서 `Kinema-Setup.exe`를 내려받아요.
2. 더블클릭해서 설치해요. 관리자 권한은 필요 없어요.
3. "알 수 없는 게시자" 경고가 뜨면 **추가 정보 → 실행**을 눌러요. (코드 서명이 아직 없어요.)
4. 시작 메뉴에서 **Kinema**을 열어요.

지우려면 설정 → 앱에서 Kinema을 제거해요. 학습 기록(`문서\Kinema`)은 남아요.

## 🖥 필요한 것
- Windows 10 또는 11, 64비트
- 메모리 8 GB 이상 권장, 디스크 약 1 GB
- GPU는 필요 없어요. 3D가 안 되는 PC에서는 소프트웨어 방식으로 자동 전환해요.

## 📁 내 데이터는 어디에 저장되나

`문서\Kinema` 폴더예요. (예전 버전이 만든 `문서\CAPEK` 폴더가 있으면 그것을 그대로 써요.)

| 폴더 | 내용 |
|---|---|
| `runs\` | 학습 기록과 학습된 두뇌 |
| `my_configs\` | 조립 화면에서 저장한 설정 |
| `logs\` | 문제가 생겼을 때 볼 로그 |

다른 폴더를 쓰려면 환경변수 `KINEMA_DATA_DIR`을 설정해요.

## 🤖 AI 조언 (선택)
- 실험 노트의 **AI 조언 받기** 버튼으로 써요. 본인의 Anthropic API 키가 필요해요.
- 처음 쓸 때 안내를 읽고 동의해야 해요. 학습 설정과 지표 요약이 Anthropic으로 전송돼요. **파일 경로와 API 키는 보내지 않아요.**
- 비용은 본인의 Anthropic 계정에 청구돼요. 호출 전에 예상 비용을 보여 주고 확인을 받아요. 한 번에 약 $0.1~0.3이에요.
- API 키는 Windows 자격 증명 관리자에 저장해요. 파일에는 저장하지 않아요.
- 조언은 참고용이에요. 자동으로 적용하거나 학습을 시작하지 않아요.

## 🛟 문제가 생기면
1. `문서\Kinema\logs\gui.log`를 열어요.
2. 로그와 화면 문구를 [이슈](https://github.com/Dawnilove/Kinema/issues)에 적어 주세요.
3. 보안 문제는 [SECURITY.md](SECURITY.md)를 봐 주세요.

## 알려진 한계
- Windows만 지원해요. 다른 운영체제는 나중에 넓혀요.
- 코드 서명이 없어 첫 실행에 경고가 떠요. 일부 백신이 새 프로그램을 의심할 수 있어요.
- 학습은 CPU로 해요. 큰 과제는 오래 걸려요.

## 📄 라이선스
개인 학습·교육·연구 목적은 무료예요. 재배포, 수정, 역공학, 상업적 사용은 허용하지 않아요. 보증은 없어요. 전문은 [LICENSE.txt](LICENSE.txt)를 봐 주세요.
