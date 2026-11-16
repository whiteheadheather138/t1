代发 wailian999

[J03] 字符串解析为日期
来源：http://cok.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://znc.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://muq.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://qrr.xinyue.icu

TS:   new Date("2024-01-02")
来源：http://kxl.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://rcw.guowangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lkl.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://rdo.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uyd.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://vvu.jinghuilouyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nay.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ohl.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://waa.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vjv.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://idz.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rkg.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://leb.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ngt.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://xvl.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://nvi.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ltk.xylfe.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qtp.xinyue.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ycv.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://zhk.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hrc.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://jnz.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://urs.snrcjt.cn

[J06] 计算两时间之差
来源：http://puk.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://ijg.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://rcq.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hdm.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wrz.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jvx.birdmap.top

Go:   end.Sub(start).Hours()
来源：http://wpg.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://cab.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://acb.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://ejw.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://lvu.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lsf.quarkkingdee.top

JS:   d1.getTime() < d2.getTime()
来源：http://scm.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://wzz.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pqb.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bbx.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rod.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://nei.gotoacloud.top

[J08] 提取年月日与星期
来源：http://utq.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kag.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vdv.yanxiufei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hci.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qia.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mta.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mll.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uce.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hsn.jqgfzy.top

[J09] 时区处理
来源：http://qgd.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uhk.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://les.cqqwz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wwe.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hch.fzhhl.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://haq.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yli.fktsv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hhn.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://phr.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://igx.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xuy.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rgc.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ksm.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://utk.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://akr.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://awq.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ogy.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ffb.cqqwz.cn

================================================================================
来源：http://bqe.jlsjyb.cn

K. JSON 与序列化
来源：http://nyd.zhaomingkeji.xyz

================================================================================
来源：http://fxu.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://dbr.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lyp.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lad.fehbvm.com

JS:   JSON.stringify(obj)
来源：http://jhw.uphjek.com

TS:   JSON.stringify(obj)
来源：http://pzq.yanxiufei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uzo.fengsongda.top

Go:   json.Marshal(obj)
来源：http://jmu.chenlongwang.top

Ruby: obj.to_json                                     // require "json"
来源：http://utf.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uhy.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://rbw.zhijiandao.cn

Py:   json.loads(s)
来源：http://sou.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hbm.sweek.top

JS:   JSON.parse(s)
来源：http://mmf.jinqigufen.top

TS:   JSON.parse(s)
来源：http://ccq.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vfa.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://mke.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://fww.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tgh.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://rym.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pjy.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oxj.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mpz.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fxg.hcnkem.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hgu.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pfi.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fod.nwbrower.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iky.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://mjy.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vhg.quarkkingdee.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://epn.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uje.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jlj.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yng.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gxy.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://pin.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lcl.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://auj.ydjk.org.cn

Py:   copy.deepcopy(obj)
来源：http://czs.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://ube.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://ves.ehwqpu.com

TS:   structuredClone(obj)
来源：http://hvr.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://egb.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pjh.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jnr.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eud.cashguo.top

[K06] 解析 URL 查询串
来源：http://frc.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://win.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xqj.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gkr.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yrj.shzxlz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://djp.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://obv.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dec.cashguo.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ftk.jiagoushi.top

[K07] 进制转换
来源：http://avf.ywan-chungtsiang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tdb.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fgf.xziqi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rfv.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tzm.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xga.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wqx.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pqd.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hwo.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://eed.sysykeji.top

Py:   pickle.dumps(obj)
来源：http://rpz.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lyo.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://mqu.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://lmz.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hfm.zdbjq.cn

Go:   encoding/gob
来源：http://bxa.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://bok.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lrv.hywenlv.cn

================================================================================
来源：http://lyq.xinyue.icu

L. 网络请求
来源：http://mvy.nanxuanxn.top

================================================================================
来源：http://gps.hnqzz.top

[L01] 发送 GET 请求
来源：http://ebl.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fjr.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://edj.uphjek.com

JS:   await fetch(url)
来源：http://oqe.dianchejie.cn

TS:   await fetch(url)
来源：http://isb.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cgg.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://sze.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xuc.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mds.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://myb.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nwd.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lvl.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rak.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://omr.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://myn.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hdu.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pbj.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qnq.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://vuf.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ucw.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://whn.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lqh.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pkv.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mjm.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gbh.zhiwuduotai.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tun.redwolf501.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tmt.zycfv.cn

[L04] 设置超时
来源：http://ytg.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://xrw.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aoh.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xxe.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lbf.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kkp.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dea.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oxs.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ici.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://lok.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ktk.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://crw.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pol.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hrl.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://znl.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mzc.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bzw.kuanghao11.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gtr.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://lmg.yj20258.top

Py:   resp.json()
来源：http://ehy.xylfe.cn

PHP:  json_decode($body, true);
来源：http://nar.yonumen.top

JS:   await resp.json()
来源：http://gdk.ehwqpu.com

TS:   await resp.json()
来源：http://lqn.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bsr.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qtr.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://tmo.fanxiaobao.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ubj.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://qpk.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hti.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rlv.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://cjf.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://pdh.fktsv.cn

Java: resp.statusCode()
来源：http://yai.wangdashe.top

Go:   resp.StatusCode
来源：http://btr.hongshengwenyu.top

Ruby: resp.code.to_i
来源：http://jmr.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://zcb.gzhubu.top

[L08] 并发请求多个地址
来源：http://cfi.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lim.zhongyouzk.top

PHP:  curl_multi_init() 系列
来源：http://wgn.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zbs.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zrd.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gvq.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sns.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wul.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://slb.zdbjq.cn

================================================================================
来源：http://pgx.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://sax.cheryme.top

================================================================================
来源：http://agr.sysykeji.top

[M01] 读取命令行参数
来源：http://wbr.cdnleiting.top

Py:   sys.argv[1:]
来源：http://jqn.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://khq.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://tri.xziqi.cn

TS:   process.argv.slice(2)
来源：http://qem.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://axz.9152youxi.cn

Go:   os.Args[1:]
来源：http://alb.cashguo.top

Ruby: ARGV
来源：http://qis.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://ytv.shangyingyoupin.top

[M02] 读取环境变量
来源：http://mqx.shanyushiyangkeji.top

Py:   os.environ.get("HOME")
来源：http://upc.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nfh.jyoumei.cn

JS:   process.env.HOME
来源：http://hdm.yj202588.top

TS:   process.env.HOME
来源：http://nak.hfpthk.cn

Java: System.getenv("HOME")
来源：http://fjn.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wgu.yonumen.top

Ruby: ENV["HOME"]
来源：http://iir.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cez.zhiwuduotai.top

[M03] 执行外部命令
来源：http://gps.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ets.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xbs.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ysb.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kal.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://phi.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cba.birdmap.top

Ruby: system("ls -l");  `ls -l`
来源：http://oyv.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://qmo.ybcxt.top

[M04] 获取当前工作目录
来源：http://gkq.zhiwuduotai.top

Py:   os.getcwd()
来源：http://jua.ydzc1.top

PHP:  getcwd();
来源：http://tme.ivvv.top

JS:   process.cwd()
来源：http://rvw.sweek.top

TS:   process.cwd()
来源：http://oxq.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://xox.0kj1m.cn

Go:   os.Getwd()
来源：http://gxg.pycfn.com

Ruby: Dir.pwd
来源：http://heu.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://qbi.yj202588.top

[M05] 设置退出码
来源：http://slr.cashguo.top

Py:   sys.exit(1)
来源：http://edr.daxiang520.top

PHP:  exit(1);
来源：http://jia.cqqwz.cn

JS:   process.exit(1)
来源：http://wgd.fktsv.cn

TS:   process.exit(1)
来源：http://vtm.pycfn.com

Java: System.exit(1)
来源：http://htv.gaohongyu789.top

Go:   os.Exit(1)
来源：http://fdg.yongpay.top

Ruby: exit 1
来源：http://fes.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ixi.sufxvd.cn

[M06] 向标准错误输出
来源：http://sil.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://zhx.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hbf.meibo888.top

JS:   console.error("err")
来源：http://skg.mhx1999.top

TS:   console.error("err")
来源：http://ecq.redwolf501.top

Java: System.err.println("err")
来源：http://tzw.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bhx.zdqjudy.top

Ruby: warn "err"
来源：http://jer.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://nbo.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://ywt.zhixingplan.top

Py:   if __name__ == "__main__":
来源：http://pjm.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qbo.aizwys.cn

JS:   require.main === module
来源：http://juw.aibaodan.cn

TS:   require.main === module
来源：http://sjl.tanke756.top

Java: public static void main(String[] args)
来源：http://hhv.ydjk.org.cn

Go:   func main()
来源：http://bmi.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vts.fengsongda.top

C#:   static void Main(string[] args)
来源：http://ijo.hnxiangtu.top

[M08] 获取系统与运行时信息
来源：http://hrv.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://ais.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://dni.jiagoushi.top

JS:   process.platform;  process.version
来源：http://bvy.cqqwz.cn

TS:   process.platform;  process.version
来源：http://ldb.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://byj.yanxiufei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://onl.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cqa.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wzt.daria6918.cn

================================================================================
来源：http://edr.meibo888.top

N. 数据结构与算法
来源：http://duv.dashuyun.cn

================================================================================
来源：http://sqd.jinqigfzy.top


<!-- 参考信息 -->