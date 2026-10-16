# 00_Master_Index.md — 2046 聯邦正史總索引 v5.40

> **系統最高路由指令**  
> 任何正史消費、模擬、新聞、論壇或資料整理，均先讀本索引，再讀 `source/Lore_Ontology.md`，最後依主題讀取本索引指定的專檔。  
> 本索引只決定來源地位、成熟度與衝突優先序；它不取代專檔內容。

本庫依`source/`、`patch/`、`dict/`、`regulation/`、`history/`分層；路徑是定位，不是效力。`history/ptt/`原始口述與`history/legacy/`舊檔只供編輯考證，不能直接上傳為正史來源。既有主題子目錄暫維持原路徑。目錄用途另見根目錄`README.md`。

## 0. 狀態標記與衝突規則

### 0.1 狀態標記

| 標記 | 意義 |
|---|---|
| `[FINAL]` | 該檔明定範圍已完成定檔，可以建立正史。後續新增不得默默推翻既有內容。 |
| `[STABLE]` | 既有內容已穩定且可直接引用，但屬持續生長型資料；可新增詞條或受控修訂，不得把「尚未收錄」解讀為不存在。 |
| `[beta]` | 已確認部分可以使用，但整體覆蓋仍不完整。不得從已寫內容推論尚未完成的城市、人物或制度。 |
| `[LIVE]` | 持續更新的賽程、賽果或當期狀態。其時間性內容以最新版本為準。 |
| `[REFERENCE]` | 補充資料；不能單獨推翻 `[FINAL]` 或 `[LIVE]` 來源。 |
| `[CRITICAL]` | 讀取優先級極高。此標記描述重要性，不等同成熟度；可與其他狀態並列。 |
| `[SUPERSEDED]` | 已被取代，不得作為現行正史來源或上傳至衍生產品。 |

### 0.2 衝突優先序

1. 使用者最新明確定檔及其已建立的專檔。
2. `[FINAL][CRITICAL]` 本體論、憲法處罰法及制度專檔；憲法正文另列`[ongoing beta]`，不因引用其名稱而自動取得FINAL地位。
3. 與問題直接對應的 `[FINAL]` 專題檔。
4. 與問題直接對應的 `[STABLE]` 持續生長型資料；既有條目有效，但未收錄不等於不存在。
5. `[LIVE]` 檔中的已發生賽果、日期與當期狀態。
6. `[beta]` 檔中已明文確認的部分。
7. `[REFERENCE]` 摘要與舊制背景。

人物生死、案件結局與組織存續有衝突時，優先讀取具體年代與結局的專題編年檔；不得因名冊、舊摘要或論壇文章仍出現姓名，就使已死亡人物復活。

`[beta]` 表示覆蓋不完整，不表示其中每一條都可任意改寫。已明文定檔的城市或制度仍有約束力。

## 1. 核心本體論、制度與穩定資料

### 1.1 世界及運動本體論

- **`source/Federal_Education_lore.md`** — [beta][CRITICAL]：已鎖定學校沿革、人物教育登錄與出生地／資格分流的完整條目；制度本體論與機器表效力不變。
- **`patch/patch_Federal_Education.md`** — [CRITICAL]：教育生成、招生防錯、人物登錄與全量來源定位界線；各節FINAL／beta沿用原專檔，不新增資格或校網。教育專檔須與對應章節合讀。

- **`source/Lore_Ontology.md`** — `[FINAL][CRITICAL]`：世界觀名詞、物理定義、前線隔離、地緣政治辨析及通用防錯規則。
- **`source/State_Succession_Ontology.md`** — `[FINAL][CRITICAL]`：2024–2046國家與政權的時間有效性、北韓偏安與朝鮮國繼承、後俄羅斯實體、流亡政府及國際組織分類的唯一正式定義。 時間／輸出操作規則另見`patch/patch_History_International_Order.md`對應章節；本體、日期表與原效力不變。
- **`source/Education_Credential_Ontology.md`** — `[FINAL][CRITICAL]`：國小至高中E3共同序列、三條學歷路徑、A至F評量、GSD及國中升高中聯邦聯合招生之模組命題與非名次錄取的唯一正式定義。 完整內容依本檔章節連結分流至教育_lore／patch；舊檔名仍保留查找入口。
- **`source/Course_Tree_World_Xplorer_Ontology.md`** — `[FINAL][CRITICAL]`：課程樹的World Xplorer式節點結構、E0至E4深度軸、先修、跨域與終身回修。 完整內容依本檔章節連結分流至教育_lore／patch；舊檔名仍保留查找入口。
- **`source/Federal_Education_Core_Basic_Ontology.md`** — `[FINAL][CRITICAL]`：Core／Natural Reality與Basic／Social Reality之分類、科學證據狀態、歷史事實底線及「暴政如何美化行為」課程的唯一正式定義。 完整內容依本檔章節連結分流至教育_lore／patch；舊檔名仍保留查找入口。
- **`source/Federal_Education_Institution_Map_2046.md`** — `[beta][CRITICAL]`：2046高中存在性、前身／後繼、聯邦市校址、課程樹供給及GSD聯招／跨校修課映射；跨區自由與反學區房仍以前述學歷本體論的制度硬鎖為準。 完整內容依本檔章節連結分流至教育_lore／patch；舊檔名仍保留查找入口。
- **`source/Federal_Education_Institution_Map_2046.csv`** — `[beta][CRITICAL]`：學校時間有效性與城市映射機器表；只有`confirmed`且`bio_assignment_allowed=true`的列可供人物母校自動指派。2030年代新增四校之校史見`source/Federal_Education_lore.md`，限定課程及GSD會員同步登錄；新增校的自動人物指派保持關閉。
- **`source/Federal_Education_Course_Tree_Offerings_2046.csv`** — `[beta][CRITICAL]`：已確認及校務輪廓推定的課程樹供給；`profile_mapped`不得反推人物已修讀。
- **`source/Federal_Education_GSD_2046.csv`** — `[beta][CRITICAL]`：第一版GSD會員、聯招、跨校修課及跨GSD申請表；所有列均禁止設籍或房產優先。
- **`source/Federal_Education_GSD_Capability_Matrix_2046.md`** — `[beta][CRITICAL]`：P1校際供給邊界與GSD互補矩陣；原校、跨校E4節點與能力缺口必須分列，禁止萬用校推論。 完整內容依本檔章節連結分流至教育_lore／patch；舊檔名仍保留查找入口。
- **`C:/hammershot/notebooklm_imports/csv_working_only/Federal_Education_P1_Reality_School_Candidates_2046.csv`** — 工作區稽核表：按教育部115學年度校名錄建立的2046候選校映射；全數`mapped`，不得作Notebook正史來源或自動指派人物。
- **`C:/hammershot/notebooklm_imports/csv_working_only/Federal_Education_P1_Course_Routing_2046.csv`** — 工作區待核表：P0人物課程樹路由、候選與能力缺口，供P2逐筆覆核；不得作Notebook正史來源。
- **`C:/hammershot/notebooklm_imports/csv_working_only/Federal_Education_P2_Individual_Reassignment_2046.csv`** — 工作區稽核帳本：57筆性別錯配重派的原行號、原校、跨校節點與理由；不得作Notebook正史來源。
- **`source/Federal_Education_Person_Credential_Registry_2046.md`** — `[beta][CRITICAL]`：人物原文已明示的母校、舊制學歷、課程樹節點與轉軌登錄；空白不得自動補校。 完整內容依本檔章節連結分流至教育_lore／patch；舊檔名仍保留查找入口。
- **`source/Federal_Education_Person_Credential_Registry_2046.csv`** — `[beta][CRITICAL]`：人物教育紀錄機器表；只有`assignment_status=exact_current`者可直接連至2046機構表。
- **`source/Federal_Education_Foreign_Institution_Registry_2046.csv`** — `[beta][CRITICAL]`：外籍人物的海外教育登錄；分列原文明示校名與僅有地域／類型的待核對資料。全部`eligible_for_auto_assignment=false`，不得從校名推論畢業、在學、居住地或2046存續。
- **`source/Federal_Education_Foreign_Institution_Map_2046.csv`** — `[beta][CRITICAL]`：人物原文已明示的海外教育機構正規化表；只證明文本中的校名可辨，不單獨證明2046存續、人物完成學業或自動指派資格。
- **`source/Federal_Education_Legacy_Higher_Institution_Map_2046.csv`** — `[beta][CRITICAL]`：選手原文直接出現的舊制、大專、軍警與海外高等教育校名正規化表；不能倒寫成2046高中、G.H.或課程樹資格。
- **`source/Federal_Education_Legacy_Higher_Credential_Registry_2046.csv`** — `[beta][CRITICAL]`：逐列回溯的舊制／高等教育具名紀錄；僅依原文標示畢業、肄業或就讀關聯，並禁止自動指派。
- **`source/Federal_Education_Player_Source_Inventory_2046.md`** — `[beta][CRITICAL]`：四聯盟選手教育欄的全量回溯規則；同名及跨梯隊重複列不得自動合併。 完整內容依本檔章節連結分流至教育_lore／patch；舊檔名仍保留查找入口。
- **`C:/hammershot/notebooklm_imports/csv_working_only/Federal_Education_Player_Source_Inventory_2046.csv`** — 工作區來源定位清冊；不是母校名冊，不得作Notebook正史來源。
- **`C:/hammershot/notebooklm_imports/csv_working_only/Federal_Education_Player_Education_Source_Inventory_2046.csv`** — 工作區教育來源中繼清冊；不得作Notebook正史來源或人物學歷判定。
- **`C:/hammershot/notebooklm_imports/csv_working_only/Federal_Education_Player_Normalization_Queue_2046.csv`** — 工作區機械分流待核隊列；`exact_current_candidate`仍須人工覆核，不得作Notebook正史來源。
- **`C:/hammershot/notebooklm_imports/csv_working_only/Federal_Education_New_System_School_Audit_2046.csv`** — 工作區母校記載狀態稽核表；只報告原文有無校名，不得作Notebook正史來源或補造特定母校。
- **`source/Federal_Education_Birthplace_Tandem_Projection_2046.md`** — `[beta][CRITICAL]`：四聯盟全部新制教育人物的2046出生年代地名、原校錨點、課程樹與資格路線登錄；既有教育內容保留，原未記母校者已完成回填，難民身分不可考者不得以國籍、球隊或姓名代填。 完整內容依本檔章節連結分流至教育_lore／patch；舊檔名仍保留查找入口。
- **`source/Federal_Education_Birthplace_Tandem_Projection_2046.csv`** — `[beta][CRITICAL]`：前項895筆出生／教育登錄的機器表；`G.H.`與E0–E4節點分欄記載，原校可配合GSD跨市修課但不得改寫為居住地或學區優先。
- **`source/Emoji_Protocol_Ontology.md`** — `[FINAL][CRITICAL]`：西門町四區Emoji、家庭角色計數串，以及竹科良率臉的文化象徵／暫時神經狀態及其消歧定義。
- **`source/Taiwan_Japan_Inner_MSSB_Ontology.md`** — `[beta][CRITICAL]`：衝突時代後臺日「內」的擴大、自洽神話、在台族四個移入層與二世／三世家族代數、姓名書寫層次、跨產業JDM技術內化，以及MSSB之Service ID／邏輯頻道／實體頻率動態映射。不得將3.5代自動標成外籍，也不得把Ch. 11永久綁定單一頻段。
- **`source/FNC_UNN_Ontology.md`** — `[FINAL][CRITICAL]`：FNC平等公會、丘仲堯總代表權限、2029年3v3和平分家、UNN分散式節點，以及兩者查核方法的唯一正式定義。
- **`source/Hammershot_Absolute_Ontology.md`** — `[FINAL][CRITICAL]`：Hammershot唯一運動本體論；器材、動作、場地、四隊序列、Arsenal及L-M語義均以此檔為準。
- **`source/Hammershot_Public_Terminology_Protocol.md`** — `[FINAL][CRITICAL]`：Hammershot公開角色名、判決名、競賽層級、統計名及HSE舊欄位轉譯的唯一正式規範；公開內容使用Deliverer、Striker、Good、Miss、2GA、AA、BA、FG、RHI及AMA。
- **`source/Hammershot_CAPS_IFAST_Ecosystem.md`** — `[FINAL][CRITICAL]`：2030年後合法穿戴式IFAST、CAPS電腦輔助配球系統及至少11家供應體系的正式定義。
- **`source/FFA_Equipment_Allocation_2046.md`** — `[beta]`：2046年60隊CAPS／IFAST及氣錘槍雙軌配置備忘錄；除明標已見使用者外，均為文化適配提案，不證明採購、贊助或排他合約。市場供應體系與器材物理仍以上述FINAL專檔為準。
- **`source/Hammer_Homologation_Register_2046.md`** — `[FINAL][CRITICAL]`：Hammer供應者、型式認證與地域限制的首批完整名冊；神崎雙持250 g×2按不可拆分整組認證。型式核准不證明任一球隊已購買、簽約或於過去場次使用；16個隊伍自製工坊只列待申請附表。
- **`source/hammershot_rulebook_fulltext.md`** — `[FINAL][CRITICAL]`：競賽執法全文；與摘要衝突時，以本檔及絕對本體論共同裁決。
- **`history/legacy/Hammershot_Rulebook.md`** — `[SUPERSEDED][REFERENCE]`：早期 HRE 摘要，保留供規則演進查核；含舊座標、名單與棒球式欄位殘留，不得上傳 Notebook 或用於現行正史。
- **`source/FFA Charter.md`** — `[FINAL][CRITICAL]`：方程式前線管理局之憲章、權力、賽程窗口、FGPS拓撲與FFC治理；2046–47起THCL C／H、H／N各採上層末位對下層前三的四隊升降級賽，業餘A級第一名經認證後另觸發The Gauntlet。三者在同一季後賽期間並行，不互作開賽前提；N組現行六隊，不沿用舊制五隊守關數量。
- **`source/League_Structure_Spec.md`** — `[FINAL]`：聯盟分級、隊伍結構及制度規格；2046–47 THCL正式三級為C、H、N，THHL只作歷史名稱。
- **`source/League_Lore.md`** — `[FINAL]`：FFA錘擊生態、國際錘擊聯賽、Breakthrough Series、特殊迴避及競賽文化；包含THCL Level N與CL Grade III。其他運動的生態分別由下列專檔收錄。涉及其他運動的歷史關聯或比喻，不因此視為其他運動的競賽規則。
- **`source/Hammershot_Satellite_Player_Registry_2046.md`** — `[STABLE][CRITICAL]`：2046年480名FFA衛星球員之存在、永久識別與靜態競技登錄；當期徵召、傷病、合約及賽果仍以HSE-02為準。
- **`source/Hammershot_Roster_Provenance_Quarantine_2046.md`** — `[STABLE][CRITICAL]`：高頻同名球員的永久識別／隊籍消歧與性別不相容校名映射修正；不得因同名而自動合併人物，也不得把男性登錄為女子高中畢業。
- **`source/Hammershot_Same_Name_Disambiguation_Registry_2046.csv`** — `[STABLE][CRITICAL]`：80筆高頻占位姓名現役列的FPR資料連結與現行姓名表；三人保留原名，其餘77人完成資料層姓名修正。

### 1.2 聯邦法統

- **`source/Federal_Central_Institutions_lore.md`** — [FINAL][CRITICAL]：中央機關產生方式、2028／2029制度切換、首長任期表與現任名冊的完整條目；承接原Lineage專檔。
- **`patch/patch_Politics_Law_Governance.md`** — [CRITICAL]：中央首長消歧、刑罰報導、兵役資料投影、選舉介面、三旗未定參數、P0／AP授權，以及日美戰後法律的資料欄位與生成判讀。各節FINAL／beta不變；法律正文另留原專檔。

- **`source/Federal_Constitution.md`** — `[ongoing beta]`：持續編纂中的憲法正文，目前收錄至第四章第十九條；涉及96個組成城市、國民大會、城市自治、特區及聯邦受讓權力，不以編纂狀態補造未收錄章節。犯罪構成、刑度及緊急阻卻違法事由依`source/punishmentlaw.md`等專檔。
- **`source/Federal_Election_Ballot_And_Tournament_Ontology.md`** — `[beta][CRITICAL]`：一般聯邦市WSC／萌戰制的流程邊界、候選人專用圈選工具、帶法定浮水印之白紙選票與連續多日投票的正式Beta定義。 資料表示或生成判讀章節見`patch/patch_Politics_Law_Governance.md`對應條目，制度正文與法律效力不變。
- **`source/Federal_Central_Institutions_Lineage.md`** — [REFERENCE]：舊檔名查找入口；全文已移至`source/Federal_Central_Institutions_lore.md`（FINAL／CRITICAL），使用消歧見`patch/patch_Politics_Law_Governance.md`。
- **`source/HRO_System_Ontology.md`** — `[FINAL][CRITICAL]`：HRO、SSR、Buff與Obligation、戶籍／國籍／現居／送達分離、四種特種HRO、二十二個一般HRO正式名冊及邦聯接口。任何HRO個別介紹或生活指南與本檔衝突時，以本檔為準。
- **`source/Federal_Criminal_Penalty_Ontology.md`** — `[FINAL][CRITICAL]`：各市實體法自治、聯邦統一程序及刑罰效果。 資料表示或生成判讀章節見`patch/patch_Politics_Law_Governance.md`對應條目，制度正文與法律效力不變。
- **`source/punishmentlaw.md`** — `[FINAL][CRITICAL]`：個別犯罪構成與刑度；須與刑罰本體論合讀。
- **`source/Unjust_Property_Copyright_Disposition_Act.md`** — `[FINAL]`：不義著作權與數位平台處分。 資料表示或生成判讀章節見`patch/patch_Politics_Law_Governance.md`對應條目，制度正文與法律效力不變。
- **`source/Anti_Resurrection_Act.md`** — `[FINAL]`：衝突時代受害者影像生成禁制。 資料表示或生成判讀章節見`patch/patch_Politics_Law_Governance.md`對應條目，制度正文與法律效力不變。
- **`source/DJT_Legal_Review_Resolution.md`** — `[FINAL]`：DJT時代法律的三軌審查與承接。 資料表示或生成判讀章節見`patch/patch_Politics_Law_Governance.md`對應條目，制度正文與法律效力不變。
- **`source/Conflict_Era_Military_Actions_Resolution.md`** — `[FINAL]`：美國衝突時代軍事法統及傷亡追認。 資料表示或生成判讀章節見`patch/patch_Politics_Law_Governance.md`對應條目，制度正文與法律效力不變。
- **`source/Federal_Defense_Service_Ontology.md`** — `[FINAL][CRITICAL]`：聯邦正規軍、契約預備人力、非戰鬥專業徵用與舊制役籍不自動教召的正式定義。 資料表示或生成判讀章節見`patch/patch_Politics_Law_Governance.md`對應條目，制度正文與法律效力不變。
- **`source/Federal_CMYK_RGB_Signal_Flag_System.md`** — `[beta][CRITICAL]`：聯邦三旗信號的CMYK負面警示、RGB正面節慶／成就、已確認的1–9級尺度及其與0001／0002法定程序的邊界；未定義代碼不得自行補寫。 資料表示或生成判讀章節見`patch/patch_Politics_Law_Governance.md`對應條目，制度正文與法律效力不變。
- **`source/New_UN_P0_Apex_Predators_Ontology.md`** — `[FINAL][CRITICAL]`：P0個人通緝層級、Apex Predators活捉契約與石山伊佐男行動邊界；不得與MPD工程P0優先級混用。 資料表示或生成判讀章節見`patch/patch_Politics_Law_Governance.md`對應條目，制度正文與法律效力不變。
- **`source/Japan_Designated_Anti_Constitutional_Works.md`** — `[FINAL]`：日本國反憲政秩序創作認定。 資料表示或生成判讀章節見`patch/patch_Politics_Law_Governance.md`對應條目，制度正文與法律效力不變。
- **`source/Japan_Post_Conflict_Resolution_Act.md`** — `[FINAL]`：日本戰後法統、合約與法人清理。 資料表示或生成判讀章節見`patch/patch_Politics_Law_Governance.md`對應條目，制度正文與法律效力不變。

### 1.3 歷史連續性與已定結局

- **`patch/patch_History_International_Order.md`** — [CRITICAL]：時間判讀、史料連續性、證據階級、主權連續性、早期家系待考及北歐生成界線；各節FINAL／STABLE效力沿用原專檔。
- **`source/Early_Historical_Continuities_lore.md`** — [FINAL]：1511神諭、1945留臺政策與Raina假死及逃亡路徑全文；待考關係另見歷史patch。
- **`source/Japan_Entertainment_Trials_lore.md`** — [FINAL]：日本雙重法統、部分原告代理、PONR、平山偽證、木谷及LoveLive／Liella案件的完整條目。
- **`source/Echo_Terra_lore.md`** — [FINAL]：The Echo三階段使命、新聯合國、Peaceholder及Terra工程與標準戰爭的完整沿革。
- **`source/Echo_Terra_Ontology.md`** — [FINAL]：MPD之分子分解／重構、能耗、原子來源與物理限制的完整本體。

- **`source/World_Master_Timeline.md`** — `[STABLE][CRITICAL]`：1392–2046國名、法統、制度及組織有效期間的主年表；任何Gemini Notebook資料包均應優先載入，用於阻止未來狀態倒灌與無根據補日期。 時間／輸出操作規則另見`patch/patch_History_International_Order.md`對應章節；本體、日期表與原效力不變。
- **`source/Place_Name_Era_Protocol.md`** — `[beta][CRITICAL]`：完整協議已移至 `patch/patch_City_Regions.md`「地名年代協議」，本檔保留路由。地名的年代、制度層級、同名市、邊界重組、舊址對照及機器消歧欄位；先定日期再使用地名，禁止把2046聯邦市代碼或區名倒填至單一制時代。
- **`source/Historical_Continuity_Guide.md`** — [REFERENCE]：舊檔名入口；完整FINAL／CRITICAL編纂規則已移至`patch/patch_History_International_Order.md`「史料連續性、缺載與主權判定」。
- **`source/Early_Historical_Continuities.md`** — [REFERENCE]：舊檔名入口；完整條目改由`source/Early_Historical_Continuities_lore.md`承接，維持原FINAL效力。
- **`source/Conflict_Era_Addendum.md`** — [REFERENCE]：舊檔名入口；全文已併入`source/Conflict.md`「V. 衝突時代動機、法統與戰場補編」，維持原FINAL／CRITICAL效力。
- **`source/Hammershot_History.md`** — `[FINAL][CRITICAL]`：Hammershot與棒球並存、聯盟政治分裂及歷史硬鎖。
- **`source/Post_DSH_Game_Culture.md`** — `[FINAL]`：DSH後遊戲、主機與作品權利文化。
- **`source/Taiwan_Transition_Crime_Network.md`** — [REFERENCE]：舊檔名入口；全文已併入`source/Conflict.md`「VII. 臺灣退選、大逃亡與CSSE資產來源」，維持原FINAL效力。
- **`source/Ximending_Wanshuanghedian_Boundary_History.md`** — `[FINAL]`：早期Nexus／Old Bones／Clean Boots生活圈、現行跨市寧靜區及竹林路聯盟關係；正文已併入 `source/Federal_City_Ximending_Districts.md` 第十一節，本檔保留路由。
- **`source/Japan_Entertainment_Trials.md`** — [REFERENCE]：舊檔名入口；完整條目改由`source/Japan_Entertainment_Trials_lore.md`承接，維持原FINAL效力。
- **`source/Echo_Terra.md`** — [REFERENCE]：舊檔名入口；完整條目改由`source/Echo_Terra_lore.md`承接，維持原FINAL效力。
- **`source/Nordic_Conflict_Era_Addendum.md`** — [REFERENCE]：舊檔名入口；全文已併入`source/Conflict.md`「VI. 北歐防衛、冰島與白澄家族」，維持原FINAL效力。
- **`source/HydroTran_Mobility_Ontology.md`** — `[FINAL][CRITICAL]`：HydroTran載具正式定義；北美county seat、日本私鐵補充、聯邦海線與UAN運用的完整生活條目已併入`source/Federal_Life_Guide.md`「區域移動與都市艙乘用生活」，使用界線見`patch/patch_Life_Mobility_Technology.md`。
- **`source/Federal_F_Road_Network.md`** — `[beta][CRITICAL]`：聯邦 F 路網、F／G 編號消歧、已確認縱橫線、F7 跨境行車側切換、F11 爭議；未定參數與輸出限制見`patch/patch_Life_Mobility_Technology.md`。

### 1.4 世界觀字典檔案群 `[STABLE]`

- **`patch/patch_Dictionary_Retrieval.md`** — `[STABLE][CRITICAL]`：以Sense ID、主體鑰匙及Scope Gate連結字典與Lore，禁止錯接事實。
- **`dict/Dictionary_Entry_Ontology.md`** — `[STABLE][CRITICAL]`：詞條欄位、Scope、消歧及Gemini Notebook判讀規則。
- **`dict/dic_Entity_Alias_Registry.md`** — `[STABLE][CRITICAL]`：人物、組織、隊伍、城市與產品的`ENT-*`、正式名、異體、縮寫、舊名及綽號登錄；只負責辨識實體，不取代日期化名冊或事件取證。
- **`dict/dic_01_Mobility_Technology.md`** — `[STABLE][CRITICAL]`：交通、Roster、UPFB、都市艙及個人科技；TapWin／Call詞義與消歧。
- **`dict/dic_02A_Hammershot.md`** — `[STABLE][CRITICAL]`：Hammershot物理、器材、場地、動作及賽局詞義。
- **`dict/dic_02B_Leagues.md`** — `[STABLE][CRITICAL]`：FFA、雙前線、四聯盟、升降、准入及年度冠軍。
- **`dict/dic_03A_Government_HRO.md`** — `[STABLE][CRITICAL]`：聯邦、城市、領地、HRO及竹科治理。
- **`dict/dic_03B_Law_Security.md`** — `[STABLE][CRITICAL]`：法律、刑罰、憲政防衛及保安警察。
- **`dict/dic_04_Society_Education.md`** — `[STABLE][CRITICAL]`：教育路徑、聯招、地址、住宅、1+n、CIV、SLEK、FoT及Emoji。
- **`dict/dic_05_Organizations_Media.md`** — `[STABLE][CRITICAL]`：FNC、UNN、查核方法、Host、DSH、ASMD、清潔工及衍生產品介面。
- **`dict/dic_06_History_Geopolitics.md`** — `[STABLE][CRITICAL]`：國家延續、後繼國、衝突時代、後中國／後俄羅斯實體、APR、韓國複合共和制及石油美元崩潰。

字典負責辨義，Lore專檔負責事實；衝突時以相應`[FINAL][CRITICAL]`專檔為準。未收錄不表示不存在。

### 1.4.1 完整詞卡與相容入口

- **dict/dic_00_Disambiguation.md** — [STABLE][CRITICAL]：高風險詞義碰撞表及UMX-40／氣錘詞卡。
- **dict/Dictionary_Entry_Ontology.md** — 定義Lexical Entry v2、別名類型、Sense ID／ENT／EVT／SYS及Scope Gate；不是事件來源。
- **dict/dic_Entry_Locator.md** — [REFERENCE]：只定位既有詞條章節，不增加詞義、別名或人物。
- **舊檔名備份** — World_Dictionary各分冊、World_Dictionary_00_Protocol、Lore_Dictionary_Link_Protocol與Entity_Alias_Registry已移至工作區`C:/hammershot/notebooklm_imports/dict_legacy_entries/`，不作Notebook來源；現行詞義只由dic／本體／patch承接。

## 2. 當期狀態與賽程

- **`source/2045-46.md`** — `[LIVE][CRITICAL]`：2045–46繼續前線賽程、休整與已發生結果。
- **`source/2046.md`** — `[LIVE][CRITICAL]`：2046希爾塔前線賽程、活動日期與已發生結果。
- **`source/2046-47.md`** — `[LIVE][CRITICAL]`：2046–47 Continuation Front官方賽程、12隊輪替、60個HD比賽日、12站FGPS／72 Nodes、春節休兵與已發布賽務規則。

凡涉及2046–47的日期、下一場、參賽隊、FGPS Nodes或衛冕軍，必須路由至`source/2046-47.md`；2046希爾塔前線仍查`source/2046.md`。`source/2045-46.md`保留為歷史賽季來源，其HD表的39／42／39槽位失衡只屬矩陣勘誤，不得標成`[SUPERSEDED]`，也不得從不存在的telemetry或match logs回算成績。2045-46 FFC時程治理查`source/FFA Charter.md`。Hammershot為四隊序列，不得改寫成普通一對一賽制。

## 3. 聯邦城市資料群 `[beta]`

### 3.1 全國城市骨架

- **`source/Federal_Cities_List.md`** — `[FINAL]`：96個現行組成城市的代碼、正式名稱及基礎轄域，逐市對照1987–2010年12月24日、2010年12月25日至聯邦化前兩段歷史縣市／鄉鎮市區；原住民族市依民族誌定界、現行地理錨點另列，人工島不倒填為舊行政區。新見市的括號候選代碼`(100)`不增加現行城市數。城市代碼與城市存在性以此檔為準；歷史對照不產生現行行政權。
- **`source/Federal_Cities_Lore.md`** — `[beta]`：96市風土、政治與生活摘要；個別城市若已有專用定檔檔案，專檔優先。
- **`source/Federal_Cities_Famous_person.md`** — `[beta]`：96市公共人物索引；城市覆蓋已建立，但人物狀態仍須與人物專檔及 `source/Social_Graph.md` 交叉核對。
- **`source/Federal_Life_Guide.md`** — `[beta]`：聯邦生活、HRO、1+n經濟、通訊與公共服務指南；CMB收件、十九家郵務服務商與地方轉運文化。
- **`source/Villians.md`** — `[FINAL]`：重大加害者排除索引；不得將名列者改寫為城市正面代表。

### 3.2 96市分區檔案群 `[beta]`

本檔案群整體標記為 `[beta]`，因目前只完成96市中的六市。下列六份檔案在各自城市範圍內均為 `[FINAL]`：

1. **`source/Federal_City_Neisong_Districts_V3.md`** — 06內松聯合市：十三區、企業聯合與機場體制。
2. **`source/Federal_City_Songxin_Districts_V1R.md`** — 09松信自由市：九區、市界、Building及都市艙體系。
3. **`source/Federal_City_Ximending_Districts.md`** — 12西門町市：四區、2034構成選舉、夜間自治、第211條、ASMD地下城及拉維式責任自由。
4. **`source/Federal_City_Zhuke_Clusters.md`** — 21竹科市：九個Cluster、X1–X9、Node與CSR治理。
5. **`source/Federal_City_Hsinchu_Districts.md`** — 22新竹市：市界、國防部第99特區及十三區。
6. **`source/Federal_City_Tunqu_Districts_V1_5R.md`** — 33屯區市：二十六區、里界積木與棒球復興。

- **source/City_Administrative_Ontology.md** — [FINAL]：內松CBD／Borough、松信區／Building／里、竹科Cluster／Node與X體系的定義及權責；與各市正文合讀。
- **逐市行政權責** — 六市專檔均直接記載各自市級、區級、基層／設施分工、跨區協作及權限限制；不以共同摘要取代，不跨市套用權限。內松、松信及竹科的完整權責並保留於各自專檔；未定細部授權繼續留空。後續每一市專檔同樣必須明記。
- **六市市治與地址** — 六市市治位置見`patch/patch_City_Regions.md`同名表及各市專檔。未指定路名沿用現實名稱、行政歸屬用聯邦區劃；竹科市治在關埔Cluster，屯區在七期市政區，西門町記N/A。不補造未指定建築或門牌。
- **竹科😑文化** — `source/Federal_City_Zhuke_Clusters.md`第十一節收錄Six Sigma、神經調節起源與家庭／日常／球迷文化的演化；文化標記不證明使用神經技術。
- **`source/Artificial_Islands_lore.md`** — `[beta][CRITICAL]`：新見島、交換站島及琉球國豐美島的三節點走廊、居住與生活、國境換側及尚未指定事項。新見現屬羅東市新見區，2046年年底進行設市公投；`(100)`僅是未來可能依16-2分立之候選代碼，不是現行正式市代碼或第97個組成城市。不將日本其他構成體一併升格。
- **patch/patch_City_Regions.md** — 六市既有判定與測繪保留維持 [FINAL]，地名年代協議維持 [beta][CRITICAL]；不生成新界線。

未列城市不得仿照上述六市自動生成正式區界。二林市等已討論但尚未形成定檔專檔者，仍屬待整理範圍。

- **`patch/patch_Person_Social_Graph.md`** — 人物與社會關係的記述邊界；各節保留原FINAL／beta成熟度，與人物正文合讀。

## 4. 人物、組織與社會關係 `[beta]`

- **新聞組織前置規則：** 凡涉及FNC、UNN、丘仲堯職權、新加坡六人組分家或插值查核法，必須先讀 **`source/FNC_UNN_Ontology.md`**；人物檔與舊論壇稱呼不得反推公司階級。
- **`source/Key_Figures_tech.md`** — `[beta][CRITICAL]`：關鍵人物、科技史、企業與重大事件；1.1.4記載TapWin手機系統與Call介面。雙前線月份只作制度摘要，精確日期仍須查當季LIVE賽程，具體案件須與編年及法律專檔交叉核對。
- **`source/Social_Graph.md`** — `[beta][CRITICAL]`：血緣、婚姻、戰友、師徒及敵對關係；第五章收錄五名人物完整條目，第六章承接新竹人物生平。各條目成熟度分別標記，不能因合併抹去FINAL專題優先權。
- **`source/Chiu_Chung_Yao_Lore.md`** — `[FINAL]`：丘仲堯生平、家庭、債務協商、公共人格與2044年後活動之人物專檔；FNC職權仍以`source/FNC_UNN_Ontology.md`為準。債務「約77萬元」是本人不記得尾數的回憶，不得寫成精確770,000元或由月付額反推本金。其早年體型紀錄不能單獨解決仲村曉雲身分疑雲。
- **`source/Household_lore.md`** — `[beta]`：HRO作為身分別行會的會員文化、福利與已收錄生活細節；收錄條目不等於正式名冊全部組織均已完成個別生活或章程。新聯合國聯合身分中心以難民與無國籍者保護為核心，權限見`source/HRO_System_Ontology.md`第10.5節，判讀見`patch/patch_Life_Mobility_Technology.md`。法定名冊、身分及章程邊界仍以HRO本體論為準。舊`history/legacy/household.md`、`history/legacy/household2.md`及`history/legacy/mail.md`不恢復正史資格；十九家郵務服務商及CMB內容歸入`source/Federal_Life_Guide.md`。
- **`source/Political_Parties.md`** — `[beta]`：聯邦政黨與意識形態。
- **`source/Team_Rivalry_Matrix.md`** — `[beta]`：隊伍宿敵、階級衝突與互動基調。
- **`history/legacy/Roster_Lore.md`** — `[SUPERSEDED]`：已由四聯盟選手檔及對應隊伍檔取代；只供編輯考證，不得上傳或作現役名冊來源。
- **`source/coach.md`** — `[beta]`：教練、GM及球隊治理人物。
- **`source/Yamada_Mao_Lore.md`** — `[REFERENCE]`：舊檔名查找入口；完整人物條目已併入`source/Social_Graph.md`第五章「山田麻央」（[beta]），記述邊界見`patch/patch_Person_Social_Graph.md`同名章節。人物條目的原成熟度及專題優先權不變。
- **`source/Saeki_Kana_Lore.md`** — `[REFERENCE]`：舊檔名查找入口；完整人物條目已併入`source/Social_Graph.md`第五章「佐伯加奈」（[beta]），記述邊界見`patch/patch_Person_Social_Graph.md`同名章節。人物條目的原成熟度及專題優先權不變。
- **`source/Nishiimori_Yoko_Lore.md`** — `[REFERENCE]`：舊檔名查找入口；完整人物條目已併入`source/Social_Graph.md`第五章「西井森陽子」（[beta][CRITICAL]），記述邊界見`patch/patch_Person_Social_Graph.md`同名章節。人物條目的原成熟度及專題優先權不變。
- **`source/Makita_Kaede_Lore.md`** — `[REFERENCE]`：舊檔名查找入口；完整人物條目已併入`source/Social_Graph.md`第五章「蒔田楓」（[beta][CRITICAL]），記述邊界見`patch/patch_Person_Social_Graph.md`同名章節。人物條目的原成熟度及專題優先權不變。
- **`source/Xiao_Baozhan_Lore.md`** — `[REFERENCE]`：舊檔名查找入口；完整人物條目已併入`source/Social_Graph.md`第五章「蕭寶棧」（[FINAL][CRITICAL]），記述邊界見`patch/patch_Person_Social_Graph.md`同名章節。人物條目的原成熟度及專題優先權不變。
- **`source/Hsinchu_Rhodanthes_People_Ontology.md`** — `[FINAL][CRITICAL]`：新竹以絆而非偶像選人的本體；王忠根、林育信、上村藍等完整人物事實見`source/Social_Graph.md`第六章，邊界見`patch/patch_Person_Social_Graph.md`。
- **`source/Kinmen_Civil_Defense_Team_Philosophy.md`** — [REFERENCE]：舊檔名入口；完整專題已併入`source/League_Lore.md`，維持原效力；生成界線見`patch/patch_Sports_Source_and_Generation.md`。
- **`source/Japan_PostConflict_Fame_Tax.md`** — [REFERENCE]：舊檔名入口；完整專題已併入`source/CPBL_lore.md`，維持原效力；生成界線見`patch/patch_Sports_Source_and_Generation.md`。

`[beta]` 人物檔不能覆蓋已確認的死亡、定讞、婚姻或職位專檔。未記載不等於不存在，也不得用自動補完製造新親屬或新罪行。

## 5. 聯盟及隊伍資料群 `[beta]`

### 5.1 繼續前線（冬季）

以下四檔保存跨賽季、跨層級的球隊與選手Lore，不自行決定2046-47第一級參賽權；當季隊伍與賽程一律先查`source/2046-47.md`。

- **`hammershot/CPHL_Lore.md`** — CPHL選手資料。
- **`hammershot/CPHL_team_lore.md`** — CPHL隊伍資料。
- **`hammershot/THCL_lore.md`** — THCL選手資料。
- **`hammershot/THCL_team_lore.md`** — THCL隊伍資料。

### 5.2 希爾塔前線（夏季）

- **`hammershot/IHA_lore.md`** — IHA選手資料。
- **`hammershot/IHA_team_lore.md`** — IHA隊伍資料。
- **`hammershot/CL_lore.md`** — CL選手資料。
- **`hammershot/CL_team_lore.md`** — CL隊伍資料。

上述八份檔案群整體為 `[beta]`：已登錄隊伍與人物可以使用，但不得推論所有層級、歷史賽季及未登錄名單均已完成。

### 5.2.1 FFA 現行第一級主場（24 隊）

以下四檔各記六座主場，合計覆蓋 CPHL、IHA、THCL、CL 在本批登錄的第一級隊伍。球場名稱、地理錨點、建築意象、地面材質及 FENCES 節點均可作為主場資料；當季參賽資格、日期、主客及賽果仍以第 2 節的 LIVE 賽程與正式比賽輸出為準。四檔為持續校訂的 `[beta][CRITICAL]` 主場資料，不因已覆蓋第一級而推定其他級別主場已完成。

- **`hammershot/CPHL1.md`** — `[beta] [CRITICAL]`：CPHL 第一級六座主場。
- **`hammershot/IHA1.md`** — `[beta] [CRITICAL]`：IHA 第一級六座主場，含新竹 Rhodanthes 位於美山聯絡道的主場、「大壩」建築與計分板；不得誤置於茄苳或聯合高中。
- **`hammershot/THCL1.md`** — `[beta] [CRITICAL]`：THCL 第一級六座主場。
- **`hammershot/CL1.md`** — `[beta] [CRITICAL]`：CL 第一級六座主場。

四檔保留原有 FENCES 數值；舊稿中的戰術效果、人物職位、物理絕對化敘述及教練發言不單獨建立新規則或新事件。器材、動作、Q-Lock、場地合法性與公開術語須同讀 `source/Hammershot_Absolute_Ontology.md`、`source/Hammershot_Public_Terminology_Protocol.md` 及 `source/hammershot_rulebook_fulltext.md`；發現節點數值與規則衝突時標記待核，不以改字暗改座標。第二級及以下主場仍待逐隊確認。

- **THCL Level N／CL Grade III隊伍治理** — `[beta]`：十二隊贊助／會員基礎、受託人物及所有者共同體，併入`source/League_Lore.md`對應層級章節；不建立當期現役名冊或賽程。
- **`patch/patch_THCL_N_CL_III_Governance.md`** — `[beta]`：受託執行、所有權、隊名與法人辨析、新見市民隊的16-2界線及尚未定檔項目。
- **`source/THCL_N_CL_III_Governance.md`** — `[REFERENCE]`：保留舊檔名的查找入口，正文已分流至聯盟條目及治理patch。

### 5.3 中華職棒（CPBL）2046資料群 `[beta]`

- **`source/CPBL_lore.md`** — `[beta]`：棒球十二隊的分區、生態、名冊分工與勝點文化；與FFA錘擊分開。

- **`source/CPBL_2046_Postseason_Rules.md`** — `[FINAL][CRITICAL]`：2046季後賽第一輪A、B、C、D四組共用的東京六大學式勝點制、對戰優勢1勝開局、`勝點 > 組內對戰成績 > Team Balance`排名順序、Team Balance排除延長賽，以及台灣大賽開局與2–3–2主場組態之正式規則。
- **`source/CPBL_2046_Rosters.md`** — `[beta][CRITICAL]`：12隊、28人名單結構、數值本體、已確認總教練、五名明星球員及模擬邊界。
- **`source/CPBL_2046_Teams.csv`** — `[beta]`：12隊分區、總教練、粗略團隊能力值及主場欄位；天母體育會主場已定為包道格大都會巨蛋，其餘未定者維持TBD。
- **`source/CPBL_2046_Rosters_A.csv`** — `[beta]`：CPBL-A四隊共112名球員之機器可讀名單。
- **`source/CPBL_2046_Rosters_B.csv`** — `[beta]`：CPBL-B四隊共112名球員之機器可讀名單。
- **`source/CPBL_2046_Rosters_IBA.csv`** — `[beta]`：IBA四隊共112名球員之機器可讀名單。

本資料群用於棒球聯賽模擬。季後賽第一輪規則以`source/CPBL_2046_Postseason_Rules.md`為準；名冊群尚未定義外籍名額、薪資、合約控制、傷病史與完整交易紀錄。CPBL為棒球；任何衍生產品均不得將Hammershot的器材、動作或術語套入這些檔案。

### 5.4 台灣1籃球聯賽（T1BL）2046–47資料群 `[FINAL]`

- **`source/Basketball_League_lore.md`** — `[beta]`：T1BL、T2BL、T3BL的分級生態、教練與球風、Break Light及總決賽文化。詳細規則與逐人名冊仍以本節FINAL專檔為準。

- **`source/T1BL_2046_League_and_Rosters.md`** — `[FINAL][CRITICAL]`：T1BL、T2BL、T3BL最後一季4–4–4分級、十二隊各15人開季名冊、總教練、主場、球風、NBA式正規賽基礎、Break Light、非法防守、ADD 6延長賽、積分與總決賽制度，以及四十輪主客配對。

本檔的逐輪配對與主客關係已定案；日期、開賽時間與賽果仍待正式公告。T1BL是籃球，不得混入Hammershot、棒球、足球或美式足球術語。早期`T1L`稱呼僅為舊稿簡稱，現行一律使用T1BL、T2BL、T3BL。

### 5.5 台灣美式足球聯盟（TGL）`[STABLE]`

- **`source/Gridiron_League_lore.md`** — `[beta]`：TGL四隊的地方市場、人物與球風，以及NFL重建背景；不合併兩個聯盟的名冊。

- **`source/TGL_League_and_Pence_Rules.md`** — `[STABLE][CRITICAL]`：TGL四隊、53人合約／45人啟用名冊、十二職位教練團；**2046賽季十八週36場例行賽結構定案**，舊口述的15週不適用。另載NFL式勝率、Taiwan Bowl twice-to-beat制度，以及彭斯制的區域過線、抵死重打、雙錶、後場多次前傳、活球、接球防守與動態越位規則。
- **`source/TGL_2046_Season_Data.md`** — `[STABLE][CRITICAL]`：2046球隊基調、資料表關係、四隊固定主場、十八週對戰摘要、勝率更新及跨運動防錯。
- **`source/TGL_2046_Venues.md`** — `[FINAL][CRITICAL]`：包道格大都會巨蛋、芎林體育場、澄清湖體育場與靈魂之地的固定主場身分、容量、屋頂／草皮機制及跨運動邊界。
- **`source/TGL_2046_Teams.csv`** — `[STABLE]`：四隊名稱、地理錨點、固定主場及競技基調。
- **`source/TGL_2046_Rosters.csv`** — `[STABLE][CRITICAL]`：四隊共212名球員；每隊53名合約球員，分為45名active與8名reserve。
- **`source/TGL_2046_Coaches.csv`** — `[STABLE]`：四隊共48名主要教練及其職責。
- **`source/TGL_2046_Schedule.csv`** — `[STABLE][CRITICAL]`：十八週36場例行賽的完整對戰、主客場及四隊固定主場，以及Taiwan Bowl第一場和條件式第二場。實際日期與開球時間維持TBD。
- **`source/TGL_2046_Standings.csv`** — `[LIVE][CRITICAL]`：2046戰績表；勝率為`(W + 0.5T) / GP`，比賽前為0-0-0及`.000`，只能由正式賽果更新。

TGL為全碰撞美式足球聯盟。任何衍生產品不得將Association Football、棒球或Hammershot術語套入TGL；涉及制度先讀規則專檔，涉及場館先讀`source/TGL_2046_Venues.md`，涉及2046名冊、教練與對戰再讀賽季資料及對應CSV。實際日期、開球時間與賽果未公告前不得自行補完。

### 5.6 NFL四聯會與戰後Ownership `[STABLE]`

- **`source/NFL_2046_Conference_and_Ownership.md`** — `[STABLE][CRITICAL]`：2036擴編後AFC、NFC、GFC、SFC四個平行聯會的2046年四十八隊名冊；Albuquerque、Boise、Des Moines與Honolulu中型市場席位；以及衝突時代大量Private Equity因向政治、武裝及企業陣營押寶而遭非法化後，Franchise right、Operating entity及Local continuity interest分離的球團所有權制度。2028年美債違約是加速資金鏈失能的背景，不是非法化的主要法律原因。四個新席位的正式隊名、球場、經營法人及出資人仍為TBD，不得自動補完。
- **`source/NFL_2046_Season_Data.md`** — `[beta][CRITICAL]`：2046 NFL資料表關係、53人名冊、十二個主要教練職位、勝率與十八週／每隊十七場之可替換賽程模型。日期、球場、季後賽、傷病、交易及賽果仍未定檔。
- **`source/NFL_2046_Teams.csv`** — `[beta]`：四十八隊／席位的聯會、城市市場、來源、場館與戰後Ownership欄位；四個未命名席位的`franchise_name`維持`TBD`。
- **`source/NFL_2046_Rosters.csv`** — `[beta][CRITICAL]`：四十八隊各53人、共2,544人的2046 beta登錄名冊；只建立姓名、背號、位置與名冊槽位，不建立人物傳記。
- **`source/NFL_2046_Coaches.csv`** — `[beta]`：四十八隊各十二個主要教練職位、共576筆beta職員資料；不表示完整球團職員只有十二人。
- **`source/NFL_2046_Schedule.csv`** — `[beta][CRITICAL]`：十八週408場可替換對戰草案；每隊十七場、一個bye、同聯會十一場與跨聯會六場。日期、開球時間與場館均為TBD，不能當成已公告賽程。
- **`source/NFL_2046_Standings.csv`** — `[beta][LIVE]`：四十八隊季前戰績底稿；勝率為`(W + 0.5T) / GP`，只可由正式賽果更新。

NFL與TGL均為美式足球，但屬不同國家、聯盟及賽季資料。兩者共用彭斯制的場上本體時，先讀`source/TGL_League_and_Pence_Rules.md`第六至第十章；該檔的TGL名冊、十八場賽制與Taiwan Bowl不適用NFL。`history/ptt/football.md`為舊論壇式談話紀錄，只供編輯追溯，不得用來覆蓋本專檔，也不得由其中的評論生成未定檔隊名、Ownership或賽果。

### 5.7 台灣足球（TFPL）`[beta]`

- **`source/TFPL_lore.md`** — `[beta]`：十二球會、已確認的五名教練及MAFC歷史連結；未核准的名冊草案不因此升格。

### 5.8 FFA人物登錄補充

`hammershot/CPHL_Lore.md`、`hammershot/THCL_lore.md`、`hammershot/IHA_lore.md`與`hammershot/CL_lore.md`的人物欄位收錄經隊伍、姓名及永久ID核對的CSV守備位置。斜線表示多位置登錄；名冊位置不等於每場先發站位。PIA_rank、BAA_rank為本輪指定的雙軸敘薪評等方向，完整分級與薪級換算尚待舊規則確認，不得用CSV單一Rank代填。

### 5.10 體育正文、本體與判讀界線

- **patch/patch_Sports_Source_and_Generation.md** — [CRITICAL]：各節沿用原專檔效力；完整生成、資料消費與發布界線，必須與聯盟、場館及規則正文合讀。
- **source/CAPS_IFAST_Ontology.md** — [FINAL][CRITICAL]：IFAST上位框架與CAPS子系統完整定義；供應商及企業沿革仍見source/Hammershot_CAPS_IFAST_Ecosystem.md。
- **source/CPBL_Rating_Ontology.md** — [beta]：完整20–99評等欄位定義；不代表薪資、聲望或合約。
- **source/CPBL_lore.md** — 日本職業體育與有名稅完整專題已併入第五章，該章保留原FINAL效力；其餘聯盟主幹仍為beta。
- **source/League_Lore.md** — 金門民防與球隊哲學完整專題已併入同名章，保留FINAL／CRITICAL；既有正文不改。
- **source/TGL_2046_Venues.md** — 第六章收錄包道格巨蛋完整沿革、Hefty Bag、社區棒球與LLB國際分區，保留FINAL／CRITICAL。

## 6. 世界背景與公共生活

- **`patch/patch_Life_Mobility_Technology.md`** — HRO、都市艙、HydroTran、氣候、F路網及臺日／MSSB的既有適用界線；FINAL與beta分節維持，不新增事件、航線班表或法定參數。
- **`source/Federal_Life_Guide.md`區域移動與都市艙乘用生活** — 飲料Cell及HydroTran地域分工條目維持原專題FINAL效力；其他生活指南內容仍依原成熟度及專檔優先序。

- **`source/Nineties_Exploration_Spirit_lore.md`** — `[FINAL][CRITICAL]`：按舊式條目收錄2029年後90拓荒精神、大鳴大放、SLEK、飲食實驗、體育參與感與建築信任。電視分季及《同在厝下》細節併入`source/TV_Media_Lore.md`第四章；RunOS／UMPC細節併入`source/Key_Figures_tech.md`1.1.2及1.1.3。
- **`patch/patch_Nineties_Exploration_Spirit.md`** — `[FINAL][CRITICAL]`：90拓荒精神的年代、競爭、媒體、技術及建築適用邊界；與前檔合讀。
- **`source/Nineties_Exploration_Spirit.md`** — `[REFERENCE]`：保留舊檔名的路由入口，正文已分流至上述兩檔。
- **`source/TV_Media_Lore.md`** — `[beta]`：TVCO頻道、聯播網及媒體內容的既有資料；第三章〈Understand? Understand〉劇集的婚姻「主旋律」連結衝突時代世代缺口、男性死亡人數偏高，以及政府鼓勵就業冰河期與低薪失業世代男性於中年結婚。第五章收錄仲村曉雲的2010年代網路偶像身分疑雲，與丘仲堯同一人的說法尚無直接證據。舊式統獨對立是歷史立場，2029年後的創作方向以本節前列的90拓荒精神專檔為準。頻道與法人細目仍須同TVCO及媒體專檔交叉核對。
- **`source/Conflict.md`** — `[beta][CRITICAL]`：2025–2028衝突時代主幹紀事；具體結局以專題編年檔優先。 第五至第七章承接衝突時代、北歐與臺灣轉型補編全文，各章維持原FINAL效力，不將舊主幹整份升格。
- **`source/Geo_Politics.md`** — `[beta][CRITICAL]`：國家、聯盟、5+2 PAC及國際秩序。
- **`source/Cultural_Sphere.md`** — `[beta]`：語言、宗教、文化圈及跨國共同體。
- **`source/IMAS_Postwar_RAG_and_Song_Culture.md`** — `[beta][CRITICAL]`：狹間和歌子接手後的IM@S歌曲／正史包、私人RAG邊界、死亡與司法終局的合成演出，以及〈Automatic〉、〈真夏のダイヤ〉、〈Understand? Understand〉的公共文化語法。
- **釜山和解／Namco／三民體育會** — `[beta]`：企業重組與學園市三民區基地見`source/Key_Figures_tech.md`8.0；球隊營運、技術與演出關係見`source/League_Lore.md`「高雄三民體育會：Namco基地與765 Pro」。
- **`patch/patch_Busan_Reconciliation_Namco_Sanmin.md`** — `[beta]`：BNEI共同品牌、受託執行與控制權、競賽權限及未定資料的判定邊界。
- **`source/Busan_Reconciliation_Namco_Sanmin.md`** — `[REFERENCE]`：保留舊檔名的查找入口，正文已併入上述原檔。
- **`source/Climate_Weather.md`** — `[FINAL][CRITICAL]`：2046氣候基準、低溫與熱帶氣旋特徵；天氣生成界線與未決參數見`patch/patch_Life_Mobility_Technology.md`。
- **`source/Federal_Life_Guide.md`** — `[beta]`：一般生活制度。
- **`source/Urban_Pod_System_Ontology.md`** — `[FINAL][CRITICAL]`：都市艙一般型態、Hub與Hub 99及醫療／法警／軍用／CC／CT／BT1特殊艙的唯一正式定義；飲料Cell完整條目見`source/Federal_Life_Guide.md`，繞行、緊急降落與消歧見`patch/patch_Life_Mobility_Technology.md`，合讀效力不變。
- **`source/Tienmu_Bao_Doug_Metropolitan_Dome.md`** — [REFERENCE]：舊檔名入口；完整專題已併入`source/TGL_2046_Venues.md`，維持原效力；生成界線見`patch/patch_Sports_Source_and_Generation.md`。

### 6.1 媒體、演藝、歌曲與遊戲完整條目

- **source/TV_Media_Lore.md** — 保留既有媒體正文；第五章收錄演藝人物完整條目（原檔未標整體成熟度，不自動升格），第六章歌曲文化[beta][CRITICAL]，第七章FNC／UNN沿革及搭檔[FINAL][CRITICAL]。
- **source/IMAS_Public_Private_Continuity_Ontology.md** — [beta][CRITICAL]：公共正史／私人RAG、死亡與司法終局、合成聲紋完整定義。
- **source/Post_DSH_Game_Culture_lore.md** — [FINAL]：平台、作品、權利處理及遊戲文化完整條目；原檔名保留入口。
- **patch/patch_Media_Entertainment_Culture.md** — FNC／UNN生成硬鎖及IMAS待定項目；各節原效力不變。
- **patch/patch_Notebook_Journalist_Generation.md** — 記者候選生成及登錄流程，不能當作人物存在的正史證據。
- 舊source/Entertainment_2040s.md及source/IMAS_Postwar_RAG_and_Song_Culture.md保留查找入口；hammershot/TVCO.md、source/Cultural_Sphere.md及Bluebird人格檔本輪不改。

## 7. 2046衍生產品來源路由

### 7.1 PTT 2046 Generator R4

PTT 2046 Generator R4生成普通市民論壇，不使用Bluebird實名帳號。Notebook供應來源，PTT Gem是接收使用者事件與生成發／回文的前端；完整來源清單依目前Notebook實際收錄及本索引路由確認，舊發布包不是現行權威。

PTT Gem參照`regulation/Regulation_mother.md`與`regulation/Regulation_PTT.md`；前者管共同背景與消歧，後者管匿名論壇選角、推噓文及語氣。兩者為`[PRODUCT-CONTROL]`，不建立正史。Notebook不得再充當發／回文平台。

生成前至少遵守：

1. 先讀本索引、`source/Lore_Ontology.md`及`source/World_Master_Timeline.md`；Hammershot內容再讀`source/Hammershot_Absolute_Ontology.md`與`source/Hammershot_Public_Terminology_Protocol.md`，競賽執法細節另讀`source/hammershot_rulebook_fulltext.md`。
2. 城市話題須讀`source/Federal_Cities_List.md`，已定檔六市另讀對應城市專檔。
3. 人物話題須交叉核對`source/Social_Graph.md`、人物專檔及具體編年。
4. 賽程話題必須依日期查本索引第2節所列的相應`[LIVE]`賽季檔。
5. 論壇中的謠言、猜測與角色偏見不得升格為正史。

### 7.2 Bluebird 2046 R1

Bluebird 2046 R1生成實名公眾人物、組織與城市帳號動態。它與PTT 2046 Generator R4是不同介面，不得混用匿名論壇與認證身分。

`bluebird/Bluebird_Account_Registry*.md`、`bluebird/Bluebird_Personality_*.md`、`bluebird/Bluebird_Roster_Personality_*.md`及`bluebird/Bluebird_Casting_Rules.md`已收於專用資料夾，標記為`[PRODUCT-CONTROL]`：供名人Bluebird Gem查帳號資格、人格語氣與選角規則，但不建立人物生死、事件、隊籍、城市或制度正史。名人Gem參照`regulation/Regulation_mother.md`與`regulation/Regulation_Famous_person.md`；一般人Gem參照`regulation/Regulation_mother.md`與`regulation/Regulation_normal_person.md`，不得把名人帳號表當一般人名冊。兩種Notebook都只供應來源，不再生成貼文。`notebooklm_imports/*`只作編輯工作區、版本備份與舊包對照，不是可取用來源；同名檔既存時保留本庫版本，不由舊包覆寫。

生成前至少遵守：

1. 世界事實仍先讀本索引、`source/Lore_Ontology.md`、`source/World_Master_Timeline.md`及主題專檔；Bluebird帳號表與人格檔只控制誰能發言及如何發言，不能建立正史。
2. 城市話題須遵守六市專檔優先及96市分區檔案群`[beta]`的覆蓋限制。
3. 只有登錄於Bluebird帳號表且符合當期資格者可以本人發文；公開人物存在不等於自動具有認證帳號。
4. `source/Yamada_Mao_Lore.md`目前沒有為山田麻央建立Bluebird帳號。她可以被其他公開帳號討論，但不得由系統替她生成本人貼文。
5. 產品控制檔、帳號表與人格檔是生成約束，不是人物生死、案件結局或歷史事實的高階來源。

### 7.3 Gemini Notebook時間、詞義與別名防錯

Notebook來源集保留`patch/patch_Dictionary_Retrieval.md`、`dict/Dictionary_Entry_Ontology.md`、`dict/dic_Entity_Alias_Registry.md`、相關主題字典及`source/World_Master_Timeline.md`供Gem遇到歧義、年代或專業問題時檢索；普通閒聊不必逐詞跑完整辨義程序。`NEAR-CANDIDATE`與`MISNOMER-NEGATIVE`不得當成已命中別名。字典與別名表都不能單獨證明事件、當期所屬或職務；「日期未記載」不得自動補日。舊產品包的`PATCH_*` Hotfix已由本節所列四份現行Regulation吸收及校正，只保留於工作區備份，不再單獨上傳或作為Notebook來源。正史小寫`patch_*.md`仍依各主題索引使用，兩者不得混淆。

涉及Hammershot時，Notebook資料包必須同時載入`source/Hammershot_Absolute_Ontology.md`、`source/Hammershot_Public_Terminology_Protocol.md`、`source/hammershot_rulebook_fulltext.md`及`dict/dic_02A_Hammershot.md`。其中`history/legacy/Hammershot_Rulebook.md`為`[SUPERSEDED]`歷史摘要，不得上傳。若原始賽務資料包含Pitcher、Batter、Strike、Ball、Inning、Home Run、RBI、ERA等欄位，必須先依公開術語協議轉譯，再生成敘事或回答。

### 7.4 CSV作為Notebook來源的選擇閘門

`source/*.csv`是可在對應本體論及狀態欄約束下查詢的現行機器表，不代表應整批上傳Notebook。先載入對應`_lore`、`_ontology`及賽季說明；只有提問需要精確逐列查姓名、隊籍、賽程、學校或GSD時，才挑選該領域、該年度的CSV。候選學校、教育來源清冊、正規化隊列及P1/P2待核稽核表已存入工作區`C:/hammershot/notebooklm_imports/csv_working_only/`，不作Notebook來源；逐檔判定見`C:/hammershot/notebooklm_imports/csv_source_decisions_20261003.md`。NFL草案賽程不得寫成正式公告；`[LIVE]`戰績表需於變更後更新來源，舊上傳副本不可當最新結果。口述談話紀錄不因具有檔名或被字典提過就取得上傳資格。

## 8. 禁止作為正史來源

下列資料不得上傳至兩套Generator，也不得單獨建立正史：

- `LORE_CONSUMPTION.md`、`modification_compare.md`、`thread_import_*`。
- `lore_revision_staging/*`、`archive/*`、備份、差異檔及稽核報告。
- `notebooklm_imports/*`中的舊快取；發布包只是正史鏡像，不是更高權威。
- `history/ptt/megapack1.md`、`history/ptt/megapack2.md`、`history/ptt/UN.md`、`history/ptt/FS.md`、`history/ptt/football.md`、`history/ptt/HS2.md`、日期式論壇輸出、PTT生成稿及`prototype/*`。這些談話紀錄只供編輯追溯，不得直接充當正史來源。其中陽子的舊「😊→😐→🫥→😭」固定階段、金髮及身材比較敘事已撤銷，不能因原始文字仍供編輯考證便回填任何產品；現行人物設定只查`source/Social_Graph.md`及`patch/patch_Person_Social_Graph.md`。
- `history/legacy/household.md`、`history/legacy/household2.md` — `[SUPERSEDED]`：HRO名冊已抽取至`source/HRO_System_Ontology.md`；兩檔只供編輯考證。
- `history/legacy/fedaddress.md`等早期衍生稿只供編輯考證；已抽取至定檔專檔的內容以專檔為準。
- Season Sim的handoff、health、telemetry、GM私密資料與測試輸出。
- 名稱含stage、smoke、replay、integration、calibration、balance或test的測試資料夾。

上述檔案可以供編輯考證，但不得把其中的推測、`[Source]`、`[Conversation History]`或生成式解說直接複製成正史。

## 9. 維護規則

1. 新專檔完成時，同步更新本索引的成熟度、主題路由及衝突優先序。
2. 檔案由`[beta]`升為`[FINAL]`，必須有明確定檔決定；不得因篇幅很長而自動升格。
3. 城市分區檔案群只有在96市覆蓋完成並完成衝突檢查後，才能移除群組層級的`[beta]`。
4. canonical lore變更後，Gemini Notebook發布包必須重新同步；本機檔案不會自動更新遠端Notebook。
5. 衍生產品發現矛盾時，只能回報；未經授權不得直接改寫canonical lore。
