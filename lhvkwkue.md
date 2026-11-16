代发 wailian999

TS:   new Date("2024-01-02")
来源：http://qml.sjlbkw.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iok.feifeiyinyue.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xht.yonumen.top

Ruby: Date.parse("2024-01-02")
来源：http://clj.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qqu.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://rvz.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gqy.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ygn.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hlo.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kok.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ddy.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kga.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wje.pengpengdd.cyou

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vwz.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://ufx.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://evu.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://nkb.meibo888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zan.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qhm.shanyushiyangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://qlv.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rdd.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://ghd.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://wem.hfpthk.cn

[J06] 计算两时间之差
来源：http://ceo.ehwqpu.com

Py:   (end - start).total_seconds()
来源：http://vzj.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://bxz.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fem.zhengqikj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://umv.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qar.birdmap.top

Go:   end.Sub(start).Hours()
来源：http://lby.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://nkx.wangdashe.top

C#:   (end - start).TotalSeconds
来源：http://uer.zhixingplan.top

[J07] 比较两个日期
来源：http://zzi.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://zdr.gzhubu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://svd.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://axu.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://puo.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://six.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kpo.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://whf.nanxuanxn.top

C#:   d1 < d2;  d1 == d2
来源：http://zyv.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://coo.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wqg.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://igo.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zmz.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pnl.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jrt.birdmap.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jhj.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wnp.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lkj.xziqi.cn

[J09] 时区处理
来源：http://kuw.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aoj.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bzj.dianchejie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uzu.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://azm.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ceu.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://abr.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://xbk.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pho.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://qwu.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lfb.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aff.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zgz.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://idn.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://swj.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dyo.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://unx.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ayz.hywenlv.cn

================================================================================
来源：http://emp.jinghuilouyu.cn

K. JSON 与序列化
来源：http://iir.ctjpmb.com

================================================================================
来源：http://aov.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://dtn.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nsn.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bhl.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://wel.daxiang520.top

TS:   JSON.stringify(obj)
来源：http://sst.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gpw.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://wbl.chenlongwang.top

Ruby: obj.to_json                                     // require "json"
来源：http://oot.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mtp.yvedp.cn

[K02] JSON 字符串转对象
来源：http://jey.ppjwa.cn

Py:   json.loads(s)
来源：http://ohf.jinyuanbaomall.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wrv.yj202588.top

JS:   JSON.parse(s)
来源：http://svv.svipenyu.cn

TS:   JSON.parse(s)
来源：http://bfh.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tre.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://rfo.iojbl.cn

Ruby: JSON.parse(s)
来源：http://xfq.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nev.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://qpa.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ivu.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zve.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://him.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://xwv.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yef.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iat.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hcq.shuidangran.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bli.sxryk.cn

[K04] 读取 JSON 文件
来源：http://yvx.svipenyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kzr.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mtm.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://koq.ydzc1.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qaq.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eem.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wmu.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mzb.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dnt.jianghu66.top

[K05] 深拷贝对象
来源：http://ebg.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://xex.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://urn.ywan-chungtsiang.top

JS:   structuredClone(obj)
来源：http://whn.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://fdm.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://gzq.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://crg.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hzj.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://ycu.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://fni.hcnkem.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dow.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mhw.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sbl.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ysj.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://opb.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://vpm.yangfankeji.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qvw.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fyy.bbcook.cn

[K07] 进制转换
来源：http://ljq.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mzs.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eku.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tef.hywenlv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lxn.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wqg.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ipd.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hyi.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tam.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://tlo.yfazqb.com

Py:   pickle.dumps(obj)
来源：http://gdu.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://anw.sysykeji.top

JS:   v8.serialize(obj)        // Node
来源：http://owx.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://zlg.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vnk.xuanzx.com

Go:   encoding/gob
来源：http://nsv.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://yej.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kml.nanxuanxn.top

================================================================================
来源：http://ytj.ydjk.org.cn

L. 网络请求
来源：http://cyz.ydzc1.top

================================================================================
来源：http://hqe.tarul.cn

[L01] 发送 GET 请求
来源：http://kgb.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tmd.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zny.ctjpmb.com

JS:   await fetch(url)
来源：http://yqx.hfpthk.cn

TS:   await fetch(url)
来源：http://vhc.9152youxi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jew.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://rkm.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://aui.daria6918.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ejx.xuetiantiany.cn

[L02] 发送 POST JSON
来源：http://xsx.aizwys.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jib.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rnq.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wax.fanxiaobao.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hya.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://akw.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ypr.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://utp.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://urq.cashguo.top

[L03] 设置自定义请求头
来源：http://ujo.jianghu66.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sqg.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://isr.ywan-chungtsiang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yqe.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mci.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qiv.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jum.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nez.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zlq.fzhhl.top

[L04] 设置超时
来源：http://jkt.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://bph.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ugn.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wtv.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mik.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kky.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kal.yj20258888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vno.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://evs.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://ofn.yj20258888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://unx.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://weo.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lan.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nlp.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oon.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uhz.uphjek.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ygc.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://czn.xziqi.cn

[L06] 解析响应为 JSON
来源：http://iwr.shanyushiyangtech.top

Py:   resp.json()
来源：http://ucs.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://qnp.iojbl.cn

JS:   await resp.json()
来源：http://grr.guannengcc.top

TS:   await resp.json()
来源：http://orb.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rjn.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jfh.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://urt.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://opv.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://jql.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bzz.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tww.jiagoushi.top

JS:   resp.ok;  resp.status
来源：http://xsm.xuetiantiany.cn

TS:   resp.ok;  resp.status
来源：http://prs.gogol.net.cn

Java: resp.statusCode()
来源：http://hfz.bbcook.cn

Go:   resp.StatusCode
来源：http://srs.wangshuangyany.cn

Ruby: resp.code.to_i
来源：http://mwk.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://cjy.havefunace.top

[L08] 并发请求多个地址
来源：http://lbr.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qow.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://sct.52xcode.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sxw.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ufn.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hqx.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pxq.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lxz.ivvv.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cxk.nwbrower.top

================================================================================
来源：http://sur.jinqigfzy.top

M. 命令行 / 进程 / 环境
来源：http://fzm.jinqigufen.top

================================================================================
来源：http://tkn.quarkkingdee.top

[M01] 读取命令行参数
来源：http://dkt.mhx1999.top

Py:   sys.argv[1:]
来源：http://trn.guannengcc.top

PHP:  $argv;  $argc;
来源：http://xqa.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://tqt.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://qby.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://hcb.havefunace.top

Go:   os.Args[1:]
来源：http://plw.tianlin.xyz

Ruby: ARGV
来源：http://qqg.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://gik.yongpay.top

[M02] 读取环境变量
来源：http://feo.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://jfs.yuanzhike.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qxd.chenzaomai.com

JS:   process.env.HOME
来源：http://uhr.shangyingyoupin.top

TS:   process.env.HOME
来源：http://xda.redwolf501.top

Java: System.getenv("HOME")
来源：http://dgu.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zzk.yuanzhike.top

Ruby: ENV["HOME"]
来源：http://gai.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ndm.ehwqpu.com

[M03] 执行外部命令
来源：http://pss.sufxvd.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vtn.bbcook.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dav.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hcp.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://pdf.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gas.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lnh.gzhubu.top

Ruby: system("ls -l");  `ls -l`
来源：http://vvw.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://hdp.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://tde.ppjwa.cn

Py:   os.getcwd()
来源：http://gmg.yonumen.top

PHP:  getcwd();
来源：http://qgu.0kj1m.cn

JS:   process.cwd()
来源：http://yki.cashguo.top

TS:   process.cwd()
来源：http://uko.yuxming.cn

Java: Path.of("").toAbsolutePath()
来源：http://kin.xylfe.cn

Go:   os.Getwd()
来源：http://ztw.hammf.cn

Ruby: Dir.pwd
来源：http://ayz.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tyi.fehbvm.com

[M05] 设置退出码
来源：http://dng.c1oappe.top

Py:   sys.exit(1)
来源：http://evz.zhaomingkeji.xyz

PHP:  exit(1);
来源：http://grq.cqqwz.cn

JS:   process.exit(1)
来源：http://tey.aibaodan.cn

TS:   process.exit(1)
来源：http://yal.xziqi.cn

Java: System.exit(1)
来源：http://tmh.cucudq.cn

Go:   os.Exit(1)
来源：http://aqc.zhengqikj.top

Ruby: exit 1
来源：http://agk.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jka.tian-w.cn

[M06] 向标准错误输出
来源：http://yvc.fengsongda.top

Py:   print("err", file=sys.stderr)
来源：http://roe.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://imt.svipenyu.cn

JS:   console.error("err")
来源：http://ggk.xuanzx.com

TS:   console.error("err")
来源：http://mlm.zhiwuduotai.top

Java: System.err.println("err")
来源：http://yse.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pks.wangdashe.top

Ruby: warn "err"
来源：http://rmf.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://hzo.birdmap.top

[M07] 判断是否为主入口
来源：http://usx.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://sox.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ngf.xuetiantiany.cn

JS:   require.main === module
来源：http://fes.cashguo.top

TS:   require.main === module
来源：http://poy.iojbl.cn

Java: public static void main(String[] args)
来源：http://dkh.jqgufenzy.top

Go:   func main()
来源：http://xjj.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xhg.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://dkx.guowangkeji.top

[M08] 获取系统与运行时信息
来源：http://ibr.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://tum.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://mvv.hammf.cn

JS:   process.platform;  process.version
来源：http://erv.tarul.cn

TS:   process.platform;  process.version
来源：http://bdv.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gfl.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sgp.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wqm.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://psz.fktsv.cn

================================================================================
来源：http://qth.meibo888.top

N. 数据结构与算法
来源：http://djp.pengpengdd.cyou

================================================================================
来源：http://iob.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://zef.ivvv.top

Py:   bisect.bisect_left(arr, x)
来源：http://xpo.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vrl.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://stk.cashguo.top


<!-- 参考信息 -->