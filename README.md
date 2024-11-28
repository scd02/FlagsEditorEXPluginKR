# 플래그에디터EX(pert) 플러그인
고급 사용자를 위한 [PKHeX](https://github.com/kwsch/PKHeX) 플러그인입니다.
세이브 파일에서 모든 종류의 플래그 및 이벤트 작업 데이터를 편집할 수 있습니다.

## 설정 지침
- [여기](https://projectpokemon.org/pkhex/) 에서 최신 PKHeX 버전을 사용해야 합니다
- [여기](https://github.com/fattard/FlagsEditorEXPlugin/releases/latest) 에서 최신 릴리스에서 플러그인 다운로드 하십시오.
- Windows의 속성 메뉴에서 해당 항목을 추출하고 차단을 해제합니다.
- PKHeX 프로그램 경로와 동일한 폴더에 있는 *plugins* 폴더에 넣습니다.
- *plugins* 폴더가 없는 경우, 모두 소문자로 새 폴더를 만듭니다.
- 문제가 있는 경우 자세한 지침 예제를 확인(특히 4단계와 5단계): [PKHeX 플러그인 수동 설치](https://github.com/architdate/PKHeX-Plugins/wiki/Installing-PKHeX-Plugins#manual-installation-or-installing-older-releases).

## 행동

**참고: 목록에는 사용하지 않는 데이터가 포함될 수 있으며, 플래그에 대한 문서화가 진행됨에 따라 나중에 필터링됩니다.**  

### 플래그 편집

이 작업을 수행하면 플러그인의 기본 창이 열립니다.  
모든 종류의 플래그 및 이벤트 작업 데이터는 여러 탭을 통해 편집할 수 있으며, 이 탭을 통해 전용 편집기와 기본 필터가 열립니다.  

![image](https://github.com/fattard/FlagsEditorEXPlugin/assets/1159052/bdc96090-d506-49b6-9c21-3283a999a0bf)
![image](https://github.com/fattard/FlagsEditorEXPlugin/assets/1159052/5d7ccace-e6de-4a54-9a08-f39d2458c1ee)
![image](https://github.com/fattard/FlagsEditorEXPlugin/assets/1159052/5aff3825-be2f-4f3d-aee2-489a599eb354)
![image](https://github.com/fattard/FlagsEditorEXPlugin/assets/1159052/640c5696-6939-4ba6-8d7a-23d40264bc68)

편집을 완료한 후 기본 응용 프로그램에서 세이브 데이터를 내보냅니다.

**안전 점검은 전혀 수행되지 않으므로 변경 사항을 조합하면 소프트락, 충돌, 영구 데이터 손실과 같은 문제가 발생할 수 있습니다.**
**플래그 편집을 시작하기 전에 데이터 세이브 백업을 강력히 권장합니다.**

### 모든 플래그 추출

이 작업은 현재 플래그 상태(참/거짓) 및 이벤트 작업 값과 함께 전체 플래그 데이터베이스를 내보냅니다(사용 가능한 경우).  
이 작업은 주로 플래그 상태를 조사하고 이전/현재 상태를 구분하여 플래그 사용을 발견하고 문서화하여 사람이 읽을 수 있는 정보로 추가하기 위한 것입니다.  

## 지원되는 게임
모든 메인 게임이 지원됩니다(많은 게임에 대한 설명은 제한적입니다)

- 레드 / 블루 / 옐로우 (국제 및 일본 버전)
- 금 / 은 / 크리스탈 (국제, 일본 및 한국 버전)
- 루비 / 사파이어 / 에메랄드 / 파이어레드 / 리프그린
- 디아루가 / 펄기아 / 기라티나 / 하트골드 / 소울실버
- 블랙 / 화이트 / 블랙 2 / 화이트 2
- X / Y / 오메가루비 / 알파사파이어
- 썬 / 문 / 울트라 썬 / 울트라 문 / 레츠고! 피카츄 / 레츠고! 이브이
- 소드 / 실드 / 브릴리언트 다이아몬드 / 샤이닝 펄 / LEGENDS: 아르세우스
- 스칼렛 / 바이올렛

## 기여하다(도움)

### 현지화된 콘텐츠

UI 현지화 파일은 '=' 문자로 키=값 쌍을 지정하여 PKHeX 현지화 리소스와 동일한 형식을 따릅니다.  
파일은 [_localization_](/localization) 폴더에 있습니다.

현재 기본 PKHeX 애플리케이션이 사용 중인 언어와 동일한 언어를 감지합니다.

이 언어는 스페인어나 독일어만큼 UI 공간 제약이 심하기 때문에 UI에 레이블을 넣을 공간을 확보하는 데 사용하는 pt-BR 언어용 언어 파일을 추가로 포함했습니다.  
또한 UI의 현지화 작동 방식에 대한 주어진 예시로도 사용할 수 있습니다.

다음 표에는 기여할 수 있는 언어가 있습니다
| 키  | 언어                 | 기여자   |
|-----|---------------------|----------------|
| de  | 독일어              |                |
| en  | 영어              | Fattard             |
| es  | 스페인어           |                |
| fr  | 프랑스어           |                |
| it  | 이탈리아어           |                |
| ja  | 일본어              |                |
| ko  | 한국어              |                |
| zh  | 중국어 간체       |pplloufh 그리고 wubinwww|
| zh2 | 중국어 번체       |                |

플래그 리소스 데이터베이스도 현지화할 수 있지만, 해당 리소스가 지속적으로 변경되므로 현재로서는 권장되지 않습니다.

해당 파일은 [_flagslist_](/flagslist) 폴더에 있는 간단한 _tsv_ 텍스트 파일입니다.

몇 가지 예를 들어 파일의 헤더:
| 날것 Idx | 이벤트 유형 | 지역        | 보완        | 텍스트 설명                                   | 유효한 값                        | 식별자                  |
|---------|------------|--------------|------------|----------------------------------------------|---------------------------------|-------------------------|
| 0x0008  | 아이템 선물  | 도라지시티   | 체육관     | 관장 비상으로부터 TM31(진흙뿌리기) 획득         |                                 | EVENT_GOT_TM31_MUD_SLAP |
| 0x0034  |             | 챔피언로드   | 1층        | 라이벌 상태                                  | 0:당신과 싸울 것 입니다,1:사라짐   | wVictoryRoadSceneID     |

다음 열은 내부 논리의 일부이므로 **NOT**을 수정해야 합니다
- 날것 Idx
- 이벤트 유형
- 식별자

현지화 가능한 열은 다음과 같습니다:
- 위치(마을 이름, 도시, 던전 등 이벤트 플래그의 주요 위치)
- 보완 사항(층수 또는 누군가의 집과 같은 장소의 이름과 같은 유용한 보완 사항)
- 텍스트 설명(플래그의 목적에 대한 설명)
- 유효한 값(이벤트 작업 플래그에만 사용되며, 키:값 쌍은 문자 ':'로 표시되며 각 항목은 ','로 구분됩니다.)

### 새로 발견된 플래그

이벤트 플래그는 조금씩 연구되고 있습니다.  
플래그가 문서화되고 설명이 생성되면 다음 버전의 플러그인에 포함됩니다.

모든 연구 작업은 여기에서 확인할 수 있습니다

[이벤트 플래그 - 리서치 스프레드시트](https://docs.google.com/spreadsheets/d/1PkY3AVafdOEqKiD_TzD4hTDRvf39ad-eI7e4JylyVII/copy)

기여하려면 위의 사본을 만들고 조사한 정보를 작성한 다음 병합해야 할 정보로 다시 연락하세요.

커뮤니티 기여의 우선순위는 3DS 게임입니다.  
스위치 게임은 현재 어느 정도 진전이 있었습니다.

## 크레딧

[Kurt](https://github.com/kwsch) 위해서 [PKHeX](https://github.com/kwsch/PKHeX) 그리고 [pkNX](https://github.com/kwsch/pkNX)  
이벤트 플래그 및 데이터 마이닝에 대한 많은 연구를 위한 [Matt](https://github.com/sora10pls)
[Pret](https://github.com/Pret) 그리고 모든 분해물  
이벤트 플래그 연구에 기여한 [PPOrg](https://projectpokemon.org) 의 모든 사람들
