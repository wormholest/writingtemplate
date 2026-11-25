<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>學測英文作文模板</title>
<style>
  :root {
    --basic: #2E7D32;
    --basic-bg: #E8F5E9;
    --inter: #1565C0;
    --inter-bg: #E3F2FD;
    --adv: #6A1B9A;
    --adv-bg: #F3E5F5;
    --border: #CFD8DC;
    --text: #222222;
    --muted: #546E7A;
    --zebra: #F8FAFC;
  }

  * { box-sizing: border-box; }

  body {
    font-family: 'Microsoft JhengHei', 'PingFang TC', 'Noto Sans TC', 'Calibri', sans-serif;
    color: var(--text);
    max-width: 980px;
    margin: 0 auto;
    padding: 24px 20px 56px 20px;
    line-height: 1.65;
    background-color: #FFFFFF;
  }

  /* 標題區 */
  .doc-header {
    border-bottom: 2.5px solid #1A237E;
    padding-bottom: 10px;
    margin-bottom: 16px;
  }
  .doc-header h1 {
    font-size: 22pt;
    color: #1A237E;
    margin: 0 0 4px 0;
  }
  .doc-header h2 {
    font-size: 13pt;
    color: #37474F;
    margin: 4px 0 4px 0;
    font-weight: bold;
  }
  .doc-header p {
    font-size: 10.5pt;
    color: var(--muted);
    margin: 0;
  }

  /* 原題圖片區 */
  .prompt-img-wrap {
    text-align: center;
    margin: 14px 0 20px 0;
  }
  .prompt-img-wrap img {
    max-width: 100%;
    height: auto;
    border: 1px solid #E0E0E0;
    border-radius: 6px;
  }

  /* 分頁切換按鈕列（整合三版本總覽） */
  .tab-bar {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 12px;
    margin: 18px 0 22px 0;
  }
  .tab-btn {
    text-align: left;
    padding: 12px 14px;
    border-radius: 10px;
    border: 2px solid transparent;
    cursor: pointer;
    transition: all 0.2s ease;
    background-color: #F5F7FA;
    color: #37474F;
    font-family: inherit;
    line-height: 1.5;
  }
  .tab-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0,0,0,0.08);
  }
  .tab-btn .tab-title {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    font-size: 12.5pt;
    font-weight: bold;
    margin-bottom: 4px;
  }
  .tab-btn .tab-words {
    font-size: 9.5pt;
    font-weight: normal;
    opacity: 0.9;
  }
  .tab-btn .tab-meta {
    font-size: 9.8pt;
    display: block;
  }
  .tab-btn .tab-focus {
    font-size: 9pt;
    display: block;
    margin-top: 2px;
    opacity: 0.92;
  }

  /* 各分頁啟用狀態 */
  .tab-btn[data-tab="basic"] { border-color: #C8E6C9; }
  .tab-btn[data-tab="basic"].active {
    background-color: var(--basic);
    border-color: var(--basic);
    color: #FFFFFF;
    box-shadow: 0 4px 14px rgba(46, 125, 50, 0.28);
  }

  .tab-btn[data-tab="inter"] { border-color: #BBDEFB; }
  .tab-btn[data-tab="inter"].active {
    background-color: var(--inter);
    border-color: var(--inter);
    color: #FFFFFF;
    box-shadow: 0 4px 14px rgba(21, 101, 192, 0.28);
  }

  .tab-btn[data-tab="adv"] { border-color: #E1BEE7; }
  .tab-btn[data-tab="adv"].active {
    background-color: var(--adv);
    border-color: var(--adv);
    color: #FFFFFF;
    box-shadow: 0 4px 14px rgba(106, 27, 154, 0.28);
  }

  /* 分頁內容區塊 */
  .tab-panel {
    display: none;
    animation: fadeIn 0.2s ease;
  }
  .tab-panel.active {
    display: block;
  }
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(4px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .version-banner {
    color: #FFFFFF;
    padding: 10px 16px;
    border-radius: 8px;
    font-size: 13pt;
    font-weight: bold;
    margin-bottom: 16px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 8px;
  }
  .version-banner span {
    font-size: 10.5pt;
    font-weight: normal;
  }
  .theme-basic .version-banner { background-color: var(--basic); }
  .theme-inter .version-banner { background-color: var(--inter); }
  .theme-adv   .version-banner { background-color: var(--adv); }

  .section-title {
    font-size: 11.5pt;
    margin: 18px 0 8px 0;
    font-weight: bold;
  }
  .theme-basic .section-title { color: var(--basic); }
  .theme-inter .section-title { color: var(--inter); }
  .theme-adv   .section-title { color: var(--adv); }

  /* 表格樣式 */
  .table-wrap {
    width: 100%;
    overflow-x: auto;
    margin-bottom: 20px;
  }
  table {
    width: 100%;
    border-collapse: collapse;
    font-size: 10.5pt;
    min-width: 600px;
  }
  th {
    color: #FFFFFF;
    font-weight: bold;
    padding: 9px 11px;
    border: 1px solid var(--border);
    text-align: left;
    vertical-align: middle;
  }
  .theme-basic th { background-color: var(--basic); }
  .theme-inter th { background-color: var(--inter); }
  .theme-adv   th { background-color: var(--adv); }

  td {
    padding: 9px 11px;
    border: 1px solid var(--border);
    vertical-align: top;
    line-height: 1.6;
  }
  tbody tr:nth-child(odd) td { background-color: #FFFFFF; }
  tbody tr:nth-child(even) td { background-color: var(--zebra); }
  tbody tr td:first-child {
    font-weight: bold;
    color: #263238;
  }

  .theme-basic .fill { color: var(--basic); font-weight: bold; }
  .theme-inter .fill { color: var(--inter); font-weight: bold; }
  .theme-adv   .fill { color: var(--adv); font-weight: bold; }

  @media (max-width: 720px) {
    .tab-bar { grid-template-columns: 1fr; }
  }
  @media print {
    body { max-width: 100%; padding: 0; }
    .tab-bar { display: none; }
    .tab-panel { display: block !important; page-break-after: always; }
    .tab-panel:last-child { page-break-after: auto; }
  }
</style>
</head>
<body>

<header class="doc-header">
  <h1>學測英文作文模板</h1>
  <h2>第一段：兩圖比較＋第二段：我的看法與經驗</h2>
  <p>題目來源：114 學測（颱風假）｜點擊下方分頁切換不同難度版本</p>
</header>

<!-- 如需顯示原題圖片，可將原檔中的 <img src="data:image/png;base64,..." ...> 貼在下方 div 內 -->
<div class="prompt-img-wrap">
  <!-- 在此貼上原題圖片 <img> 標籤 -->
</div>

<!-- 三版本切換分頁列 -->
<nav class="tab-bar" role="tablist" aria-label="作文模板難度分頁">
  <button class="tab-btn active" role="tab" aria-selected="true" data-tab="basic">
    <div class="tab-title">簡易版 <span class="tab-words">約 150 字</span></div>
    <span class="tab-meta">5–8 級分（作文約 8–11 分）</span>
    <span class="tab-focus">重點：寫對、寫完、不離題</span>
  </button>

  <button class="tab-btn" role="tab" aria-selected="false" data-tab="inter">
    <div class="tab-title">一般版 <span class="tab-words">約 220–230 字</span></div>
    <span class="tab-meta">9–12 級分（作文約 12–15 分）</span>
    <span class="tab-focus">重點：分詞片語、細節延伸、轉折自然</span>
  </button>

  <button class="tab-btn" role="tab" aria-selected="false" data-tab="adv">
    <div class="tab-title">高級版 <span class="tab-words">約 250 字</span></div>
    <span class="tab-meta">13–15 級分（作文約 16–19 分）</span>
    <span class="tab-focus">重點：高階句型、精準詞彙、思辨深度</span>
  </button>
</nav>

<!-- ==================== 分頁一：簡易版 ==================== -->
<section id="panel-basic" class="tab-panel theme-basic active" role="tabpanel">
  <div class="version-banner">
    <div>版本一：簡易版（5–8 級分）</div>
    <span>作文約 8–11 分｜約 150 字</span>
  </div>

  <h3 class="section-title">結構拆解：通用句＋本題範例</h3>
  <div class="table-wrap">
    <table>
      <thead>
        <tr>
          <th width="20%">結構</th>
          <th width="38%">通用句（空格只填關鍵字）</th>
          <th width="42%">範例（粗體＝填入）</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>第一段｜開頭：背景介紹</td>
          <td>Nowadays, people have different ways of ________（主題／V-ing）.</td>
          <td>Nowadays, people have different ways of <span class="fill">spending a typhoon day</span>.</td>
        </tr>
        <tr>
          <td>第一段｜主題句：兩圖描述什麼</td>
          <td>These pictures show two of them.</td>
          <td>These pictures show two of them.</td>
        </tr>
        <tr>
          <td>第一段｜論點：描寫圖 A</td>
          <td>In Picture A, ________.</td>
          <td>In Picture A, <span class="fill">a lot of people are waiting in line at a busy food counter</span>.</td>
        </tr>
        <tr>
          <td>第一段｜論點：描寫圖 B</td>
          <td>In Picture B, ________.</td>
          <td>In Picture B, <span class="fill">some people are riding scooters in heavy rain</span>.</td>
        </tr>
        <tr>
          <td>第一段｜結論</td>
          <td>The main difference is that Picture A looks ________（adj.）, while Picture B looks ________（adj.）.</td>
          <td>The main difference is that Picture A looks <span class="fill">relaxed and crowded</span>, while Picture B looks <span class="fill">dangerous</span>.</td>
        </tr>
        <tr>
          <td>第二段｜開頭：表明立場</td>
          <td>（觀點題）In my opinion, ________.<br>（二選一題）If I had to choose, I would choose Picture A／B.</td>
          <td>In my opinion, <span class="fill">a typhoon day off is necessary for our safety</span>.</td>
        </tr>
        <tr>
          <td>第二段｜主題句</td>
          <td>I have two reasons for this.</td>
          <td>I have two reasons for this.</td>
        </tr>
        <tr>
          <td>第二段｜論點：理由一＋解釋</td>
          <td>First, ________.<br>This is because ________.</td>
          <td>First, <span class="fill">a day off keeps us away from danger</span>.<br>This is because <span class="fill">strong winds and heavy rain can hurt people on the road</span>.</td>
        </tr>
        <tr>
          <td>第二段｜論點：理由二</td>
          <td>Second, ________.</td>
          <td>Second, <span class="fill">we can spend more time with our family</span>.</td>
        </tr>
        <tr>
          <td>第二段｜論點：舉例／經驗</td>
          <td>For example, ________.<br>I felt ________.</td>
          <td>For example, <span class="fill">last year my school closed during a typhoon, and I stayed home with my family</span>.<br>I felt <span class="fill">safe and warm</span>.</td>
        </tr>
        <tr>
          <td>第二段｜結論：重申立場</td>
          <td>In conclusion, ________.</td>
          <td>In conclusion, <span class="fill">a typhoon day off protects us and gives us a chance to rest</span>.</td>
        </tr>
      </tbody>
    </table>
  </div>

  <h3 class="section-title">更多寫法與搭配用字</h3>
  <div class="table-wrap">
    <table>
      <thead>
        <tr>
          <th width="20%">結構</th>
          <th width="48%">其他通用句（可替換）</th>
          <th width="32%">常用搭配</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>第一段｜開頭：背景介紹</td>
          <td>① Nowadays, there are many different ways to ________（V）.<br>② ________ is common in our daily life.</td>
          <td>many different ＋ kinds of／ways to／choices of；nowadays, these days</td>
        </tr>
        <tr>
          <td>第一段｜主題句：兩圖描述什麼</td>
          <td>① The two pictures show two different ________.<br>② Here are two pictures about ________.</td>
          <td>show／be about；two different ＋ 名詞；clear differences</td>
        </tr>
        <tr>
          <td>第一段｜怎麼描寫圖片</td>
          <td>位置：On the left, ________. On the right, ________. ｜ In the front, ________. In the back, ________.<br>人物：There are ________（N）________（V-ing／p.p.）in Picture A.<br>They look／seem ________.</td>
          <td>動作：listen to, look at, take notes, take photos, talk with, laugh, wait in line<br>形容詞：quiet, noisy, serious, relaxed, excited, curious, tired</td>
        </tr>
        <tr>
          <td>第一段｜結論</td>
          <td>① Picture A is more ________ than Picture B.（注意：單音節形容詞用 -er，如 safer）<br>② Unlike Picture A, Picture B is ________.<br>③ The two pictures are different in ________.</td>
          <td>more ＋ 形容詞 ＋ than；unlike；while；different in mood／purpose</td>
        </tr>
        <tr>
          <td>第二段｜表明立場</td>
          <td>① I think ________ is a good idea.<br>② I like ________ because it is ________.<br>③ If I had to choose, I would choose Picture ________.<br>④ I like Picture ________ better than Picture ________.</td>
          <td>useful, helpful, interesting, fun, safe, important；a good way to</td>
        </tr>
        <tr>
          <td>第二段｜主題句</td>
          <td>① There are two reasons why I think so.<br>② Here are my reasons.<br>③ I have two reasons to support my idea.</td>
          <td>reason；support；why I think so</td>
        </tr>
        <tr>
          <td>第二段｜闡述論點</td>
          <td>理由：First, ________. ｜ Second, ________. ｜ Besides, ________. ｜ Finally, ________.<br>解釋：This is because ________.<br>舉例：For example, ________.<br>經驗：Last year, I ________. I felt ________.</td>
          <td>萬用：stay safe, save time, spend time with family, relax, feel happy<br>校園：learn new things, make friends, get closer to classmates, have fun, take a break from school</td>
        </tr>
        <tr>
          <td>第二段｜結論</td>
          <td>① To sum up, ________.<br>② That is why I think ________.<br>③ In conclusion, ________.</td>
          <td>in conclusion, to sum up, overall</td>
        </tr>
      </tbody>
    </table>
  </div>

  <h3 class="section-title">轉折詞</h3>
  <div class="table-wrap">
    <table>
      <thead>
        <tr>
          <th width="20%">功能</th>
          <th width="80%">用字</th>
        </tr>
      </thead>
      <tbody>
        <tr><td>對比</td><td>but, however, while, on the other hand, unlike；相同：both, too</td></tr>
        <tr><td>補充</td><td>and, also, too, besides</td></tr>
        <tr><td>原因／結果</td><td>because, so, that is why</td></tr>
        <tr><td>順序</td><td>first, second, then, finally, last</td></tr>
        <tr><td>舉例</td><td>for example, such as</td></tr>
        <tr><td>結論</td><td>in conclusion, to sum up, overall, all in all</td></tr>
      </tbody>
    </table>
  </div>
</section>

<!-- ==================== 分頁二：一般版 ==================== -->
<section id="panel-inter" class="tab-panel theme-inter" role="tabpanel">
  <div class="version-banner">
    <div>版本二：一般版（9–12 級分）</div>
    <span>作文約 12–15 分｜約 220–230 字</span>
  </div>

  <h3 class="section-title">結構拆解：通用句＋本題範例</h3>
  <div class="table-wrap">
    <table>
      <thead>
        <tr>
          <th width="20%">結構</th>
          <th width="38%">通用句（空格只填關鍵字）</th>
          <th width="42%">範例（粗體＝填入）</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>第一段｜開頭：背景介紹</td>
          <td>Nowadays, ________（主題）is closely related to our daily life.</td>
          <td>Nowadays, <span class="fill">a typhoon day off</span> is closely related to our daily life.</td>
        </tr>
        <tr>
          <td>第一段｜主題句：兩圖描述什麼</td>
          <td>The two pictures illustrate two different ways of responding to it, and they differ in several respects.</td>
          <td>The two pictures illustrate two different ways of responding to it, and they differ in several respects.</td>
        </tr>
        <tr>
          <td>第一段｜論點：描寫圖 A</td>
          <td>Picture A shows ________.</td>
          <td>Picture A shows <span class="fill">a large crowd lining up at a busy food counter, as if the weather outside did not matter</span>.</td>
        </tr>
        <tr>
          <td>第一段｜論點：描寫圖 B</td>
          <td>By contrast, Picture B depicts ________.</td>
          <td>By contrast, Picture B depicts <span class="fill">several scooter riders moving slowly through the heavy rain on a city street</span>.</td>
        </tr>
        <tr>
          <td>第一段｜結論</td>
          <td>While the people in Picture A seem to ________, those in Picture B appear to ________.<br>（非人物圖改為：While Picture A focuses on ________, Picture B shows ________.）<br>Clearly, the key difference lies in ________.</td>
          <td>While <span class="fill">the people</span> in Picture A seem to <span class="fill">enjoy a relaxing day indoors</span>, <span class="fill">those</span> in Picture B appear to <span class="fill">struggle through the storm for work or errands</span>. Clearly, the key difference lies in <span class="fill">whether people are staying safe or taking risks</span>.</td>
        </tr>
        <tr>
          <td>第二段｜開頭：表明立場</td>
          <td>（觀點題）Personally, I believe that ________.<br>（二選一題）From my perspective, I would choose Picture A／B.</td>
          <td>Personally, I believe that <span class="fill">a typhoon day off is a wise decision to protect public safety</span>.</td>
        </tr>
        <tr>
          <td>第二段｜主題句</td>
          <td>There are several reasons why I hold this view.</td>
          <td>There are several reasons why I hold this view.</td>
        </tr>
        <tr>
          <td>第二段｜論點：理由一＋解釋＋舉例</td>
          <td>To begin with, ________.<br>This is because ________.<br>For example, ________.</td>
          <td>To begin with, <span class="fill">staying home keeps us out of harm’s way</span>.<br>This is because <span class="fill">strong winds and heavy rain make roads dangerous</span>.<br>For example, <span class="fill">many accidents happen when people ride scooters in a storm</span>.</td>
        </tr>
        <tr>
          <td>第二段｜論點：理由二＋經驗</td>
          <td>What is more, ________.<br>I still remember that ________.<br>That experience taught me that ________.</td>
          <td>What is more, <span class="fill">a day off gives families precious time together</span>.<br>I still remember that <span class="fill">last summer, a typhoon closed our school and I spent the whole day cooking with my parents</span>.<br>That experience taught me that <span class="fill">safety and family time are worth more than a normal school day</span>.</td>
        </tr>
        <tr>
          <td>第二段｜結論：重申立場</td>
          <td>All in all, ________.</td>
          <td>All in all, <span class="fill">typhoon days off protect our safety and bring families closer</span>.</td>
        </tr>
      </tbody>
    </table>
  </div>

  <h3 class="section-title">更多寫法與搭配用字</h3>
  <div class="table-wrap">
    <table>
      <thead>
        <tr>
          <th width="20%">結構</th>
          <th width="48%">其他通用句（可替換）</th>
          <th width="32%">常用搭配</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>第一段｜開頭：背景介紹</td>
          <td>① These days, ________ plays an increasingly important role in our lives.<br>② ________ has attracted growing attention, and people react to it in different ways.<br>③ Whether it is ________ or ________, people have many options.</td>
          <td>become more and more popular／common；play an important role；attract growing attention；have many options</td>
        </tr>
        <tr>
          <td>第一段｜主題句：兩圖描述什麼</td>
          <td>① The two pictures illustrate two different ways of ________.<br>② The two pictures present two of these options, yet they differ greatly in ________.<br>③ A careful comparison shows that they have little in common.</td>
          <td>illustrate／present／depict；differ in；in several respects；have little in common</td>
        </tr>
        <tr>
          <td>第一段｜怎麼描寫圖片</td>
          <td>位置：On the left／right of Picture A, ________.<br>In the foreground, ________, while in the background, ________.<br>人物動作：Picture A depicts ________. What catches my eye is ________.<br>氣氛：They look／appear ________, creating a ________ atmosphere.</td>
          <td>分詞片語：each doing …, surrounded by …<br>氣氛：lively, peaceful, relaxed, serious, cheerful<br>be absorbed in, be gathered, be engaged in</td>
        </tr>
        <tr>
          <td>第一段｜結論</td>
          <td>① Whereas the people in Picture A ________, those in Picture B ________.<br>② In short, Picture A is about ________, whereas Picture B is about ________.<br>③ The key difference between the two pictures lies in ________.</td>
          <td>the key difference lies in；while／whereas；appear to</td>
        </tr>
        <tr>
          <td>第二段｜表明立場</td>
          <td>① In my view, ________.<br>② I am in favor of ________.<br>③ If I had to choose, I would choose Picture ________ because ________.<br>④ I prefer Picture ________ to Picture ________.</td>
          <td>well worth, beneficial, rewarding, essential；personally, in my view</td>
        </tr>
        <tr>
          <td>第二段｜主題句</td>
          <td>① I support this idea for the following reasons.<br>② My view is based on both logic and experience.</td>
          <td>for the following reasons；be based on</td>
        </tr>
        <tr>
          <td>第二段｜闡述論點</td>
          <td>理由：To begin with, ________. In addition, ________. Finally, ________.<br>解釋：This is because ________. ｜ That is to say, ________.<br>舉例：For example, ________. ｜ Take ________ as an example.<br>經驗：I still remember that ________. ｜ This experience showed me that ________.</td>
          <td>萬用：protect public safety, relieve stress, strengthen family bonds, save time and effort<br>校園／成長：broaden our horizons, build teamwork, strengthen friendships, learn by doing</td>
        </tr>
        <tr>
          <td>第二段｜結論</td>
          <td>① In short, ________.<br>② For the reasons mentioned above, ________.<br>③ To sum up, ________.</td>
          <td>all in all, in short, for these reasons, to sum up</td>
        </tr>
      </tbody>
    </table>
  </div>

  <h3 class="section-title">轉折詞</h3>
  <div class="table-wrap">
    <table>
      <thead>
        <tr>
          <th width="20%">功能</th>
          <th width="80%">用字</th>
        </tr>
      </thead>
      <tbody>
        <tr><td>對比</td><td>while, whereas, by contrast, on the other hand, in contrast to (+ N/V-ing), unlike, however</td></tr>
        <tr><td>補充</td><td>what is more, moreover, besides, in addition, not only … but also</td></tr>
        <tr><td>因果</td><td>as a result, therefore, because of (+ N/V-ing), thanks to (+ N/V-ing), that is why</td></tr>
        <tr><td>舉例</td><td>for example, for instance, take … as an example, such as</td></tr>
        <tr><td>讓步</td><td>although, even though, despite (+ N/V-ing), still</td></tr>
        <tr><td>結論</td><td>all in all, in short, in conclusion, to sum up</td></tr>
      </tbody>
    </table>
  </div>
</section>

<!-- ==================== 分頁三：高級版 ==================== -->
<section id="panel-adv" class="tab-panel theme-adv" role="tabpanel">
  <div class="version-banner">
    <div>版本三：高級版（13–15 級分）</div>
    <span>作文約 16–19 分｜約 250 字</span>
  </div>

  <h3 class="section-title">結構拆解：通用句＋本題範例</h3>
  <div class="table-wrap">
    <table>
      <thead>
        <tr>
          <th width="20%">結構</th>
          <th width="38%">通用句（空格只填關鍵字）</th>
          <th width="42%">範例（粗體＝填入）</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>第一段｜開頭：背景介紹</td>
          <td>In today’s society, ________ has gained growing attention.</td>
          <td>In today’s society, <span class="fill">the practice of suspending work and classes whenever a typhoon approaches</span> has gained growing attention.</td>
        </tr>
        <tr>
          <td>第一段｜主題句：兩圖描述什麼</td>
          <td>The two pictures present two contrasting responses to it.</td>
          <td>The two pictures present two contrasting responses to it.</td>
        </tr>
        <tr>
          <td>第一段｜論點：描寫圖 A</td>
          <td>Picture A captures ________.</td>
          <td>Picture A captures <span class="fill">a crowd of people waiting in a long line at a busy food counter, chatting and checking their phones as if nothing unusual were happening</span>.</td>
        </tr>
        <tr>
          <td>第一段｜論點：描寫圖 B</td>
          <td>Picture B, on the other hand, depicts ________.</td>
          <td>Picture B, on the other hand, depicts <span class="fill">several scooter riders in raincoats and masks pushing through a torrential downpour while cars crawl past beside them</span>.</td>
        </tr>
        <tr>
          <td>第一段｜論點：對照</td>
          <td>Whereas Picture A emphasizes ________, Picture B highlights ________.</td>
          <td>Whereas Picture A emphasizes <span class="fill">leisure, comfort, and convenience</span>, Picture B highlights <span class="fill">risk, effort, and necessity</span>.</td>
        </tr>
        <tr>
          <td>第一段｜結論</td>
          <td>In short, what distinguishes the two scenes is not merely ________ but also ________.</td>
          <td>In short, what distinguishes the two scenes is not merely <span class="fill">the location</span> but also <span class="fill">the attitude toward safety and responsibility</span>.</td>
        </tr>
        <tr>
          <td>第二段｜開頭：表明立場</td>
          <td>（觀點題）Having thought it over, I firmly believe that ________.<br>（二選一題）Having weighed both options, I would opt for Picture A／B.</td>
          <td>Having thought it over, I firmly believe that <span class="fill">a typhoon day off is a necessary measure to protect lives rather than a free holiday for fun</span>.</td>
        </tr>
        <tr>
          <td>第二段｜主題句</td>
          <td>Several reasons lie behind this belief.</td>
          <td>Several reasons lie behind this belief.</td>
        </tr>
        <tr>
          <td>第二段｜論點：理由一＋解釋</td>
          <td>First and foremost, ________.<br>This is largely because ________.</td>
          <td>First and foremost, <span class="fill">it protects lives by keeping people off dangerous roads</span>.<br>This is largely because <span class="fill">strong winds, flooding, and falling objects pose real threats to everyone, especially commuters on scooters</span>.</td>
        </tr>
        <tr>
          <td>第二段｜論點：理由二＋經驗</td>
          <td>Furthermore, not only does it ________, but it also ________.<br>A case in point is my own experience: ________.</td>
          <td>Furthermore, not only does it <span class="fill">prevent unnecessary risks</span>, but it also <span class="fill">gives families a rare chance to slow down and reconnect</span>.<br>A case in point is my own experience: <span class="fill">last year, when classes were canceled, my family cooked hotpot together and talked for hours</span>.</td>
        </tr>
        <tr>
          <td>第二段｜結論：重申立場</td>
          <td>All things considered, ________, and that is precisely why ________.</td>
          <td>All things considered, <span class="fill">staying indoors when a typhoon strikes protects both our safety and our family bonds</span>, and that is precisely why <span class="fill">I fully support a typhoon day off</span>.</td>
        </tr>
      </tbody>
    </table>
  </div>

  <h3 class="section-title">更多寫法與搭配用字</h3>
  <div class="table-wrap">
    <table>
      <thead>
        <tr>
          <th width="20%">結構</th>
          <th width="48%">其他通用句（可替換）</th>
          <th width="32%">常用搭配</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>第一段｜開頭：背景介紹</td>
          <td>① With the rise of ________, people have developed very different ways of responding to it.<br>② ________ is no longer a simple matter, as people hold contrasting views on it.<br>③ ________ has sparked heated debate, and opinions on how to handle it differ greatly.</td>
          <td>gain growing attention；vary widely；with the rise of；hold contrasting views；spark heated debate</td>
        </tr>
        <tr>
          <td>第一段｜主題句：兩圖描述什麼</td>
          <td>① Although both pictures revolve around it, they tell two very different stories.<br>② What sets the two scenes apart is ________.</td>
          <td>revolve around；set apart；convey／illustrate／embody；contrasting</td>
        </tr>
        <tr>
          <td>第一段｜怎麼描寫圖片</td>
          <td>In the foreground, ________, while in the background, ________. Off to the left／right, ________.<br>At the center of the scene is ________.</td>
          <td>capture, portray, depict, bring out<br>absorbed in, immersed in, gathered around, posing for<br>focused, relaxed, cheerful, solemn；emphasize, highlight, stress</td>
        </tr>
        <tr>
          <td>第一段｜結論</td>
          <td>① Ultimately, the contrast boils down to ________.<br>② Put simply, one scene is about ________, while the other is about ________.<br>③ What truly separates them is ________.</td>
          <td>not merely … but also；boil down to；put simply；what truly separates them</td>
        </tr>
        <tr>
          <td>第二段｜表明立場</td>
          <td>① Although opinions may differ, I am convinced that ________.<br>② It is my belief that ________.<br>③ I hold the view that ________.<br>④ If I had to choose, I would opt for Picture ________, and the reasons are as follows.</td>
          <td>firmly believe, be convinced that, hold the view that, opt for</td>
        </tr>
        <tr>
          <td>第二段｜主題句</td>
          <td>① My conviction rests on both logic and personal experience.<br>② I would like to explain why I hold this view.</td>
          <td>lie behind, rest on, be rooted in</td>
        </tr>
        <tr>
          <td>第二段｜闡述論點</td>
          <td>理由：First and foremost, ________. Furthermore, ________. Last but not least, ________.<br>讓步反駁：Admittedly, some may argue that ________; nevertheless, ________.<br>解釋：This is largely because ________. ｜ In other words, ________.<br>舉例：A case in point is ________. ｜ To illustrate, ________.</td>
          <td>萬用：pose a threat to, strike a balance between, foster a sense of responsibility, cherish precious moments<br>校園／成長：broaden horizons, nourish the mind, foster teamwork, turn theory into practice, leave a lasting impression</td>
        </tr>
        <tr>
          <td>第二段｜結論</td>
          <td>① Without a doubt, ________.<br>②（假設／二選一題）Were I given the chance to ________, I would ________.<br>③ Only by ________（V-ing）can we ________.</td>
          <td>all things considered, in the final analysis, without a doubt, were I to …, only by … can we …</td>
        </tr>
      </tbody>
    </table>
  </div>

  <h3 class="section-title">轉折詞</h3>
  <div class="table-wrap">
    <table>
      <thead>
        <tr>
          <th width="20%">功能</th>
          <th width="80%">用字</th>
        </tr>
      </thead>
      <tbody>
        <tr><td>對比</td><td>whereas, in contrast, by contrast, conversely</td></tr>
        <tr><td>補充</td><td>furthermore, moreover, in addition to (+ N/V-ing), not merely … but also</td></tr>
        <tr><td>因果</td><td>consequently, as a consequence, owing to (+ N/V-ing), give rise to, lead to</td></tr>
        <tr><td>舉例</td><td>a case in point, for instance, to illustrate, take … for example</td></tr>
        <tr><td>讓步</td><td>admittedly, granted that, despite (+ N/V-ing), albeit, even so, nonetheless, nevertheless</td></tr>
        <tr><td>結論</td><td>all things considered, in the final analysis, ultimately, on the whole</td></tr>
      </tbody>
    </table>
  </div>
</section>

<script>
  const tabs = document.querySelectorAll('.tab-btn');
  const panels = document.querySelectorAll('.tab-panel');

  function activateTab(tabName) {
    tabs.forEach(btn => {
      const isActive = btn.dataset.tab === tabName;
      btn.classList.toggle('active', isActive);
      btn.setAttribute('aria-selected', isActive ? 'true' : 'false');
    });
    panels.forEach(panel => {
      panel.classList.toggle('active', panel.id === 'panel-' + tabName);
    });
  }

  tabs.forEach(btn => {
    btn.addEventListener('click', () => activateTab(btn.dataset.tab));
  });
</script>
<footer>
    <p>&copy; 2026 @Maxine</p>
</footer>
</body>
</html>
