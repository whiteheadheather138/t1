代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://keq.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ytp.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vbh.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ebq.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kbc.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://clx.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qug.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ekh.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vuv.shangyingyoupin.top

TS:   /error/gim
来源：http://wxc.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oug.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://adt.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://grt.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ymy.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://vqy.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vkq.guowangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nyz.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qup.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://llu.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cdf.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://irb.redwolf501.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iys.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kgg.sjlbkw.cn

================================================================================
来源：http://nmw.gogol.net.cn

J. 日期与时间
来源：http://iri.aizwys.cn

================================================================================
来源：http://bfp.yj202588.top

[J01] 获取当前时间
来源：http://soj.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://olt.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qmh.epnwcf.com

JS:   new Date();  Date.now()
来源：http://gxq.hesvh.cn

TS:   new Date();  Date.now()
来源：http://nnq.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wyn.zhongyouzk.top

Go:   time.Now()
来源：http://itq.sjlbkw.cn

Ruby: Time.now
来源：http://pqu.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sjc.ppjwa.cn

[J02] 格式化输出
来源：http://xqf.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vnl.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uwu.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uae.havefunace.top

TS:   d.toISOString()
来源：http://saa.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zwy.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eev.vqdsnc.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://poy.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kqr.wangdashe.top

[J03] 字符串解析为日期
来源：http://qia.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ijb.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://llp.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://ppj.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://zbz.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hwf.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mhv.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://xor.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dcr.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://fqm.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iia.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jll.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fsi.zhiwuduotai.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ons.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eky.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pcr.jqgufenzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bvq.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xfe.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://cjr.epnwcf.com

Py:   now + timedelta(days=7)
来源：http://zyc.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ctw.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xun.yvedp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mpy.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://awp.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jzw.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://jha.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://fpr.vqdsnc.cn

[J06] 计算两时间之差
来源：http://xry.yongpay.top

Py:   (end - start).total_seconds()
来源：http://lqp.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://vzb.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zgs.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zcs.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://rih.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://fwx.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://azt.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://vvw.havefunace.top

[J07] 比较两个日期
来源：http://nou.vehdjk.com

Py:   d1 < d2;  d1 == d2
来源：http://nsd.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ssd.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wvd.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://yvl.jinqigufen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kji.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rqq.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://akx.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://ley.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://oyp.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nmi.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qvj.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lnx.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ozo.gaohongyu789.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uho.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uth.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xkm.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jsu.zdbjq.cn

[J09] 时区处理
来源：http://klw.jqgufenzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qia.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kjv.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ucw.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://laz.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kok.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://try.wangshuangyany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://odt.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zln.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://lkd.yanxiufei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sgf.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aaf.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ijt.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tbi.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mwm.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hcu.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vzo.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bog.yfazqb.com

================================================================================
来源：http://akp.guowangkeji.top

K. JSON 与序列化
来源：http://mmp.yueranfly.top

================================================================================
来源：http://soo.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://aqq.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rvh.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fjf.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://xry.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://zno.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dus.xingfuxueyuan.xyz

Go:   json.Marshal(obj)
来源：http://ere.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://xzm.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hgs.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://oxz.ydjk.org.cn

Py:   json.loads(s)
来源：http://mxh.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gfk.cashguo.top

JS:   JSON.parse(s)
来源：http://cfr.yuanzhike.top

TS:   JSON.parse(s)
来源：http://pua.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://edn.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://mkg.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://nvv.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://srk.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://lvw.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jfr.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mgy.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pmc.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hgq.ivvv.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pii.zhongyouzk.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uph.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://tti.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iir.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://gkq.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nkx.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xlx.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kak.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qkw.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fgy.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://crp.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://odr.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yfx.xuanzx.com

[K05] 深拷贝对象
来源：http://lgm.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://kmf.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://eej.nanxinkj.top

JS:   structuredClone(obj)
来源：http://wxk.jianghu66.top

TS:   structuredClone(obj)
来源：http://auq.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fym.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xql.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bhy.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jac.hfpthk.cn

[K06] 解析 URL 查询串
来源：http://zka.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ipz.hfpthk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sfc.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://smg.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fbt.sysykeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vxr.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xsh.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ahj.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://erg.pengpengdd.cyou

[K07] 进制转换
来源：http://pqi.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://emw.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dai.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ike.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rrl.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blg.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ykh.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jkk.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ydz.ybcxt.top

[K08] 二进制序列化（非 JSON）
来源：http://dil.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://tlh.svipenyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yfz.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://nmf.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://gtf.xingfuxueyuan.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gbv.dashuyun.cn

Go:   encoding/gob
来源：http://vrr.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://sxl.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qwj.ydjk.org.cn

================================================================================
来源：http://owc.chenjidiqi.icu

L. 网络请求
来源：http://dym.zhijiandao.cn

================================================================================
来源：http://iak.ivvv.top

[L01] 发送 GET 请求
来源：http://wsa.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qmb.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eyz.tianlin.xyz

JS:   await fetch(url)
来源：http://tba.vqdsnc.cn

TS:   await fetch(url)
来源：http://lku.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rre.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://mwq.ctjpmb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://jjh.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pfm.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://fmc.epnwcf.com

Py:   requests.post(url, json={"a": 1})
来源：http://kvr.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xyv.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qsz.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sum.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jpl.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dtf.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yjm.sysykeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ile.yfazqb.com

[L03] 设置自定义请求头
来源：http://cfv.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uuv.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gph.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dvx.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kfr.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oqd.xuanzx.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wjt.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dxq.andypj.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wop.quarkkingdee.top

[L04] 设置超时
来源：http://gax.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://npv.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lfm.fktsv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mkt.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ewt.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iqm.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xej.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ivb.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rdz.andypj.xyz

[L05] 上传文件（multipart）
来源：http://rhe.0kj1m.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mrm.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nbz.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://roa.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ohc.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://foi.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gzc.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://roq.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kse.zycfv.cn

[L06] 解析响应为 JSON
来源：http://hdq.yj202588.top

Py:   resp.json()
来源：http://buk.xylfe.cn

PHP:  json_decode($body, true);
来源：http://jtu.bbcook.cn

JS:   await resp.json()
来源：http://trb.gotoacloud.top

TS:   await resp.json()
来源：http://qvf.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ouj.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kzh.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://aov.havefunace.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mhq.aizwys.cn

[L07] 处理 HTTP 状态码
来源：http://pnt.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fff.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fgs.hysaishi.cn

JS:   resp.ok;  resp.status
来源：http://bun.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://qgm.pycfn.com

Java: resp.statusCode()
来源：http://ydf.sweek.top

Go:   resp.StatusCode
来源：http://loj.tanke756.top

Ruby: resp.code.to_i
来源：http://hup.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://tmo.ppjwa.cn

[L08] 并发请求多个地址
来源：http://mde.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uzn.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://keh.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jqt.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://phm.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://urc.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qmf.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nnz.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://scz.gogol.net.cn

================================================================================
来源：http://pec.ivvv.top

M. 命令行 / 进程 / 环境
来源：http://zqp.zhijiandao.cn

================================================================================
来源：http://zfp.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://nmp.cqqwz.cn

Py:   sys.argv[1:]
来源：http://kip.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://fiz.smart0.xyz

JS:   process.argv.slice(2)
来源：http://lie.jianghu66.top

TS:   process.argv.slice(2)
来源：http://gyb.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://dhg.fktsv.cn

Go:   os.Args[1:]
来源：http://obx.nwbrower.top

Ruby: ARGV
来源：http://rab.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://ycv.ctjpmb.com

[M02] 读取环境变量
来源：http://xhq.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://hqd.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ias.0kj1m.cn

JS:   process.env.HOME
来源：http://vxy.birdmap.top

TS:   process.env.HOME
来源：http://ocg.zhengqikj.top

Java: System.getenv("HOME")
来源：http://xls.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yxa.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://nio.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nph.iojbl.cn

[M03] 执行外部命令
来源：http://rbv.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ezb.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dsd.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ovw.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vzv.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qux.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ncm.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jfq.yj20258888.top

C#:   Process.Start("ls", "-l");
来源：http://ffc.havefunace.top

[M04] 获取当前工作目录
来源：http://bek.hongshengwenyu.top

Py:   os.getcwd()
来源：http://gbc.hnxiangtu.top

PHP:  getcwd();
来源：http://olq.c1oappe.top

JS:   process.cwd()
来源：http://yme.9152youxi.cn


<!-- 参考信息 -->