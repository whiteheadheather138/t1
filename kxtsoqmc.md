代发 wailian999

[J03] 字符串解析为日期
来源：http://kee.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jws.yonumen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wai.chenjidiqi.icu

JS:   new Date("2024-01-02")
来源：http://hzk.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://poz.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://slz.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ace.pycfn.com

Ruby: Date.parse("2024-01-02")
来源：http://yqe.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wzm.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://ban.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ssp.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ole.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ver.yangfankeji.com

TS:   Math.floor(Date.now() / 1000)
来源：http://jkk.hnxiangtu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ldr.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zxw.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rcr.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fri.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://oss.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://vzb.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aat.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xam.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wgw.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://eph.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://naq.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://vwd.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vzp.wangdashe.top

[J06] 计算两时间之差
来源：http://qsy.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://xti.havefunace.top

PHP:  $end->diff($start)->days;
来源：http://dfc.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sfo.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pre.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vjq.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://tlk.cqqwz.cn

Ruby: end - start                 # 返回秒数
来源：http://eff.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://fim.tianlin.xyz

[J07] 比较两个日期
来源：http://dbk.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://avm.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fax.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://yzg.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://kng.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cpa.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mqf.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://xue.tianlin.xyz

C#:   d1 < d2;  d1 == d2
来源：http://flj.vehdjk.com

[J08] 提取年月日与星期
来源：http://qao.jinghuilouyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lnq.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ynf.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kjm.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cws.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kbb.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dun.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nea.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://khl.zycfv.cn

[J09] 时区处理
来源：http://jfe.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uye.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hhg.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wzk.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hxq.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rqf.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pvn.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mft.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ymf.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://yjv.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://soy.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pgj.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://evo.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pkf.jinyuanbaomall.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bgz.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bhl.52xcode.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wug.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lfc.nanxinkj.top

================================================================================
来源：http://ecc.chenzaomai.com

K. JSON 与序列化
来源：http://lkv.yvedp.cn

================================================================================
来源：http://jyf.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://myc.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eev.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://teb.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://zyy.havefunace.top

TS:   JSON.stringify(obj)
来源：http://nlv.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ntn.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://eke.daria6918.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xgi.jianghu66.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lbi.xylfe.cn

[K02] JSON 字符串转对象
来源：http://ncb.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://ywc.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://syd.cheryme.top

JS:   JSON.parse(s)
来源：http://baw.fehbvm.com

TS:   JSON.parse(s)
来源：http://izv.ppjwa.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://naj.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://opb.cashguo.top

Ruby: JSON.parse(s)
来源：http://ohw.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zqk.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://uia.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pec.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zeo.zhoulong.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://zez.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cpa.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aav.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cox.ydzc1.top

Ruby: JSON.pretty_generate(obj)
来源：http://lvr.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wxz.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://brr.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nfb.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uqr.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://roo.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cnq.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lsq.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zrh.hywenlv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qnt.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hqa.yfazqb.com

[K05] 深拷贝对象
来源：http://qny.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://asc.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://hwg.nanxinkj.top

JS:   structuredClone(obj)
来源：http://ssy.epnwcf.com

TS:   structuredClone(obj)
来源：http://oib.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gxs.zhoulong.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vsd.iojbl.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qav.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tlr.zhiwuduotai.top

[K06] 解析 URL 查询串
来源：http://wmv.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sco.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xuy.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oef.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nmh.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vdk.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://jzd.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jci.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aeh.bbcook.cn

[K07] 进制转换
来源：http://ceq.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wnr.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uil.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tjp.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xjv.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fhz.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ext.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gsj.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yid.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://pbg.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://eou.zhijiandao.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ypf.c1oappe.top

JS:   v8.serialize(obj)        // Node
来源：http://tgp.yvedp.cn

TS:   v8.serialize(obj)        // Node
来源：http://vmm.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ilt.haohaochexian.top

Go:   encoding/gob
来源：http://kvf.xylfe.cn

Ruby: Marshal.dump(obj)
来源：http://cht.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ufq.cdnleiting.top

================================================================================
来源：http://jve.smart0.xyz

L. 网络请求
来源：http://xws.yangfankeji.com

================================================================================
来源：http://ear.yueranfly.top

[L01] 发送 GET 请求
来源：http://fva.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cvc.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://koi.aibaodan.cn

JS:   await fetch(url)
来源：http://mgu.smart0.xyz

TS:   await fetch(url)
来源：http://mvy.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hki.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://svm.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rwp.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ksj.bbcook.cn

[L02] 发送 POST JSON
来源：http://tsx.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rsc.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ocq.iojbl.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fmj.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zaz.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gja.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gjv.nanxuanxn.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://muk.nanxinkj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ppt.aizwys.cn

[L03] 设置自定义请求头
来源：http://hcm.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vdq.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nbd.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qit.jqgfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fpy.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hof.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yfo.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nsw.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wwl.yuanzhike.top

[L04] 设置超时
来源：http://vhh.sysykeji.top

Py:   requests.get(url, timeout=5)
来源：http://cdr.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tib.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uts.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vzl.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://enr.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gss.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://obo.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://avr.cucudq.cn

[L05] 上传文件（multipart）
来源：http://qoz.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ymi.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vhm.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ofp.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tyt.sxryk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mcg.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uye.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ndn.chenlongwang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ovo.havefunace.top

[L06] 解析响应为 JSON
来源：http://gqx.hywenlv.cn

Py:   resp.json()
来源：http://bht.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://xpf.havefunace.top

JS:   await resp.json()
来源：http://qrs.vehdjk.com

TS:   await resp.json()
来源：http://cbg.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bfb.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hic.xuetiantiany.cn

Ruby: JSON.parse(resp.body)
来源：http://xpv.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oph.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://rdv.svipenyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hng.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dkm.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://xai.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://xnl.haohaochexian.top

Java: resp.statusCode()
来源：http://pqc.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://fdy.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://bda.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://yli.jiagoushi.top

[L08] 并发请求多个地址
来源：http://nsd.jqgfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qcf.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://xxv.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lte.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aad.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kqh.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cwa.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ojt.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zbn.yj20258888.top

================================================================================
来源：http://bfl.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://zdj.yfazqb.com

================================================================================
来源：http://ofp.hesvh.cn

[M01] 读取命令行参数
来源：http://khm.yuxming.cn

Py:   sys.argv[1:]
来源：http://flp.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://eai.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://ugy.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://ypz.sxryk.cn

Java: args 数组（main 方法参数）
来源：http://xbm.jinyuanbaomall.cn

Go:   os.Args[1:]
来源：http://frr.dianchejie.cn

Ruby: ARGV
来源：http://jss.jiagoushi.top

C#:   args 数组（Main 方法参数）
来源：http://ypf.ydzc1.top

[M02] 读取环境变量
来源：http://oiw.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://uhk.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iqk.wangshuangyany.cn

JS:   process.env.HOME
来源：http://xqc.52xcode.cn

TS:   process.env.HOME
来源：http://aan.gzhubu.top

Java: System.getenv("HOME")
来源：http://aqb.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xta.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://uke.jinqigufen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pgk.chenlongwang.top

[M03] 执行外部命令
来源：http://eme.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xvm.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kko.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dxu.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://jyw.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sfa.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://npu.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://lwy.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://hdg.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://sfq.cashguo.top

Py:   os.getcwd()
来源：http://cif.ivvv.top

PHP:  getcwd();
来源：http://luk.iojbl.cn

JS:   process.cwd()
来源：http://hon.mhx1999.top

TS:   process.cwd()
来源：http://nrj.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://ajg.cucudq.cn

Go:   os.Getwd()
来源：http://ifs.snrcjt.cn

Ruby: Dir.pwd
来源：http://cot.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://fik.zhixingplan.top

[M05] 设置退出码
来源：http://dne.andypj.xyz

Py:   sys.exit(1)
来源：http://gtq.quarkkingdee.top

PHP:  exit(1);
来源：http://pzw.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://eva.hysaishi.cn

TS:   process.exit(1)
来源：http://gqw.hcnkem.com

Java: System.exit(1)
来源：http://fdc.yuanzhike.top

Go:   os.Exit(1)
来源：http://hsq.wangshuangyany.cn

Ruby: exit 1
来源：http://tyb.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eff.xziqi.cn

[M06] 向标准错误输出
来源：http://xjs.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://jao.ywan-chungtsiang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wje.cdnleiting.top

JS:   console.error("err")
来源：http://aus.andypj.xyz

TS:   console.error("err")
来源：http://gbs.fktsv.cn

Java: System.err.println("err")
来源：http://coj.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://euu.yfazqb.com

Ruby: warn "err"
来源：http://xxc.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://tge.cqqwz.cn

[M07] 判断是否为主入口
来源：http://mlt.tanke756.top

Py:   if __name__ == "__main__":
来源：http://shq.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zxk.meibo888.top

JS:   require.main === module
来源：http://yrt.fktsv.cn

TS:   require.main === module
来源：http://wqh.xylfe.cn

Java: public static void main(String[] args)
来源：http://pne.jyoumei.cn

Go:   func main()
来源：http://wzh.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wac.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://vca.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://xti.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://rzf.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://ucz.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://tzn.epnwcf.com

TS:   process.platform;  process.version
来源：http://kgq.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mnb.aizwys.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://you.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qpf.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rvs.zhixingplan.top

================================================================================
来源：http://wtr.tanke756.top

N. 数据结构与算法
来源：http://dlx.52xcode.cn

================================================================================
来源：http://ahg.zdbjq.cn


<!-- 参考信息 -->