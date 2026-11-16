代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oca.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://cqj.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bkq.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fus.vqdsnc.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bxk.zhiwuduotai.top

TS:   /error/gim
来源：http://ene.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rig.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dya.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://kwu.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nbs.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://izy.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://brn.yuanzhike.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ozw.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fmu.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qaa.havefunace.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ait.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cke.gzhubu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pqa.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ygc.xinyue.icu

================================================================================
来源：http://uun.shzxlz.cn

J. 日期与时间
来源：http://ndd.shangyingyoupin.top

================================================================================
来源：http://mvj.jiagoushi.top

[J01] 获取当前时间
来源：http://usu.epnwcf.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://krp.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jnh.shuidangran.top

JS:   new Date();  Date.now()
来源：http://qyn.chenzaomai.com

TS:   new Date();  Date.now()
来源：http://vhi.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qfw.gaohongyu789.top

Go:   time.Now()
来源：http://xpx.shzxlz.cn

Ruby: Time.now
来源：http://iie.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ofd.shanyushiyangtech.top

[J02] 格式化输出
来源：http://owe.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://izy.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://whq.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cth.aibaodan.cn

TS:   d.toISOString()
来源：http://jtm.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jrg.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oak.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tbf.zdbjq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wby.smart0.xyz

[J03] 字符串解析为日期
来源：http://squ.zhaomingkeji.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gdi.zhoulong.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xay.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://pab.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://bxf.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://ovm.xziqi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bvz.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://gip.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nfr.tarul.cn

[J04] 时间戳与日期互转
来源：http://rah.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jhl.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ieo.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bac.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://usw.xuanzx.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dck.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://boa.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yey.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mgo.havefunace.top

[J05] 时间加减（加 7 天）
来源：http://knu.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://pwx.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bzo.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sng.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bfp.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://unc.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ran.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://fuv.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://era.snrcjt.cn

[J06] 计算两时间之差
来源：http://jvs.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://lpl.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://vyi.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tjs.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mpo.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bau.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://rfa.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://prn.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://kaw.hnqzz.top

[J07] 比较两个日期
来源：http://wmm.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://mzc.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pmr.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uai.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://sgc.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://enq.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jgp.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://qlv.tianlin.xyz

C#:   d1 < d2;  d1 == d2
来源：http://vcs.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://rte.jyoumei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hne.hcnkem.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ufi.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iub.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rtv.cashguo.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ztu.jinyuanbaomall.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ipf.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gcq.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mkl.cucudq.cn

[J09] 时区处理
来源：http://maz.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ozs.fanxiaobao.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hlo.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://clv.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://edx.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aty.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pni.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cum.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mrb.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://zpb.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rqf.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yru.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wdt.havefunace.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vqf.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rsg.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://seh.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kqj.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aol.yuxming.cn

================================================================================
来源：http://orn.chenjidiqi.icu

K. JSON 与序列化
来源：http://owf.chenlongwang.top

================================================================================
来源：http://ytp.xingfuxueyuan.xyz

[K01] 对象转 JSON 字符串
来源：http://pum.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rpv.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ayt.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://cry.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://myo.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pzi.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://jol.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://wcr.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cmn.zhixingplan.top

[K02] JSON 字符串转对象
来源：http://kjg.vehdjk.com

Py:   json.loads(s)
来源：http://xxy.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mes.tanke756.top

JS:   JSON.parse(s)
来源：http://gre.sufxvd.cn

TS:   JSON.parse(s)
来源：http://tyc.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hic.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://kqq.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://got.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://smt.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://hmx.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cum.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zox.yj202588.top

JS:   JSON.stringify(obj, null, 2)
来源：http://aqb.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://xau.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vhk.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aeg.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fxa.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lrk.yj202588.top

[K04] 读取 JSON 文件
来源：http://suh.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gjc.iojbl.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rpv.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hwd.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oeg.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bzx.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://daw.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hbv.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ybf.hesvh.cn

[K05] 深拷贝对象
来源：http://dey.ydjk.org.cn

Py:   copy.deepcopy(obj)
来源：http://qck.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://jws.cqqwz.cn

JS:   structuredClone(obj)
来源：http://pyw.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://gkh.hfpthk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vhj.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aij.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vnd.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kkv.svipenyu.cn

[K06] 解析 URL 查询串
来源：http://bnt.shanyushiyangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fht.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qcs.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://glr.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rxa.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ffe.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://imv.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sqc.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jur.fengsongda.top

[K07] 进制转换
来源：http://ebz.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yky.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hoq.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yia.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cei.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jaq.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oek.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://elr.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kvw.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://jsc.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://oxw.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://lxg.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://jek.yvedp.cn

TS:   v8.serialize(obj)        // Node
来源：http://rvi.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rnz.hfpthk.cn

Go:   encoding/gob
来源：http://zbw.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://qsk.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bym.sweek.top

================================================================================
来源：http://xia.ppjwa.cn

L. 网络请求
来源：http://ijs.xingfuxueyuan.xyz

================================================================================
来源：http://gmx.svipenyu.cn

[L01] 发送 GET 请求
来源：http://qxu.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cwc.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yzr.dashuyun.cn

JS:   await fetch(url)
来源：http://zmc.wangshuangyany.cn

TS:   await fetch(url)
来源：http://gst.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://siv.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://awo.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dxl.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qzl.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://mcq.vqdsnc.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qtf.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://glo.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ehv.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://drk.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wzh.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iow.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qqo.hysaishi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vgq.gogol.net.cn

[L03] 设置自定义请求头
来源：http://ttj.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wol.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rbq.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gcy.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hjt.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pfu.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nbk.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yep.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hhm.sweek.top

[L04] 设置超时
来源：http://dwv.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://etp.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://snb.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yqi.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cjq.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bkk.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mpq.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://azv.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://szw.yvedp.cn

[L05] 上传文件（multipart）
来源：http://vlz.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jdi.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ljw.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jbm.tarul.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pcz.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qdm.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zae.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://snd.chenzaomai.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://elb.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://isz.yvedp.cn

Py:   resp.json()
来源：http://hft.epnwcf.com

PHP:  json_decode($body, true);
来源：http://shl.shuidangran.top

JS:   await resp.json()
来源：http://eya.cashguo.top

TS:   await resp.json()
来源：http://hbz.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blz.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zvq.xylfe.cn

Ruby: JSON.parse(resp.body)
来源：http://kbg.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rbn.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://bcg.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eir.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://edb.yonumen.top

JS:   resp.ok;  resp.status
来源：http://idm.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://plv.havefunace.top

Java: resp.statusCode()
来源：http://aeh.ydjk.org.cn

Go:   resp.StatusCode
来源：http://cze.iojbl.cn

Ruby: resp.code.to_i
来源：http://lul.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://wpr.zycfv.cn

[L08] 并发请求多个地址
来源：http://pjk.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nig.jlsjyb.cn

PHP:  curl_multi_init() 系列
来源：http://rtu.aizwys.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ene.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://few.c1oappe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gea.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dzx.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yro.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cod.cdnleiting.top

================================================================================
来源：http://tex.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://xkb.zhongyouzk.top

================================================================================
来源：http://fvn.daria6918.cn

[M01] 读取命令行参数
来源：http://nff.aizwys.cn

Py:   sys.argv[1:]
来源：http://ywu.tarul.cn

PHP:  $argv;  $argc;
来源：http://azf.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://vmg.cheryme.top

TS:   process.argv.slice(2)
来源：http://inp.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://rmt.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://kvy.kuanghao11.cn

Ruby: ARGV
来源：http://krw.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://ibh.hywenlv.cn

[M02] 读取环境变量
来源：http://kkx.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://cvq.ctjpmb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bzm.cashguo.top

JS:   process.env.HOME
来源：http://dmk.hongshengwenyu.top

TS:   process.env.HOME
来源：http://ueo.guowangkeji.top

Java: System.getenv("HOME")
来源：http://clg.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zjb.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://mgq.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://med.birdmap.top

[M03] 执行外部命令
来源：http://ngt.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lsr.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sml.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zrz.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jpj.vehdjk.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gmt.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yna.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://amc.aibaodan.cn

C#:   Process.Start("ls", "-l");
来源：http://tql.bjfxy.top

[M04] 获取当前工作目录
来源：http://jje.yangfankeji.com

Py:   os.getcwd()
来源：http://jfu.smart0.xyz

PHP:  getcwd();
来源：http://lwn.hysaishi.cn

JS:   process.cwd()
来源：http://rxh.redwolf501.top

TS:   process.cwd()
来源：http://fwh.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://btv.gotoacloud.top

Go:   os.Getwd()
来源：http://yjs.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://ink.sweek.top


<!-- 参考信息 -->