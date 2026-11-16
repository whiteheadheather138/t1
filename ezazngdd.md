代发 wailian999

[J03] 字符串解析为日期
来源：http://awh.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jhp.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aia.cashguo.top

JS:   new Date("2024-01-02")
来源：http://zqy.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://cyu.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://nev.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nos.gotoacloud.top

Ruby: Date.parse("2024-01-02")
来源：http://wsn.cdnleiting.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lge.tian-w.cn

[J04] 时间戳与日期互转
来源：http://xcm.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ybj.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pkw.yuxming.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://udt.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://qpp.bbcook.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://stw.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sox.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uze.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://deq.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://ngt.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://zsq.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dna.bjfxy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xez.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jrc.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://jhg.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://syk.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://lja.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://txp.andypj.xyz

[J06] 计算两时间之差
来源：http://ect.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://gij.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://spb.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rir.nanxinkj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://obm.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://nri.nanxinkj.top

Go:   end.Sub(start).Hours()
来源：http://iml.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://xjg.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://khq.sufxvd.cn

[J07] 比较两个日期
来源：http://fuk.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://fos.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lwk.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xtn.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://ygf.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://azw.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cle.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://dru.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://kfw.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://ayg.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ire.jyoumei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mhm.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sjm.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://quh.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zyx.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oxs.sjlbkw.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hdd.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fbu.yj202588.top

[J09] 时区处理
来源：http://shv.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bvk.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lqw.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vac.sufxvd.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://klp.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hmk.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rpq.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rdw.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vuc.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://xfk.cashguo.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lwt.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xbr.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://anw.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xwb.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://amr.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://byl.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pwg.ydjk.org.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kcf.52xcode.cn

================================================================================
来源：http://dta.52xcode.cn

K. JSON 与序列化
来源：http://ixh.shzxlz.cn

================================================================================
来源：http://edm.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://vgl.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kri.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bch.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://mic.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://sav.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gwg.jianghu66.top

Go:   json.Marshal(obj)
来源：http://cdw.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://egu.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ian.smart0.xyz

[K02] JSON 字符串转对象
来源：http://fod.jianghu66.top

Py:   json.loads(s)
来源：http://tui.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://irh.cheryme.top

JS:   JSON.parse(s)
来源：http://wzu.xingfuxueyuan.xyz

TS:   JSON.parse(s)
来源：http://pvr.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ads.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://gzs.xziqi.cn

Ruby: JSON.parse(s)
来源：http://oxx.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kvm.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://dtt.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://arr.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uze.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jsz.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://buk.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wbl.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ocl.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wdt.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gbo.cucudq.cn

[K04] 读取 JSON 文件
来源：http://mqq.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hvy.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qgn.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uhb.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tet.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bzh.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hbq.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jnq.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fjs.sxryk.cn

[K05] 深拷贝对象
来源：http://loi.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://gcb.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://hyx.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://zye.jinyuanbaomall.cn

TS:   structuredClone(obj)
来源：http://vtc.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hna.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xhh.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ymz.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://umf.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://kyo.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oka.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fqw.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lxp.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cll.tanke756.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qwm.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://qph.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wqe.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yvf.sufxvd.cn

[K07] 进制转换
来源：http://xph.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pet.jqgufenzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nkn.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fyf.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://urj.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rqq.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uxy.tianlin.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pcq.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://afk.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://kaz.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://xps.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://otm.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://zbp.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://imj.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hxz.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://huf.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://kug.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nla.zhijiandao.cn

================================================================================
来源：http://yvw.gaohongyu789.top

L. 网络请求
来源：http://odl.xuetiantiany.cn

================================================================================
来源：http://owb.zdbjq.cn

[L01] 发送 GET 请求
来源：http://ijk.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wun.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gvu.jinqigufen.top

JS:   await fetch(url)
来源：http://zje.ydjk.org.cn

TS:   await fetch(url)
来源：http://mfv.shzxlz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rqq.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://erv.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yof.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yxp.9152youxi.cn

[L02] 发送 POST JSON
来源：http://uxa.yangfankeji.com

Py:   requests.post(url, json={"a": 1})
来源：http://wlf.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sfn.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aay.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dek.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iov.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://akf.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jni.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zet.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://ubp.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yiw.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fsi.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://awp.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ccc.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ghk.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cpy.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jiw.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vcy.xuanzx.com

[L04] 设置超时
来源：http://whn.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://ygz.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mnq.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rdl.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nod.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cgn.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bjp.havefunace.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ayx.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nwi.fengsongda.top

[L05] 上传文件（multipart）
来源：http://nmq.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://egf.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gjc.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cst.haohaochexian.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jhh.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eqt.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vij.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uqe.gogol.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yfm.shuidangran.top

[L06] 解析响应为 JSON
来源：http://msp.ehwqpu.com

Py:   resp.json()
来源：http://dfj.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://shv.uphjek.com

JS:   await resp.json()
来源：http://dvc.nanxuanxn.top

TS:   await resp.json()
来源：http://aym.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bkb.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://buy.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://aop.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hwn.fengsongda.top

[L07] 处理 HTTP 状态码
来源：http://iyp.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qnb.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xqe.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://iih.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://jsj.guowangkeji.top

Java: resp.statusCode()
来源：http://nxf.dianchejie.cn

Go:   resp.StatusCode
来源：http://gna.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://svo.ctjpmb.com

C#:   (int)resp.StatusCode
来源：http://tyy.bbcook.cn

[L08] 并发请求多个地址
来源：http://yra.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oyh.jinghuilouyu.cn

PHP:  curl_multi_init() 系列
来源：http://lpq.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pay.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yfj.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xfd.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zfr.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lyw.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rgx.tanke756.top

================================================================================
来源：http://rzd.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://qat.tanke756.top

================================================================================
来源：http://crp.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://bgf.tianlin.xyz

Py:   sys.argv[1:]
来源：http://ncd.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://hrj.hammf.cn

JS:   process.argv.slice(2)
来源：http://xmy.smart0.xyz

TS:   process.argv.slice(2)
来源：http://abp.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://qct.jinyuanbaomall.cn

Go:   os.Args[1:]
来源：http://jvi.zdqjudy.top

Ruby: ARGV
来源：http://kpk.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://ucx.sysykeji.top

[M02] 读取环境变量
来源：http://okz.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://yfe.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rem.andypj.xyz

JS:   process.env.HOME
来源：http://jcr.yuanzhike.top

TS:   process.env.HOME
来源：http://qkk.guowangkeji.top

Java: System.getenv("HOME")
来源：http://vuu.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lav.fengsongda.top

Ruby: ENV["HOME"]
来源：http://ixc.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://msp.jinqigfzy.top

[M03] 执行外部命令
来源：http://rgi.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gbm.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jwe.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fnc.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tfo.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xad.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qhh.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hng.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://mph.cashguo.top

[M04] 获取当前工作目录
来源：http://zqu.hongshengwenyu.top

Py:   os.getcwd()
来源：http://vpj.jinqigufen.top

PHP:  getcwd();
来源：http://ngj.sweek.top

JS:   process.cwd()
来源：http://ngn.tianlin.xyz

TS:   process.cwd()
来源：http://ujz.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://ays.yuanzhike.top

Go:   os.Getwd()
来源：http://xfh.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://xbf.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://igg.dianchejie.cn

[M05] 设置退出码
来源：http://eve.fengsongda.top

Py:   sys.exit(1)
来源：http://ivy.zhoulong.xyz

PHP:  exit(1);
来源：http://ioe.vehdjk.com

JS:   process.exit(1)
来源：http://ijx.gaohongyu789.top

TS:   process.exit(1)
来源：http://jaj.yanxiufei.cn

Java: System.exit(1)
来源：http://cho.shuidangran.top

Go:   os.Exit(1)
来源：http://vqx.feifeiyinyue.top

Ruby: exit 1
来源：http://qwo.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nrj.tanke756.top

[M06] 向标准错误输出
来源：http://utb.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://xrz.hcnkem.com

PHP:  fwrite(STDERR, "err\n");
来源：http://zlv.daria6918.cn

JS:   console.error("err")
来源：http://bde.kuanghao11.cn

TS:   console.error("err")
来源：http://yuh.dianchejie.cn

Java: System.err.println("err")
来源：http://dwp.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hkh.wangdashe.top

Ruby: warn "err"
来源：http://rof.hysaishi.cn

C#:   Console.Error.WriteLine("err")
来源：http://zek.jiagoushi.top

[M07] 判断是否为主入口
来源：http://hgx.meibo888.top

Py:   if __name__ == "__main__":
来源：http://pqb.guannengcc.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yae.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://yej.yj20258.top

TS:   require.main === module
来源：http://bqz.bjfxy.top

Java: public static void main(String[] args)
来源：http://aup.fzhhl.top

Go:   func main()
来源：http://lwb.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hkh.yj202588.top

C#:   static void Main(string[] args)
来源：http://apr.gaohongyu789.top

[M08] 获取系统与运行时信息
来源：http://znv.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://ema.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://ulq.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://fut.ybcxt.top

TS:   process.platform;  process.version
来源：http://ezb.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oqd.yueranfly.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lgw.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://psm.havefunace.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ccl.0kj1m.cn

================================================================================
来源：http://xzk.cqqwz.cn

N. 数据结构与算法
来源：http://iyp.tianlin.xyz

================================================================================
来源：http://jfb.zhoulong.xyz


<!-- 参考信息 -->