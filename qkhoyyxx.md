代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ria.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://ekd.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dyx.cucudq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jgq.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eve.c1oappe.top

TS:   /error/gim
来源：http://qvy.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qpj.pycfn.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hop.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://cas.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bkb.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://dky.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tdx.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tsw.andypj.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cgn.vehdjk.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gfa.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mrq.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://utt.ivvv.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fra.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ple.nwbrower.top

================================================================================
来源：http://xpd.52xcode.cn

J. 日期与时间
来源：http://kfn.nanxinkj.top

================================================================================
来源：http://eml.kuanghao11.cn

[J01] 获取当前时间
来源：http://hvh.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pxy.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rmo.zhijiandao.cn

JS:   new Date();  Date.now()
来源：http://msa.bjfxy.top

TS:   new Date();  Date.now()
来源：http://clo.xingfuxueyuan.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://hxi.zhengqikj.top

Go:   time.Now()
来源：http://iox.jinqigfzy.top

Ruby: Time.now
来源：http://ntf.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ywn.daxiang520.top

[J02] 格式化输出
来源：http://zgr.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wwu.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bij.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wnc.jinqigufen.top

TS:   d.toISOString()
来源：http://pkb.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zfn.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gqz.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rdy.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rti.epnwcf.com

[J03] 字符串解析为日期
来源：http://ebw.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yrc.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ajx.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://ubs.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://sqx.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ycb.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tvf.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://lrz.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://unk.daxiang520.top

[J04] 时间戳与日期互转
来源：http://hgq.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mmx.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wee.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://csg.zdqjudy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://maj.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aar.cheryme.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://biw.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qui.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://usb.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://bie.jinqigufen.top

Py:   now + timedelta(days=7)
来源：http://fyq.c1oappe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mva.ehwqpu.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kxh.hnxiangtu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jla.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://uvu.aizwys.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gyd.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://auo.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ejv.ydjk.org.cn

[J06] 计算两时间之差
来源：http://ldt.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://txc.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://rlz.cashguo.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gdc.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zua.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://mpa.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://ibg.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://nxu.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://kkv.jiagoushi.top

[J07] 比较两个日期
来源：http://gur.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://mpw.fehbvm.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://toq.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://qna.jiagoushi.top

TS:   d1.getTime() < d2.getTime()
来源：http://lhj.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xnr.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ror.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://msa.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://azy.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://wwq.bbcook.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nip.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zdt.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ywl.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xqc.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hrt.52xcode.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lpk.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jdt.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ndo.xinyue.icu

[J09] 时区处理
来源：http://fjg.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://upm.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wwa.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rkh.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hho.yuxming.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://snt.ehwqpu.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://puj.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kbk.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pfl.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://cwy.hnxiangtu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://czb.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xqp.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kkj.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jmz.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wly.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sad.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hsp.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nfr.nanxuanxn.top

================================================================================
来源：http://zns.sufxvd.cn

K. JSON 与序列化
来源：http://cvq.hysaishi.cn

================================================================================
来源：http://wbv.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://jlv.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pvo.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://geb.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://ppi.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://rew.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pmu.bbcook.cn

Go:   json.Marshal(obj)
来源：http://uaf.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://ggf.cdnleiting.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vpi.sxryk.cn

[K02] JSON 字符串转对象
来源：http://hmh.hysaishi.cn

Py:   json.loads(s)
来源：http://gxq.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bzc.vehdjk.com

JS:   JSON.parse(s)
来源：http://ass.fehbvm.com

TS:   JSON.parse(s)
来源：http://jtc.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ydo.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://txh.zycfv.cn

Ruby: JSON.parse(s)
来源：http://fjj.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://soh.andypj.xyz

[K03] JSON 美化输出（带缩进）
来源：http://jpy.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vyx.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qvy.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gdv.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ckl.shangyingyoupin.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xnf.cashguo.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vjn.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pvb.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aed.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://alk.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ucx.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mzi.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xqr.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dyf.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aps.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jin.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rzh.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fdt.jinghuilouyu.cn

[K05] 深拷贝对象
来源：http://yfv.sysykeji.top

Py:   copy.deepcopy(obj)
来源：http://qjv.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://qfv.redwolf501.top

JS:   structuredClone(obj)
来源：http://ayi.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://vax.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fcv.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nnj.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uah.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yau.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://qlm.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cge.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cji.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zlt.yongpay.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qpz.pengpengdd.cyou

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ozk.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://odc.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mki.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xry.zycfv.cn

[K07] 进制转换
来源：http://lii.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ebp.ivvv.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ako.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dvm.guowangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jmc.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rhv.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rnb.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iyp.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dqq.hammf.cn

[K08] 二进制序列化（非 JSON）
来源：http://ftr.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://hqv.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jqe.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://rix.jianghu66.top

TS:   v8.serialize(obj)        // Node
来源：http://dbn.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bve.c1oappe.top

Go:   encoding/gob
来源：http://xbz.vqdsnc.cn

Ruby: Marshal.dump(obj)
来源：http://rqo.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://muv.316326.xyz

================================================================================
来源：http://eyd.jlsjyb.cn

L. 网络请求
来源：http://etm.snrcjt.cn

================================================================================
来源：http://vdt.birdmap.top

[L01] 发送 GET 请求
来源：http://mde.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vnu.sufxvd.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qzs.jqgfzy.top

JS:   await fetch(url)
来源：http://oxs.chenzaomai.com

TS:   await fetch(url)
来源：http://rpd.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ksd.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://ypb.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wai.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ekz.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://uol.shanyushiyangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://hxf.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xit.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zyg.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wyp.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dti.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eue.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://luj.yj20258888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://slq.jinghuilouyu.cn

[L03] 设置自定义请求头
来源：http://dpz.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eyl.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nhd.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kez.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bez.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rho.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bkw.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kpj.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iou.ydzc1.top

[L04] 设置超时
来源：http://zfw.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://cmr.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://udp.yuanzhike.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://imb.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kbp.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mxp.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mbl.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://psz.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eah.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://nmt.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vre.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jqg.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kig.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xnf.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qer.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nfb.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uix.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://glm.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://pfq.meibo888.top

Py:   resp.json()
来源：http://pas.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://rhg.jiagoushi.top

JS:   await resp.json()
来源：http://moy.dashuyun.cn

TS:   await resp.json()
来源：http://djb.jianghu66.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tir.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://feq.guannengcc.top

Ruby: JSON.parse(resp.body)
来源：http://yos.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://msm.zhijiandao.cn

[L07] 处理 HTTP 状态码
来源：http://umi.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fqj.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mlm.yj202588.top

JS:   resp.ok;  resp.status
来源：http://dwv.havefunace.top

TS:   resp.ok;  resp.status
来源：http://ckw.xinyue.icu

Java: resp.statusCode()
来源：http://zqu.wangshuangyany.cn

Go:   resp.StatusCode
来源：http://ons.fktsv.cn

Ruby: resp.code.to_i
来源：http://kcr.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://iru.meibo888.top

[L08] 并发请求多个地址
来源：http://xlw.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jlv.guowangkeji.top

PHP:  curl_multi_init() 系列
来源：http://loa.hywenlv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eez.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gik.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wng.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sna.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gyf.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ycm.xylfe.cn

================================================================================
来源：http://lmb.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://fjc.fktsv.cn

================================================================================
来源：http://ypq.9152youxi.cn

[M01] 读取命令行参数
来源：http://pis.shuidangran.top

Py:   sys.argv[1:]
来源：http://epp.gzhubu.top

PHP:  $argv;  $argc;
来源：http://uqq.vehdjk.com

JS:   process.argv.slice(2)
来源：http://cnh.fehbvm.com

TS:   process.argv.slice(2)
来源：http://jcv.meibo888.top

Java: args 数组（main 方法参数）
来源：http://wzo.yj20258888.top

Go:   os.Args[1:]
来源：http://ywx.yj20258888.top

Ruby: ARGV
来源：http://hwl.hammf.cn

C#:   args 数组（Main 方法参数）
来源：http://cqa.tanke756.top

[M02] 读取环境变量
来源：http://omv.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://kuf.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gfl.wangdashe.top

JS:   process.env.HOME
来源：http://mdc.redwolf501.top

TS:   process.env.HOME
来源：http://rlh.cashguo.top

Java: System.getenv("HOME")
来源：http://ppv.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aah.aizwys.cn

Ruby: ENV["HOME"]
来源：http://rjx.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cqw.yuxming.cn

[M03] 执行外部命令
来源：http://zcr.andypj.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iln.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zqv.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uxw.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://mrz.xuanzx.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xji.vqdsnc.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://evq.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://kxd.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://knc.bjfxy.top

[M04] 获取当前工作目录
来源：http://dfz.zdqjudy.top

Py:   os.getcwd()
来源：http://hpi.hcnkem.com

PHP:  getcwd();
来源：http://uqc.hysaishi.cn

JS:   process.cwd()
来源：http://cdl.jinghuilouyu.cn

TS:   process.cwd()
来源：http://reh.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://kvo.shangyingyoupin.top

Go:   os.Getwd()
来源：http://iac.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://grk.iojbl.cn


<!-- 参考信息 -->