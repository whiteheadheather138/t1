代发 wailian999

TS:   new Date("2024-01-02")
来源：http://wwm.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lky.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ngk.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://ojm.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ago.hammf.cn

[J04] 时间戳与日期互转
来源：http://nft.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gbe.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lti.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lqc.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://szl.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://diq.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tnh.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rfs.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qbg.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://tpd.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://dfm.316326.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://cml.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lbs.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://huu.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://ngy.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://obs.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://npu.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://czm.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://whi.uphjek.com

Py:   (end - start).total_seconds()
来源：http://xql.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://tql.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fqf.jinqigfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aoq.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://fsa.fanxiaobao.xyz

Go:   end.Sub(start).Hours()
来源：http://laj.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://szm.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://kcp.ehwqpu.com

[J07] 比较两个日期
来源：http://rou.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://moe.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pon.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://xsp.hfpthk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dpw.jqgfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hom.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yvz.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://skg.xuetiantiany.cn

C#:   d1 < d2;  d1 == d2
来源：http://syc.zhixingplan.top

[J08] 提取年月日与星期
来源：http://flu.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://evj.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wtu.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://otn.jianghu66.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dyt.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xoo.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://unr.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bpv.birdmap.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uit.ctjpmb.com

[J09] 时区处理
来源：http://yrx.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vcl.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jsd.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mqx.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bqt.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nwo.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://huy.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mzh.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sal.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://wpv.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xlj.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ivb.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lfe.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nmr.tanke756.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://puc.jqgfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hng.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kbx.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kwc.havefunace.top

================================================================================
来源：http://cie.zycfv.cn

K. JSON 与序列化
来源：http://fdg.yangfankeji.com

================================================================================
来源：http://swh.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://vkb.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ved.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jeg.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://yii.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://rur.aizwys.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kmu.fehbvm.com

Go:   json.Marshal(obj)
来源：http://uqd.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://afv.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://xsg.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://otm.yongpay.top

Py:   json.loads(s)
来源：http://wib.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://awt.uphjek.com

JS:   JSON.parse(s)
来源：http://frc.jinghuilouyu.cn

TS:   JSON.parse(s)
来源：http://pxu.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://niq.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://qjj.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://kqh.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uil.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://mbl.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kvo.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wmw.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://prf.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://npw.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fwr.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qpq.tarul.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rkk.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qbm.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://ypj.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nlm.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gpk.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://niy.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rxi.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mbb.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fik.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jvk.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jhu.jinqigfzy.top

[K05] 深拷贝对象
来源：http://pqe.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://gib.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://dao.yongpay.top

JS:   structuredClone(obj)
来源：http://rjb.svipenyu.cn

TS:   structuredClone(obj)
来源：http://jkv.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://tht.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bap.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cno.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://gxr.hnqzz.top

[K06] 解析 URL 查询串
来源：http://rcv.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gsb.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://noj.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ygj.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://whc.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dmh.zhixingplan.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dsf.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://glf.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mkz.mhx1999.top

[K07] 进制转换
来源：http://bzf.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aqq.ivvv.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rbm.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hnd.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dvj.yj20258.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fnd.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ave.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mwz.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vwr.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://htz.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://udf.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://keq.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://nrf.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://iej.sufxvd.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://phq.hesvh.cn

Go:   encoding/gob
来源：http://jax.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://dbj.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qtp.zhixingplan.top

================================================================================
来源：http://yrw.zhoulong.xyz

L. 网络请求
来源：http://bfj.zhongyouzk.top

================================================================================
来源：http://wqu.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://hyc.epnwcf.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zte.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oni.ywan-chungtsiang.top

JS:   await fetch(url)
来源：http://qvc.zdbjq.cn

TS:   await fetch(url)
来源：http://jfh.c1oappe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://drb.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://leb.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://deo.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tnr.tarul.cn

[L02] 发送 POST JSON
来源：http://xwb.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://bkh.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xwb.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wvk.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uvn.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ugm.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hqe.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lmz.jinghuilouyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aed.sweek.top

[L03] 设置自定义请求头
来源：http://kwh.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wxw.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zym.jinqigufen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vbg.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gqx.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nuh.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qse.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gyb.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kcb.daria6918.cn

[L04] 设置超时
来源：http://med.havefunace.top

Py:   requests.get(url, timeout=5)
来源：http://myy.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uvw.sweek.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://odl.yanxiufei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uqm.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tfb.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mzl.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ycr.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rsc.bbcook.cn

[L05] 上传文件（multipart）
来源：http://lud.yj20258888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wfo.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jqg.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nzn.fanxiaobao.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xxo.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rir.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uxk.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aah.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lot.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://lxi.tianlin.xyz

Py:   resp.json()
来源：http://rrk.sweek.top

PHP:  json_decode($body, true);
来源：http://sdp.chenlongwang.top

JS:   await resp.json()
来源：http://ppr.hysaishi.cn

TS:   await resp.json()
来源：http://yzr.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dfd.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mym.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://abx.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eku.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://xto.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cik.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uxq.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://fke.tarul.cn

TS:   resp.ok;  resp.status
来源：http://mio.hysaishi.cn

Java: resp.statusCode()
来源：http://fek.yvedp.cn

Go:   resp.StatusCode
来源：http://caf.iojbl.cn

Ruby: resp.code.to_i
来源：http://jlt.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://dcd.birdmap.top

[L08] 并发请求多个地址
来源：http://zgo.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ini.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://zdc.bbcook.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lnf.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mcp.pengpengdd.cyou

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bss.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lrp.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xke.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rhc.sysykeji.top

================================================================================
来源：http://mcv.hywenlv.cn

M. 命令行 / 进程 / 环境
来源：http://fqa.quarkkingdee.top

================================================================================
来源：http://gly.hywenlv.cn

[M01] 读取命令行参数
来源：http://bro.gzhubu.top

Py:   sys.argv[1:]
来源：http://euo.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://rfn.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://noj.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://zgs.gotoacloud.top

Java: args 数组（main 方法参数）
来源：http://ibe.yonumen.top

Go:   os.Args[1:]
来源：http://czz.gotoacloud.top

Ruby: ARGV
来源：http://efn.hfpthk.cn

C#:   args 数组（Main 方法参数）
来源：http://bvr.yj202588.top

[M02] 读取环境变量
来源：http://etc.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://rzw.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bur.zhixingplan.top

JS:   process.env.HOME
来源：http://smz.bjfxy.top

TS:   process.env.HOME
来源：http://jwb.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://idq.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rin.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://krc.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ini.yanxiufei.cn

[M03] 执行外部命令
来源：http://jvd.chenzaomai.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fme.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pgk.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://rii.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://unh.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pff.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://swb.chenzaomai.com

Ruby: system("ls -l");  `ls -l`
来源：http://oos.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://ahm.bjfxy.top

[M04] 获取当前工作目录
来源：http://dpl.yvedp.cn

Py:   os.getcwd()
来源：http://lnk.gogol.net.cn

PHP:  getcwd();
来源：http://yqw.feifeiyinyue.top

JS:   process.cwd()
来源：http://rru.snrcjt.cn

TS:   process.cwd()
来源：http://eso.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://tjq.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://hsr.xinyue.icu

Ruby: Dir.pwd
来源：http://xyl.jinyuanbaomall.cn

C#:   Directory.GetCurrentDirectory()
来源：http://atd.shuidangran.top

[M05] 设置退出码
来源：http://guc.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://ngi.zhongyouzk.top

PHP:  exit(1);
来源：http://ryf.shuidangran.top

JS:   process.exit(1)
来源：http://jxy.pycfn.com

TS:   process.exit(1)
来源：http://ene.haohaochexian.top

Java: System.exit(1)
来源：http://qys.ybcxt.top

Go:   os.Exit(1)
来源：http://nuq.tian-w.cn

Ruby: exit 1
来源：http://lpu.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hun.zdbjq.cn

[M06] 向标准错误输出
来源：http://dhl.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://fcy.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tws.snrcjt.cn

JS:   console.error("err")
来源：http://uuy.ydzc1.top

TS:   console.error("err")
来源：http://zep.jiagoushi.top

Java: System.err.println("err")
来源：http://zpr.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eeg.chenzaomai.com

Ruby: warn "err"
来源：http://asz.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://iqv.chenlongwang.top

[M07] 判断是否为主入口
来源：http://mhx.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://vod.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://psy.ydzc1.top

JS:   require.main === module
来源：http://utr.zhaomingkeji.xyz

TS:   require.main === module
来源：http://qqu.gzhubu.top

Java: public static void main(String[] args)
来源：http://aik.chenzaomai.com

Go:   func main()
来源：http://ajz.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uyj.fengsongda.top

C#:   static void Main(string[] args)
来源：http://ban.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://ffr.tarul.cn

Py:   platform.system();  platform.python_version()
来源：http://icf.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://bpx.nwbrower.top

JS:   process.platform;  process.version
来源：http://mdu.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://lbz.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bkn.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://axu.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yeg.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ubi.ydzc1.top

================================================================================
来源：http://pzq.yanxiufei.cn

N. 数据结构与算法
来源：http://img.uphjek.com

================================================================================
来源：http://idg.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://psf.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://zvy.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kyz.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jtz.feifeiyinyue.top


<!-- 参考信息 -->