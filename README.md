
<p>初賽的相關規則如下：</p>
<ol>
    <li>預測結果每日提交上限 2 次。</li>
    <li>提交預測結果之內容格式需符合比賽規定(請參閱 <a href="javascript:;" onclick="handle_partialDownloadDatasetLinkClick()">Dataset Download 區</a>之文件)。</li>
    <li>請於期限內繳交賽後文件，若逾期繳交視同放棄進入決賽之資格。</li>
    <li>務必使用Machine Learning來進行辨識與分類，禁止使用任何人工標記。</li>
    <li>禁止使用非開源 Auto Machine Learning 相關之服務 (MLOps服務除外)。</li>
    <li>禁止使用非開源 Machine Learning Classification/Labeling 相關之服務 (例如:Cognitive Services)。</li>
    <li>不可私下共享程式及特徵值，但可在官方<a href="https://tbrain.trendmicro.com.tw/Discussion/Forum/15">討論區</a>公開討論。</li>
    <li>資料集僅限於此次比賽使用，參賽者不得為自己或他人利益而洩漏或交付資料集予非參賽者。</li>
    <li>參賽隊伍可以使用自行製作之資料，或額外之開源資源來增進模型訓練結果，惟務必使用Machine Learning來進行(測試資料集)辨識與分類，禁止使用任何人工標記。若有使用額外之開源資料，須於比賽結束繳交之書面報告文件中提供相關來源；若有使用自行製作之資料，需於比賽結束後提供該資料內容，以利進行審核。如有爭議，主辦單位保有最終決定權。</li>
    <li>如有需要，主辦單位有權在比賽途中調整資料集。</li>
    <li>如有下列情事，主辦單位得無需告知參賽者，逕行取消參賽者資格或領獎資格：</li>
    <ul>
        <li>已有具體事證，所屬隊伍有任何抄襲、作弊、或詐欺等行為</li>
        <li>已有具體事證，所屬隊伍有侵害他人智慧財產權之情事</li>
        <li>已有具體事證，所屬隊伍有對Leaderboard系統進行攻擊</li>
        <li>已有具體事證，所屬隊伍影響其他參賽隊伍導致不公平事例發生</li>
        <li>已有具體事證，所屬隊伍違反本比賽活動辦法、或「T-Brain AI實戰吧平台服務」 使用條款、或「Tomofun 狗音辨識 AI 百萬挑戰賽」參賽者使用條款</li>
    </ul>
    <li>主辦單位保有對活動與競賽規則解釋及裁決的權利。</li>
</ol>
<p>&nbsp;</p>
<h4 style="font-weight:normal">決賽進行與規則</h4>
<p>決賽的進行方式如下：</p>
<ol>
    <li>進入決賽之隊伍，主辦方會提供比賽專用 email 與 AWS 帳號 (包含免費使用額度，參賽者若於額度內使用便不會進行扣款) 作為決賽使用。並於決賽結束後一個月回收此比賽專用 email (參賽者可自行修改 AWS 帳號的 email 設定以繼續使用此 AWS 帳號)。</li>
    <li>進入決賽之隊伍，需於 2021/07/03 參加 AWS 線上 Workshop，了解如何操作決賽時將會使用的 AWS 相關服務。</li>
    <li>主辦單位將於決賽前 3 天開始透過 endpoint API 打資料，參賽隊伍可利用此 API 測試是否正常運作。</li>
    <li>參賽隊伍於競賽當日報到後，現場將有 tutorial 和競賽說明，並於說明結束後開始進行 6 小時的比賽。</li>
    <li>比賽過程將模擬 AI 服務落地的實作，主辦單位會發送 HTTP request (POST 方法) 送出音檔（wav檔），以每 2 秒送出一筆音檔的速度進行比賽，參賽隊伍需事先利用 AWS 提供之服務建立好 pipeline 並即時送出模型預測結果 (建議使用 AWS SageMaker 實作，若使用其他做法，僅能使用 AWS 所提供之服務)。</li>
    <li>為了模擬 MLOps 之運行，參賽者可使用 AWS GroudTruth 來標記收到的資料，即時重新訓練模型，以提供更好的 AI 服務。</li>
    <li>比賽計分方式以最後 2 小時之 3600 筆資料作為算分依據，按照分數高低進行排名。</li>
    <li>進入前五名之隊伍需上台分享實作內容，可至 <a href="javascript:;" onclick="handle_partialDownloadDatasetLinkClick()">Dataset Download </a> 區下載 PPT 範本。 並由評審選出一組隊伍獲得評審獎。</li>
</ol>
<p>決賽的相關規則如下：</p>
<ol>
    <li>最後兩小時之 3600 筆資料之算分以當下模型預測之結果為主，不接受事後補上預測結果。</li>
    <li>timeout 時間為 3 秒，若參賽者 API Server 沒有回應，主辦單位會重新呼叫，最多呼叫 2 次，若皆無回應或是逾時則此題以 0 分計算。</li>
    <li>務必使用Machine Learning來進行辨識與分類。</li>
    <li>禁止使用非開源 Auto Machine Learning 相關之服務 (MLOps服務除外)。</li>
    <li>禁止使用非開源 Machine Learning Classification/Labeling 相關之服務 (例如:Cognitive Services)。</li>
    <li>不可私下共享程式及特徵值，但可在官方<a href="https://tbrain.trendmicro.com.tw/Discussion/Forum/15">討論區</a>公開討論。</li>
    <li>資料集僅限於此次比賽使用，參賽者不得為自己或他人利益而洩漏或交付資料集予非參賽者。</li>
    <li>參賽隊伍可以使用自行製作之資料，或額外之開源資源來增進模型訓練結果，惟務必使用Machine Learning來進行(測試資料集)辨識與分類，禁止使用任何人工標記。若有使用額外之開源資料，須於比賽結束繳交之書面報告文件中提供相關來源；若有使用自行製作之資料，需於比賽結束後提供該資料內容，以利進行審核。如有爭議，主辦單位保有最終決定權。</li>
    <li>如有需要，主辦單位有權在比賽途中調整資料集。</li>
    <li>如有下列情事，主辦單位得無需告知參賽者，逕行取消參賽者資格或領獎資格：</li>
    <ul>
        <li>已有具體事證，所屬隊伍有任何抄襲、作弊、或詐欺等行為</li>
        <li>已有具體事證，所屬隊伍有侵害他人智慧財產權之情事</li>
        <li>已有具體事證，所屬隊伍影響其他參賽隊伍導致不公平事例發生</li>
        <li>已有具體事證，所屬隊伍違反本比賽活動辦法、或「Tomofun 狗音辨識 AI 百萬挑戰賽」參賽者使用條款</li>
    </ul>
    <li>主辦單位保有活動變動、競賽規則解釋及裁決之權利。若因應政府防疫規定或其他不可抗力之因素，須取消活動或調整活動內容，主辦單位得以參賽者報名時所提供之聯絡方式，提前通知相關活動變動之訊息，並同時公告於本報名頁面。</li>
</ol></p>
        <hr class="mt-5 mb-4" />
        <h3 class="mb-2"><h3 style="color:#002339;">獎項說明</h3></h3>
        <p>
            <ul class="list-group">
                    <li class="list-group-item prize-first-bg d-flex justify-content-between align-items-center">
                        <span class="badge prize-first-label badge-pill prize-badge">第一名</span>
                        <strong style="width:100%;margin-left:20px">
                                <span>新台幣</span> 15 <span>萬元</span>
                            + 獎狀一只 + AWS 獨家獎品
                        </strong>
                    </li>
                    <li class="list-group-item prize-bg d-flex justify-content-between align-items-center">
                        <span class="badge badge-bg-2 badge-pill prize-badge">第二名</span>
                        <strong style="width:100%;margin-left:20px">
                                <span>新台幣</span> 10 <span>萬元</span>
                            + 獎狀一只 + AWS 獨家獎品
                        </strong>
                    </li>
                    <li class="list-group-item prize-bg d-flex justify-content-between align-items-center">
                        <span class="badge badge-bg-3 badge-pill prize-badge">第三名</span>
                        <strong style="width:100%;margin-left:20px">
                                <span>新台幣</span> 5 <span>萬元</span>
                            + 獎狀一只 + AWS 獨家獎品
                        </strong>
                    </li>
                    <li class="list-group-item prize-bg d-flex justify-content-between align-items-center">
                        <span class="badge badge-bg-4 badge-pill prize-badge">第四名</span>
                        <strong style="width:100%;margin-left:20px">
                                <span>新台幣</span> 3 <span>萬元</span>
                            + 獎狀一只 + AWS 獨家獎品
                        </strong>
                    </li>
                    <li class="list-group-item prize-bg d-flex justify-content-between align-items-center">
                        <span class="badge badge-bg-5 badge-pill prize-badge">第五名</span>
                        <strong style="width:100%;margin-left:20px">
                                <span>新台幣</span> 2 <span>萬元</span>
                            + 獎狀一只 + AWS 獨家獎品
                        </strong>
                    </li>
                    <li class="list-group-item prize-bg d-flex justify-content-between align-items-center">
                        <span class="badge badge-bg-6 badge-pill prize-badge">評審獎</span>
                        <strong style="width:100%;margin-left:20px">
                                <span>新台幣</span> 5 <span>萬元</span>
                            + 獎狀一只 + AWS 獨家獎品
                        </strong>
                    </li>
                    <li class="list-group-item prize-bg d-flex justify-content-between align-items-center">
                        <span class="badge badge-bg-7 badge-pill prize-badge">晉級獎</span>
                        <strong style="width:100%;margin-left:20px">
                                <span>新台幣</span> 60 <span>萬元</span>
                            晉級決賽之參賽者每人贈送一台 Furbo，每台價值新台幣 6 千元
                        </strong>
                    </li>
            </ul>
            <span id="winnerlist"><ul><li>參賽者需至決賽現場才有資格領取一台 Furbo 與參賽證明</li><li>總獎項之價值包含贈送晉級決賽之參賽者獎品 Furbo、與各得獎隊伍之獎金</li><li>正式獎狀預計於賽後寄送，得獎隊伍需配合主辦單位提供獎狀之寄送地址</li></ul></span>
<table style="height:678px;">
    <thead>
        <tr>
            <th bgcolor="yellow" width="20%" data-role="resizable">時程</th>
            <th width="30%" bgcolor="yellow" data-role="resizable">項目</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td data-title="時程">2021/05/10 12:00 - 2021/06/02 12:00</td>
            <td data-title="說明">開放報名</td>
        </tr>
        <tr>
            <td data-title="時程">2021/05/10 12:00 - 2021/06/10 12:00 </td>
            <td data-title="說明">線上初賽期間，競賽隊伍可上傳答案，評分系統將開始針對每個隊伍的答案進行評分</td>
        </tr>
        <tr>
            <td data-title="時程">2021/06/08 12:00 - 2021/06/10 12:00 </td>
            <td data-title="說明">公開私人測試集</td>
        </tr>
        <tr>
            <td data-title="時程">2021/06/11 12:00 </td>
            <td data-title="說明">公佈線上初賽之 Private Leaderboard 成績</td>
        </tr>
        <tr>
            <td data-title="時程">2021/06/14 - 2021/06/21 23:59</td>
            <td data-title="說明">繳交初賽文件</td>
        </tr>
        <tr>
            <td data-title="時程">2021/06/22 - 2021/06/28</td>
            <td data-title="說明">審核初賽繳交文件</td>
        </tr>
        <tr>
            <td data-title="時程">2021/06/30 12:00</td>
            <td data-title="說明">公告晉級決賽之隊伍</td>
        </tr>
        <tr>
            <td data-title="時程">2021/07/03 09:00 - 2021/07/03 16:30</td>
            <td data-title="說明">線上 workshop</td>
        </tr>
        <tr>
            <td data-title="時程">2021/07/17 08:30 - 2021/07/17 18:30</td>
            <td data-title="說明">黑客松現場決賽暨頒獎典禮</td>
        </tr>
    </tbody>
</table>
<p><b>線上 Workshop: Running frequent incremental training and real time serving</b></p>
<ul>
    <li>此 workshop 為 AWS 對外公開之活動</li>
    <li>Final round rules introduction 僅開放給決賽隊伍參與</li>
</ul>
<table>
    <thead>
        <tr>
            <th>時程</th>
            <th>議題</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td data-title="時程">09:00 - 12:00</td>
            <td data-title="說明">Basic elements of incremental training and serving</td>
        </tr>
        <tr>
            <td data-title="時程">12:00 - 12:30</td>
            <td data-title="說明">Q&A</td>
        </tr>
        <tr>
            <td colspan="2" align="center">中餐休息</td>
        </tr>
        <tr>
            <td data-title="時程">14:00 - 15:00</td>
            <td data-title="說明">Final round rules introduction (僅開放給決賽隊伍參與)</td>
        </tr>
        <tr>
            <td data-title="時程">15:00 - 16:00</td>
            <td data-title="說明">Automation by step function orchestration</td>
        </tr>
        <tr>
            <td data-title="時程">16:00 - 16:30</td>
            <td data-title="說明">Q&A</td>
        </tr>
    </tbody>
</table>
<p> <b>黑客松現場決賽</b> </p>
<table>
    <thead>
        <tr>
            <th>時程</th>
            <th>項目</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td data-title="時程">08:30 - 09:00</td>
            <td data-title="說明">參賽者報到與檢錄</td>
        </tr>
        <tr>
            <td data-title="時程">09:00 - 09:30</td>
            <td data-title="說明">Tomofun/AWS 致詞</td>
        </tr>
        <tr>
            <td data-title="時程">09:30 - 09:45</td>
            <td data-title="說明">評分標準說明與裁判介紹</td>
        </tr>
        <tr>
            <td data-title="時程">09:45 - 10:30</td>
            <td data-title="說明">AWS MLOps 重點與 template 介紹</td>
        </tr>
        <tr>
            <td data-title="時程">10:30 - 16:00</td>
            <td data-title="說明">Hack Time (現場供餐)</td>
        </tr>
        <tr>
            <td data-title="時程">16:00 - 16:30</td>
            <td data-title="說明">Final CountDown Hack Time</td>
        </tr>
        <tr>
            <td data-title="時程">16:30 - 17:00</td>
            <td data-title="說明">中場休息</td>
        </tr>
        <tr>
            <td data-title="時程">17:00 - 18:00</td>
            <td data-title="說明">前五名隊伍分享實作內容</td>
        </tr>
        <tr>
            <td data-title="時程">18:00 - 18:30</td>
            <td data-title="說明">中場休息/評審會議</td>
        </tr>
        <tr>
            <td data-title="時程">18:30 - 19:00</td>
            <td data-title="說明">頒獎 (包含主辦單位致詞)</td>
        </tr>
    </tbody>
</table>
<p id="ceremony">備註：以上時程皆為UTC+08:00時區。</p>
        </p>
        <hr class="mt-5 mb-4" />
        <p><h3 class="mb-2">主辦單位:Tomofun 友愉股份有限公司 </h3><div class="container-fluid"><div class="row"><div class="col-md-3" style="margin:auto;"><img width="150" src="/Content/img/upload/15/Tomofun_logo.png" alt="" align="middle" style="display:block;margin-left:auto;margin-right:auto;" /></div><div class="col-md-9"><p>Tomofun是一間國際化的寵物科技新創公司，由Victor Chang及Maggie Cheung共同成立，並由趨勢科技創辦人Steve作為Mentor，運用最先進的技術-IoT物聯網、AI人工智慧、雲端大數據等，致力於帶給全世界寵物主人源源不絕的歡樂與創新！</p><p>「Furbo狗狗攝影機」是我們推出的第一個革命性產品，讓飼主透過手機隨時隨地與狗狗遠端互動，解決當主人不在寵物身邊時的焦慮，還能進一步追蹤、分析狗狗的行為，真正實踐寵物就是家人、永遠緊緊相依的願景。 </p><p>Furbo不只在台灣受注目，更在全世界超過五十個國家熱銷，於美國、加拿大、英國及日本等全球10國亞馬遜上，連續三年都是最暢銷的狗狗攝影機，是至今最成功的寵物科技新創品牌。 </p><p>我們持續開發世界級的產品、拓展國際市場，因而決定擴大延攬擁有企圖心的研發及行銷高手，與我們一同透過創新來改變寵物與主人的生活。目前Tomofun在美國西雅圖、德國慕尼黑、日本東京、台灣台北皆設有辦公室。 </p></div></div></div><hr /><h3 class="mb-2">協辦單位：Amazon Web Services Taiwan Ltd. </h3><div class="container-fluid"><div class="row"><div class="col-md-4" style="margin:auto;"><img width="190" src="/Content/img/upload/15/PB_AWS_logo_RGB.png" alt="" align="middle" style="display:block;margin-left:auto;margin-right:auto;" /></div><div class="col-md-8"><p>15年以來，Amazon Web Services一直是世界上服務豐富、應用廣泛的雲端服務平台。AWS為客戶提供超過200種功能全面的雲端服務，包括運算、儲存、資料庫、聯網、分析、機器人、機器學習與人工智慧、物聯網、行動、安全、混合雲、虛擬和擴增實境(VR 和AR)、媒體，以及應用開發、部署和管理等方面，遍及25個地理區域內的 80個可用區域(Availability Zones)，並已公佈計畫在澳洲、印度、印尼、西班牙和瑞士建立5個AWS地理區域、15個可用區域。全球超過百萬客戶信任AWS，包含發展迅速的新創公司、大型企業和政府機構。</p><p>AWS協助客戶強化自身基礎設施，提高營運上的彈性與應變能力，同時降低成本。欲瞭解更多AWS的相關資訊，請至：aws.amazon.com</p></div></div></div><br /><hr /><h3 class="mb-2">平台贊助單位：趨勢科技</h3><div class="container-fluid"><div class="row"><div class="col-md-3"><img src="/Content/img/upload/TM_Logo_49.png" width="150" alt="" align="middle" style="display:block;margin-left:auto;margin-right:auto;" /></div><div class="col-md-9"><p>趨勢科技為資訊安全解決方案全球領導廠商，致力建立一個安全的資訊交換世界。我們專為消費者、企業及政府機構設計的創新解決方案，能為資料中心、雲端工作負載、網路、端點裝置提供多層式安全防護。我們的產品皆彼此整合、共享威脅情報，提供環環相扣的威脅防禦與集中式的掌握及調查能力，實現更好、更快的防護。趨勢科技全球共超過 6,000 名員工，遍及 50 個國家，並擁有全世界最先進的全球威脅研究及情報，是企業保護連網環境的最佳夥伴。 </p></div></div></div></p>
            
