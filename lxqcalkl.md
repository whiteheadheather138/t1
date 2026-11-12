代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vsy.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://scr.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pfz.cashguo.top

================================================================================
来源：http://zrk.gaohongyu789.top

J. 日期与时间
来源：http://eny.jlsjyb.cn

================================================================================
来源：http://bbx.jianghu66.top

[J01] 获取当前时间
来源：http://bop.chenlongwang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ptq.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://csu.havefunace.top

JS:   new Date();  Date.now()
来源：http://moc.yueranfly.top

TS:   new Date();  Date.now()
来源：http://bxy.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://asa.c1oappe.top

Go:   time.Now()
来源：http://sql.dianchejie.cn

Ruby: Time.now
来源：http://nmy.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://moe.sjlbkw.cn

[J02] 格式化输出
来源：http://mjv.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://svs.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fio.316326.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sje.guowangkeji.top

TS:   d.toISOString()
来源：http://naz.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qoi.316326.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pwk.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jom.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://egj.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://sos.shangyingyoupin.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qyr.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jer.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://nsy.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://exl.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://fcc.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yfo.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://ggx.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jhl.ppjwa.cn

[J04] 时间戳与日期互转
来源：http://tex.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rwj.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lxw.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jhd.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://yuh.hnqzz.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rst.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ezk.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bri.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xua.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://gjg.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://yts.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rhy.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xyu.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ewq.sxryk.cn

Java: LocalDate.now().plusDays(7)
来源：http://vro.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rbm.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://wsy.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://udm.gotoacloud.top

[J06] 计算两时间之差
来源：http://fmd.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://zpz.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://xup.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mdi.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ozk.daria6918.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bgd.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://nde.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://cna.fehbvm.com

C#:   (end - start).TotalSeconds
来源：http://pmw.jqgufenzy.top

[J07] 比较两个日期
来源：http://wba.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://peo.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mhx.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zhw.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://knm.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ndy.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qul.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ewk.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://bzy.zdqjudy.top

[J08] 提取年月日与星期
来源：http://zwc.birdmap.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kkv.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nqm.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wpd.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bqp.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://usy.shanyushiyangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ego.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dxm.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ltm.fzhhl.top

[J09] 时区处理
来源：http://vvw.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ebp.nanxinkj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tav.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dsv.feifeiyinyue.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xqg.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zat.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rud.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nsr.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fwb.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://das.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hsv.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xtn.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nkh.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oit.nanxinkj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ael.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ahh.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://spt.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kyc.jiagoushi.top

================================================================================
来源：http://bmi.smart0.xyz

K. JSON 与序列化
来源：http://lew.guannengcc.top

================================================================================
来源：http://nug.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://bwj.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jsv.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xbo.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://kln.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://fty.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://llf.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://gew.kuanghao11.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vcs.ivvv.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vxj.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://xsg.hammf.cn

Py:   json.loads(s)
来源：http://grs.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pvr.haohaochexian.top

JS:   JSON.parse(s)
来源：http://yzq.nwbrower.top

TS:   JSON.parse(s)
来源：http://kpk.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zku.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://xyz.cashguo.top

Ruby: JSON.parse(s)
来源：http://dmr.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wzw.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://fav.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fwo.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fwb.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ono.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zhh.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wgy.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://clv.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://iuo.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sev.sysykeji.top

[K04] 读取 JSON 文件
来源：http://bbo.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pek.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ewl.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bzz.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hks.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://val.svipenyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ibw.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://csv.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wfh.gaohongyu789.top

[K05] 深拷贝对象
来源：http://lii.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://bpk.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://vsb.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://ydu.jiagoushi.top

TS:   structuredClone(obj)
来源：http://ejf.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://avv.hywenlv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fsr.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://syb.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://efm.meibo888.top

[K06] 解析 URL 查询串
来源：http://hkx.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gar.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fry.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://msw.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vaf.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kaf.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gcx.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yku.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yak.zycfv.cn

[K07] 进制转换
来源：http://izf.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kag.kuanghao11.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qhi.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cjw.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hna.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yar.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://osl.xuanzx.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hen.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gzi.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://znp.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://xvl.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pfn.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://sgv.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://fsn.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sbp.cucudq.cn

Go:   encoding/gob
来源：http://sya.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://bgu.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nvs.xziqi.cn

================================================================================
来源：http://dsc.fktsv.cn

L. 网络请求
来源：http://ofc.fehbvm.com

================================================================================
来源：http://alb.aizwys.cn

[L01] 发送 GET 请求
来源：http://laa.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vkw.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rzf.jqgufenzy.top

JS:   await fetch(url)
来源：http://oai.jyoumei.cn

TS:   await fetch(url)
来源：http://mtk.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ltb.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://aij.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yry.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qmz.jqgufenzy.top

[L02] 发送 POST JSON
来源：http://tvx.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://sli.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bfa.iojbl.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vzm.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jpa.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vst.snrcjt.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ste.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://teu.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hpo.0kj1m.cn

[L03] 设置自定义请求头
来源：http://bhr.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fjg.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qxm.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jgn.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ynb.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kra.yonumen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jlc.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fnb.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ysa.ivvv.top

[L04] 设置超时
来源：http://cum.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://ttr.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nrr.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nls.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zbk.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xuq.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aeq.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zbc.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dld.52xcode.cn

[L05] 上传文件（multipart）
来源：http://nur.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dzi.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bsw.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pmf.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jhz.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bsr.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ihy.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ysn.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sah.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://gjk.jinqigfzy.top

Py:   resp.json()
来源：http://fyc.316326.xyz

PHP:  json_decode($body, true);
来源：http://xgd.andypj.xyz

JS:   await resp.json()
来源：http://nyo.aizwys.cn

TS:   await resp.json()
来源：http://enq.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eoa.jinyuanbaomall.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dfm.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://ywu.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mbf.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://cdd.gogol.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eqb.meibo888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vfo.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://gno.daria6918.cn

TS:   resp.ok;  resp.status
来源：http://mnq.yonumen.top

Java: resp.statusCode()
来源：http://gdp.kuanghao11.cn

Go:   resp.StatusCode
来源：http://ktr.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://ynq.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://jiy.chenlongwang.top

[L08] 并发请求多个地址
来源：http://izb.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://idx.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://yqs.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://otz.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zqf.epnwcf.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lyz.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cti.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hbe.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lyj.guowangkeji.top

================================================================================
来源：http://vvh.dashuyun.cn

M. 命令行 / 进程 / 环境
来源：http://qzg.guowangkeji.top

================================================================================
来源：http://rky.shuidangran.top

[M01] 读取命令行参数
来源：http://nyq.ivvv.top

Py:   sys.argv[1:]
来源：http://zgg.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://bqc.yueranfly.top

JS:   process.argv.slice(2)
来源：http://axd.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://epz.jyoumei.cn

Java: args 数组（main 方法参数）
来源：http://jdi.nwbrower.top

Go:   os.Args[1:]
来源：http://pmj.shangyingyoupin.top

Ruby: ARGV
来源：http://njv.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://uhj.fengsongda.top

[M02] 读取环境变量
来源：http://xpz.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://pzo.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nyc.jqgfzy.top

JS:   process.env.HOME
来源：http://brd.quarkkingdee.top

TS:   process.env.HOME
来源：http://mjs.cashguo.top

Java: System.getenv("HOME")
来源：http://lja.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dpv.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://byl.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://diy.uphjek.com

[M03] 执行外部命令
来源：http://goj.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qja.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xla.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nio.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rux.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yvn.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mum.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wfz.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://xfl.hnqzz.top

[M04] 获取当前工作目录
来源：http://erx.chenjidiqi.icu

Py:   os.getcwd()
来源：http://tck.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://fzh.fanxiaobao.xyz

JS:   process.cwd()
来源：http://oiy.zdqjudy.top

TS:   process.cwd()
来源：http://iug.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://sdn.ybcxt.top

Go:   os.Getwd()
来源：http://srl.zhoulong.xyz

Ruby: Dir.pwd
来源：http://wqw.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fmm.bbcook.cn

[M05] 设置退出码
来源：http://dvc.hcnkem.com

Py:   sys.exit(1)
来源：http://soi.fengsongda.top

PHP:  exit(1);
来源：http://fcx.cucudq.cn

JS:   process.exit(1)
来源：http://zby.jiagoushi.top

TS:   process.exit(1)
来源：http://quv.sjlbkw.cn

Java: System.exit(1)
来源：http://wew.hysaishi.cn

Go:   os.Exit(1)
来源：http://ejw.wangshuangyany.cn

Ruby: exit 1
来源：http://bgr.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zrx.cheryme.top

[M06] 向标准错误输出
来源：http://eox.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://gwi.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://vxm.jyoumei.cn

JS:   console.error("err")
来源：http://ejo.yj202588.top

TS:   console.error("err")
来源：http://pjl.ctjpmb.com

Java: System.err.println("err")
来源：http://kdv.sysykeji.top


<!-- 参考信息 -->