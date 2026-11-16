代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://zni.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zis.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tls.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uuq.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rxs.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tpt.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hkl.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nek.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jrd.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mpy.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nvo.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://agi.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iqx.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://kuh.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://clu.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nzz.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ujj.jinyuanbaomall.cn

TS:   /error/gim
来源：http://kgy.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zuc.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iww.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://nyc.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dfb.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://wta.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jbo.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gdy.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zot.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pzb.aibaodan.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hbk.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ndy.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zrc.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pnm.birdmap.top

================================================================================
来源：http://hte.xuetiantiany.cn

J. 日期与时间
来源：http://nva.gaohongyu789.top

================================================================================
来源：http://xjr.jqgfzy.top

[J01] 获取当前时间
来源：http://jbv.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sgu.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gzs.fktsv.cn

JS:   new Date();  Date.now()
来源：http://ymu.yuanzhike.top

TS:   new Date();  Date.now()
来源：http://wcx.ywan-chungtsiang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vrh.ivvv.top

Go:   time.Now()
来源：http://hst.snrcjt.cn

Ruby: Time.now
来源：http://ihe.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sse.jlsjyb.cn

[J02] 格式化输出
来源：http://maw.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sul.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vtj.ivvv.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://znv.fzhhl.top

TS:   d.toISOString()
来源：http://bbj.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://klp.mhx1999.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://smq.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://doq.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cqf.c1oappe.top

[J03] 字符串解析为日期
来源：http://sln.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pbe.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uiu.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://qml.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://wul.nwbrower.top

Java: LocalDate.parse("2024-01-02")
来源：http://ixl.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vve.ppjwa.cn

Ruby: Date.parse("2024-01-02")
来源：http://ofr.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://udc.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://ral.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://azr.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ylm.zhoulong.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vuk.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://khe.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wti.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dgb.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fhb.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dej.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://ais.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://fwk.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cym.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gxt.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nbq.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://nhb.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rwk.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://svb.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://zzl.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://vkk.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://ewm.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://bvy.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zgh.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dms.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://wyp.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://kzf.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://iyz.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://pvi.dashuyun.cn

[J07] 比较两个日期
来源：http://nyb.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://uft.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kap.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://gcy.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gkl.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://alr.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jbr.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://nqy.hcnkem.com

C#:   d1 < d2;  d1 == d2
来源：http://xni.fehbvm.com

[J08] 提取年月日与星期
来源：http://zvn.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tdg.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vhb.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mdv.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dwt.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xid.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bxi.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oqy.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rfk.cucudq.cn

[J09] 时区处理
来源：http://odm.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pkt.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://urv.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vqc.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dua.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xzh.uphjek.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ckj.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rfe.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qjv.bbcook.cn

[J10] 取今天 / 本月第一天
来源：http://cvv.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fjm.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tye.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://msi.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://akg.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uvr.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://liy.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ytl.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jia.hfpthk.cn

================================================================================
来源：http://stg.gotoacloud.top

K. JSON 与序列化
来源：http://ffc.xuanzx.com

================================================================================
来源：http://cqr.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://qpn.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jmc.uphjek.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://srb.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://rxp.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://dza.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lwg.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://ouo.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://cgs.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lww.bbcook.cn

[K02] JSON 字符串转对象
来源：http://bid.jianghu66.top

Py:   json.loads(s)
来源：http://nsx.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vsx.52xcode.cn

JS:   JSON.parse(s)
来源：http://cbn.cqqwz.cn

TS:   JSON.parse(s)
来源：http://myq.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://obh.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://vvz.daxiang520.top

Ruby: JSON.parse(s)
来源：http://rzs.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vnm.dashuyun.cn

[K03] JSON 美化输出（带缩进）
来源：http://eiw.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gpm.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bpr.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eww.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xye.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gvm.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://brq.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://ujn.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://amx.cucudq.cn

[K04] 读取 JSON 文件
来源：http://szk.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xhk.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cad.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://umx.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://brq.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ozr.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fyr.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rlg.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://muo.chenlongwang.top

[K05] 深拷贝对象
来源：http://gqu.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://tee.cdnleiting.top

PHP:  unserialize(serialize($obj));
来源：http://ybe.vehdjk.com

JS:   structuredClone(obj)
来源：http://mry.cheryme.top

TS:   structuredClone(obj)
来源：http://vti.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fki.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hcb.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ser.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qoq.hcnkem.com

[K06] 解析 URL 查询串
来源：http://wae.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wvq.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kza.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wzq.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nuv.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nzy.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cxx.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nba.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jzw.daxiang520.top

[K07] 进制转换
来源：http://poj.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qin.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kui.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sfq.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cyf.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yzm.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pub.yonumen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dix.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xrd.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://fto.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://gan.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cka.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://dvo.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://phw.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://grb.hysaishi.cn

Go:   encoding/gob
来源：http://zvh.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://wtm.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tsj.jqgfzy.top

================================================================================
来源：http://ogb.cdnleiting.top

L. 网络请求
来源：http://jdr.wangshuangyany.cn

================================================================================
来源：http://vkh.mhx1999.top

[L01] 发送 GET 请求
来源：http://exv.wangshuangyany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kvs.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wjz.zdbjq.cn

JS:   await fetch(url)
来源：http://syh.guowangkeji.top

TS:   await fetch(url)
来源：http://ddr.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ptg.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://ail.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qjf.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://obn.hammf.cn

[L02] 发送 POST JSON
来源：http://gln.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://iqc.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dqe.guowangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ynk.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uwu.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ipd.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fej.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ppk.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ecn.fengsongda.top

[L03] 设置自定义请求头
来源：http://ebt.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ksn.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jnq.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zzo.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mkr.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://frj.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cpr.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fom.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://elb.shangyingyoupin.top

[L04] 设置超时
来源：http://aur.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://xmi.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://igh.jqgfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mca.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zuv.cqqwz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oum.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yog.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uvh.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mcg.yueranfly.top

[L05] 上传文件（multipart）
来源：http://tgx.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iwi.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://alr.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iqq.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xtg.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nfp.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mxg.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://clq.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wni.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://jbj.bbcook.cn

Py:   resp.json()
来源：http://brz.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://pge.meibo888.top

JS:   await resp.json()
来源：http://fux.zhengqikj.top

TS:   await resp.json()
来源：http://ydi.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iwf.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sht.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://tgg.sjlbkw.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fhn.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://vmw.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ywz.ydzc1.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rhc.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://wfq.ctjpmb.com

TS:   resp.ok;  resp.status
来源：http://atg.zdbjq.cn

Java: resp.statusCode()
来源：http://tmi.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://uzj.sweek.top

Ruby: resp.code.to_i
来源：http://qyi.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://hbl.yj20258888.top

[L08] 并发请求多个地址
来源：http://gco.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fkh.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://boh.dashuyun.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hwd.quarkkingdee.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dts.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zqw.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nxz.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ilm.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ajj.0kj1m.cn

================================================================================
来源：http://ibt.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://zqg.yj20258.top

================================================================================
来源：http://wrx.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://nle.ppjwa.cn

Py:   sys.argv[1:]
来源：http://qrw.meibo888.top

PHP:  $argv;  $argc;
来源：http://lal.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://wwu.yj20258888.top

TS:   process.argv.slice(2)
来源：http://jky.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://wzc.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://rnm.jlsjyb.cn

Ruby: ARGV
来源：http://tfz.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://qxt.mhx1999.top

[M02] 读取环境变量
来源：http://eaz.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://vgf.yueranfly.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vjz.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://ymr.hesvh.cn

TS:   process.env.HOME
来源：http://hov.tianlin.xyz

Java: System.getenv("HOME")
来源：http://lqp.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yyf.hcnkem.com

Ruby: ENV["HOME"]
来源：http://fda.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bre.0kj1m.cn

[M03] 执行外部命令
来源：http://ygh.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jci.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cbx.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kjy.ehwqpu.com

TS:   child_process.execSync("ls -l").toString()
来源：http://gyr.ctjpmb.com


<!-- 参考信息 -->