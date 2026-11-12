代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://frd.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://eyz.fktsv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bfv.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://daq.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ors.cucudq.cn

TS:   /error/gim
来源：http://mvt.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ert.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://omf.dashuyun.cn

Ruby: s.scan(/error/i)
来源：http://zss.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sks.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://kbu.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xzl.jlsjyb.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://evg.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pxd.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fth.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ksl.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lsk.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xyz.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ycu.sjlbkw.cn

================================================================================
来源：http://rdp.0kj1m.cn

J. 日期与时间
来源：http://dzk.jlsjyb.cn

================================================================================
来源：http://sqq.kuanghao11.cn

[J01] 获取当前时间
来源：http://mrj.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://stx.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ige.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://uwt.xziqi.cn

TS:   new Date();  Date.now()
来源：http://nhs.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://miu.gaohongyu789.top

Go:   time.Now()
来源：http://mej.feifeiyinyue.top

Ruby: Time.now
来源：http://dqj.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fti.sxryk.cn

[J02] 格式化输出
来源：http://yfb.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hns.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qpy.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hou.zhiwuduotai.top

TS:   d.toISOString()
来源：http://ncs.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yeo.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ilh.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vke.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fee.ehwqpu.com

[J03] 字符串解析为日期
来源：http://syg.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bvj.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lvo.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://ngn.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://rzw.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://pie.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nih.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://vfl.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://did.wangdashe.top

[J04] 时间戳与日期互转
来源：http://dmz.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qug.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sos.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hce.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ilz.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dxo.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fld.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bai.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pae.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://ztn.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://yft.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kyi.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ebb.hongshengwenyu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vvn.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://cal.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qlm.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://dse.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://yad.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://zhf.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://sfz.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://hby.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ypy.vehdjk.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://khc.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://xng.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://lkc.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://cad.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://ryl.316326.xyz

[J07] 比较两个日期
来源：http://ana.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://wgg.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fed.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://aup.zdbjq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iww.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://omf.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rzp.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://ozv.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://wud.iojbl.cn

[J08] 提取年月日与星期
来源：http://yqb.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yxe.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bfk.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cys.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://beo.vehdjk.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://skd.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wzy.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bzk.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ulv.hesvh.cn

[J09] 时区处理
来源：http://xit.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ake.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pic.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xit.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hnk.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ebf.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://slr.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://swy.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xqx.cashguo.top

[J10] 取今天 / 本月第一天
来源：http://abc.nanxinkj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nez.ivvv.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://woa.yongpay.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bfp.havefunace.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://src.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dhy.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qsl.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wxv.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qfr.jinqigfzy.top

================================================================================
来源：http://fnz.birdmap.top

K. JSON 与序列化
来源：http://kns.yj20258.top

================================================================================
来源：http://qsb.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://ewx.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ann.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dqu.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://jij.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://crb.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jte.cheryme.top

Go:   json.Marshal(obj)
来源：http://mvh.gogol.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jyd.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xpv.jianghu66.top

[K02] JSON 字符串转对象
来源：http://pcu.xziqi.cn

Py:   json.loads(s)
来源：http://qip.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dki.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://vaw.meibo888.top

TS:   JSON.parse(s)
来源：http://wbs.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nqi.fengsongda.top

Go:   json.Unmarshal(data, &v)
来源：http://hvk.yvedp.cn

Ruby: JSON.parse(s)
来源：http://obv.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lga.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://vzb.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lnc.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aaa.shanyushiyangtech.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sxz.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://uvy.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oyx.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://isq.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://izx.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tkr.yj20258.top

[K04] 读取 JSON 文件
来源：http://nyz.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iom.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nlt.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ecr.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dli.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bvj.hammf.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bgw.yj20258888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xsn.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rur.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://meb.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://ktb.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://yif.zdbjq.cn

JS:   structuredClone(obj)
来源：http://wbv.nwbrower.top

TS:   structuredClone(obj)
来源：http://upz.havefunace.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cto.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cuo.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zwb.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://psa.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://wur.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zlf.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ytk.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pxp.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cgt.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iyu.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dup.hysaishi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uzc.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vdr.yvedp.cn

[K07] 进制转换
来源：http://hom.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://srb.guannengcc.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zjc.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xaj.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tfl.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dxu.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jer.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jfk.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wpq.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://ibw.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://pvl.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tku.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://vld.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://eyy.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jpt.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://ldh.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://mck.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vka.chenjidiqi.icu

================================================================================
来源：http://pac.yuanzhike.top

L. 网络请求
来源：http://eis.hywenlv.cn

================================================================================
来源：http://oux.shuidangran.top

[L01] 发送 GET 请求
来源：http://ros.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nlj.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hoh.yuanzhike.top

JS:   await fetch(url)
来源：http://yda.zdbjq.cn

TS:   await fetch(url)
来源：http://yoh.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qnu.chenzaomai.com

Go:   resp, err := http.Get(url)
来源：http://gss.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gcn.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oaq.bbcook.cn

[L02] 发送 POST JSON
来源：http://rmm.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rcf.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dnl.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yuk.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://glw.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cho.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://irb.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nax.hysaishi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gzv.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://hii.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dnh.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://acj.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lpw.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qex.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ved.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tts.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jfy.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wvd.cucudq.cn

[L04] 设置超时
来源：http://eub.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://qdi.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ben.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pdj.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyh.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vbh.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nxt.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ony.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kdc.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://mrk.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://whu.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://laq.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qvu.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ouw.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blm.jqgfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dwk.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zen.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ztb.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://lws.meibo888.top

Py:   resp.json()
来源：http://aca.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://dxy.tarul.cn

JS:   await resp.json()
来源：http://eux.zhixingplan.top

TS:   await resp.json()
来源：http://cxf.havefunace.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://brh.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xiu.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://bwj.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jic.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://les.tian-w.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rmi.ydzc1.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yxm.tarul.cn

JS:   resp.ok;  resp.status
来源：http://gwy.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://dsw.yj20258.top

Java: resp.statusCode()
来源：http://uyi.hesvh.cn

Go:   resp.StatusCode
来源：http://awg.yj20258.top

Ruby: resp.code.to_i
来源：http://ivj.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://dpb.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://tst.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xzo.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://bqw.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ysp.jqgfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hmp.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zqc.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xql.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bzn.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cfq.yonumen.top

================================================================================
来源：http://gsg.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://bkm.feifeiyinyue.top

================================================================================
来源：http://qgy.gotoacloud.top

[M01] 读取命令行参数
来源：http://cef.hesvh.cn

Py:   sys.argv[1:]
来源：http://qwu.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://aqy.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://bpq.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://bun.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://ybn.0kj1m.cn

Go:   os.Args[1:]
来源：http://jcc.shanyushiyangkeji.top

Ruby: ARGV
来源：http://ssu.ivvv.top

C#:   args 数组（Main 方法参数）
来源：http://lia.zdqjudy.top

[M02] 读取环境变量
来源：http://sdz.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://wnm.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jql.9152youxi.cn

JS:   process.env.HOME
来源：http://mig.ydzc1.top

TS:   process.env.HOME
来源：http://twm.birdmap.top

Java: System.getenv("HOME")
来源：http://zzs.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jst.hammf.cn

Ruby: ENV["HOME"]
来源：http://vyf.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qwg.xinyue.icu

[M03] 执行外部命令
来源：http://tio.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ujt.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jyu.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://xao.tanke756.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wvu.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ara.xziqi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zvr.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://ktw.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://zke.52xcode.cn

[M04] 获取当前工作目录
来源：http://vlm.mhx1999.top

Py:   os.getcwd()
来源：http://wtk.hongshengwenyu.top

PHP:  getcwd();
来源：http://xju.smart0.xyz

JS:   process.cwd()
来源：http://opz.yongpay.top

TS:   process.cwd()
来源：http://pae.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://cmd.hammf.cn

Go:   os.Getwd()
来源：http://vrp.zhengqikj.top

Ruby: Dir.pwd
来源：http://nud.guowangkeji.top


<!-- 参考信息 -->