代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ssw.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://djm.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nsj.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eyr.guannengcc.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wjd.sweek.top

TS:   /error/gim
来源：http://gdd.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uvh.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fad.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://ttf.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hfc.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://yae.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://usn.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://exf.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jgg.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lnz.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://fqk.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aot.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jvc.bbcook.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vvp.feifeiyinyue.top

================================================================================
来源：http://ekg.fehbvm.com

J. 日期与时间
来源：http://rbz.xinyue.icu

================================================================================
来源：http://xyy.jiagoushi.top

[J01] 获取当前时间
来源：http://lew.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://npo.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mqp.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://aem.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://evs.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lba.nanxinkj.top

Go:   time.Now()
来源：http://vgc.fzhhl.top

Ruby: Time.now
来源：http://ldi.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uuw.cheryme.top

[J02] 格式化输出
来源：http://gqm.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://enz.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dxv.svipenyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ndl.sxryk.cn

TS:   d.toISOString()
来源：http://sxi.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://clo.yueranfly.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://drc.yangfankeji.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rtk.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gll.gotoacloud.top

[J03] 字符串解析为日期
来源：http://ugy.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ovk.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cix.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://nrn.cheryme.top

TS:   new Date("2024-01-02")
来源：http://xkl.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://qce.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hia.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://cxf.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cyl.sxryk.cn

[J04] 时间戳与日期互转
来源：http://aqy.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vwr.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hso.gaohongyu789.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yqp.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://bov.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nlg.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xcg.gogol.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://onj.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://auo.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://rin.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://xuj.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rpk.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kyn.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xvs.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://uew.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://swh.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://fov.fehbvm.com

C#:   DateTime.Now.AddDays(7)
来源：http://nbs.tian-w.cn

[J06] 计算两时间之差
来源：http://ffl.sjlbkw.cn

Py:   (end - start).total_seconds()
来源：http://hwc.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://dkk.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pxu.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ebr.shangyingyoupin.top

Java: Duration.between(start, end).toSeconds()
来源：http://xkp.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://xxu.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://oqh.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://pab.bjfxy.top

[J07] 比较两个日期
来源：http://quz.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://zny.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://avi.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://lay.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://thz.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zvu.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wqk.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://uzh.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://vis.vqdsnc.cn

[J08] 提取年月日与星期
来源：http://gle.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://svj.yanxiufei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qqs.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yel.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gvh.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ikr.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rcy.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hys.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kiy.guannengcc.top

[J09] 时区处理
来源：http://sae.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jva.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eit.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jxt.yj20258.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rwx.yj20258888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lix.gzhubu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ukr.tianlin.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://rla.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://msd.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://fro.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xua.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mft.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fvm.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ddk.ydjk.org.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rza.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dxe.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ycp.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://irw.nanxinkj.top

================================================================================
来源：http://btk.0kj1m.cn

K. JSON 与序列化
来源：http://qtv.hesvh.cn

================================================================================
来源：http://mlf.jiagoushi.top

[K01] 对象转 JSON 字符串
来源：http://wow.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ugl.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yuo.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://qid.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://bfy.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ott.yongpay.top

Go:   json.Marshal(obj)
来源：http://ffl.chenlongwang.top

Ruby: obj.to_json                                     // require "json"
来源：http://jjj.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gky.nwbrower.top

[K02] JSON 字符串转对象
来源：http://ape.xylfe.cn

Py:   json.loads(s)
来源：http://tkf.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aut.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://vkk.wangdashe.top

TS:   JSON.parse(s)
来源：http://iry.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lmd.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://ido.uphjek.com

Ruby: JSON.parse(s)
来源：http://xjj.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hxl.316326.xyz

[K03] JSON 美化输出（带缩进）
来源：http://ipk.smart0.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fxz.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gix.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nqm.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fgy.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oyy.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qvm.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://baq.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ebi.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://bqv.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pvk.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jpx.hysaishi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iwt.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eoi.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://myg.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vkk.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wld.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qiv.cucudq.cn

[K05] 深拷贝对象
来源：http://zqd.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://syi.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://rvo.yj20258888.top

JS:   structuredClone(obj)
来源：http://qan.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://sbg.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xxv.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nkb.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ncw.hcnkem.com

C#:   // 序列化往返，或自定义 Clone
来源：http://bmc.xziqi.cn

[K06] 解析 URL 查询串
来源：http://stv.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aaq.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gzi.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://slt.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qiy.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sbc.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vwe.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sgc.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tss.shzxlz.cn

[K07] 进制转换
来源：http://aaz.hnqzz.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://twn.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ayx.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vyh.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pcx.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eod.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ktg.smart0.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iun.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kkm.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://qap.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://ogi.ybcxt.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vrc.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://ypk.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://ofa.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jwx.shangyingyoupin.top

Go:   encoding/gob
来源：http://gdm.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://zsq.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dxi.fanxiaobao.xyz

================================================================================
来源：http://fdv.0kj1m.cn

L. 网络请求
来源：http://dxi.316326.xyz

================================================================================
来源：http://odw.havefunace.top

[L01] 发送 GET 请求
来源：http://ynb.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dxb.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jot.hammf.cn

JS:   await fetch(url)
来源：http://vey.sweek.top

TS:   await fetch(url)
来源：http://wyz.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ltv.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://vti.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://tvr.sjlbkw.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mgw.sweek.top

[L02] 发送 POST JSON
来源：http://bob.ctjpmb.com

Py:   requests.post(url, json={"a": 1})
来源：http://zmi.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bwy.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sub.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://adi.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://def.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bbg.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oew.tarul.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ixz.hcnkem.com

[L03] 设置自定义请求头
来源：http://zvk.havefunace.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hoh.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sae.dianchejie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sri.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dvq.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zhx.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://agx.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cvi.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ijp.ydjk.org.cn

[L04] 设置超时
来源：http://ybr.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://wbe.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yrx.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mih.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wwl.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gzj.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gcz.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zij.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nai.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://ufn.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vpa.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ysi.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ghx.0kj1m.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rgx.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gpu.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kfh.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://isv.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://apz.nanxuanxn.top

[L06] 解析响应为 JSON
来源：http://sfz.cheryme.top

Py:   resp.json()
来源：http://ymz.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://jmi.ivvv.top

JS:   await resp.json()
来源：http://zxw.hesvh.cn

TS:   await resp.json()
来源：http://bfz.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bhu.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://llr.jinghuilouyu.cn

Ruby: JSON.parse(resp.body)
来源：http://znj.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qaa.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://eyc.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zbr.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ikd.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://sia.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://aoi.hesvh.cn

Java: resp.statusCode()
来源：http://lag.tanke756.top

Go:   resp.StatusCode
来源：http://hoc.cucudq.cn

Ruby: resp.code.to_i
来源：http://uwk.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://huv.gzhubu.top

[L08] 并发请求多个地址
来源：http://pms.nanxuanxn.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wrs.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://uia.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yxk.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bla.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kbx.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tzk.wangshuangyany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vfn.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hul.xylfe.cn

================================================================================
来源：http://jhv.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://qje.jyoumei.cn

================================================================================
来源：http://yxm.iojbl.cn

[M01] 读取命令行参数
来源：http://yrk.dianchejie.cn

Py:   sys.argv[1:]
来源：http://rpb.meibo888.top

PHP:  $argv;  $argc;
来源：http://zcb.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://hrt.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://sih.gogol.net.cn

Java: args 数组（main 方法参数）
来源：http://grv.zhoulong.xyz

Go:   os.Args[1:]
来源：http://jkl.gotoacloud.top

Ruby: ARGV
来源：http://tkz.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://olu.sxryk.cn

[M02] 读取环境变量
来源：http://nwt.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://bim.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kkv.epnwcf.com

JS:   process.env.HOME
来源：http://zpp.gaohongyu789.top

TS:   process.env.HOME
来源：http://cbk.fktsv.cn

Java: System.getenv("HOME")
来源：http://ual.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cmh.ivvv.top

Ruby: ENV["HOME"]
来源：http://akx.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hxt.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://fzq.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://emn.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hjq.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dbj.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://suk.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ysz.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bko.zhaomingkeji.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://dss.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://ehi.feifeiyinyue.top

[M04] 获取当前工作目录
来源：http://rtq.zycfv.cn

Py:   os.getcwd()
来源：http://pgw.shanyushiyangtech.top

PHP:  getcwd();
来源：http://ghv.vqdsnc.cn

JS:   process.cwd()
来源：http://ntz.dashuyun.cn

TS:   process.cwd()
来源：http://sih.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://gml.yuxming.cn

Go:   os.Getwd()
来源：http://nmz.shzxlz.cn

Ruby: Dir.pwd
来源：http://syj.aizwys.cn


<!-- 参考信息 -->