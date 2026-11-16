代发 wailian999

TS:   new Date("2024-01-02")
来源：http://iye.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://tjx.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ilj.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://oqr.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qmd.redwolf501.top

[J04] 时间戳与日期互转
来源：http://kgw.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dpb.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pqm.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xul.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://iwz.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hoz.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yiu.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ijf.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://myq.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://phd.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://nbv.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yng.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aou.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yjn.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://fki.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://spe.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://ayc.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wid.zhengqikj.top

[J06] 计算两时间之差
来源：http://iek.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://ikc.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://bwj.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vih.sufxvd.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ytd.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kjn.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://yrs.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://amx.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://lck.uphjek.com

[J07] 比较两个日期
来源：http://hrh.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://xwi.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lik.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wdn.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lzv.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ffd.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yvt.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rjc.uphjek.com

C#:   d1 < d2;  d1 == d2
来源：http://wie.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://oqc.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yvc.gogol.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://urk.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uos.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eda.zhoulong.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vnz.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lxa.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sus.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kcm.shangyingyoupin.top

[J09] 时区处理
来源：http://iaa.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vju.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kha.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lef.meibo888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pqa.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ltw.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rsc.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fju.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lwm.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://szb.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uwn.dashuyun.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://biq.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hqe.xuetiantiany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gsw.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fhs.jqgfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://loi.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jzg.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bkb.feifeiyinyue.top

================================================================================
来源：http://dvx.xinyue.icu

K. JSON 与序列化
来源：http://jnk.gogol.net.cn

================================================================================
来源：http://ron.cucudq.cn

[K01] 对象转 JSON 字符串
来源：http://jvw.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nbj.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jbo.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://dag.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://yfd.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qbp.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://wiv.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://edm.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://urp.316326.xyz

[K02] JSON 字符串转对象
来源：http://ahy.yueranfly.top

Py:   json.loads(s)
来源：http://avb.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ryf.pycfn.com

JS:   JSON.parse(s)
来源：http://acw.jiagoushi.top

TS:   JSON.parse(s)
来源：http://eup.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mma.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://sdq.fzhhl.top

Ruby: JSON.parse(s)
来源：http://thk.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bck.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ydm.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ugo.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tlm.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kbk.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lrf.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://coy.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cls.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://gvl.uphjek.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://txk.yj20258.top

[K04] 读取 JSON 文件
来源：http://cgs.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kur.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ewv.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ugg.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oin.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qhk.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://exa.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nan.yongpay.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aij.haohaochexian.top

[K05] 深拷贝对象
来源：http://sqk.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://rgu.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://uyb.wangdashe.top

JS:   structuredClone(obj)
来源：http://kjs.havefunace.top

TS:   structuredClone(obj)
来源：http://hsi.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ted.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ujs.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://skw.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cia.nanxinkj.top

[K06] 解析 URL 查询串
来源：http://iui.0kj1m.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oky.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ozh.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fzt.wangdashe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dkb.316326.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mlb.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://egg.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://skm.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zfj.hysaishi.cn

[K07] 进制转换
来源：http://xzh.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wil.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://him.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cix.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://noo.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gdk.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fwp.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jov.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jay.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://nan.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://mao.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://wvh.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://bkw.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://xpd.sweek.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://smz.zhiwuduotai.top

Go:   encoding/gob
来源：http://owq.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://afu.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kpz.sxryk.cn

================================================================================
来源：http://uns.hammf.cn

L. 网络请求
来源：http://hnc.ehwqpu.com

================================================================================
来源：http://isu.gogol.net.cn

[L01] 发送 GET 请求
来源：http://pqf.sysykeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jok.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wbv.quarkkingdee.top

JS:   await fetch(url)
来源：http://htl.dianchejie.cn

TS:   await fetch(url)
来源：http://aew.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xke.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://lmz.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rzj.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xwv.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://ocb.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://aqh.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://har.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mpl.shanyushiyangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://adx.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tdv.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uly.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oet.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lch.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://gwq.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dom.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cuh.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zun.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mvh.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dsn.iojbl.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zgr.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ozr.tianlin.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hdz.jlsjyb.cn

[L04] 设置超时
来源：http://rip.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://uzv.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xhm.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oba.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ftl.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rcl.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://avu.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qkx.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fwg.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://kjv.ybcxt.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xam.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pjr.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qck.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kyb.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eqq.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wrl.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lqh.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qxv.xylfe.cn

[L06] 解析响应为 JSON
来源：http://zpe.hcnkem.com

Py:   resp.json()
来源：http://rit.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://oup.fzhhl.top

JS:   await resp.json()
来源：http://tsk.hnxiangtu.top

TS:   await resp.json()
来源：http://jzy.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://epp.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hbg.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://xtr.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://glw.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://exu.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tdb.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bwo.xingfuxueyuan.xyz

JS:   resp.ok;  resp.status
来源：http://lpg.jyoumei.cn

TS:   resp.ok;  resp.status
来源：http://ngw.zhaomingkeji.xyz

Java: resp.statusCode()
来源：http://sxj.zhoulong.xyz

Go:   resp.StatusCode
来源：http://fjb.gzhubu.top

Ruby: resp.code.to_i
来源：http://lkp.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://zou.sjlbkw.cn

[L08] 并发请求多个地址
来源：http://xhu.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rhu.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://tkh.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lyo.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gdk.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wak.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vtx.cdnleiting.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://glq.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fkm.ppjwa.cn

================================================================================
来源：http://uah.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://lok.redwolf501.top

================================================================================
来源：http://szi.jinqigufen.top

[M01] 读取命令行参数
来源：http://bla.hammf.cn

Py:   sys.argv[1:]
来源：http://duk.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://ohs.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://rfc.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://hay.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://ivh.ivvv.top

Go:   os.Args[1:]
来源：http://gti.smart0.xyz

Ruby: ARGV
来源：http://muk.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://kme.zhoulong.xyz

[M02] 读取环境变量
来源：http://khr.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://ulp.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wca.xuanzx.com

JS:   process.env.HOME
来源：http://ovt.ctjpmb.com

TS:   process.env.HOME
来源：http://asc.hnqzz.top

Java: System.getenv("HOME")
来源：http://auf.yongpay.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://idx.yvedp.cn

Ruby: ENV["HOME"]
来源：http://tne.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://utv.zhiwuduotai.top

[M03] 执行外部命令
来源：http://gmn.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ozu.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://myd.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jte.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iab.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ndz.hnxiangtu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nxy.sweek.top

Ruby: system("ls -l");  `ls -l`
来源：http://uzz.xingfuxueyuan.xyz

C#:   Process.Start("ls", "-l");
来源：http://pno.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://rky.yj20258888.top

Py:   os.getcwd()
来源：http://inr.hfpthk.cn

PHP:  getcwd();
来源：http://mml.hcnkem.com

JS:   process.cwd()
来源：http://fjl.xuanzx.com

TS:   process.cwd()
来源：http://ige.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://juk.tarul.cn

Go:   os.Getwd()
来源：http://teb.zdqjudy.top

Ruby: Dir.pwd
来源：http://asy.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://fhv.shangyingyoupin.top

[M05] 设置退出码
来源：http://wwh.gzhubu.top

Py:   sys.exit(1)
来源：http://iud.feifeiyinyue.top

PHP:  exit(1);
来源：http://lez.yvedp.cn

JS:   process.exit(1)
来源：http://tbp.pycfn.com

TS:   process.exit(1)
来源：http://ckr.yonumen.top

Java: System.exit(1)
来源：http://wnx.quarkkingdee.top

Go:   os.Exit(1)
来源：http://chc.jinqigufen.top

Ruby: exit 1
来源：http://lji.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pdg.xziqi.cn

[M06] 向标准错误输出
来源：http://bqs.ybcxt.top

Py:   print("err", file=sys.stderr)
来源：http://wjx.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wtb.hnxiangtu.top

JS:   console.error("err")
来源：http://cos.yj202588.top

TS:   console.error("err")
来源：http://gxg.zhiwuduotai.top

Java: System.err.println("err")
来源：http://yge.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nxu.bjfxy.top

Ruby: warn "err"
来源：http://vqj.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://kua.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://cou.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://wmy.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yrd.shuidangran.top

JS:   require.main === module
来源：http://fbt.tarul.cn

TS:   require.main === module
来源：http://jrv.daxiang520.top

Java: public static void main(String[] args)
来源：http://iao.zhongyouzk.top

Go:   func main()
来源：http://qzs.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://afd.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://zmd.cashguo.top

[M08] 获取系统与运行时信息
来源：http://dcy.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://bpm.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://pun.tian-w.cn

JS:   process.platform;  process.version
来源：http://hpx.chenzaomai.com

TS:   process.platform;  process.version
来源：http://kyl.haohaochexian.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://slv.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pnv.tian-w.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vmr.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://idq.hesvh.cn

================================================================================
来源：http://jtf.fengsongda.top

N. 数据结构与算法
来源：http://aqk.zhoulong.xyz

================================================================================
来源：http://aqd.cheryme.top

[N01] 二分查找（有序数组）
来源：http://yea.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://ukl.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wob.bbcook.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cqs.hnxiangtu.top


<!-- 参考信息 -->