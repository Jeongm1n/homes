<p align="center">
<img src="./.github/logo.png" alt="logo" width="125" />
<br />
<br />
통합 주택관리시스템 홈즈 (캡스톤 프로젝트)
</p>
<br />

- [구글 플레이스토어 Homes](https://play.google.com/store/apps/details?id=com.nemobros.homes)
- [실무중심산학프로젝트 결과보고서](./.github/report.pdf)
- [App 시연 영상](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/45795d3a-c2fa-4f6a-8522-611c1c8d992a/vllo.mp4?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20210222%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20210222T133017Z&X-Amz-Expires=86400&X-Amz-Signature=3f4da966d9ed68cfae6a90f9b24af876ad1286e26ad2a8abd231d7d69c740e90&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22vllo.mp4%22)

<br />
<p align="center">
<img src="./.github/homes.png" alt="homes" />
</p>

## 👨‍👨‍👦‍👦 Team Members
팀 네모난형제들(NemoBros)
- 허전진 [@zinirun](https://github.com/zinirun)
  - Leader (PM, DevOps, Infra)
- 조정민 [@Jeongm1n](https://github.com/Jeongm1n)
  - Backend (Node.js)
- 이건욱 [@ukunV](https://github.com/ukunV)
  - Frontend (HTML/CSS/JS)
- 김승준 [@jason4181](https://github.com/jason4181)
  - Database (MySQL)

## 📚 Stacks
- Backend - `Node.js`
- Frontend - `HTML/CSS/JS` `EJS`
- Database - `MySQL` `Firebase`
- Application - `React Native` `Expo`
- Infra - `Docker` `shell-script` `NHN ToastCloud` `NCP SENS`

## ⛳ Motivation and Core Functions
- 통합적인 관리가 이루어지는 아파트 단지와 달리 대학가, 주택가 등 일반 임대형 주택에서는 건물에 대한 관리가 이루어지기 힘들고, 건물주와 세입자와의 소통이 어려움
- **건물주**
    - 소유 건물 입주현황 관리
    - 월세, 전세, 보증금 통합 관리 → 세입자 알림
- **세입자**
    - 월세, 전세 내역 관리
    - 건물 하자 관련 관리인/건물주 수리 의뢰
    - 세입자간 쪽지알림 (층간소음 등)
    - 원터치 119 긴급 신고
    - 세입자 간 건물 내 직거래 "판다"
- **관리인**
    - 세입자 통합 알림 (분리수거, 소방점검 등)
    - 관리 건물 유지보수 통합 관리

## Usage

1. You need to install basic tools and Docker (If you already have all requirements, skip this step)
    ```bash
    sudo apt-get update
    sudo apt-get install -y wget
    sudo wget -qO- https://get.docker.com/ | sh
    ```

2. Clone this git and change permission of auto-script
    ```bash
    git clone https://github.com/zinirun/homes-app
    chmod +x homes-app/database-app/build_n_run.sh
    chmod +x homes-app/build_n_run.sh
    ```

3. Run database container with auto-script and **wait at least 30 seconds** (Database will be initialized)
    ```bash
    ./<project folder>/database-app/build_n_run.sh
    ```

4. Run node container with auto-script
    ```bash
    ./<project folder>/build_n_run.sh
    ```
