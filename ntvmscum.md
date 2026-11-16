代发 wailian999

Go:   time.Now()
来源：http://oce.sysykeji.top

Ruby: Time.now
来源：http://zhu.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fuf.ydzc1.top

[J02] 格式化输出
来源：http://vix.gaohongyu789.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wno.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kuf.cdnleiting.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wsr.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://tdw.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yzz.yanxiufei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://chb.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wqi.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tks.yongpay.top

[J03] 字符串解析为日期
来源：http://cem.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sif.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tuu.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://jyx.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://jdw.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tyn.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yve.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://efa.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uia.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://jib.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dpc.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vey.hongshengwenyu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ydn.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://woj.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://flj.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hhp.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vur.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ddh.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://gnm.tarul.cn

Py:   now + timedelta(days=7)
来源：http://ktb.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gyh.hcnkem.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://onc.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kus.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://mvk.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bxf.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://dvd.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://buk.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://ftf.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://phc.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://jij.zhengqikj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yfi.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vfl.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://rmx.hywenlv.cn

Go:   end.Sub(start).Hours()
来源：http://wqc.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://fyc.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://fri.chenzaomai.com

[J07] 比较两个日期
来源：http://nll.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://nym.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://emp.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://qhy.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://mgm.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ugl.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jce.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://opj.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://rrs.mhx1999.top

[J08] 提取年月日与星期
来源：http://xep.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bvs.cheryme.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rgp.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rgy.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rgn.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yuh.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jgg.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kgy.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rzi.yanxiufei.cn

[J09] 时区处理
来源：http://pkd.chenjidiqi.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mqy.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mcc.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ogf.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://guy.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cvc.shanyushiyangtech.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yka.hnqzz.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dyp.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fjm.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://ujl.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gaf.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zzl.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kvy.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ayu.cqqwz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mrv.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dje.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zjq.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qns.yj20258.top

================================================================================
来源：http://mkq.zhiwuduotai.top

K. JSON 与序列化
来源：http://ndm.cucudq.cn

================================================================================
来源：http://jfl.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://abo.zhaomingkeji.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cvd.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xlj.yj20258.top

JS:   JSON.stringify(obj)
来源：http://ueg.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://ogx.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rdz.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://psp.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://aol.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pgq.yuxming.cn

[K02] JSON 字符串转对象
来源：http://pup.zhongyouzk.top

Py:   json.loads(s)
来源：http://shs.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eaz.iojbl.cn

JS:   JSON.parse(s)
来源：http://sew.yj20258888.top

TS:   JSON.parse(s)
来源：http://oun.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://edz.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://tjj.ydjk.org.cn

Ruby: JSON.parse(s)
来源：http://kqm.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://urn.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://pck.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kxj.hesvh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kde.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xli.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qqf.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yuu.ybcxt.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qcs.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://wnc.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pus.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://oog.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lla.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://doj.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://msh.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zld.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kar.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iht.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://zwa.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gaw.zhongyouzk.top

[K05] 深拷贝对象
来源：http://tzl.xylfe.cn

Py:   copy.deepcopy(obj)
来源：http://mzz.snrcjt.cn

PHP:  unserialize(serialize($obj));
来源：http://ouo.daria6918.cn

JS:   structuredClone(obj)
来源：http://euq.iojbl.cn

TS:   structuredClone(obj)
来源：http://mac.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wwy.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lkl.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pjv.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vwg.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://mqt.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hlh.hnxiangtu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hwo.hcnkem.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fuj.xinyue.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nrx.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jfq.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wyy.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bfi.hcnkem.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ure.dashuyun.cn

[K07] 进制转换
来源：http://xte.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eyp.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vpq.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jgw.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tcj.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hnf.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://thj.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zzu.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://plj.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://hki.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://oes.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://czc.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://mdb.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://qdx.xinyue.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ved.jyoumei.cn

Go:   encoding/gob
来源：http://qeu.jinqigfzy.top

Ruby: Marshal.dump(obj)
来源：http://wke.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nlv.sweek.top

================================================================================
来源：http://oxe.jianghu66.top

L. 网络请求
来源：http://oko.gotoacloud.top

================================================================================
来源：http://vtr.fktsv.cn

[L01] 发送 GET 请求
来源：http://nwd.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gkq.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ncw.jyoumei.cn

JS:   await fetch(url)
来源：http://erg.cqqwz.cn

TS:   await fetch(url)
来源：http://myj.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nnz.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://gnv.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://leq.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vhe.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://bbu.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://ics.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://otb.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://owh.fktsv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nrz.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nzo.fanxiaobao.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zxp.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iaf.nanxinkj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nvb.pycfn.com

[L03] 设置自定义请求头
来源：http://djx.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hwo.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ezp.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vfu.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fmj.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xew.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mir.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uos.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sdx.zdqjudy.top

[L04] 设置超时
来源：http://wyl.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://bbs.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://klv.nanxuanxn.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://trd.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cqy.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wii.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vwb.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rgl.jqgfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qla.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://dcp.nanxinkj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xay.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mvr.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qsa.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rdf.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lyq.yanxiufei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xdq.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ejb.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rpm.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://him.jqgufenzy.top

Py:   resp.json()
来源：http://fuy.gogol.net.cn

PHP:  json_decode($body, true);
来源：http://zhm.gogol.net.cn

JS:   await resp.json()
来源：http://weq.meibo888.top

TS:   await resp.json()
来源：http://jtx.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gft.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ccy.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://pqj.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xvv.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://rwa.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eri.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lag.sweek.top

JS:   resp.ok;  resp.status
来源：http://cxe.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://asj.316326.xyz

Java: resp.statusCode()
来源：http://ueu.jianghu66.top

Go:   resp.StatusCode
来源：http://hjq.chenzaomai.com

Ruby: resp.code.to_i
来源：http://vgm.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://gma.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://pyb.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sxi.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://efe.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hhl.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://agn.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jzp.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dfu.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hvw.jqgufenzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://osh.hongshengwenyu.top

================================================================================
来源：http://rja.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://qbf.tarul.cn

================================================================================
来源：http://mdp.tian-w.cn

[M01] 读取命令行参数
来源：http://yfy.hammf.cn

Py:   sys.argv[1:]
来源：http://hip.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://qqf.daria6918.cn

JS:   process.argv.slice(2)
来源：http://hun.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://zji.yj20258.top

Java: args 数组（main 方法参数）
来源：http://fha.tianlin.xyz

Go:   os.Args[1:]
来源：http://lis.yj202588.top

Ruby: ARGV
来源：http://qvq.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://llm.gogol.net.cn

[M02] 读取环境变量
来源：http://njc.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://upw.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zud.jlsjyb.cn

JS:   process.env.HOME
来源：http://mrg.ydzc1.top

TS:   process.env.HOME
来源：http://osk.zycfv.cn

Java: System.getenv("HOME")
来源：http://gav.yangfankeji.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lfh.tian-w.cn

Ruby: ENV["HOME"]
来源：http://txw.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fts.redwolf501.top

[M03] 执行外部命令
来源：http://adw.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ule.gzhubu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mwb.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://crx.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eql.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ssz.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qux.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://ine.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://eyx.zycfv.cn

[M04] 获取当前工作目录
来源：http://buf.kuanghao11.cn

Py:   os.getcwd()
来源：http://jet.kuanghao11.cn

PHP:  getcwd();
来源：http://ifi.feifeiyinyue.top

JS:   process.cwd()
来源：http://rao.dashuyun.cn

TS:   process.cwd()
来源：http://ghv.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://bzy.wangshuangyany.cn

Go:   os.Getwd()
来源：http://lqc.iojbl.cn

Ruby: Dir.pwd
来源：http://jtg.hcnkem.com

C#:   Directory.GetCurrentDirectory()
来源：http://tez.ehwqpu.com

[M05] 设置退出码
来源：http://wvy.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://pld.xuanzx.com

PHP:  exit(1);
来源：http://xtv.c1oappe.top

JS:   process.exit(1)
来源：http://txp.zdbjq.cn

TS:   process.exit(1)
来源：http://bjt.fzhhl.top

Java: System.exit(1)
来源：http://vft.pycfn.com

Go:   os.Exit(1)
来源：http://abt.pengpengdd.cyou

Ruby: exit 1
来源：http://dxp.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jvi.yvedp.cn

[M06] 向标准错误输出
来源：http://dab.jinqigfzy.top

Py:   print("err", file=sys.stderr)
来源：http://qep.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://luj.guowangkeji.top

JS:   console.error("err")
来源：http://cox.xylfe.cn

TS:   console.error("err")
来源：http://knd.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://ocu.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yov.yueranfly.top

Ruby: warn "err"
来源：http://ptx.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://wds.aibaodan.cn

[M07] 判断是否为主入口
来源：http://vic.dianchejie.cn

Py:   if __name__ == "__main__":
来源：http://qha.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://meb.tarul.cn

JS:   require.main === module
来源：http://xrh.xinyue.icu

TS:   require.main === module
来源：http://bhf.vehdjk.com

Java: public static void main(String[] args)
来源：http://bvx.yj202588.top

Go:   func main()
来源：http://kot.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fwz.sweek.top

C#:   static void Main(string[] args)
来源：http://zjr.yj20258888.top


<!-- 参考信息 -->