代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xgf.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mhr.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://imr.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://els.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sib.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://ana.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lck.chenlongwang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pon.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tiz.c1oappe.top

TS:   /error/gim
来源：http://plp.hfpthk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ogf.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mtg.jqgfzy.top

Ruby: s.scan(/error/i)
来源：http://sxf.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kdy.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://lry.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oms.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zmr.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://voi.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://liy.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wat.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yfo.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kgl.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ehk.ehwqpu.com

================================================================================
来源：http://rst.chenzaomai.com

J. 日期与时间
来源：http://ukt.chenjidiqi.icu

================================================================================
来源：http://ebi.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://mcn.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wkc.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://svx.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://gfy.cheryme.top

TS:   new Date();  Date.now()
来源：http://fqj.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wyg.sysykeji.top

Go:   time.Now()
来源：http://bjx.gotoacloud.top

Ruby: Time.now
来源：http://bdu.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ujl.vehdjk.com

[J02] 格式化输出
来源：http://bqb.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bwy.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wjy.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vux.yuxming.cn

TS:   d.toISOString()
来源：http://uok.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ugc.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xnt.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ztu.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wam.52xcode.cn

[J03] 字符串解析为日期
来源：http://gaf.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xzi.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://azj.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://rwl.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://hdm.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://uco.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vyk.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://utg.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ezk.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://qhr.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qsz.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hrq.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cyy.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lsr.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vty.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ibp.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fxw.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oau.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://pyk.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://zrz.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://goe.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://imr.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bsm.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://qxo.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xna.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://vov.aibaodan.cn

C#:   DateTime.Now.AddDays(7)
来源：http://akw.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://ref.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://sxi.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://evj.daria6918.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wnp.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dnl.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://vjq.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://rwz.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://onh.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://phu.52xcode.cn

[J07] 比较两个日期
来源：http://yum.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://cqw.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fui.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://mag.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://aej.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uey.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lea.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://cwd.hcnkem.com

C#:   d1 < d2;  d1 == d2
来源：http://spu.nwbrower.top

[J08] 提取年月日与星期
来源：http://jhv.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qsn.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uqo.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://edr.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vjh.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qnn.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vho.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wod.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rkr.xuetiantiany.cn

[J09] 时区处理
来源：http://nwc.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://exz.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ybe.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tvl.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ezt.jlsjyb.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://twn.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uwt.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gjs.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qnb.ydjk.org.cn

[J10] 取今天 / 本月第一天
来源：http://cdl.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qvz.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://umz.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qwp.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dpk.yfazqb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nhf.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tad.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bgh.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hat.hammf.cn

================================================================================
来源：http://rvs.sufxvd.cn

K. JSON 与序列化
来源：http://ovv.guowangkeji.top

================================================================================
来源：http://lkg.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://sij.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://obk.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bwh.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://lpz.birdmap.top

TS:   JSON.stringify(obj)
来源：http://dsr.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ajv.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://yuy.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://djs.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tur.fktsv.cn

[K02] JSON 字符串转对象
来源：http://yjw.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://zue.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nbr.smart0.xyz

JS:   JSON.parse(s)
来源：http://frd.ydzc1.top

TS:   JSON.parse(s)
来源：http://fhu.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://upx.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://nrp.guannengcc.top

Ruby: JSON.parse(s)
来源：http://wfw.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://udm.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://xhj.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hix.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jsn.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://eff.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cly.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fee.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zts.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dyh.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rmy.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://ixe.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://omn.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://knv.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://amq.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lrk.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lnx.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qsx.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wdn.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iul.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://frr.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://htr.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://faj.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://rpj.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://uhc.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://uij.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://syi.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rze.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://erw.yongpay.top

[K06] 解析 URL 查询串
来源：http://ksh.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jnt.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tmf.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hrq.c1oappe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mtw.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jvo.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ynl.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wdr.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cgq.zhaomingkeji.xyz

[K07] 进制转换
来源：http://tof.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nfe.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oaa.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ede.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pcx.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sxq.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zvq.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uum.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ucd.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://art.sjlbkw.cn

Py:   pickle.dumps(obj)
来源：http://arh.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pmk.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://uki.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://wiu.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ktm.quarkkingdee.top

Go:   encoding/gob
来源：http://kdf.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://zyo.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hon.smart0.xyz

================================================================================
来源：http://niw.jqgufenzy.top

L. 网络请求
来源：http://jqa.chenlongwang.top

================================================================================
来源：http://llb.yj20258888.top

[L01] 发送 GET 请求
来源：http://bvw.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nyr.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kfl.cdnleiting.top

JS:   await fetch(url)
来源：http://cxo.epnwcf.com

TS:   await fetch(url)
来源：http://emk.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xxb.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://qwe.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zxu.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tfd.sxryk.cn

[L02] 发送 POST JSON
来源：http://cgk.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://sbm.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bqv.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zlm.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://del.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cuv.ydjk.org.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yqy.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fll.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yut.aibaodan.cn

[L03] 设置自定义请求头
来源：http://xkd.0kj1m.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ght.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dye.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lyg.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ooo.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jyn.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ruw.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nih.feifeiyinyue.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bum.hysaishi.cn

[L04] 设置超时
来源：http://ddj.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://qfu.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ccg.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jrf.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://myn.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xtj.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://age.ydjk.org.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tdc.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://coj.fehbvm.com

[L05] 上传文件（multipart）
来源：http://fnr.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mpb.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dud.tianlin.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ptx.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ejx.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://grb.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rzp.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sga.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sbp.bbcook.cn

[L06] 解析响应为 JSON
来源：http://rtw.zhengqikj.top

Py:   resp.json()
来源：http://vwe.smart0.xyz

PHP:  json_decode($body, true);
来源：http://dop.hfpthk.cn

JS:   await resp.json()
来源：http://liy.bbcook.cn

TS:   await resp.json()
来源：http://isk.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://suc.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dlr.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://qsj.zycfv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kih.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://wuc.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eay.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://erg.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://hsk.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://fdv.redwolf501.top

Java: resp.statusCode()
来源：http://ana.fzhhl.top

Go:   resp.StatusCode
来源：http://dhr.nwbrower.top

Ruby: resp.code.to_i
来源：http://fbe.yongpay.top

C#:   (int)resp.StatusCode
来源：http://evx.sysykeji.top

[L08] 并发请求多个地址
来源：http://hzc.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zlf.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://ijv.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nbd.sjlbkw.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kch.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lkw.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kji.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bpc.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rkr.tianlin.xyz

================================================================================
来源：http://uwh.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://hee.shzxlz.cn

================================================================================
来源：http://kji.xinyue.icu

[M01] 读取命令行参数
来源：http://zxo.havefunace.top

Py:   sys.argv[1:]
来源：http://jms.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://obq.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://oby.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://pri.yueranfly.top

Java: args 数组（main 方法参数）
来源：http://xsf.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://udc.yueranfly.top

Ruby: ARGV
来源：http://xma.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://ubn.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://fta.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://wyy.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wes.vehdjk.com

JS:   process.env.HOME
来源：http://elv.yangfankeji.com

TS:   process.env.HOME
来源：http://nac.yj202588.top

Java: System.getenv("HOME")
来源：http://kbc.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://buf.52xcode.cn

Ruby: ENV["HOME"]
来源：http://pok.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qfj.feifeiyinyue.top

[M03] 执行外部命令
来源：http://ffn.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jcg.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hxa.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lbg.ydzc1.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zso.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rbb.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://xjy.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://hsu.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://ekm.hesvh.cn

[M04] 获取当前工作目录
来源：http://ihc.fanxiaobao.xyz

Py:   os.getcwd()
来源：http://czv.wangdashe.top

PHP:  getcwd();
来源：http://tcm.shangyingyoupin.top

JS:   process.cwd()
来源：http://itg.birdmap.top


<!-- 参考信息 -->