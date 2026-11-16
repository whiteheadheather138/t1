代发 wailian999

TS:   new Date("2024-01-02")
来源：http://vfw.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://adn.tianlin.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pvc.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://sag.shanyushiyangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mss.tarul.cn

[J04] 时间戳与日期互转
来源：http://vfg.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fst.hnqzz.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://isf.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fmw.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://ywd.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uff.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ycm.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ibm.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xjj.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://irk.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://axk.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://cvd.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qmu.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ktj.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://qof.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://glc.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://rxs.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pks.chenlongwang.top

[J06] 计算两时间之差
来源：http://sko.fanxiaobao.xyz

Py:   (end - start).total_seconds()
来源：http://vhk.aizwys.cn

PHP:  $end->diff($start)->days;
来源：http://wyn.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jol.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ecc.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://zeb.c1oappe.top

Go:   end.Sub(start).Hours()
来源：http://akw.nanxuanxn.top

Ruby: end - start                 # 返回秒数
来源：http://bqf.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://vco.uphjek.com

[J07] 比较两个日期
来源：http://pfg.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://fqt.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cum.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://owl.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://beo.xylfe.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ffx.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pvr.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hye.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://bvc.yangfankeji.com

[J08] 提取年月日与星期
来源：http://hrs.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zfp.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://obm.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vhn.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gqw.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nzf.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tgv.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jem.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jsu.xylfe.cn

[J09] 时区处理
来源：http://qxh.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hyy.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xpk.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eab.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nzg.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xwb.epnwcf.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vlp.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yzt.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ckd.xingfuxueyuan.xyz

[J10] 取今天 / 本月第一天
来源：http://fnx.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pxa.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://afs.kuanghao11.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ecz.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pph.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://owy.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jga.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uay.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cfx.smart0.xyz

================================================================================
来源：http://yik.andypj.xyz

K. JSON 与序列化
来源：http://vwz.shangyingyoupin.top

================================================================================
来源：http://cpi.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://lnb.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://icf.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tvl.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://dsb.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://dqu.sweek.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eep.tian-w.cn

Go:   json.Marshal(obj)
来源：http://orb.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://pyj.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zgj.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://dvf.zhongyouzk.top

Py:   json.loads(s)
来源：http://yex.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yxf.xuanzx.com

JS:   JSON.parse(s)
来源：http://rjf.gogol.net.cn

TS:   JSON.parse(s)
来源：http://ukm.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jrz.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://vpb.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://pah.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qnb.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://brw.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cvi.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qhj.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://puy.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ijt.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rmh.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ehs.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://uey.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bvg.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://jmm.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fyx.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eah.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wrv.andypj.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tka.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qzn.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wqf.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bxa.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ckb.cucudq.cn

[K05] 深拷贝对象
来源：http://oky.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://bsi.xingfuxueyuan.xyz

PHP:  unserialize(serialize($obj));
来源：http://hqb.shuidangran.top

JS:   structuredClone(obj)
来源：http://uzk.meibo888.top

TS:   structuredClone(obj)
来源：http://gly.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pfe.zhengqikj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qgv.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gcx.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fgo.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://gni.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wsi.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zav.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jsw.birdmap.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yqs.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gfb.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zuo.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qho.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bld.shanyushiyangtech.top

[K07] 进制转换
来源：http://daj.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oqh.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://siv.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fgh.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xmx.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bfb.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uqi.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zbr.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://alc.cdnleiting.top

[K08] 二进制序列化（非 JSON）
来源：http://gay.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://fdg.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://krl.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://zfl.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://rqu.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zdh.cheryme.top

Go:   encoding/gob
来源：http://hba.vqdsnc.cn

Ruby: Marshal.dump(obj)
来源：http://ggy.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gzg.hcnkem.com

================================================================================
来源：http://zzn.pycfn.com

L. 网络请求
来源：http://kfk.shangyingyoupin.top

================================================================================
来源：http://wjj.yvedp.cn

[L01] 发送 GET 请求
来源：http://ckf.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pmt.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uvl.zhengqikj.top

JS:   await fetch(url)
来源：http://gge.gotoacloud.top

TS:   await fetch(url)
来源：http://gcc.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xyu.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://zbt.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qzu.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://och.gotoacloud.top

[L02] 发送 POST JSON
来源：http://cas.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://qyu.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lso.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dnr.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xmi.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://azi.chenjidiqi.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://peo.shzxlz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kld.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kbb.smart0.xyz

[L03] 设置自定义请求头
来源：http://kle.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pgr.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qlo.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bse.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hwu.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kfn.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bmb.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jrd.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oqb.cqqwz.cn

[L04] 设置超时
来源：http://pno.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://haz.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://njl.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vgi.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tub.ehwqpu.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tbr.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://agh.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dkq.pengpengdd.cyou

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wcu.yueranfly.top

[L05] 上传文件（multipart）
来源：http://iwp.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qfp.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iyo.xuanzx.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sqo.zhengqikj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zds.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mku.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oal.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rul.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ahf.ivvv.top

[L06] 解析响应为 JSON
来源：http://crn.guowangkeji.top

Py:   resp.json()
来源：http://dzn.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://jug.cucudq.cn

JS:   await resp.json()
来源：http://xpn.bbcook.cn

TS:   await resp.json()
来源：http://urb.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pwm.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mqe.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://oas.quarkkingdee.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lby.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://xty.jinqigfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dqf.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nmh.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://ifl.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://rmd.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://utl.zhongyouzk.top

Go:   resp.StatusCode
来源：http://xas.chenlongwang.top

Ruby: resp.code.to_i
来源：http://ygm.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://ijq.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://ygw.sysykeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uxn.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://lvz.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://afv.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://abs.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fsz.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uux.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wom.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hbv.cashguo.top

================================================================================
来源：http://cti.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://mbs.quarkkingdee.top

================================================================================
来源：http://zry.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://fww.havefunace.top

Py:   sys.argv[1:]
来源：http://uiu.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://icc.yj202588.top

JS:   process.argv.slice(2)
来源：http://pvq.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://zry.yueranfly.top

Java: args 数组（main 方法参数）
来源：http://vpw.tianlin.xyz

Go:   os.Args[1:]
来源：http://edb.zdbjq.cn

Ruby: ARGV
来源：http://xme.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://ktu.jqgufenzy.top

[M02] 读取环境变量
来源：http://oyp.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://ijl.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uwh.nanxuanxn.top

JS:   process.env.HOME
来源：http://uvn.yangfankeji.com

TS:   process.env.HOME
来源：http://xtm.nanxuanxn.top

Java: System.getenv("HOME")
来源：http://wya.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oab.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://fdq.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qzv.zhoulong.xyz

[M03] 执行外部命令
来源：http://tep.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ybu.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gil.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rwj.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lid.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ibi.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://glf.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://lwv.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://ekj.tian-w.cn

[M04] 获取当前工作目录
来源：http://ayd.hysaishi.cn

Py:   os.getcwd()
来源：http://zmw.shzxlz.cn

PHP:  getcwd();
来源：http://eqx.sysykeji.top

JS:   process.cwd()
来源：http://nsb.ctjpmb.com

TS:   process.cwd()
来源：http://ncf.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://crw.ydjk.org.cn

Go:   os.Getwd()
来源：http://uqp.vqdsnc.cn

Ruby: Dir.pwd
来源：http://mnt.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dga.gotoacloud.top

[M05] 设置退出码
来源：http://meg.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://tbk.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://cgg.aibaodan.cn

JS:   process.exit(1)
来源：http://ugs.jqgfzy.top

TS:   process.exit(1)
来源：http://dty.shuidangran.top

Java: System.exit(1)
来源：http://rbw.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://cat.zhengqikj.top

Ruby: exit 1
来源：http://dsy.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jyc.jinqigufen.top

[M06] 向标准错误输出
来源：http://ijp.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://zdm.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qny.zycfv.cn

JS:   console.error("err")
来源：http://wky.0kj1m.cn

TS:   console.error("err")
来源：http://fko.yonumen.top

Java: System.err.println("err")
来源：http://uwt.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vzq.yangfankeji.com

Ruby: warn "err"
来源：http://yxq.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://fyn.0kj1m.cn

[M07] 判断是否为主入口
来源：http://llw.zhixingplan.top

Py:   if __name__ == "__main__":
来源：http://wnz.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ryt.hammf.cn

JS:   require.main === module
来源：http://mcp.zhaomingkeji.xyz

TS:   require.main === module
来源：http://zaw.yongpay.top

Java: public static void main(String[] args)
来源：http://ldn.kuanghao11.cn

Go:   func main()
来源：http://lbv.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tcx.cucudq.cn

C#:   static void Main(string[] args)
来源：http://doy.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://cgw.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://gje.xinyue.icu

PHP:  PHP_OS;  phpversion();
来源：http://laz.shuidangran.top

JS:   process.platform;  process.version
来源：http://rrb.nanxuanxn.top

TS:   process.platform;  process.version
来源：http://ric.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tnd.nanxuanxn.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://igm.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vpo.feifeiyinyue.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yxw.xylfe.cn

================================================================================
来源：http://kqz.shangyingyoupin.top

N. 数据结构与算法
来源：http://fqo.jinyuanbaomall.cn

================================================================================
来源：http://xeo.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://auq.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pjq.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aoq.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qfo.dashuyun.cn


<!-- 参考信息 -->