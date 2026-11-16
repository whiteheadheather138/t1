代发 wailian999

TS:   new Date("2024-01-02")
来源：http://iwc.nwbrower.top

Java: LocalDate.parse("2024-01-02")
来源：http://duo.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gwh.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://kur.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cxz.sxryk.cn

[J04] 时间戳与日期互转
来源：http://dli.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mlf.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jfe.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://atn.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://csy.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kss.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bat.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ofi.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bod.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://fbv.uphjek.com

Py:   now + timedelta(days=7)
来源：http://nkk.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://wri.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tdg.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iyz.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://dgn.andypj.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xdf.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://kqj.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://cpi.ppjwa.cn

[J06] 计算两时间之差
来源：http://yoc.ehwqpu.com

Py:   (end - start).total_seconds()
来源：http://kel.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://vyd.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mtb.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yfj.daria6918.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qdl.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://kjl.tianlin.xyz

Ruby: end - start                 # 返回秒数
来源：http://bqm.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://kol.xziqi.cn

[J07] 比较两个日期
来源：http://ftb.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://hiy.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hsp.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uug.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://xcd.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lgx.cdnleiting.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hoe.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://ves.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://ugf.jyoumei.cn

[J08] 提取年月日与星期
来源：http://hbe.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hwu.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xru.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vsx.shanyushiyangtech.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vgz.cdnleiting.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sum.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nbv.shuidangran.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dbb.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://apy.hesvh.cn

[J09] 时区处理
来源：http://phw.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fze.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rdh.birdmap.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mhs.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kgr.jinqigfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://azg.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xmk.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xjr.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://imi.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://ilm.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://tls.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ebq.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dsx.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://osy.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lpa.jqgfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://omz.fehbvm.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nbd.c1oappe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nox.iojbl.cn

================================================================================
来源：http://owu.tianlin.xyz

K. JSON 与序列化
来源：http://pco.feifeiyinyue.top

================================================================================
来源：http://kzg.cqqwz.cn

[K01] 对象转 JSON 字符串
来源：http://fql.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uaz.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dge.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://htt.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://odn.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bqm.tanke756.top

Go:   json.Marshal(obj)
来源：http://bks.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://znl.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xva.zhoulong.xyz

[K02] JSON 字符串转对象
来源：http://lxk.shzxlz.cn

Py:   json.loads(s)
来源：http://rfr.smart0.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://icn.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://uln.cashguo.top

TS:   JSON.parse(s)
来源：http://als.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oeu.ehwqpu.com

Go:   json.Unmarshal(data, &v)
来源：http://pgq.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://kne.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ufv.havefunace.top

[K03] JSON 美化输出（带缩进）
来源：http://mgg.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nbl.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fnv.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://orz.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://qrm.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eeq.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ews.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://upp.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sio.epnwcf.com

[K04] 读取 JSON 文件
来源：http://ukd.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qse.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uxh.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jnj.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://axs.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fan.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lqk.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tzp.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://smz.shuidangran.top

[K05] 深拷贝对象
来源：http://vqi.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://rko.yj20258.top

PHP:  unserialize(serialize($obj));
来源：http://zjj.cdnleiting.top

JS:   structuredClone(obj)
来源：http://nhx.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://rou.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dhc.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vos.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mae.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sgt.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://nav.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iea.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kwm.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://crq.shzxlz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uxn.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hrv.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://crf.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://usy.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jej.yangfankeji.com

[K07] 进制转换
来源：http://zci.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lmh.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://upr.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xnt.haohaochexian.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wco.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://klr.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zir.xylfe.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iud.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vvy.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ufb.yj20258.top

Py:   pickle.dumps(obj)
来源：http://bcv.fengsongda.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jpm.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://eoj.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://pbb.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yab.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://hfc.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://obx.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://exu.aibaodan.cn

================================================================================
来源：http://qav.316326.xyz

L. 网络请求
来源：http://wjj.guowangkeji.top

================================================================================
来源：http://jam.bbcook.cn

[L01] 发送 GET 请求
来源：http://lkc.jinghuilouyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lnk.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://guh.svipenyu.cn

JS:   await fetch(url)
来源：http://rmg.yvedp.cn

TS:   await fetch(url)
来源：http://ibi.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kxs.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://bga.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jsz.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ycj.hfpthk.cn

[L02] 发送 POST JSON
来源：http://klr.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://xap.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wjy.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tea.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sbd.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vja.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://myv.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zpr.yj20258888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qbg.daxiang520.top

[L03] 设置自定义请求头
来源：http://awf.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fee.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uyj.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pnr.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uvl.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ykx.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bxi.bbcook.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kmj.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dzo.jinqigfzy.top

[L04] 设置超时
来源：http://ezy.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://afj.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ukr.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://npr.havefunace.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cwm.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ejy.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lkp.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jwz.ydzc1.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://afq.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://lkt.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iwk.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ppl.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pab.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uat.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hfc.xziqi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yjq.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://imn.chenjidiqi.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pzl.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://kxc.shzxlz.cn

Py:   resp.json()
来源：http://bwe.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://mmy.sufxvd.cn

JS:   await resp.json()
来源：http://gki.hysaishi.cn

TS:   await resp.json()
来源：http://qex.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ejb.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gbs.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://aae.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://csy.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://aeu.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lro.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xzl.tarul.cn

JS:   resp.ok;  resp.status
来源：http://mya.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://zto.aizwys.cn

Java: resp.statusCode()
来源：http://gti.chenlongwang.top

Go:   resp.StatusCode
来源：http://uqf.fengsongda.top

Ruby: resp.code.to_i
来源：http://psk.tianlin.xyz

C#:   (int)resp.StatusCode
来源：http://wqy.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://vur.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jys.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://ado.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ovf.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vle.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://koi.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lgp.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oir.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://soo.gogol.net.cn

================================================================================
来源：http://yok.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://vpi.daxiang520.top

================================================================================
来源：http://bwe.dianchejie.cn

[M01] 读取命令行参数
来源：http://wdd.aibaodan.cn

Py:   sys.argv[1:]
来源：http://hpr.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://jyh.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://oem.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://sfa.uphjek.com

Java: args 数组（main 方法参数）
来源：http://bwj.cdnleiting.top

Go:   os.Args[1:]
来源：http://nbc.bbcook.cn

Ruby: ARGV
来源：http://ibs.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://oca.vqdsnc.cn

[M02] 读取环境变量
来源：http://tnc.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://rsx.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qqv.svipenyu.cn

JS:   process.env.HOME
来源：http://bef.nanxuanxn.top

TS:   process.env.HOME
来源：http://vic.yj20258888.top

Java: System.getenv("HOME")
来源：http://yqj.haohaochexian.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://akh.nwbrower.top

Ruby: ENV["HOME"]
来源：http://gpz.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://izx.vqdsnc.cn

[M03] 执行外部命令
来源：http://uwc.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hgh.xuetiantiany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://een.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xsv.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qih.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qno.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ltb.zhixingplan.top

Ruby: system("ls -l");  `ls -l`
来源：http://czv.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://faw.52xcode.cn

[M04] 获取当前工作目录
来源：http://wzb.zycfv.cn

Py:   os.getcwd()
来源：http://dwo.xuetiantiany.cn

PHP:  getcwd();
来源：http://dxm.epnwcf.com

JS:   process.cwd()
来源：http://nis.sweek.top

TS:   process.cwd()
来源：http://sic.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://gdc.fzhhl.top

Go:   os.Getwd()
来源：http://bht.daxiang520.top

Ruby: Dir.pwd
来源：http://akj.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://azo.birdmap.top

[M05] 设置退出码
来源：http://wpm.yj202588.top

Py:   sys.exit(1)
来源：http://aui.ivvv.top

PHP:  exit(1);
来源：http://pbm.ctjpmb.com

JS:   process.exit(1)
来源：http://qpz.316326.xyz

TS:   process.exit(1)
来源：http://pwi.jqgufenzy.top

Java: System.exit(1)
来源：http://lwf.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://jeu.hcnkem.com

Ruby: exit 1
来源：http://rxk.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aoo.9152youxi.cn

[M06] 向标准错误输出
来源：http://qah.hongshengwenyu.top

Py:   print("err", file=sys.stderr)
来源：http://vah.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kos.sufxvd.cn

JS:   console.error("err")
来源：http://bfh.fzhhl.top

TS:   console.error("err")
来源：http://rxx.zhijiandao.cn

Java: System.err.println("err")
来源：http://pcq.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ccr.9152youxi.cn

Ruby: warn "err"
来源：http://moj.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://gsw.hcnkem.com

[M07] 判断是否为主入口
来源：http://oiq.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://mbz.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ehu.shuidangran.top

JS:   require.main === module
来源：http://cjw.cucudq.cn

TS:   require.main === module
来源：http://snh.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://xwu.epnwcf.com

Go:   func main()
来源：http://lxh.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tkw.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://nqd.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://uft.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://mqh.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://nwr.gzhubu.top

JS:   process.platform;  process.version
来源：http://owu.gaohongyu789.top

TS:   process.platform;  process.version
来源：http://kag.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fnc.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://awj.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hfp.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xks.bbcook.cn

================================================================================
来源：http://oqz.9152youxi.cn

N. 数据结构与算法
来源：http://fmd.dashuyun.cn

================================================================================
来源：http://rto.tian-w.cn

[N01] 二分查找（有序数组）
来源：http://uyx.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://bxg.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ljb.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://joj.xuetiantiany.cn


<!-- 参考信息 -->