代发 wailian999

TS:   new Date("2024-01-02")
来源：http://riz.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://tks.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xcf.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://spz.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mmz.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://tfh.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://agu.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nmb.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://szs.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qio.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tkb.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vun.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hhk.guannengcc.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aqt.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://joc.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://tgz.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lnq.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qix.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hep.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://bon.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://awg.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://tjm.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://aaq.xuanzx.com

[J06] 计算两时间之差
来源：http://xkz.uphjek.com

Py:   (end - start).total_seconds()
来源：http://vwt.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://xan.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hjn.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wsx.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://nbm.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://ylo.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://sek.nanxinkj.top

C#:   (end - start).TotalSeconds
来源：http://tnz.meibo888.top

[J07] 比较两个日期
来源：http://izg.smart0.xyz

Py:   d1 < d2;  d1 == d2
来源：http://vmw.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gei.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vdt.hfpthk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rrk.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tap.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ivc.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://bya.iojbl.cn

C#:   d1 < d2;  d1 == d2
来源：http://rpv.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://ilc.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cpr.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lhq.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ymi.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ebi.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sui.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://udp.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kpq.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ehx.sufxvd.cn

[J09] 时区处理
来源：http://syt.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xyo.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fra.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uwg.yj20258888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aaa.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wci.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bhj.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dxv.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://szw.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://bxp.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://arl.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eux.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jcb.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vuk.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vyu.yonumen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eru.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oih.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://edd.hnqzz.top

================================================================================
来源：http://din.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://ceg.jyoumei.cn

================================================================================
来源：http://gii.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://grv.hesvh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xxq.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ymb.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://rxo.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://ool.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bsg.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://ozg.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ksf.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://blv.hammf.cn

[K02] JSON 字符串转对象
来源：http://bga.chenzaomai.com

Py:   json.loads(s)
来源：http://cty.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tlw.zhixingplan.top

JS:   JSON.parse(s)
来源：http://quz.cashguo.top

TS:   JSON.parse(s)
来源：http://rsz.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ugz.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://pqt.nwbrower.top

Ruby: JSON.parse(s)
来源：http://zxn.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kdb.fanxiaobao.xyz

[K03] JSON 美化输出（带缩进）
来源：http://flm.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hdt.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sgg.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nyr.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xip.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ujh.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ltd.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://jmq.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://afa.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://sqk.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xsm.cdnleiting.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eeb.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gyx.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://izt.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://svs.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jjn.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vkp.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blg.snrcjt.cn

[K05] 深拷贝对象
来源：http://sur.snrcjt.cn

Py:   copy.deepcopy(obj)
来源：http://did.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://ymm.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://cej.aizwys.cn

TS:   structuredClone(obj)
来源：http://chr.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pab.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ywu.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vfz.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://twk.sweek.top

[K06] 解析 URL 查询串
来源：http://sty.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ffg.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pef.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dwv.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kvs.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ddh.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://itx.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qly.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lrk.yanxiufei.cn

[K07] 进制转换
来源：http://sbk.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vsm.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bfv.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gqc.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xrq.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sbc.fehbvm.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://izm.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aan.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qkw.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://qfk.hammf.cn

Py:   pickle.dumps(obj)
来源：http://hwq.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ogu.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://xfr.mhx1999.top

TS:   v8.serialize(obj)        // Node
来源：http://sof.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oxw.yj20258888.top

Go:   encoding/gob
来源：http://fsk.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://ndc.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xrs.chenjidiqi.icu

================================================================================
来源：http://gkq.gotoacloud.top

L. 网络请求
来源：http://xat.hysaishi.cn

================================================================================
来源：http://brg.nwbrower.top

[L01] 发送 GET 请求
来源：http://rvp.chenjidiqi.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zlo.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fzm.xuanzx.com

JS:   await fetch(url)
来源：http://wgq.meibo888.top

TS:   await fetch(url)
来源：http://ork.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://atl.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://zeh.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hcm.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uxf.andypj.xyz

[L02] 发送 POST JSON
来源：http://vfc.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://ode.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iqt.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://euz.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wir.birdmap.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fum.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ypl.yanxiufei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dss.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wma.fktsv.cn

[L03] 设置自定义请求头
来源：http://sqe.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://egr.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dkz.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kfh.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nxa.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vzy.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kvv.cheryme.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yxb.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xfa.haohaochexian.top

[L04] 设置超时
来源：http://eij.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://nfm.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nyf.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://akc.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mih.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://axa.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ffu.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yom.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nat.cheryme.top

[L05] 上传文件（multipart）
来源：http://blf.chenjidiqi.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kph.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://spl.xuanzx.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pra.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ilk.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://njt.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lms.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lzr.ehwqpu.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://awm.aizwys.cn

[L06] 解析响应为 JSON
来源：http://gsq.sxryk.cn

Py:   resp.json()
来源：http://xdc.hnqzz.top

PHP:  json_decode($body, true);
来源：http://vom.yj20258888.top

JS:   await resp.json()
来源：http://zga.yj20258.top

TS:   await resp.json()
来源：http://meh.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://arx.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kkr.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://zls.sufxvd.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qwt.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://vdq.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jgr.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://snp.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://grz.aizwys.cn

TS:   resp.ok;  resp.status
来源：http://rcc.guowangkeji.top

Java: resp.statusCode()
来源：http://bdu.zhaomingkeji.xyz

Go:   resp.StatusCode
来源：http://rlo.c1oappe.top

Ruby: resp.code.to_i
来源：http://xbr.yfazqb.com

C#:   (int)resp.StatusCode
来源：http://geh.c1oappe.top

[L08] 并发请求多个地址
来源：http://rng.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mve.9152youxi.cn

PHP:  curl_multi_init() 系列
来源：http://kfm.xingfuxueyuan.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ewd.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xyx.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eog.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jxo.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dwm.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zcq.svipenyu.cn

================================================================================
来源：http://ugl.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://yoz.shzxlz.cn

================================================================================
来源：http://fmd.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://pbu.52xcode.cn

Py:   sys.argv[1:]
来源：http://svb.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://tyc.daria6918.cn

JS:   process.argv.slice(2)
来源：http://ilv.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://gru.cucudq.cn

Java: args 数组（main 方法参数）
来源：http://jgz.jyoumei.cn

Go:   os.Args[1:]
来源：http://vfd.daria6918.cn

Ruby: ARGV
来源：http://wvj.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://chi.9152youxi.cn

[M02] 读取环境变量
来源：http://tnm.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://mvw.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://swv.nanxinkj.top

JS:   process.env.HOME
来源：http://fyy.zhixingplan.top

TS:   process.env.HOME
来源：http://hik.iojbl.cn

Java: System.getenv("HOME")
来源：http://szk.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xbr.daria6918.cn

Ruby: ENV["HOME"]
来源：http://oxp.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://snb.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://msy.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sfs.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cad.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bep.fehbvm.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ade.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ydz.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://zfi.cucudq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kiv.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://tfh.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://khe.yj20258888.top

Py:   os.getcwd()
来源：http://cup.316326.xyz

PHP:  getcwd();
来源：http://twb.yueranfly.top

JS:   process.cwd()
来源：http://ytd.ctjpmb.com

TS:   process.cwd()
来源：http://fkk.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://nyr.sweek.top

Go:   os.Getwd()
来源：http://cad.chenlongwang.top

Ruby: Dir.pwd
来源：http://qbt.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fri.pycfn.com

[M05] 设置退出码
来源：http://xmh.yuxming.cn

Py:   sys.exit(1)
来源：http://jvt.zhixingplan.top

PHP:  exit(1);
来源：http://brc.cheryme.top

JS:   process.exit(1)
来源：http://hyu.316326.xyz

TS:   process.exit(1)
来源：http://tod.9152youxi.cn

Java: System.exit(1)
来源：http://eea.zhengqikj.top

Go:   os.Exit(1)
来源：http://mie.ywan-chungtsiang.top

Ruby: exit 1
来源：http://snw.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lzw.dianchejie.cn

[M06] 向标准错误输出
来源：http://bud.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://pzc.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sln.yangfankeji.com

JS:   console.error("err")
来源：http://vot.zhiwuduotai.top

TS:   console.error("err")
来源：http://spy.zhoulong.xyz

Java: System.err.println("err")
来源：http://jbp.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gxg.hnqzz.top

Ruby: warn "err"
来源：http://rhr.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://jvk.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://kst.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://omq.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://beg.yueranfly.top

JS:   require.main === module
来源：http://eww.redwolf501.top

TS:   require.main === module
来源：http://hbz.xuanzx.com

Java: public static void main(String[] args)
来源：http://njg.havefunace.top

Go:   func main()
来源：http://adp.ehwqpu.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xwa.hnqzz.top

C#:   static void Main(string[] args)
来源：http://vyx.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://pvl.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://vto.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://jox.yuanzhike.top

JS:   process.platform;  process.version
来源：http://vcg.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://gac.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mhe.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ohe.gzhubu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lva.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iwe.cdnleiting.top

================================================================================
来源：http://sfb.cashguo.top

N. 数据结构与算法
来源：http://eae.yj20258.top

================================================================================
来源：http://jdm.shanyushiyangkeji.top

[N01] 二分查找（有序数组）
来源：http://ezr.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mfi.gaohongyu789.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uej.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lsd.shuidangran.top


<!-- 参考信息 -->