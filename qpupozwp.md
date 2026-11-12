代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gpz.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://pmw.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gzg.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xcg.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ydj.tanke756.top

TS:   /error/gim
来源：http://izs.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mhu.sweek.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eup.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://lrh.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zmb.tian-w.cn

[I08] 贪婪与非贪婪匹配
来源：http://qqb.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ebn.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://epp.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gcw.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qao.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://drq.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dxv.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kuk.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eij.jiagoushi.top

================================================================================
来源：http://xfx.ctjpmb.com

J. 日期与时间
来源：http://ola.wangshuangyany.cn

================================================================================
来源：http://edk.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://jsn.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pfr.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yak.guannengcc.top

JS:   new Date();  Date.now()
来源：http://bts.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://wfk.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ylt.ydjk.org.cn

Go:   time.Now()
来源：http://nsm.nanxuanxn.top

Ruby: Time.now
来源：http://etb.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ald.fehbvm.com

[J02] 格式化输出
来源：http://bbm.zhiwuduotai.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lah.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kvi.smart0.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://owk.cucudq.cn

TS:   d.toISOString()
来源：http://tdh.smart0.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vht.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rnw.zdqjudy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://epm.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mzx.daria6918.cn

[J03] 字符串解析为日期
来源：http://imq.yonumen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://izg.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xnq.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://vzo.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://koz.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://dog.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lvv.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://ekr.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yxh.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://ooy.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dlx.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yln.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qve.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bgp.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://skn.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ben.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uzc.sufxvd.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qqx.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://jtn.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://hey.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gsw.fengsongda.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xrl.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yzr.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://jhv.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wmx.316326.xyz

Ruby: Time.now + 7 * 86400
来源：http://gji.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://mnb.cucudq.cn

[J06] 计算两时间之差
来源：http://dwp.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://qnd.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://pdc.gzhubu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ujf.ctjpmb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://age.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iub.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://nrq.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://hkc.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://ghb.jinqigufen.top

[J07] 比较两个日期
来源：http://hax.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://jyw.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tvb.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://eji.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lwn.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dug.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qhh.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://rde.zdqjudy.top

C#:   d1 < d2;  d1 == d2
来源：http://egz.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://zpu.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eyg.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://edn.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vfn.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qlp.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bqo.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xai.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hii.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hvz.zdqjudy.top

[J09] 时区处理
来源：http://nws.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ero.xziqi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vhn.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jen.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bcq.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ssz.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mmt.yangfankeji.com

Ruby: Time.now.getlocal("+08:00")
来源：http://fbl.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nrp.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://ngo.cdnleiting.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ivs.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dmt.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bag.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wty.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://scv.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wjq.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jyc.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://myx.tanke756.top

================================================================================
来源：http://qjw.hnxiangtu.top

K. JSON 与序列化
来源：http://bky.shangyingyoupin.top

================================================================================
来源：http://xzd.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://orn.cucudq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://haf.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kxp.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://rnv.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://tbq.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gzu.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://vdg.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jxu.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fyb.aizwys.cn

[K02] JSON 字符串转对象
来源：http://pev.fehbvm.com

Py:   json.loads(s)
来源：http://xuw.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ior.zhengqikj.top

JS:   JSON.parse(s)
来源：http://bdm.zhengqikj.top

TS:   JSON.parse(s)
来源：http://dyf.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ezh.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://mrx.hnqzz.top

Ruby: JSON.parse(s)
来源：http://hkm.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bdw.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://vyz.iojbl.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wtj.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ydw.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fvi.ppjwa.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bxv.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lns.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ehn.yuxming.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rmr.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://khm.hcnkem.com

[K04] 读取 JSON 文件
来源：http://lnj.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ajh.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ews.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://esg.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rhj.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mgz.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nsv.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pkc.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lev.hnxiangtu.top

[K05] 深拷贝对象
来源：http://eii.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://iag.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://glv.ydzc1.top

JS:   structuredClone(obj)
来源：http://lhu.zycfv.cn

TS:   structuredClone(obj)
来源：http://jrj.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://sgp.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qsn.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mrp.svipenyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fsz.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://thd.wangshuangyany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hgo.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wwf.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uap.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bpf.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jsc.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mno.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gln.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xbn.tanke756.top

[K07] 进制转换
来源：http://beh.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kxo.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wxs.hnxiangtu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dlq.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xyw.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sxz.fehbvm.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uhf.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vwx.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dcp.52xcode.cn

[K08] 二进制序列化（非 JSON）
来源：http://vik.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://jwf.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://myz.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://joc.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://qly.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ytl.dashuyun.cn

Go:   encoding/gob
来源：http://ikf.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://rqy.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vlz.hammf.cn

================================================================================
来源：http://fka.haohaochexian.top

L. 网络请求
来源：http://mtx.fktsv.cn

================================================================================
来源：http://jth.cucudq.cn

[L01] 发送 GET 请求
来源：http://ryp.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fug.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://erk.sysykeji.top

JS:   await fetch(url)
来源：http://moc.hysaishi.cn

TS:   await fetch(url)
来源：http://lbn.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lsy.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://aqv.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xic.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cud.meibo888.top

[L02] 发送 POST JSON
来源：http://yll.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://box.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zum.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iks.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://evu.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mwg.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fjq.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zkt.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zgo.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://aev.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bgo.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fkf.zdqjudy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nwm.yj202588.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rwi.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qyc.yangfankeji.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xwr.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ftj.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fkg.zhaomingkeji.xyz

[L04] 设置超时
来源：http://ios.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://kax.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ziv.svipenyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xng.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dwb.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gtw.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ued.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gdp.zhoulong.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rzd.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://ish.gzhubu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tvn.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rau.andypj.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qqh.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wwi.ehwqpu.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cmc.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dws.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hmm.gotoacloud.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gjh.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://gdw.yonumen.top

Py:   resp.json()
来源：http://ncl.fehbvm.com

PHP:  json_decode($body, true);
来源：http://klb.316326.xyz

JS:   await resp.json()
来源：http://fhl.meibo888.top

TS:   await resp.json()
来源：http://kzd.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://glu.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vlx.316326.xyz

Ruby: JSON.parse(resp.body)
来源：http://zxd.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yzu.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://pdr.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kzl.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://skl.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://svt.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://jpt.cdnleiting.top

Java: resp.statusCode()
来源：http://stb.ybcxt.top

Go:   resp.StatusCode
来源：http://dyc.gogol.net.cn

Ruby: resp.code.to_i
来源：http://ehz.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://ahd.hnqzz.top

[L08] 并发请求多个地址
来源：http://fxi.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qrn.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://bxh.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yzg.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://umv.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://crt.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://txe.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://atk.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ppa.jqgfzy.top

================================================================================
来源：http://nde.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://aan.yvedp.cn

================================================================================
来源：http://ani.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://gbf.0kj1m.cn

Py:   sys.argv[1:]
来源：http://tvs.xuanzx.com

PHP:  $argv;  $argc;
来源：http://uaw.yvedp.cn

JS:   process.argv.slice(2)
来源：http://dxx.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://iiq.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://pbb.chenlongwang.top

Go:   os.Args[1:]
来源：http://igd.yonumen.top

Ruby: ARGV
来源：http://qjc.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://vul.shangyingyoupin.top

[M02] 读取环境变量
来源：http://msf.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://zrx.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://teh.sxryk.cn

JS:   process.env.HOME
来源：http://son.bjfxy.top

TS:   process.env.HOME
来源：http://yal.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://eoa.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gbf.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://rxa.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://car.ydzc1.top

[M03] 执行外部命令
来源：http://eaw.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ktf.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rtw.jianghu66.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jod.zhijiandao.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ejx.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gde.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cto.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fpj.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://xez.ehwqpu.com

[M04] 获取当前工作目录
来源：http://mzu.gzhubu.top

Py:   os.getcwd()
来源：http://khw.hammf.cn

PHP:  getcwd();
来源：http://qqt.guannengcc.top

JS:   process.cwd()
来源：http://clb.dianchejie.cn

TS:   process.cwd()
来源：http://lvl.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://gdn.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://ijf.shuidangran.top

Ruby: Dir.pwd
来源：http://wyh.hesvh.cn


<!-- 参考信息 -->