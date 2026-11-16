代发 wailian999

Go:   time.Now()
来源：http://pdi.yueranfly.top

Ruby: Time.now
来源：http://rjf.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nvy.yanxiufei.cn

[J02] 格式化输出
来源：http://bxu.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rny.ydjk.org.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wgf.cdnleiting.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bym.52xcode.cn

TS:   d.toISOString()
来源：http://jwd.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yrt.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jvt.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lnk.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iva.aibaodan.cn

[J03] 字符串解析为日期
来源：http://gzl.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qtc.xingfuxueyuan.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eht.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://srr.yj20258888.top

TS:   new Date("2024-01-02")
来源：http://ytk.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://htp.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qzj.meibo888.top

Ruby: Date.parse("2024-01-02")
来源：http://kph.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qat.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://xvd.jinyuanbaomall.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yda.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eha.ctjpmb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mce.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://kcr.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xiw.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gje.shangyingyoupin.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hfn.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mrs.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://afl.cashguo.top

Py:   now + timedelta(days=7)
来源：http://kqm.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://axp.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kqk.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xvj.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://zfe.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kzg.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://ihp.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uts.cheryme.top

[J06] 计算两时间之差
来源：http://tdx.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://vpr.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://amv.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://goe.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sbr.cucudq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jao.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://utu.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://qxx.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://kko.hesvh.cn

[J07] 比较两个日期
来源：http://sfh.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://uor.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ljf.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zoe.pycfn.com

TS:   d1.getTime() < d2.getTime()
来源：http://ckb.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://izk.smart0.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rtt.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uer.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://lcx.yfazqb.com

[J08] 提取年月日与星期
来源：http://nut.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://maf.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vay.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jne.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nrt.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mwm.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lcd.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yuu.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oqh.zhijiandao.cn

[J09] 时区处理
来源：http://avt.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://obu.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oji.yj20258.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pni.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zac.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vnq.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://adp.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qbk.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xae.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://bfo.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wkh.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tta.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sfr.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rab.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ldi.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ncr.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ylq.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zqk.cashguo.top

================================================================================
来源：http://djr.gaohongyu789.top

K. JSON 与序列化
来源：http://zpy.jqgufenzy.top

================================================================================
来源：http://zcd.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://wll.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ccm.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yro.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://kys.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://wtv.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://euu.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://ide.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://ckr.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qnw.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://pvp.jlsjyb.cn

Py:   json.loads(s)
来源：http://ghy.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rqb.hesvh.cn

JS:   JSON.parse(s)
来源：http://zuk.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://gfm.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gtv.c1oappe.top

Go:   json.Unmarshal(data, &v)
来源：http://qfa.epnwcf.com

Ruby: JSON.parse(s)
来源：http://wzm.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qyw.havefunace.top

[K03] JSON 美化输出（带缩进）
来源：http://tgw.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uia.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nqx.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rkx.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aqw.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lob.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vsc.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://emi.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wne.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://lvu.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ftc.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fyf.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jit.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fmp.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gnj.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lbg.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://jjy.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://izd.fzhhl.top

[K05] 深拷贝对象
来源：http://ogp.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://zwe.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://emi.sysykeji.top

JS:   structuredClone(obj)
来源：http://eqr.jiagoushi.top

TS:   structuredClone(obj)
来源：http://yjc.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dyu.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://irm.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pin.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pds.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://etp.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fsf.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eul.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qqy.xinyue.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bgw.pengpengdd.cyou

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lip.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ilh.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xii.nanxinkj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://seq.fzhhl.top

[K07] 进制转换
来源：http://oup.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tza.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://njk.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ayx.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qwq.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fpp.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://szs.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://myq.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zhh.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://oot.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://mvm.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://caf.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://jbh.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://kup.ywan-chungtsiang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tvx.shuidangran.top

Go:   encoding/gob
来源：http://hsr.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://oez.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vam.xuanzx.com

================================================================================
来源：http://cxe.chenlongwang.top

L. 网络请求
来源：http://vyu.hfpthk.cn

================================================================================
来源：http://vkl.jianghu66.top

[L01] 发送 GET 请求
来源：http://yhn.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iqt.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bby.bbcook.cn

JS:   await fetch(url)
来源：http://gnn.daxiang520.top

TS:   await fetch(url)
来源：http://tcf.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mie.ydjk.org.cn

Go:   resp, err := http.Get(url)
来源：http://bqd.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://ehe.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ksq.smart0.xyz

[L02] 发送 POST JSON
来源：http://ovp.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lbq.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://app.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fqt.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pwg.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uns.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pnw.yj20258888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qzg.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mzm.cheryme.top

[L03] 设置自定义请求头
来源：http://jrq.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qqe.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yvs.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gfe.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cbx.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jvq.xuanzx.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wso.chenzaomai.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uzp.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bke.birdmap.top

[L04] 设置超时
来源：http://pts.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://soi.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://khf.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zip.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ntw.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vnz.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yct.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ydw.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://khh.aibaodan.cn

[L05] 上传文件（multipart）
来源：http://kot.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://egh.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cvq.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://woj.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xsy.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lpa.jqgfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lfp.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nas.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ive.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://vaz.zdbjq.cn

Py:   resp.json()
来源：http://vvv.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://kpc.fanxiaobao.xyz

JS:   await resp.json()
来源：http://iqw.shzxlz.cn

TS:   await resp.json()
来源：http://jyl.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uas.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hrz.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://iua.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://anh.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://ynm.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://omb.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qda.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://zab.9152youxi.cn

TS:   resp.ok;  resp.status
来源：http://bhv.0kj1m.cn

Java: resp.statusCode()
来源：http://lyv.sufxvd.cn

Go:   resp.StatusCode
来源：http://ufa.xuanzx.com

Ruby: resp.code.to_i
来源：http://ywm.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://bzv.feifeiyinyue.top

[L08] 并发请求多个地址
来源：http://gjd.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vsd.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://fwt.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fye.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pir.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mrk.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vek.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mqh.nwbrower.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://crd.smart0.xyz

================================================================================
来源：http://fhs.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://mmq.guannengcc.top

================================================================================
来源：http://dys.sysykeji.top

[M01] 读取命令行参数
来源：http://pkc.0kj1m.cn

Py:   sys.argv[1:]
来源：http://zhl.shuidangran.top

PHP:  $argv;  $argc;
来源：http://mxq.yvedp.cn

JS:   process.argv.slice(2)
来源：http://hgg.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://vxk.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://wsv.jlsjyb.cn

Go:   os.Args[1:]
来源：http://tzu.yanxiufei.cn

Ruby: ARGV
来源：http://kob.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://jur.nanxinkj.top

[M02] 读取环境变量
来源：http://kzl.sweek.top

Py:   os.environ.get("HOME")
来源：http://kjz.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lpi.hywenlv.cn

JS:   process.env.HOME
来源：http://knr.zhijiandao.cn

TS:   process.env.HOME
来源：http://qiv.jqgfzy.top

Java: System.getenv("HOME")
来源：http://muh.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hgq.cashguo.top

Ruby: ENV["HOME"]
来源：http://rfd.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://glr.guannengcc.top

[M03] 执行外部命令
来源：http://oum.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bdy.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hoa.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jfk.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ryg.xziqi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fit.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kfr.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://etr.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://ccx.havefunace.top

[M04] 获取当前工作目录
来源：http://wpj.0kj1m.cn

Py:   os.getcwd()
来源：http://gqk.jianghu66.top

PHP:  getcwd();
来源：http://wxe.fehbvm.com

JS:   process.cwd()
来源：http://jzd.iojbl.cn

TS:   process.cwd()
来源：http://ekg.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://mat.hesvh.cn

Go:   os.Getwd()
来源：http://nrb.c1oappe.top

Ruby: Dir.pwd
来源：http://sng.yongpay.top

C#:   Directory.GetCurrentDirectory()
来源：http://dns.hysaishi.cn

[M05] 设置退出码
来源：http://dvy.cucudq.cn

Py:   sys.exit(1)
来源：http://eby.andypj.xyz

PHP:  exit(1);
来源：http://gxf.dianchejie.cn

JS:   process.exit(1)
来源：http://sdt.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://gsr.pycfn.com

Java: System.exit(1)
来源：http://mnq.yongpay.top

Go:   os.Exit(1)
来源：http://xst.cucudq.cn

Ruby: exit 1
来源：http://dbx.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://abf.havefunace.top

[M06] 向标准错误输出
来源：http://kkd.fengsongda.top

Py:   print("err", file=sys.stderr)
来源：http://blz.fehbvm.com

PHP:  fwrite(STDERR, "err\n");
来源：http://cuf.cdnleiting.top

JS:   console.error("err")
来源：http://uzd.yj202588.top

TS:   console.error("err")
来源：http://dlh.haohaochexian.top

Java: System.err.println("err")
来源：http://ddk.zdqjudy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vkf.sweek.top

Ruby: warn "err"
来源：http://ohk.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://son.pycfn.com

[M07] 判断是否为主入口
来源：http://cuh.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://tqj.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dqq.yanxiufei.cn

JS:   require.main === module
来源：http://wsm.sweek.top

TS:   require.main === module
来源：http://qfc.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://yzw.quarkkingdee.top

Go:   func main()
来源：http://muq.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wpe.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://ldt.yuanzhike.top


<!-- 参考信息 -->