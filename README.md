[index.html](https://github.com/user-attachments/files/32084423/MockUp.html)
# 便利商店中的我

<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>店中的我｜產品 Mockup</title>
<style>
:root{
  --navy:#0c2446;
  --navy2:#183b68;
  --ice:#f5f7f9;
  --ink:#233042;
  --muted:#8290a3;
  --line:#dfe5eb;
  --white:#fff;
  --cyan:#31b9c7;
  --gold:#f7c64a;
  --shadow:0 20px 50px rgba(12,36,70,.14);
}
*{box-sizing:border-box}
body{
  margin:0;font-family:Inter,"Noto Sans TC","Microsoft JhengHei",Arial,sans-serif;
  background:linear-gradient(180deg,#edf2f6,#f8fafb); color:var(--ink);
}
button{font:inherit}
.wrap{max-width:1360px;margin:0 auto;padding:28px 28px 60px}
.topbar{
  display:flex;justify-content:space-between;align-items:center;margin-bottom:22px;
}
.brand{font-weight:900;color:var(--navy);letter-spacing:.02em}
.badge{font-size:12px;color:#52708f;background:#eaf0f5;border:1px solid #dbe4ec;padding:7px 12px;border-radius:99px}
.layout{display:grid;grid-template-columns:240px 1fr;gap:24px}
.side{
  background:rgba(255,255,255,.82);border:1px solid var(--line);border-radius:22px;padding:16px;
  box-shadow:var(--shadow);height:max-content;position:sticky;top:20px;
}
.side h3{margin:5px 8px 14px;font-size:13px;color:var(--muted);font-weight:800}
.navbtn{
  width:100%;border:0;background:transparent;text-align:left;padding:13px 14px;border-radius:14px;
  color:#5e6d7f;cursor:pointer;margin-bottom:6px;font-weight:800;
}
.navbtn.active{background:var(--navy);color:white}
.navbtn small{display:block;font-size:10px;opacity:.68;margin-top:3px;font-weight:600}
.stage{
  min-height:760px;background:var(--white);border:1px solid var(--line);border-radius:28px;
  box-shadow:var(--shadow);overflow:hidden;
}
.screen{display:none;min-height:760px}
.screen.active{display:block}
.screen-head{padding:28px 34px 18px;border-bottom:1px solid var(--line);display:flex;justify-content:space-between;align-items:flex-end}
.eyebrow{font-size:12px;color:#7f8da0;font-weight:900;letter-spacing:.12em}
.screen-title{font-size:28px;font-weight:950;color:var(--navy);margin-top:6px}
.screen-sub{font-size:13px;color:#8490a0;margin-top:6px}
.browser{
  margin:24px 34px;background:#f6f0e3;border:1px solid #ccd5de;border-radius:18px;overflow:hidden;
  box-shadow:0 16px 40px rgba(12,36,70,.12)
}
.browserbar{height:44px;background:#11376c;display:flex;align-items:center;padding:0 14px;gap:10px}
.dot{width:11px;height:11px;border-radius:50%}.d1{background:#f7c64a}.d2{background:#36a9c9}.d3{background:#f16a63}
.address{height:26px;border-radius:8px;background:#fff;opacity:.94;flex:1;color:#9aa7b6;font-size:11px;padding:6px 10px;margin-left:10px}
.home{font-size:16px;color:#fff;margin-right:2px}
.hero{
  min-height:620px;display:grid;grid-template-columns:1.1fr .9fr;gap:16px;padding:30px;
  background:radial-gradient(circle at 30% 15%,#dbe9ea 0,#eef4f3 30%,#f6f0e3 70%);
}
.hero-left{display:flex;flex-direction:column;justify-content:center;padding:24px}
.logo{font-size:15px;color:#1d6b78;font-weight:900;letter-spacing:.08em}
.hero h1{font-size:48px;line-height:1.08;margin:14px 0;color:var(--navy);letter-spacing:-.03em}
.hero p{font-size:18px;line-height:1.8;color:#596878;max-width:800px}
.cta{display:inline-flex;align-items:center;gap:10px;background:var(--navy);color:#fff;border:0;border-radius:14px;padding:15px 22px;font-weight:900;cursor:pointer;width:max-content;box-shadow:0 12px 26px rgba(12,36,70,.2)}
.cta.secondary{background:#fff;color:var(--navy);border:1px solid #c9d5e1;box-shadow:none}
.card-stack{display:flex;align-items:center;justify-content:center;position:relative}
.idcard{
  width:320px;border-radius:24px;background:linear-gradient(155deg,#0e2a53,#173a68);
  padding:22px;box-shadow:0 24px 55px rgba(12,36,70,.28);color:#fff;transform:rotate(2deg);
}
.idchip{display:flex;justify-content:space-between;align-items:center;font-size:10px;color:#b8cadf}
.avatar{
  width:118px;height:118px;border-radius:50%;margin:22px auto 14px;display:flex;align-items:center;justify-content:center;
  background:linear-gradient(145deg,#4cb0c3,#edf5f3);font-size:52px;
  border:4px solid #fff;box-shadow:0 8px 28px rgba(0,0,0,.18)
}
.result-name{font-size:26px;font-weight:950;text-align:center}.tags{text-align:center;color:#ffda63;font-size:12px;margin-top:7px}
.quote{margin-top:16px;background:rgba(255,255,255,.08);border-radius:13px;padding:13px;font-size:11px;line-height:1.7;color:#e6eef7}
.progress{display:flex;gap:8px;padding:18px 34px;border-top:1px solid var(--line);background:#fbfcfd}
.step{height:6px;border-radius:99px;background:#dde4eb;flex:1}.step.done{background:var(--cyan)}
.quiz{display:grid;grid-template-columns:1fr 1fr;gap:22px;padding:28px 34px}
.question{
  padding:28px;border:1px solid var(--line);border-radius:20px;background:#fff;box-shadow:0 10px 24px rgba(12,36,70,.06)
}
.qn{font-size:12px;font-weight:900;color:var(--cyan);letter-spacing:.12em}.question h2{font-size:22px;color:var(--navy);margin:8px 0 20px}
.option{display:block;width:100%;text-align:left;border:1px solid #dce4eb;background:#f9fbfc;border-radius:14px;padding:14px;margin:9px 0;cursor:pointer;color:#405267}
.option:hover{border-color:#8abcc6;background:#f2fbfc}.option.selected{background:#eaf7f8;border-color:#4bb8c2;color:#0b4651;font-weight:800}
.ai{
  display:grid;grid-template-columns:1fr 1fr;gap:22px;padding:34px;align-items:center
}
.ai-card{border:1px solid var(--line);border-radius:22px;min-height:520px;background:#fbfcfd;padding:28px}
.scan{height:100%;display:flex;flex-direction:column;justify-content:center;align-items:center}
.ring{
  width:180px;height:180px;border-radius:50%;border:6px solid #d6ebee;position:relative;margin-bottom:22px
}
.ring:after{content:"";position:absolute;inset:10px;border-radius:50%;border:5px dashed var(--cyan);animation:spin 7s linear infinite}
@keyframes spin{to{transform:rotate(360deg)}}
.scan h2{color:var(--navy);font-size:26px;margin:0 0 8px}.scan p{color:#788698;text-align:center;line-height:1.7}
.chips{display:flex;flex-wrap:wrap;gap:8px;margin-top:20px}.chip{background:#eff3f7;border:1px solid #dbe3ea;border-radius:999px;padding:8px 11px;font-size:11px;color:#516173}
.upload{
  border:2px dashed #b8cad8;border-radius:20px;min-height:360px;display:flex;flex-direction:column;align-items:center;justify-content:center;
  background:linear-gradient(180deg,#fcfeff,#f5f8fa)
}
.upload .face{font-size:58px;margin-bottom:12px}.upload strong{font-size:20px;color:var(--navy)}.upload span{font-size:12px;color:#8793a0;margin-top:8px}
.final{
  padding:34px;display:grid;grid-template-columns:1fr 1fr;gap:22px
}
.mock-card{border-radius:24px;background:#0e2a53;color:white;min-height:500px;padding:28px;position:relative;overflow:hidden}
.mock-card:before{content:"";position:absolute;width:240px;height:240px;border-radius:50%;background:rgba(49,185,199,.12);right:-70px;top:-60px}
.smallbrand{font-size:12px;letter-spacing:.12em;color:#c5d4e4;font-weight:900}.person{display:flex;gap:18px;align-items:center;margin-top:34px}
.person .portrait{width:108px;height:108px;border-radius:22px;background:linear-gradient(145deg,#5bb9c4,#efddd0);display:flex;align-items:center;justify-content:center;font-size:46px}
.person h2{margin:0;font-size:32px}.person p{margin:7px 0;color:#ffda63;font-size:12px}
.final .quote2{margin-top:22px;color:#dce8f3;line-height:1.8;font-size:14px}
.qr{position:absolute;right:28px;bottom:28px;width:90px;height:90px;background:repeating-linear-gradient(45deg,#fff 0 6px,#151515 6px 11px);border-radius:8px}
.handoff{
  background:#f7f9fb;border:1px solid var(--line);border-radius:24px;padding:30px;min-height:500px
}
.handoff h2{color:var(--navy);font-size:24px;margin:0}.handoff p{color:#748295;line-height:1.7}
.flow{margin:26px 0}.flowitem{display:flex;align-items:center;gap:12px;margin:14px 0}.num{width:34px;height:34px;border-radius:50%;background:var(--navy);color:#fff;display:flex;align-items:center;justify-content:center;font-size:12px;font-weight:900}
.gama{margin-top:20px;background:#fff;border:1px solid var(--line);border-radius:18px;padding:18px;display:flex;gap:14px;align-items:center}.gama-icon{width:54px;height:54px;border-radius:16px;background:var(--navy);color:white;display:flex;align-items:center;justify-content:center;font-size:22px}
.note{font-size:11px;color:#91a0b0;margin-top:16px}
@media(max-width:980px){.layout{grid-template-columns:1fr}.side{position:static}.hero,.ai,.final{grid-template-columns:1fr}.quiz{grid-template-columns:1fr}.stage,.screen{min-height:0}}
</style>
</head>
<body>
<div class="wrap">
  <div class="topbar">
    <div class="brand">便利商店中的我 <span style="opacity:.45">/ PRODUCT MOCKUP</span></div>
    <div class="badge">AI × 人格 × 角色 × Gama Play</div>
  </div>

  <div class="layout">
    <aside class="side">
      <h3>Prototype Flow</h3>
      <button class="navbtn active" data-screen="home">01｜入口<small>如果便利商店裡的那個人，是你？</small></button>
      <button class="navbtn" data-screen="quiz">02｜認識我<small>3 題創業情境測驗</small></button>
      <button class="navbtn" data-screen="upload">03｜看見我<small>上傳照片 × AI</small></button>
      <button class="navbtn" data-screen="result">04｜定義我<small>創業人格 × 身份卡</small></button>
      <button class="navbtn" data-screen="gama">05｜帶走我<small>Gama Play 收藏</small></button>
    </aside>

    <main class="stage">
      <section class="screen active" id="home">
        <div class="screen-head">
          <div><div class="eyebrow">01 / LANDING</div><div class="screen-title">如果便利商店裡的那個人，是你？</div><div class="screen-sub">不扮演店員、店長；讓 AI 找出你的便利商店創業者身份。</div></div>
          <button class="cta" onclick="go('quiz')">開始測驗 →</button>
        </div>
        <div class="browser">
          <div class="browserbar"><span class="home">⌂</span><span style="color:#fff">‹</span><span style="color:#fff">›</span><div class="address">convenience-me.tw</div><span class="dot d1"></span><span class="dot d2"></span><span class="dot d3"></span></div>
          <div class="hero">
            <div class="hero-left">
              <div class="logo">便利商店中的我</div>
              <h1>如果你開一家便利商店，<br>你會是誰？</h1>
              <p>回答 3 個創業情境，讓 AI 看見你的經營直覺，再把「你」變成便利商店世界裡的專屬角色。</p>
              <div style="display:flex;gap:10px;flex-wrap:wrap;margin-top:12px">
                <button class="cta" onclick="go('quiz')">開始認識自己</button>
                <button class="cta secondary" onclick="go('upload')">我有照片，直接開始</button>
              </div>
            </div>
            <div class="card-stack">
              <div class="idcard">
                <div class="idchip"><span>MY CONVENIENCE STORE IDENTITY</span><span>01</span></div>
                <div class="avatar">🙂</div>
                <div class="result-name">深夜守護者</div>
                <div class="tags">#溫暖　#堅持　#夜貓子</div>
                <div class="quote">「你的店，不只是賣東西的地方；而是有人在深夜裡，還為你留著一盞燈。」</div>
              </div>
            </div>
          </div>
          <div class="progress"><div class="step done"></div><div class="step"></div><div class="step"></div><div class="step"></div><div class="step"></div></div>
        </div>
      </section>

      <section class="screen" id="quiz">
        <div class="screen-head">
          <div><div class="eyebrow">02 / KNOW ME</div><div class="screen-title">3 題，測出你的經營直覺</div><div class="screen-sub">不是傳統人格題；直接問：「如果這家店是你的，你會怎麼做？」</div></div>
          <button class="cta" onclick="go('upload')">下一步 →</button>
        </div>
        <div class="quiz">
          <div class="question">
            <div class="qn">Q1</div><h2>開店第一天，你最想先做什麼？</h2>
            <button class="option" onclick="pick(this)">商品要應有盡有！</button>
            <button class="option" onclick="pick(this)">把店裝飾得漂漂亮亮</button>
            <button class="option" onclick="pick(this)">先搞懂市場需求再決定</button>
            <button class="option" onclick="pick(this)">要讓大家有強烈印象！</button>
          </div>
          <div class="question">
            <div class="qn">Q2</div><h2>突然來了一大群客人，你會？</h2>
            <button class="option" onclick="pick(this)">確保商品足夠</button>
            <button class="option" onclick="pick(this)">靜觀其變</button>
            <button class="option" onclick="pick(this)">這是推銷的好時機</button>
            <button class="option" onclick="pick(this)">有店員在，安啦！</button>
          </div>
          <div class="question">
            <div class="qn">Q3</div><h2>希望客人離開後的心情是什麼？</h2>
            <button class="option" onclick="pick(this)">這間店什麼都有！</button>
            <button class="option" onclick="pick(this)">喜歡這裡的氛圍</button>
            <button class="option" onclick="pick(this)">老闆真有趣，很懂</button>
            <button class="option" onclick="pick(this)">這裡很與眾不同！</button>
          </div>
          <div class="question" style="display:flex;flex-direction:column;justify-content:center">
            <div class="qn">DESIGN NOTE</div>
            <h2>不要立刻公布答案</h2>
            <p style="color:#758396;line-height:1.8">完成選擇後進入「AI 分析中……」，把結果揭曉做成體驗高潮，而不是普通測驗結果頁。</p>
            <button class="cta" onclick="go('upload')">交給 AI 分析</button>
          </div>
        </div>
        <div class="progress"><div class="step done"></div><div class="step done"></div><div class="step"></div><div class="step"></div><div class="step"></div></div>
      </section>

      <section class="screen" id="upload">
        <div class="screen-head">
          <div><div class="eyebrow">03 / SEE ME</div><div class="screen-title">讓 AI 看見真正的你</div><div class="screen-sub">自拍、生活照、大頭照都可以；不要求正式擺拍。</div></div>
          <button class="cta" onclick="go('result')">模擬生成 →</button>
        </div>
        <div class="ai">
          <div class="ai-card">
            <div class="upload">
              <div class="face">📸</div><strong>上傳你的照片</strong>
              <span>JPG / PNG · 建議半身或大頭照</span>
              <div style="margin-top:18px"><button class="cta" onclick="alert('Prototype：這裡接真實照片上傳')">選擇照片</button></div>
              <div class="chips"><span class="chip">生活照</span><span class="chip">自拍</span><span class="chip">證件照</span></div>
            </div>
            <div class="note">不想上傳照片？提供「使用預設角色」Fallback，避免流程中斷。</div>
          </div>
          <div class="ai-card scan">
            <div class="ring"></div>
            <h2>AI 正在讀取你的創業氣質…</h2>
            <p>臉部辨識 ✓<br>表情分析 ✓<br>創業人格同步 ✓</p>
            <div class="chips"><span class="chip">你怎麼做決策</span><span class="chip">你怎麼看客人</span><span class="chip">你想留下什麼體驗</span></div>
          </div>
        </div>
        <div class="progress"><div class="step done"></div><div class="step done"></div><div class="step done"></div><div class="step"></div><div class="step"></div></div>
      </section>

      <section class="screen" id="result">
        <div class="screen-head">
          <div><div class="eyebrow">04 / DEFINE ME</div><div class="screen-title">你是——深夜守護者</div><div class="screen-sub">生成結果不是一張 AI 圖，而是一張可以被收藏、分享、帶進遊戲的身份卡。</div></div>
          <button class="cta" onclick="go('gama')">帶走我的身份 →</button>
        </div>
        <div class="final">
          <div class="mock-card">
            <div class="smallbrand">便利商店中的我</div>
            <div class="person">
              <div class="portrait">👩🏻</div>
              <div><h2>深夜守護者</h2><p>#溫暖 #堅持 #夜貓子 #熟客派</p></div>
            </div>
            <div class="quote2">你相信便利商店不只是買東西的地方，而是有人在深夜裡，還為你留著一盞燈。</div>
            <div style="margin-top:28px;font-size:12px;color:#b8c8da">你的創業人格，適合經營深夜商圈。</div>
            <div style="margin-top:9px;font-size:20px;font-weight:900">凌晨 2:13，總有一位客人會來找你。</div>
            <div class="qr"></div>
          </div>
          <div class="handoff">
            <h2>把「我」帶進 Gama Play</h2>
            <p>把一次性的 AI 活動，轉成可以留下來的遊戲身份。</p>
            <div class="flow">
              <div class="flowitem"><div class="num">01</div><div><b>活動網站</b><div style="font-size:12px;color:#8090a0">生成我的創業者</div></div></div>
              <div class="flowitem"><div class="num">02</div><div><b>Gama Play</b><div style="font-size:12px;color:#8090a0">收藏我的身份／徽章</div></div></div>
              <div class="flowitem"><div class="num">03</div><div><b>遊戲</b><div style="font-size:12px;color:#8090a0">身份延伸成 NPC、商圈、內容</div></div></div>
              <div class="flowitem"><div class="num">04</div><div><b>社群</b><div style="font-size:12px;color:#8090a0">分享「我是什麼型老闆？」</div></div></div>
            </div>
            <div class="gama"><div class="gama-icon">G</div><div><b style="color:var(--navy)">Gama Play</b><div style="font-size:11px;color:#8a97a6">Deep Link / QR Code 均可作為轉移方式</div></div></div>
            <div style="display:flex;gap:10px;margin-top:18px">
              <button class="cta" onclick="alert('Prototype：這裡接 Gama Play Deep Link')">前往 Gama Play</button>
              <button class="cta secondary" onclick="alert('Prototype：分享身份卡')">分享我的身份</button>
            </div>
          </div>
        </div>
        <div class="progress"><div class="step done"></div><div class="step done"></div><div class="step done"></div><div class="step done"></div><div class="step"></div></div>
      </section>

      <section class="screen" id="gama">
        <div class="screen-head">
          <div><div class="eyebrow">05 / TAKE ME WITH YOU</div><div class="screen-title">Gama Play：身份正式被收藏</div><div class="screen-sub">把「便利商店創業者」從 Web 活動帶進 App，成為長期可延伸的身份資產。</div></div>
          <button class="cta" onclick="go('home')">重新體驗 ↻</button>
        </div>
        <div style="padding:30px 34px">
          <div style="display:grid;grid-template-columns:1.2fr .8fr;gap:22px">
            <div style="border:1px solid var(--line);border-radius:24px;background:#f7f8fa;min-height:540px;padding:24px">
              <div style="font-size:12px;color:#91a0af;font-weight:900">GAMA PLAY / PROFILE</div>
              <div style="background:#fff;border:1px solid var(--line);border-radius:20px;margin-top:18px;padding:24px">
                <div style="display:flex;justify-content:space-between;align-items:center">
                  <div><div style="font-size:12px;color:#8996a5">我的創業者身份</div><div style="font-size:28px;font-weight:950;color:var(--navy);margin-top:5px">深夜守護者</div></div>
                  <div style="width:68px;height:68px;border-radius:18px;background:#0e2a53;color:#fff;display:flex;align-items:center;justify-content:center;font-size:32px">👩🏻</div>
                </div>
                <div style="display:flex;gap:8px;flex-wrap:wrap;margin-top:18px">
                  <span class="chip">專屬頭像</span><span class="chip">專屬徽章</span><span class="chip">AI 小助手</span>
                </div>
                <div style="margin-top:24px;padding:16px;border-radius:16px;background:#f1f5f8;color:#68788b;line-height:1.75;font-size:13px">
                  「你的創業人格，適合經營深夜商圈。」<br>之後還可能遇到屬於你的深夜秘密客。
                </div>
                <button class="cta" style="margin-top:18px" onclick="alert('Prototype：進入遊戲內容')">進入遊戲 →</button>
              </div>
            </div>
            <div style="border:1px solid var(--line);border-radius:24px;background:#fff;min-height:540px;padding:24px">
              <div style="font-size:12px;color:#91a0af;font-weight:900">內容延伸</div>
              <div style="margin-top:22px">
                <div style="font-size:18px;font-weight:900;color:var(--navy)">你的身份，還可以變成：</div>
                <div style="margin-top:16px;display:grid;gap:12px">
                  <div style="padding:16px;border:1px solid var(--line);border-radius:16px"><b>NPC 對話形象</b><div style="font-size:11px;color:#8290a0;margin-top:5px">讓「我」在遊戲世界裡被看見</div></div>
                  <div style="padding:16px;border:1px solid var(--line);border-radius:16px"><b>專屬徽章</b><div style="font-size:11px;color:#8290a0;margin-top:5px">收藏與社群展示</div></div>
                  <div style="padding:16px;border:1px solid var(--line);border-radius:16px"><b>AI 小助手</b><div style="font-size:11px;color:#8290a0;margin-top:5px">讓人格延伸成持續互動</div></div>
                </div>
              </div>
            </div>
          </div>
          <div class="note">Prototype 目的：驗證「Web 生成 → Gama Play 收藏 → 遊戲延伸」的產品故事是否成立；實際 Deep Link / Token / QR 規格需再由技術確認。</div>
        </div>
        <div class="progress"><div class="step done"></div><div class="step done"></div><div class="step done"></div><div class="step done"></div><div class="step done"></div></div>
      </section>
    </main>
  </div>
</div>
<script>
const buttons=[...document.querySelectorAll('.navbtn')];
function go(id){
  document.querySelectorAll('.screen').forEach(s=>s.classList.remove('active'));
  document.getElementById(id).classList.add('active');
  buttons.forEach(b=>b.classList.toggle('active',b.dataset.screen===id));
  window.scrollTo({top:0,behavior:'smooth'});
}
function pick(el){
  el.parentElement.querySelectorAll('.option').forEach(x=>x.classList.remove('selected'));
  el.classList.add('selected');
}
</script>
</body>
</html>
