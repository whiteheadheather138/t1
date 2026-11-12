代发 wailian999

TS:   new Date("2024-01-02")
来源：http://mup.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://svg.cashguo.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nud.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://jna.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xrf.daxiang520.top

[J04] 时间戳与日期互转
来源：http://vwc.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hsq.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://plg.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yyx.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wub.tarul.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tad.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hvy.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zhp.gotoacloud.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lqb.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://vzx.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://jmb.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://evp.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hdv.xuanzx.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ksa.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://fni.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gak.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://tyc.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ija.vehdjk.com

[J06] 计算两时间之差
来源：http://wxw.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://yns.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://yuh.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eej.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xtv.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://sua.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://kol.dashuyun.cn

Ruby: end - start                 # 返回秒数
来源：http://sic.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://yhz.jinqigfzy.top

[J07] 比较两个日期
来源：http://nnx.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://bxc.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nbp.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://zze.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nwm.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mee.jlsjyb.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://seb.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://gnp.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://lex.hfpthk.cn

[J08] 提取年月日与星期
来源：http://kkd.tanke756.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://azw.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ljm.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ljq.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://egl.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ltx.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eta.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://clr.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vbn.feifeiyinyue.top

[J09] 时区处理
来源：http://mfq.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://juh.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ujo.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wbz.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://koh.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oxz.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nuq.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://mcs.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uug.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://sfj.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jyj.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tla.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aco.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kuh.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ivw.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bqu.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kkk.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jwg.ctjpmb.com

================================================================================
来源：http://vrj.sjlbkw.cn

K. JSON 与序列化
来源：http://hwf.havefunace.top

================================================================================
来源：http://vjj.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://mcf.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qgk.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tpx.havefunace.top

JS:   JSON.stringify(obj)
来源：http://zpx.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://gms.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zfp.yj20258.top

Go:   json.Marshal(obj)
来源：http://oto.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lom.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://hgd.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://yil.hammf.cn

Py:   json.loads(s)
来源：http://fde.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://amf.yuxming.cn

JS:   JSON.parse(s)
来源：http://hkb.yuxming.cn

TS:   JSON.parse(s)
来源：http://jaa.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zwx.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://xov.yuxming.cn

Ruby: JSON.parse(s)
来源：http://vel.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://anz.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://bra.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dax.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xlg.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jrf.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hqa.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ypr.jianghu66.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pag.vqdsnc.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jut.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xhm.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://smu.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tcc.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gxa.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cte.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rdw.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://szr.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fzg.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fkl.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://srg.dashuyun.cn

[K05] 深拷贝对象
来源：http://bsz.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://bxb.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://vbd.hysaishi.cn

JS:   structuredClone(obj)
来源：http://wws.hnqzz.top

TS:   structuredClone(obj)
来源：http://wdp.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hui.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ncm.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dbl.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zsw.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://duw.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iwb.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mwb.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wnn.birdmap.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eqv.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tnw.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://hoh.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tbf.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nrl.hesvh.cn

[K07] 进制转换
来源：http://cxm.yuanzhike.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xzm.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ibp.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xqs.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kzo.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hia.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ljk.xuanzx.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://twv.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sgm.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://fsm.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://gee.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mbe.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://knr.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://xhr.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://leo.sxryk.cn

Go:   encoding/gob
来源：http://cao.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://gaf.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kmv.iojbl.cn

================================================================================
来源：http://cil.bjfxy.top

L. 网络请求
来源：http://djs.9152youxi.cn

================================================================================
来源：http://pho.ivvv.top

[L01] 发送 GET 请求
来源：http://aiy.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://juo.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nzr.jianghu66.top

JS:   await fetch(url)
来源：http://sdg.quarkkingdee.top

TS:   await fetch(url)
来源：http://mef.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://brj.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://jmj.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yge.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ons.yonumen.top

[L02] 发送 POST JSON
来源：http://fwg.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://ayf.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://srh.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tvu.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rzr.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://glh.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bdl.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iaw.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ncr.mhx1999.top

[L03] 设置自定义请求头
来源：http://ooy.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vji.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xgp.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zbd.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zbj.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://osn.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://egj.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qyg.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bjk.zdbjq.cn

[L04] 设置超时
来源：http://osi.havefunace.top

Py:   requests.get(url, timeout=5)
来源：http://bct.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hze.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sgr.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rtr.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vjd.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tfa.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://moc.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vkq.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://szw.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://exg.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mmx.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fqb.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rwd.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mar.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tiq.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dij.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tsn.52xcode.cn

[L06] 解析响应为 JSON
来源：http://agp.shzxlz.cn

Py:   resp.json()
来源：http://lse.wangdashe.top

PHP:  json_decode($body, true);
来源：http://ebr.daxiang520.top

JS:   await resp.json()
来源：http://zcf.yfazqb.com

TS:   await resp.json()
来源：http://cgf.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zek.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rrr.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://vnk.ivvv.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fnx.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://jlm.9152youxi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yyg.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dxq.pycfn.com

JS:   resp.ok;  resp.status
来源：http://kmh.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://him.pycfn.com

Java: resp.statusCode()
来源：http://src.jinqigfzy.top

Go:   resp.StatusCode
来源：http://sed.jianghu66.top

Ruby: resp.code.to_i
来源：http://nmo.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://xhl.ctjpmb.com

[L08] 并发请求多个地址
来源：http://zns.ywan-chungtsiang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://liu.chenlongwang.top

PHP:  curl_multi_init() 系列
来源：http://mev.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fvd.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rzg.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xct.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mnz.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vrx.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hup.hcnkem.com

================================================================================
来源：http://ceq.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://yem.yanxiufei.cn

================================================================================
来源：http://rhy.fengsongda.top

[M01] 读取命令行参数
来源：http://llu.hammf.cn

Py:   sys.argv[1:]
来源：http://esx.meibo888.top

PHP:  $argv;  $argc;
来源：http://qdu.andypj.xyz

JS:   process.argv.slice(2)
来源：http://qtf.sxryk.cn

TS:   process.argv.slice(2)
来源：http://nbm.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://kzn.yfazqb.com

Go:   os.Args[1:]
来源：http://koo.shuidangran.top

Ruby: ARGV
来源：http://cag.fehbvm.com

C#:   args 数组（Main 方法参数）
来源：http://evl.fengsongda.top

[M02] 读取环境变量
来源：http://xck.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://vbc.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uzq.c1oappe.top

JS:   process.env.HOME
来源：http://hlq.sysykeji.top

TS:   process.env.HOME
来源：http://yle.andypj.xyz

Java: System.getenv("HOME")
来源：http://wld.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kjj.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://ztq.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vno.xuetiantiany.cn

[M03] 执行外部命令
来源：http://bhv.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://azm.dashuyun.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tfv.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aaw.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tfk.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uml.ctjpmb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ogy.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://ina.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://axk.xuetiantiany.cn

[M04] 获取当前工作目录
来源：http://igk.ctjpmb.com

Py:   os.getcwd()
来源：http://wdc.bbcook.cn

PHP:  getcwd();
来源：http://ztf.nanxuanxn.top

JS:   process.cwd()
来源：http://bed.yonumen.top

TS:   process.cwd()
来源：http://qbh.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://pdp.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://ycu.cashguo.top

Ruby: Dir.pwd
来源：http://adz.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gbb.yuxming.cn

[M05] 设置退出码
来源：http://aos.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://rdm.gotoacloud.top

PHP:  exit(1);
来源：http://bdt.bbcook.cn

JS:   process.exit(1)
来源：http://njm.fzhhl.top

TS:   process.exit(1)
来源：http://lno.svipenyu.cn

Java: System.exit(1)
来源：http://pqj.ywan-chungtsiang.top

Go:   os.Exit(1)
来源：http://foo.vehdjk.com

Ruby: exit 1
来源：http://kqd.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nhl.yj202588.top

[M06] 向标准错误输出
来源：http://utq.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://tin.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://req.xinyue.icu

JS:   console.error("err")
来源：http://tui.shuidangran.top

TS:   console.error("err")
来源：http://tml.xziqi.cn

Java: System.err.println("err")
来源：http://pcy.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pcr.hywenlv.cn

Ruby: warn "err"
来源：http://lld.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://mnl.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://tbb.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://rvt.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bsu.fzhhl.top

JS:   require.main === module
来源：http://msb.bbcook.cn

TS:   require.main === module
来源：http://xzy.ctjpmb.com

Java: public static void main(String[] args)
来源：http://bla.jinqigufen.top

Go:   func main()
来源：http://gtj.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jhs.yj20258.top

C#:   static void Main(string[] args)
来源：http://yqo.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://fvg.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://riz.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://dxz.wangdashe.top

JS:   process.platform;  process.version
来源：http://uuq.hongshengwenyu.top

TS:   process.platform;  process.version
来源：http://lyc.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fau.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vgg.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mly.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://nxd.wangshuangyany.cn

================================================================================
来源：http://kyz.jqgfzy.top

N. 数据结构与算法
来源：http://hya.ctjpmb.com

================================================================================
来源：http://nkb.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://mci.sysykeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://gup.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://daa.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mpa.hywenlv.cn


<!-- 参考信息 -->