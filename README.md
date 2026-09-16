[index.html](https://github.com/user-attachments/files/32283531/index.html)
<!doctype html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>VALORANT Custom Match Bot</title>
  <meta name="description" content="Discord에서 VALORANT 커스텀 매치를 만들고 팀 배정과 경기 기록을 관리하는 봇입니다.">
  <style>
*{box-sizing:border-box}html{scroll-behavior:smooth}body{margin:0;font-family:Arial,"Noto Sans KR",sans-serif;background:#0b0d12;color:#f5f7fa;line-height:1.7}header{position:sticky;top:0;background:rgba(11,13,18,.94);border-bottom:1px solid #252a35;z-index:2}.nav{max-width:1050px;margin:auto;padding:16px 22px;display:flex;gap:24px;align-items:center}.logo{font-weight:800;margin-right:auto}.logo span{color:#ff4655}.nav a{color:#b9c0cc;text-decoration:none}.nav a:hover{color:#fff}main{max-width:1050px;margin:auto;padding:0 22px}.hero{padding:110px 0 90px}.badge{color:#ff4655;font-weight:800;letter-spacing:2px}.hero h1{font-size:clamp(42px,7vw,76px);line-height:1.08;margin:15px 0}.hero h1 span{color:#ff4655}.lead{max-width:680px;color:#b9c0cc;font-size:20px}.buttons{display:flex;gap:12px;margin-top:30px}.primary,.secondary{padding:12px 20px;border-radius:8px;text-decoration:none;font-weight:700}.primary{background:#ff4655;color:#fff}.secondary{border:1px solid #3a404c;color:#fff}section{padding:70px 0;border-top:1px solid #20242d}h2{font-size:34px;margin-top:0}.grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}.grid article{background:#131720;border:1px solid #262c37;border-radius:14px;padding:24px}.grid b{font-size:19px}.grid p{color:#aeb6c3}.dark{background:#10131a;margin-left:calc(50% - 50vw);margin-right:calc(50% - 50vw);padding-left:calc(50vw - 50%);padding-right:calc(50vw - 50%)}ol{max-width:700px;padding-left:25px}li{padding:8px 0}code{background:#1b202a;padding:3px 7px;border-radius:5px;color:#ff9ca4}.small{font-size:14px;color:#7f8998}footer{border-top:1px solid #252a35;padding:35px 22px;text-align:center;color:#9aa3b1}@media(max-width:750px){.grid{grid-template-columns:1fr}.nav a{display:none}.hero{padding-top:75px}.lead{font-size:17px}}

</style>
</head>
<body>
<header>
  <div class="nav">
    <div class="logo">VALORANT <span>내전봇</span></div>
    <a href="#features">기능</a>
    <a href="#flow">사용 방법</a>
    <a href="#privacy">개인정보</a>
  </div>
</header>

<main>
  <section class="hero">
    <p class="badge">DISCORD × VALORANT</p>
    <h1>친구들과 하는<br><span>VALORANT 내전 관리 봇</span></h1>
    <p class="lead">Discord에서 내전을 만들고, 레드/블루 팀을 구성하고, 경기 결과와 서버 내전 기록을 관리합니다.</p>
    <div class="buttons">
      <a class="primary" href="#flow">사용 방법 보기</a>
      <a class="secondary" href="https://discord.com/" target="_blank" rel="noopener">Discord</a>
    </div>
  </section>

  <section id="features">
    <h2>주요 기능</h2>
    <div class="grid">
      <article><b>🎮 내전 생성</b><p>Discord 명령어로 새로운 커스텀 매치를 생성합니다.</p></article>
      <article><b>🔴🔵 팀 참가</b><p>버튼으로 레드/블루 팀에 참가할 수 있습니다.</p></article>
      <article><b>🎲 자동 5:5 배정</b><p>10명이 모이면 참가자를 5명씩 자동 배정합니다.</p></article>
      <article><b>📊 경기 기록</b><p>K/D/A, ACS와 서버 내전 점수를 기록할 수 있습니다.</p></article>
      <article><b>📚 내전 기록</b><p>서버에서 최근 내전 결과를 확인할 수 있습니다.</p></article>
      <article><b>🔐 Riot 계정 연동 준비</b><p>향후 Riot Sign On(RSO)을 통한 플레이어 데이터 공유 절차를 지원할 예정입니다.</p></article>
    </div>
  </section>

  <section id="flow" class="dark">
    <h2>사용 방법</h2>
    <ol>
      <li>Discord 서버에서 <code>/내전생성</code> 실행</li>
      <li>참가자가 🔴 레드 또는 🔵 블루 버튼으로 참가</li>
      <li>10명이 모이면 🎲 자동 5:5 배정</li>
      <li><code>/내전시작</code>으로 경기 시작</li>
      <li>경기 종료 후 결과를 기록</li>
    </ol>
  </section>

  <section>
    <h2>데이터 공유 안내</h2>
    <p>Riot 계정 정보와 게임 데이터는 사용자의 명시적인 동의가 있는 경우에만 연동하는 것을 목표로 합니다. Riot Sign On(RSO)이 적용되는 경우 사용자는 Riot 로그인 화면에서 데이터 공유에 동의한 뒤 서비스를 이용하게 됩니다.</p>
    <p class="small">현재 이 사이트는 제품 소개 및 Riot 개발자 등록/검토를 위한 프로토타입입니다. 실제 Riot 계정 로그인 기능은 Production 승인 및 RSO 접근 권한을 받은 후 연결합니다.</p>
  </section>

  <section id="privacy">
    <h2>개인정보처리방침</h2>
    <p>현재 사이트 자체는 회원가입이나 Riot 계정 로그인을 제공하지 않으며, 방문자의 개인정보를 별도로 수집하지 않습니다.</p>
    <p>향후 Riot Sign On을 도입할 경우 수집 항목, 이용 목적, 보관 기간 및 삭제 방법을 실제 운영 방식에 맞게 이 페이지에 업데이트합니다.</p>
  </section>

  <section>
    <h2>이용약관</h2>
    <p>본 서비스는 Discord 기반 VALORANT 커스텀 매치의 참가 및 경기 기록 관리를 위한 커뮤니티 도구입니다. Riot Games의 공식 서비스가 아니며 Riot Games와 별개의 서비스입니다.</p>
  </section>
</main>

<footer>
  <p>VALORANT 내전봇 · Community Project</p>
  <p class="small">VALORANT and Riot Games are trademarks of Riot Games, Inc.</p>
</footer>
</body>
</html>
