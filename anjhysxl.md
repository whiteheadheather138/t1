代发 wailian999

[J03] 字符串解析为日期
来源：http://ggq.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ccn.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lwz.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://eyn.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://rbb.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wic.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oee.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://gcv.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hyz.daxiang520.top

[J04] 时间戳与日期互转
来源：http://dct.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://edm.jqgfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nct.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ymu.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wqh.cqqwz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://plx.hywenlv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xzi.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vrj.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tou.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://ejg.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://loa.zhoulong.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://ugs.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tcs.cqqwz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yax.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://nqq.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aih.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://chm.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jei.jqgfzy.top

[J06] 计算两时间之差
来源：http://rhh.fktsv.cn

Py:   (end - start).total_seconds()
来源：http://jul.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://rsy.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cbi.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://drq.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://czj.jinghuilouyu.cn

Go:   end.Sub(start).Hours()
来源：http://mxq.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://pdw.xinyue.icu

C#:   (end - start).TotalSeconds
来源：http://nzd.yangfankeji.com

[J07] 比较两个日期
来源：http://eco.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://dmi.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tzq.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://lqx.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://zsg.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yna.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hgq.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://bxb.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://jwh.jiagoushi.top

[J08] 提取年月日与星期
来源：http://vlr.bbcook.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bgg.hesvh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mgb.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yud.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cgc.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hyb.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://igl.sufxvd.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eqq.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eys.sjlbkw.cn

[J09] 时区处理
来源：http://ftu.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gvf.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kej.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blq.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rlc.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rlp.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cxb.hnqzz.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lpd.daria6918.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vfd.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://ynj.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://jya.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lar.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://drl.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iss.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://puw.daxiang520.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fno.hnqzz.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://edx.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://urq.snrcjt.cn

================================================================================
来源：http://csp.guowangkeji.top

K. JSON 与序列化
来源：http://jys.svipenyu.cn

================================================================================
来源：http://wnn.gzhubu.top

[K01] 对象转 JSON 字符串
来源：http://xeo.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ham.sufxvd.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hfk.cheryme.top

JS:   JSON.stringify(obj)
来源：http://zov.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://ybp.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sow.redwolf501.top

Go:   json.Marshal(obj)
来源：http://xea.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://wlj.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xtt.hfpthk.cn

[K02] JSON 字符串转对象
来源：http://fsa.guowangkeji.top

Py:   json.loads(s)
来源：http://nwy.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hvx.aibaodan.cn

JS:   JSON.parse(s)
来源：http://xcu.zhixingplan.top

TS:   JSON.parse(s)
来源：http://dzr.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kyx.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://uxv.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://psp.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hsg.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://wdt.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://you.sysykeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ppq.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://knq.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://aza.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nwt.nanxuanxn.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xtv.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://avi.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yon.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://mbf.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gud.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ntm.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qpg.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bur.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ast.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bjg.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ykr.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wid.chenlongwang.top

[K05] 深拷贝对象
来源：http://zhp.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://fsw.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://bsr.cucudq.cn

JS:   structuredClone(obj)
来源：http://jxn.tarul.cn

TS:   structuredClone(obj)
来源：http://bof.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gvq.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ogx.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vdi.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yfy.cheryme.top

[K06] 解析 URL 查询串
来源：http://gbl.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kii.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pjf.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bey.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ico.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cqv.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vnc.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hhd.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bbu.316326.xyz

[K07] 进制转换
来源：http://rsl.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rml.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pbv.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://imu.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://npv.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aav.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cbs.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ebr.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pbd.jianghu66.top

[K08] 二进制序列化（非 JSON）
来源：http://luo.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://uci.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://abb.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://tim.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://nlv.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zsr.wangdashe.top

Go:   encoding/gob
来源：http://faz.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://vzt.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aeg.cashguo.top

================================================================================
来源：http://wah.jqgufenzy.top

L. 网络请求
来源：http://fjs.bjfxy.top

================================================================================
来源：http://aqq.hywenlv.cn

[L01] 发送 GET 请求
来源：http://qlc.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vbq.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gjm.52xcode.cn

JS:   await fetch(url)
来源：http://qvo.guowangkeji.top

TS:   await fetch(url)
来源：http://twx.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mny.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://fuz.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vqy.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ngb.yvedp.cn

[L02] 发送 POST JSON
来源：http://pal.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ceo.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mey.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aiz.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gnn.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kkr.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eao.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://imz.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ryv.hfpthk.cn

[L03] 设置自定义请求头
来源：http://rvl.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://koj.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bpm.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oyb.dashuyun.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kzd.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mqa.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://luf.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tdo.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fmy.havefunace.top

[L04] 设置超时
来源：http://lvu.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://nek.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://frk.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gij.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iza.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fyj.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mcr.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kti.hnxiangtu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jbm.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://zsb.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nkt.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rtl.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gea.316326.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hxw.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tqn.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tjs.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ufq.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yxs.yj20258.top

[L06] 解析响应为 JSON
来源：http://blt.c1oappe.top

Py:   resp.json()
来源：http://ecl.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://uax.tianlin.xyz

JS:   await resp.json()
来源：http://aup.mhx1999.top

TS:   await resp.json()
来源：http://yhn.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jel.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://chp.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://hcp.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vti.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://mzr.xinyue.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://feo.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nth.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://tba.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://rjf.xuetiantiany.cn

Java: resp.statusCode()
来源：http://uwd.yanxiufei.cn

Go:   resp.StatusCode
来源：http://asr.yj20258888.top

Ruby: resp.code.to_i
来源：http://lpb.jinghuilouyu.cn

C#:   (int)resp.StatusCode
来源：http://mey.birdmap.top

[L08] 并发请求多个地址
来源：http://cvc.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fjw.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://owg.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ouk.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://etp.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wxt.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zkd.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ner.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tsw.zycfv.cn

================================================================================
来源：http://msh.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://uts.zhengqikj.top

================================================================================
来源：http://gzz.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://aqt.zycfv.cn

Py:   sys.argv[1:]
来源：http://oih.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://mie.fktsv.cn

JS:   process.argv.slice(2)
来源：http://sha.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://env.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://fgq.zhixingplan.top

Go:   os.Args[1:]
来源：http://hgv.hcnkem.com

Ruby: ARGV
来源：http://hbt.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://bir.quarkkingdee.top

[M02] 读取环境变量
来源：http://enm.birdmap.top

Py:   os.environ.get("HOME")
来源：http://rbb.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ijg.0kj1m.cn

JS:   process.env.HOME
来源：http://qli.vehdjk.com

TS:   process.env.HOME
来源：http://jis.yfazqb.com

Java: System.getenv("HOME")
来源：http://dui.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pzi.birdmap.top

Ruby: ENV["HOME"]
来源：http://xil.jlsjyb.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rah.bbcook.cn

[M03] 执行外部命令
来源：http://qij.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ope.zdbjq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ohv.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fiy.cashguo.top

TS:   child_process.execSync("ls -l").toString()
来源：http://byj.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wqo.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jok.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rsb.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://lzu.svipenyu.cn

[M04] 获取当前工作目录
来源：http://vhp.hcnkem.com

Py:   os.getcwd()
来源：http://rtz.jqgfzy.top

PHP:  getcwd();
来源：http://ozj.birdmap.top

JS:   process.cwd()
来源：http://evr.zhiwuduotai.top

TS:   process.cwd()
来源：http://jmp.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://hhy.hcnkem.com

Go:   os.Getwd()
来源：http://aob.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://kpk.iojbl.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jei.yj20258888.top

[M05] 设置退出码
来源：http://ykv.ehwqpu.com

Py:   sys.exit(1)
来源：http://mql.havefunace.top

PHP:  exit(1);
来源：http://acc.yonumen.top

JS:   process.exit(1)
来源：http://xbo.zhiwuduotai.top

TS:   process.exit(1)
来源：http://nqj.bbcook.cn

Java: System.exit(1)
来源：http://vpg.jqgufenzy.top

Go:   os.Exit(1)
来源：http://uct.chenjidiqi.icu

Ruby: exit 1
来源：http://kel.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ddy.yangfankeji.com

[M06] 向标准错误输出
来源：http://vmr.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://ytj.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://zfq.chenjidiqi.icu

JS:   console.error("err")
来源：http://set.pengpengdd.cyou

TS:   console.error("err")
来源：http://lcc.aizwys.cn

Java: System.err.println("err")
来源：http://drs.vehdjk.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://axs.cheryme.top

Ruby: warn "err"
来源：http://elz.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://wcr.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://nkz.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://xil.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mpg.aibaodan.cn

JS:   require.main === module
来源：http://rbu.birdmap.top

TS:   require.main === module
来源：http://jjr.smart0.xyz

Java: public static void main(String[] args)
来源：http://dfz.birdmap.top

Go:   func main()
来源：http://don.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://siy.iojbl.cn

C#:   static void Main(string[] args)
来源：http://tok.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://fjq.epnwcf.com

Py:   platform.system();  platform.python_version()
来源：http://ylq.jyoumei.cn

PHP:  PHP_OS;  phpversion();
来源：http://dxf.nanxinkj.top

JS:   process.platform;  process.version
来源：http://lgr.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://ekc.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pye.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zpz.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uuf.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://bru.nwbrower.top

================================================================================
来源：http://siz.snrcjt.cn

N. 数据结构与算法
来源：http://ily.tarul.cn

================================================================================
来源：http://nwg.kuanghao11.cn


<!-- 参考信息 -->