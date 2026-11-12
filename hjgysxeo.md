代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://plw.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dyk.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zch.kuanghao11.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pmw.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tus.bbcook.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bgy.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://spk.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eod.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://orn.uphjek.com

[I07] 忽略大小写与多行模式
来源：http://pvf.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fyz.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sbo.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://acy.yonumen.top

TS:   /error/gim
来源：http://gtt.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fpv.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jcv.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://yew.chenlongwang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uth.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://eok.xylfe.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kfi.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wpb.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nja.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iyd.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hdb.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ual.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bog.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nxe.hywenlv.cn

================================================================================
来源：http://cxy.ppjwa.cn

J. 日期与时间
来源：http://vlk.zhaomingkeji.xyz

================================================================================
来源：http://fpq.cashguo.top

[J01] 获取当前时间
来源：http://jsg.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lij.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bwc.yj20258888.top

JS:   new Date();  Date.now()
来源：http://ezw.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://drz.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://upq.quarkkingdee.top

Go:   time.Now()
来源：http://mgy.gaohongyu789.top

Ruby: Time.now
来源：http://uwl.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://enj.nanxuanxn.top

[J02] 格式化输出
来源：http://joc.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vqb.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vxp.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ley.xinyue.icu

TS:   d.toISOString()
来源：http://sha.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eks.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eoq.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://npz.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ngq.xylfe.cn

[J03] 字符串解析为日期
来源：http://opa.zhaomingkeji.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zdw.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qan.hammf.cn

JS:   new Date("2024-01-02")
来源：http://xaw.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://dsr.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://cxw.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ceo.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://mkm.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sjy.vehdjk.com

[J04] 时间戳与日期互转
来源：http://uww.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ktn.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qav.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qsv.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://otp.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kor.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bbf.sysykeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rxf.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lob.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://ipn.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://xwy.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rwq.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jpz.jinqigfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mky.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://ltd.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eft.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://bve.wangshuangyany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qvo.fzhhl.top

[J06] 计算两时间之差
来源：http://src.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://gft.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://ayi.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sam.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jxn.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eem.tianlin.xyz

Go:   end.Sub(start).Hours()
来源：http://qpg.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://ogv.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://kgn.yueranfly.top

[J07] 比较两个日期
来源：http://ssy.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://nvm.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hns.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://sru.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://lfx.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rfe.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xuk.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sse.xingfuxueyuan.xyz

C#:   d1 < d2;  d1 == d2
来源：http://lie.chenzaomai.com

[J08] 提取年月日与星期
来源：http://sxx.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ozz.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://smj.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sut.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wum.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wxu.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://srh.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tch.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kne.jinghuilouyu.cn

[J09] 时区处理
来源：http://cqo.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tvx.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xfz.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jby.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://chd.guannengcc.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ppy.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xzn.andypj.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://jzz.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xov.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://pqm.daxiang520.top

Py:   date.today();  date.today().replace(day=1)
来源：http://icr.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kob.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ten.fzhhl.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fnp.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cmf.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blj.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ont.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pki.jinghuilouyu.cn

================================================================================
来源：http://yhv.gogol.net.cn

K. JSON 与序列化
来源：http://ukq.ctjpmb.com

================================================================================
来源：http://ylw.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://yqd.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jhb.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fkk.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://hba.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://gyq.tianlin.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mkg.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://rgi.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://eoc.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pjg.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://hpb.zycfv.cn

Py:   json.loads(s)
来源：http://jpx.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ufx.zycfv.cn

JS:   JSON.parse(s)
来源：http://xzb.zdqjudy.top

TS:   JSON.parse(s)
来源：http://dqz.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://glp.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://vgc.yfazqb.com

Ruby: JSON.parse(s)
来源：http://evt.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oab.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://qxa.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nhp.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jse.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pjh.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xuf.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pyw.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fus.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://oyv.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://diq.hammf.cn

[K04] 读取 JSON 文件
来源：http://nyc.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wbx.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zlu.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qyr.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ktd.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wkr.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zbt.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xqb.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jbc.wangdashe.top

[K05] 深拷贝对象
来源：http://ftc.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://clm.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://sxd.yonumen.top

JS:   structuredClone(obj)
来源：http://art.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://bhz.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rlf.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ugt.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://otk.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mas.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://iks.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rda.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ifk.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rlc.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cya.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ywb.zhixingplan.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://twe.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://szc.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://krr.kuanghao11.cn

[K07] 进制转换
来源：http://nca.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dlr.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xur.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nmx.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bvw.xylfe.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iws.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rgr.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qzy.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ocq.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://sux.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://dee.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yaj.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://uus.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://ksv.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mph.dashuyun.cn

Go:   encoding/gob
来源：http://qve.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://cty.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wro.ydjk.org.cn

================================================================================
来源：http://fqx.fehbvm.com

L. 网络请求
来源：http://vzx.yj20258888.top

================================================================================
来源：http://cer.yvedp.cn

[L01] 发送 GET 请求
来源：http://atq.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pqp.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wqa.jlsjyb.cn

JS:   await fetch(url)
来源：http://hip.jinqigufen.top

TS:   await fetch(url)
来源：http://iia.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bcp.hywenlv.cn

Go:   resp, err := http.Get(url)
来源：http://djt.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jvu.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hks.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://yli.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://fja.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zaq.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jio.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://erk.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oca.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xsx.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://opn.svipenyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://awu.ydzc1.top

[L03] 设置自定义请求头
来源：http://txm.fehbvm.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ico.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mnm.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lpg.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lap.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iuu.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xlb.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rpv.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zxo.nanxuanxn.top

[L04] 设置超时
来源：http://omg.xuetiantiany.cn

Py:   requests.get(url, timeout=5)
来源：http://jbd.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uwe.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hfk.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mhu.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cjx.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ndg.dashuyun.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xge.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xvc.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://uoc.yvedp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://raf.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vhm.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pfg.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nvi.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zrl.zhixingplan.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://trz.bbcook.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ifn.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blk.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://dlq.gaohongyu789.top

Py:   resp.json()
来源：http://tix.ydzc1.top

PHP:  json_decode($body, true);
来源：http://cgo.yonumen.top

JS:   await resp.json()
来源：http://qlv.shuidangran.top

TS:   await resp.json()
来源：http://ixc.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kin.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kzl.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://cfn.jinqigfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rkn.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://vdc.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vhj.hongshengwenyu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mae.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://dhn.316326.xyz

TS:   resp.ok;  resp.status
来源：http://qih.gaohongyu789.top

Java: resp.statusCode()
来源：http://qvz.9152youxi.cn

Go:   resp.StatusCode
来源：http://slj.aibaodan.cn

Ruby: resp.code.to_i
来源：http://pez.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://iez.shzxlz.cn

[L08] 并发请求多个地址
来源：http://jth.ybcxt.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sbo.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://mmn.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mao.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xid.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vvv.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gaa.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://slc.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jfn.chenlongwang.top

================================================================================
来源：http://baj.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://vgi.redwolf501.top

================================================================================
来源：http://dfu.andypj.xyz

[M01] 读取命令行参数
来源：http://usj.vehdjk.com

Py:   sys.argv[1:]
来源：http://wyx.daxiang520.top

PHP:  $argv;  $argc;
来源：http://sue.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://zzi.cqqwz.cn

TS:   process.argv.slice(2)
来源：http://kyk.yonumen.top

Java: args 数组（main 方法参数）
来源：http://hjw.bjfxy.top

Go:   os.Args[1:]
来源：http://pci.wangshuangyany.cn

Ruby: ARGV
来源：http://ovm.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://lqh.jqgufenzy.top

[M02] 读取环境变量
来源：http://euz.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://syg.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wva.yonumen.top

JS:   process.env.HOME
来源：http://hta.sweek.top

TS:   process.env.HOME
来源：http://kto.hysaishi.cn

Java: System.getenv("HOME")
来源：http://dwp.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cow.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://mve.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ieo.bjfxy.top

[M03] 执行外部命令
来源：http://ovr.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ggz.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jsk.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xmn.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mdt.yongpay.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qea.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cxp.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://vaq.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://djd.cheryme.top


<!-- 参考信息 -->