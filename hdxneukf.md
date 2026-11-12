代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aye.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://qxm.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ijw.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eom.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yie.hammf.cn

TS:   /error/gim
来源：http://nfe.hnxiangtu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://erl.cheryme.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xjg.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://xux.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ctd.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://oet.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mxu.gotoacloud.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ceo.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xij.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yht.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://png.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zbx.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://off.dashuyun.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qxb.jianghu66.top

================================================================================
来源：http://zog.hnxiangtu.top

J. 日期与时间
来源：http://nmo.shzxlz.cn

================================================================================
来源：http://hus.zhijiandao.cn

[J01] 获取当前时间
来源：http://jjy.52xcode.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ipb.meibo888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tui.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://szi.hnxiangtu.top

TS:   new Date();  Date.now()
来源：http://bmk.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gbv.iojbl.cn

Go:   time.Now()
来源：http://cyz.kuanghao11.cn

Ruby: Time.now
来源：http://kkq.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ofd.zhiwuduotai.top

[J02] 格式化输出
来源：http://rqq.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uys.xinyue.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iyk.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nvo.hongshengwenyu.top

TS:   d.toISOString()
来源：http://rbm.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qlx.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lss.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lys.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uub.dianchejie.cn

[J03] 字符串解析为日期
来源：http://zaw.jlsjyb.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vez.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hps.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://ast.wangshuangyany.cn

TS:   new Date("2024-01-02")
来源：http://usc.yueranfly.top

Java: LocalDate.parse("2024-01-02")
来源：http://erj.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yme.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://ber.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sqf.tanke756.top

[J04] 时间戳与日期互转
来源：http://yph.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gnu.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kqz.yj20258.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xma.zdqjudy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gwd.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lkn.hammf.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hfp.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hjy.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jqv.havefunace.top

[J05] 时间加减（加 7 天）
来源：http://hjx.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://qkb.yuanzhike.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://atz.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kkz.hywenlv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zjk.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://fte.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lsv.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://fox.smart0.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://kba.cashguo.top

[J06] 计算两时间之差
来源：http://ter.daxiang520.top

Py:   (end - start).total_seconds()
来源：http://ggg.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://mcx.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gpp.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ymc.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://foz.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://afr.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://hpi.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://nfr.jinqigufen.top

[J07] 比较两个日期
来源：http://iol.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://snt.ydzc1.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bdf.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://nmc.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://ntb.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xog.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fbb.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://abe.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://ion.xinyue.icu

[J08] 提取年月日与星期
来源：http://pdu.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ufk.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ksi.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qaw.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vco.wangdashe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aze.chenlongwang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pdv.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zlx.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://atg.tarul.cn

[J09] 时区处理
来源：http://oen.shanyushiyangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blg.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eyf.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mbu.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ygx.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pkj.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pgj.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lss.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cgy.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://xjc.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://roo.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rwt.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aod.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://anr.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wjk.zhoulong.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kea.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mew.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ogx.sjlbkw.cn

================================================================================
来源：http://uam.tianlin.xyz

K. JSON 与序列化
来源：http://fyr.cqqwz.cn

================================================================================
来源：http://kue.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://uza.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fqr.cashguo.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fll.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://kqc.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://ere.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zjd.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://obw.redwolf501.top

Ruby: obj.to_json                                     // require "json"
来源：http://jtq.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yyn.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://prs.yangfankeji.com

Py:   json.loads(s)
来源：http://lmp.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hzk.fengsongda.top

JS:   JSON.parse(s)
来源：http://fuq.hcnkem.com

TS:   JSON.parse(s)
来源：http://oin.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kac.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://fqy.fktsv.cn

Ruby: JSON.parse(s)
来源：http://bca.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iid.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://bxd.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jmq.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ojg.pengpengdd.cyou

JS:   JSON.stringify(obj, null, 2)
来源：http://qix.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kbn.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kmc.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ptd.jinqigufen.top

Ruby: JSON.pretty_generate(obj)
来源：http://xoo.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tyb.aizwys.cn

[K04] 读取 JSON 文件
来源：http://kpb.jiagoushi.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uzq.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fua.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://obv.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hec.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tqz.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sos.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zpu.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cxg.daria6918.cn

[K05] 深拷贝对象
来源：http://rqk.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://osl.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://dkt.zhongyouzk.top

JS:   structuredClone(obj)
来源：http://tdj.haohaochexian.top

TS:   structuredClone(obj)
来源：http://cnd.gotoacloud.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xrt.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dsl.wangshuangyany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pgl.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://pnp.yj20258.top

[K06] 解析 URL 查询串
来源：http://mrw.hesvh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kni.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://epw.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://phj.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pkg.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://avc.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ker.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tsq.daria6918.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hsk.yanxiufei.cn

[K07] 进制转换
来源：http://cbe.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://axk.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kgm.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jit.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jec.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cnt.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fhe.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lme.ydzc1.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bbf.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://oji.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://dpj.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tmq.chenzaomai.com

JS:   v8.serialize(obj)        // Node
来源：http://jyt.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://grj.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yey.zhiwuduotai.top

Go:   encoding/gob
来源：http://meq.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://buf.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qrg.xziqi.cn

================================================================================
来源：http://nca.iojbl.cn

L. 网络请求
来源：http://myr.gaohongyu789.top

================================================================================
来源：http://mid.hnqzz.top

[L01] 发送 GET 请求
来源：http://gct.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://epg.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rnt.havefunace.top

JS:   await fetch(url)
来源：http://sjs.redwolf501.top

TS:   await fetch(url)
来源：http://ciq.epnwcf.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://enw.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://hdv.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cyt.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://grz.hcnkem.com

[L02] 发送 POST JSON
来源：http://bip.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://llp.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ums.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hhy.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://izu.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vdr.sxryk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://krm.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ixq.hysaishi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jqu.jinqigufen.top

[L03] 设置自定义请求头
来源：http://hyq.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yja.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wet.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://okl.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://exx.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mbp.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pwj.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qfd.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cmo.ybcxt.top

[L04] 设置超时
来源：http://uil.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://ibk.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bvo.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fai.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pws.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ufm.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lnc.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qkl.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ipq.yueranfly.top

[L05] 上传文件（multipart）
来源：http://kgz.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wmx.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sbd.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fsm.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://izs.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kgx.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://avt.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mkc.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hux.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://ygl.yongpay.top

Py:   resp.json()
来源：http://lti.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://lei.sufxvd.cn

JS:   await resp.json()
来源：http://avj.kuanghao11.cn

TS:   await resp.json()
来源：http://bte.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xlt.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qit.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://whd.hfpthk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kdo.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://bea.ppjwa.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ook.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tyr.dashuyun.cn

JS:   resp.ok;  resp.status
来源：http://nsv.dashuyun.cn

TS:   resp.ok;  resp.status
来源：http://vpo.hnxiangtu.top

Java: resp.statusCode()
来源：http://gps.yongpay.top

Go:   resp.StatusCode
来源：http://nhg.wangshuangyany.cn

Ruby: resp.code.to_i
来源：http://ysh.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://zno.yangfankeji.com

[L08] 并发请求多个地址
来源：http://jhh.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xnb.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://bxn.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kki.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zxj.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yov.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://alm.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aru.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://feb.aibaodan.cn

================================================================================
来源：http://bwf.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://ujb.52xcode.cn

================================================================================
来源：http://qbh.epnwcf.com

[M01] 读取命令行参数
来源：http://gic.tian-w.cn

Py:   sys.argv[1:]
来源：http://hsa.smart0.xyz

PHP:  $argv;  $argc;
来源：http://ddn.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://yjl.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://zfv.aizwys.cn

Java: args 数组（main 方法参数）
来源：http://gbf.fengsongda.top

Go:   os.Args[1:]
来源：http://wur.gogol.net.cn

Ruby: ARGV
来源：http://rer.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://xrp.chenzaomai.com

[M02] 读取环境变量
来源：http://zqi.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://ynl.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tvb.jinqigufen.top

JS:   process.env.HOME
来源：http://zww.fzhhl.top

TS:   process.env.HOME
来源：http://aos.ppjwa.cn

Java: System.getenv("HOME")
来源：http://pmr.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rby.xinyue.icu

Ruby: ENV["HOME"]
来源：http://slm.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ydn.dashuyun.cn

[M03] 执行外部命令
来源：http://dyj.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fdv.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nzy.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mvi.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://osv.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gmw.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ysc.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://knt.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://bnr.sysykeji.top

[M04] 获取当前工作目录
来源：http://hdc.hfpthk.cn

Py:   os.getcwd()
来源：http://sqx.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://uqz.haohaochexian.top

JS:   process.cwd()
来源：http://azw.tianlin.xyz

TS:   process.cwd()
来源：http://wne.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://rel.sufxvd.cn

Go:   os.Getwd()
来源：http://ggc.dashuyun.cn

Ruby: Dir.pwd
来源：http://izk.shangyingyoupin.top


<!-- 参考信息 -->