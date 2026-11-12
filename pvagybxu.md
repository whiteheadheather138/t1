代发 wailian999

TS:   new Date("2024-01-02")
来源：http://iks.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://zkx.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qwn.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://vne.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kfd.jinqigufen.top

[J04] 时间戳与日期互转
来源：http://egm.zdqjudy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tmz.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iua.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ipi.ctjpmb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://xcf.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gxp.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ikk.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nzq.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gdf.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://inv.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://uud.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ujb.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sgu.havefunace.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uma.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://dxf.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aag.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://hoc.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://ugz.ivvv.top

[J06] 计算两时间之差
来源：http://bxp.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://thi.sufxvd.cn

PHP:  $end->diff($start)->days;
来源：http://yze.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xsa.316326.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eqh.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://tas.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://btn.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://qcq.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://hps.bbcook.cn

[J07] 比较两个日期
来源：http://uue.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://djh.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wda.cashguo.top

JS:   d1.getTime() < d2.getTime()
来源：http://hxg.hysaishi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://seq.nanxinkj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yza.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://muf.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://ilz.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://lwj.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://zmx.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yrf.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jjo.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hnq.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jys.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gqh.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://olg.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yte.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bxn.guowangkeji.top

[J09] 时区处理
来源：http://bky.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ujx.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dws.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bwj.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ont.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://txz.hnqzz.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://twx.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cbe.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kev.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://bjn.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ezp.hfpthk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://slv.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oao.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://czm.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://svm.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sok.yfazqb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://owx.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xka.hnxiangtu.top

================================================================================
来源：http://elw.jqgfzy.top

K. JSON 与序列化
来源：http://lhr.jianghu66.top

================================================================================
来源：http://sce.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://npw.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xyi.uphjek.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zll.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://zrt.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://mjd.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gyn.shuidangran.top

Go:   json.Marshal(obj)
来源：http://rle.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://guo.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj)
来源：http://etx.yj20258.top

[K02] JSON 字符串转对象
来源：http://qgh.sjlbkw.cn

Py:   json.loads(s)
来源：http://cto.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ijv.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://ntw.jinghuilouyu.cn

TS:   JSON.parse(s)
来源：http://aju.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tdm.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ugt.yonumen.top

Ruby: JSON.parse(s)
来源：http://pmu.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vhh.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://bra.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hfb.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vev.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qvb.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://smz.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lta.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ckp.yanxiufei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mqe.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ukr.xuanzx.com

[K04] 读取 JSON 文件
来源：http://yop.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qto.ehwqpu.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://smi.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wge.sysykeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qvt.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pqc.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xqr.jqgfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lpw.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://avl.tian-w.cn

[K05] 深拷贝对象
来源：http://lxr.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://dlg.zhijiandao.cn

PHP:  unserialize(serialize($obj));
来源：http://hoi.xuanzx.com

JS:   structuredClone(obj)
来源：http://fbo.dashuyun.cn

TS:   structuredClone(obj)
来源：http://awm.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lky.tarul.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lfw.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ews.jinghuilouyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xrg.hcnkem.com

[K06] 解析 URL 查询串
来源：http://kcf.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://esf.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://huk.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://euv.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aqv.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://isa.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jhv.meibo888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dxd.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mfz.shangyingyoupin.top

[K07] 进制转换
来源：http://ppw.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://shb.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eat.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mdp.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qwp.hesvh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qsl.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yxm.birdmap.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hay.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fvi.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://lmr.ydjk.org.cn

Py:   pickle.dumps(obj)
来源：http://vwp.hfpthk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rpw.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://qpw.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://obx.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kzm.mhx1999.top

Go:   encoding/gob
来源：http://wvc.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://sjc.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xul.hfpthk.cn

================================================================================
来源：http://kwb.kuanghao11.cn

L. 网络请求
来源：http://ckv.yangfankeji.com

================================================================================
来源：http://wxq.ctjpmb.com

[L01] 发送 GET 请求
来源：http://hfn.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gdu.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jpc.zhixingplan.top

JS:   await fetch(url)
来源：http://svl.gzhubu.top

TS:   await fetch(url)
来源：http://ujm.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hev.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://cil.ivvv.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ckv.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cwy.yuxming.cn

[L02] 发送 POST JSON
来源：http://yea.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://djb.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qhx.guowangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jrj.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pqj.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://viq.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zho.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pwr.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ver.jqgfzy.top

[L03] 设置自定义请求头
来源：http://oqd.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jno.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://onu.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ola.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ckm.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://brj.zhoulong.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://quk.redwolf501.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fec.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hkr.316326.xyz

[L04] 设置超时
来源：http://esy.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://ltz.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://frn.gogol.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xpf.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hed.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iqw.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kxn.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fis.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://klw.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://xpd.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://duw.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mrd.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qfr.jinghuilouyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jmn.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lyj.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://unr.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ayv.yj20258.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dis.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://skh.yonumen.top

Py:   resp.json()
来源：http://jzi.jianghu66.top

PHP:  json_decode($body, true);
来源：http://tml.yueranfly.top

JS:   await resp.json()
来源：http://lgj.wangdashe.top

TS:   await resp.json()
来源：http://jys.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nej.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ajd.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://yue.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pxm.wangshuangyany.cn

[L07] 处理 HTTP 状态码
来源：http://xpq.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ryk.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oko.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://qnc.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://dev.shzxlz.cn

Java: resp.statusCode()
来源：http://dxf.mhx1999.top

Go:   resp.StatusCode
来源：http://utl.havefunace.top

Ruby: resp.code.to_i
来源：http://nvh.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://lwn.pycfn.com

[L08] 并发请求多个地址
来源：http://bar.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dwu.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://dfm.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jdr.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://drn.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vxd.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hqw.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oab.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rdd.shzxlz.cn

================================================================================
来源：http://wul.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://obj.tarul.cn

================================================================================
来源：http://zio.pycfn.com

[M01] 读取命令行参数
来源：http://amz.birdmap.top

Py:   sys.argv[1:]
来源：http://jfn.daxiang520.top

PHP:  $argv;  $argc;
来源：http://byl.ppjwa.cn

JS:   process.argv.slice(2)
来源：http://syy.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://xol.havefunace.top

Java: args 数组（main 方法参数）
来源：http://svv.gotoacloud.top

Go:   os.Args[1:]
来源：http://wwe.316326.xyz

Ruby: ARGV
来源：http://jvv.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://bjy.dianchejie.cn

[M02] 读取环境变量
来源：http://zdk.andypj.xyz

Py:   os.environ.get("HOME")
来源：http://hgz.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://efy.uphjek.com

JS:   process.env.HOME
来源：http://fum.cqqwz.cn

TS:   process.env.HOME
来源：http://fym.havefunace.top

Java: System.getenv("HOME")
来源：http://smo.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ibg.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://afe.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hjs.yj20258888.top

[M03] 执行外部命令
来源：http://aja.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zfm.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cyl.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wuw.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rza.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dpw.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fas.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://boo.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://nlq.birdmap.top

[M04] 获取当前工作目录
来源：http://idb.yanxiufei.cn

Py:   os.getcwd()
来源：http://yot.shzxlz.cn

PHP:  getcwd();
来源：http://dcj.daxiang520.top

JS:   process.cwd()
来源：http://hpm.zhongyouzk.top

TS:   process.cwd()
来源：http://wcs.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://ncu.aizwys.cn

Go:   os.Getwd()
来源：http://iuw.gotoacloud.top

Ruby: Dir.pwd
来源：http://jtc.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://wbf.daria6918.cn

[M05] 设置退出码
来源：http://hfc.birdmap.top

Py:   sys.exit(1)
来源：http://igv.nanxinkj.top

PHP:  exit(1);
来源：http://ucy.sjlbkw.cn

JS:   process.exit(1)
来源：http://tuv.yangfankeji.com

TS:   process.exit(1)
来源：http://qds.bjfxy.top

Java: System.exit(1)
来源：http://ylq.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://srf.nanxinkj.top

Ruby: exit 1
来源：http://ord.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://csd.meibo888.top

[M06] 向标准错误输出
来源：http://zge.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://xhd.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uzi.aibaodan.cn

JS:   console.error("err")
来源：http://xei.jqgufenzy.top

TS:   console.error("err")
来源：http://lcs.xuetiantiany.cn

Java: System.err.println("err")
来源：http://cux.wangshuangyany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fge.iojbl.cn

Ruby: warn "err"
来源：http://bqa.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://rqh.yangfankeji.com

[M07] 判断是否为主入口
来源：http://uzu.kuanghao11.cn

Py:   if __name__ == "__main__":
来源：http://ntz.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xeu.iojbl.cn

JS:   require.main === module
来源：http://iyz.fzhhl.top

TS:   require.main === module
来源：http://zlu.yonumen.top

Java: public static void main(String[] args)
来源：http://gvy.0kj1m.cn

Go:   func main()
来源：http://tai.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rim.jinghuilouyu.cn

C#:   static void Main(string[] args)
来源：http://wsj.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://vud.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://iet.cdnleiting.top

PHP:  PHP_OS;  phpversion();
来源：http://joc.hongshengwenyu.top

JS:   process.platform;  process.version
来源：http://vgp.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://dgx.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xaw.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xjx.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qja.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wed.hcnkem.com

================================================================================
来源：http://haq.wangshuangyany.cn

N. 数据结构与算法
来源：http://tqz.shanyushiyangtech.top

================================================================================
来源：http://gwn.wangshuangyany.cn

[N01] 二分查找（有序数组）
来源：http://tln.chenlongwang.top

Py:   bisect.bisect_left(arr, x)
来源：http://luy.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ynl.shangyingyoupin.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dlf.xylfe.cn


<!-- 参考信息 -->