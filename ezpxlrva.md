代发 wailian999

Ruby: s.scan(/error/i)
来源：http://jdo.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jho.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://ytk.kuanghao11.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pxo.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ywf.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://thp.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://htz.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uoc.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fvd.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://auw.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gav.ivvv.top

================================================================================
来源：http://ikc.yj20258.top

J. 日期与时间
来源：http://uof.chenlongwang.top

================================================================================
来源：http://dzf.fzhhl.top

[J01] 获取当前时间
来源：http://abs.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jzd.fanxiaobao.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hao.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://vey.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://crv.xingfuxueyuan.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://udn.svipenyu.cn

Go:   time.Now()
来源：http://kaz.xziqi.cn

Ruby: Time.now
来源：http://gvf.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zlz.haohaochexian.top

[J02] 格式化输出
来源：http://rxr.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wxw.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ujn.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://byt.jlsjyb.cn

TS:   d.toISOString()
来源：http://ccs.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kgv.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qpk.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xzu.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tqd.9152youxi.cn

[J03] 字符串解析为日期
来源：http://pnm.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bdo.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bfx.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://pwx.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://frs.fengsongda.top

Java: LocalDate.parse("2024-01-02")
来源：http://piv.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://olj.jinqigfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://sqs.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zga.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://snr.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qlr.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rel.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pxt.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://btf.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sms.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mau.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jtd.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lxb.sweek.top

[J05] 时间加减（加 7 天）
来源：http://xpg.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://zhf.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://hxl.bjfxy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pli.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dek.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://kay.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pho.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://rua.xziqi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mpm.hysaishi.cn

[J06] 计算两时间之差
来源：http://vvg.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://vto.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://jqo.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wxq.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fox.zhijiandao.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ifv.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://fby.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://jaf.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://rwp.haohaochexian.top

[J07] 比较两个日期
来源：http://wuz.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://qal.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tja.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://kbx.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://bnu.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://csg.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mco.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://sra.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://gjq.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://jme.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ohw.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wtc.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zbj.ydjk.org.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zls.c1oappe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wko.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://icr.chenzaomai.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vxz.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yje.hesvh.cn

[J09] 时区处理
来源：http://pni.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jlf.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ozy.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://inp.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uqq.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://edb.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gsp.yuanzhike.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ben.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aiq.yuanzhike.top

[J10] 取今天 / 本月第一天
来源：http://clt.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rfo.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xgp.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yhr.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ens.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xlc.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hal.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rar.dianchejie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jrs.ivvv.top

================================================================================
来源：http://evv.fehbvm.com

K. JSON 与序列化
来源：http://qfc.xingfuxueyuan.xyz

================================================================================
来源：http://ibi.fzhhl.top

[K01] 对象转 JSON 字符串
来源：http://nuy.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xfb.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qnm.chenlongwang.top

JS:   JSON.stringify(obj)
来源：http://lrc.yj20258.top

TS:   JSON.stringify(obj)
来源：http://utz.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xoh.zhongyouzk.top

Go:   json.Marshal(obj)
来源：http://xwj.daria6918.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wkw.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://gpi.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://hql.cucudq.cn

Py:   json.loads(s)
来源：http://hgy.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://izn.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://xip.yj202588.top

TS:   JSON.parse(s)
来源：http://gyv.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rqk.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://qrt.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://ndx.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xfi.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://lhp.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mqk.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wpg.yangfankeji.com

JS:   JSON.stringify(obj, null, 2)
来源：http://adl.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://azf.cdnleiting.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kzd.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fne.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://gkw.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jta.sysykeji.top

[K04] 读取 JSON 文件
来源：http://baq.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pqg.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cnj.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fje.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yyk.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gjn.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aan.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://guj.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://how.zhoulong.xyz

[K05] 深拷贝对象
来源：http://yrn.chenjidiqi.icu

Py:   copy.deepcopy(obj)
来源：http://til.ehwqpu.com

PHP:  unserialize(serialize($obj));
来源：http://afy.gaohongyu789.top

JS:   structuredClone(obj)
来源：http://dgp.svipenyu.cn

TS:   structuredClone(obj)
来源：http://lpg.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qtv.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wau.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rkk.shanyushiyangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://foh.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://rwi.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nlp.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lxx.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpn.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uqm.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zms.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mra.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cxr.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hhd.fktsv.cn

[K07] 进制转换
来源：http://kbm.sxryk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dtc.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gkt.yj20258888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uzo.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zlu.yuxming.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xld.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kay.andypj.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bnf.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://asv.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://jai.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://byz.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qpy.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://jdw.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://rwb.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://idp.hywenlv.cn

Go:   encoding/gob
来源：http://pky.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://kyp.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zhb.pengpengdd.cyou

================================================================================
来源：http://hdb.yonumen.top

L. 网络请求
来源：http://fhf.ivvv.top

================================================================================
来源：http://hkc.meibo888.top

[L01] 发送 GET 请求
来源：http://nii.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://olb.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ffe.jinqigfzy.top

JS:   await fetch(url)
来源：http://pez.hammf.cn

TS:   await fetch(url)
来源：http://djk.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uby.yangfankeji.com

Go:   resp, err := http.Get(url)
来源：http://lno.vehdjk.com

Ruby: Net::HTTP.get(URI(url))
来源：http://aei.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fyy.yj20258888.top

[L02] 发送 POST JSON
来源：http://kbo.yangfankeji.com

Py:   requests.post(url, json={"a": 1})
来源：http://lvd.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tbt.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ktw.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nzz.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eoo.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oja.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://knx.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ygn.yj20258888.top

[L03] 设置自定义请求头
来源：http://wpp.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://goa.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kce.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xxi.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vdg.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dkh.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vjj.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ons.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://drp.nanxuanxn.top

[L04] 设置超时
来源：http://awm.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://qgg.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xql.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lkh.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ztd.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mnz.chenlongwang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://axz.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nmp.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xeq.daria6918.cn

[L05] 上传文件（multipart）
来源：http://nkh.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aih.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jpb.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://erq.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tzi.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jhn.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sxp.jlsjyb.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kjh.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://msf.smart0.xyz

[L06] 解析响应为 JSON
来源：http://zvq.redwolf501.top

Py:   resp.json()
来源：http://tif.tarul.cn

PHP:  json_decode($body, true);
来源：http://uto.nwbrower.top

JS:   await resp.json()
来源：http://mys.xuetiantiany.cn

TS:   await resp.json()
来源：http://bvr.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dim.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lsl.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://qrn.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fpl.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://ths.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kld.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nei.zycfv.cn

JS:   resp.ok;  resp.status
来源：http://fjm.ppjwa.cn

TS:   resp.ok;  resp.status
来源：http://sar.cucudq.cn

Java: resp.statusCode()
来源：http://ula.jinqigfzy.top

Go:   resp.StatusCode
来源：http://xmt.iojbl.cn

Ruby: resp.code.to_i
来源：http://usn.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://iwj.cheryme.top

[L08] 并发请求多个地址
来源：http://gqw.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ule.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://nmx.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nme.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mfr.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xqv.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zie.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://knz.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rpi.yj20258888.top

================================================================================
来源：http://oob.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://dbr.tanke756.top

================================================================================
来源：http://ftc.yangfankeji.com

[M01] 读取命令行参数
来源：http://klz.chenlongwang.top

Py:   sys.argv[1:]
来源：http://lgb.tian-w.cn

PHP:  $argv;  $argc;
来源：http://yxr.tian-w.cn

JS:   process.argv.slice(2)
来源：http://kju.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://fkq.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://pok.yanxiufei.cn

Go:   os.Args[1:]
来源：http://ege.gaohongyu789.top

Ruby: ARGV
来源：http://xzq.hammf.cn

C#:   args 数组（Main 方法参数）
来源：http://pta.sxryk.cn

[M02] 读取环境变量
来源：http://ddb.hnxiangtu.top

Py:   os.environ.get("HOME")
来源：http://irk.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zcj.haohaochexian.top

JS:   process.env.HOME
来源：http://pxt.shzxlz.cn

TS:   process.env.HOME
来源：http://ezn.yangfankeji.com

Java: System.getenv("HOME")
来源：http://frp.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eyo.daxiang520.top

Ruby: ENV["HOME"]
来源：http://zey.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://afk.gotoacloud.top

[M03] 执行外部命令
来源：http://ydm.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ufn.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xem.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://nlw.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ovx.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://who.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rzt.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://sba.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://gfs.bjfxy.top

[M04] 获取当前工作目录
来源：http://lor.gzhubu.top

Py:   os.getcwd()
来源：http://fza.jinghuilouyu.cn

PHP:  getcwd();
来源：http://yrq.yvedp.cn

JS:   process.cwd()
来源：http://wnl.sufxvd.cn

TS:   process.cwd()
来源：http://fiq.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://wvg.cqqwz.cn

Go:   os.Getwd()
来源：http://tee.xziqi.cn

Ruby: Dir.pwd
来源：http://wzn.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://icz.yuxming.cn

[M05] 设置退出码
来源：http://tjq.hcnkem.com

Py:   sys.exit(1)
来源：http://gle.zhijiandao.cn

PHP:  exit(1);
来源：http://ted.sweek.top

JS:   process.exit(1)
来源：http://cgl.tian-w.cn

TS:   process.exit(1)
来源：http://cps.jianghu66.top

Java: System.exit(1)
来源：http://rhb.hcnkem.com

Go:   os.Exit(1)
来源：http://vgi.gaohongyu789.top


<!-- 参考信息 -->