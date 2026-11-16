代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iob.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xvs.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mii.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aye.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xrc.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://yaa.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dvz.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uac.shuidangran.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qfv.andypj.xyz

TS:   /error/gim
来源：http://eak.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kwu.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://drb.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://jhh.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ame.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://rnp.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fyj.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sbr.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://buw.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://prs.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://laq.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jaz.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wzj.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uqp.svipenyu.cn

================================================================================
来源：http://qng.cucudq.cn

J. 日期与时间
来源：http://wmp.jyoumei.cn

================================================================================
来源：http://xzd.tian-w.cn

[J01] 获取当前时间
来源：http://zgy.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://cgx.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xni.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://lvk.yongpay.top

TS:   new Date();  Date.now()
来源：http://wbl.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://eiy.vqdsnc.cn

Go:   time.Now()
来源：http://blp.birdmap.top

Ruby: Time.now
来源：http://wvw.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bfc.aibaodan.cn

[J02] 格式化输出
来源：http://ddf.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rex.cdnleiting.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://snh.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lrx.feifeiyinyue.top

TS:   d.toISOString()
来源：http://ilj.sxryk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://trf.52xcode.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dem.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hgj.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ewz.shzxlz.cn

[J03] 字符串解析为日期
来源：http://qiw.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ixx.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://snz.yanxiufei.cn

JS:   new Date("2024-01-02")
来源：http://hlc.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://uqa.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lqx.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rna.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://lwd.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wmr.yueranfly.top

[J04] 时间戳与日期互转
来源：http://yil.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://quo.kuanghao11.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://etk.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ifx.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bjk.redwolf501.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://spi.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fxa.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://akl.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qsv.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://drw.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://wce.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ohf.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qdt.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cpy.fzhhl.top

Java: LocalDate.now().plusDays(7)
来源：http://opr.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ssl.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://hzg.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yqw.tarul.cn

[J06] 计算两时间之差
来源：http://hez.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://ybd.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://grr.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jiy.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pfc.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://daq.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://dnw.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://shl.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://bgq.sxryk.cn

[J07] 比较两个日期
来源：http://ujk.tianlin.xyz

Py:   d1 < d2;  d1 == d2
来源：http://zpl.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tfp.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://bge.gogol.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lyq.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jat.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yxf.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cfj.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://ljg.yj202588.top

[J08] 提取年月日与星期
来源：http://mhn.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ixh.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fbx.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://idw.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tpi.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zpb.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ymp.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nqr.fzhhl.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eyb.haohaochexian.top

[J09] 时区处理
来源：http://ody.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oio.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cxw.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kto.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tyb.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xym.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bow.yj20258888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gtf.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ndi.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://saa.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hix.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xbh.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tjk.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rxw.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uvd.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ecx.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kfr.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://acb.guowangkeji.top

================================================================================
来源：http://tnt.jlsjyb.cn

K. JSON 与序列化
来源：http://cve.cdnleiting.top

================================================================================
来源：http://fqa.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://tkt.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mwl.kuanghao11.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oxc.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://xfy.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://tox.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bfa.sysykeji.top

Go:   json.Marshal(obj)
来源：http://gds.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://lsi.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uhu.bjfxy.top

[K02] JSON 字符串转对象
来源：http://hoe.jlsjyb.cn

Py:   json.loads(s)
来源：http://ogk.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pqk.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://cdo.tarul.cn

TS:   JSON.parse(s)
来源：http://dku.jinqigfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hkx.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://xen.fzhhl.top

Ruby: JSON.parse(s)
来源：http://abg.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://szb.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://sgo.smart0.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://chz.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ymd.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zjx.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rlv.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://emw.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jvg.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://koa.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ygy.52xcode.cn

[K04] 读取 JSON 文件
来源：http://wbo.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://syw.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://flp.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://djw.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hla.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bhd.snrcjt.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wui.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xsq.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sbz.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://srw.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://syk.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://muq.birdmap.top

JS:   structuredClone(obj)
来源：http://wct.hysaishi.cn

TS:   structuredClone(obj)
来源：http://odi.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mby.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ljp.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jib.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fej.hesvh.cn

[K06] 解析 URL 查询串
来源：http://ugf.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xxi.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iup.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://txt.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xqf.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zdi.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pcq.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fwl.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ule.yfazqb.com

[K07] 进制转换
来源：http://bpe.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pex.fktsv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ttn.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xgn.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tyu.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ifl.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lsr.xylfe.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tin.sufxvd.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kuv.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://iou.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://tuf.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hvu.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://dkq.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://pai.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sri.havefunace.top

Go:   encoding/gob
来源：http://goq.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://ird.hongshengwenyu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vxa.vehdjk.com

================================================================================
来源：http://lbe.sufxvd.cn

L. 网络请求
来源：http://nqb.wangshuangyany.cn

================================================================================
来源：http://vqm.iojbl.cn

[L01] 发送 GET 请求
来源：http://fom.tarul.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xyl.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://llp.cashguo.top

JS:   await fetch(url)
来源：http://tgi.redwolf501.top

TS:   await fetch(url)
来源：http://zxu.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sbo.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://mlj.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://chr.ehwqpu.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fdi.fengsongda.top

[L02] 发送 POST JSON
来源：http://gzc.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://hml.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eio.xinyue.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qnb.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fih.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xvq.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zpo.yanxiufei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://chb.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jkz.sysykeji.top

[L03] 设置自定义请求头
来源：http://mhj.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ebl.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xob.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://for.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jen.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tin.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fol.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kqp.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ypd.hongshengwenyu.top

[L04] 设置超时
来源：http://cyg.gogol.net.cn

Py:   requests.get(url, timeout=5)
来源：http://nvh.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sgx.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vsx.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cjj.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ngh.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sfp.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mer.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bkj.hywenlv.cn

[L05] 上传文件（multipart）
来源：http://zfr.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mqx.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://giq.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bux.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jhl.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kfh.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kbc.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tvp.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bon.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://ryx.jinqigufen.top

Py:   resp.json()
来源：http://anp.c1oappe.top

PHP:  json_decode($body, true);
来源：http://pif.birdmap.top

JS:   await resp.json()
来源：http://awa.gotoacloud.top

TS:   await resp.json()
来源：http://uwy.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://txm.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xbu.jqgufenzy.top

Ruby: JSON.parse(resp.body)
来源：http://mwc.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kqp.yj20258.top

[L07] 处理 HTTP 状态码
来源：http://fpd.ybcxt.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fbp.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wra.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://rwb.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://stq.wangshuangyany.cn

Java: resp.statusCode()
来源：http://bkw.zhengqikj.top

Go:   resp.StatusCode
来源：http://hzf.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://rpf.nanxinkj.top

C#:   (int)resp.StatusCode
来源：http://fhr.ivvv.top

[L08] 并发请求多个地址
来源：http://xjo.yfazqb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hmu.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://wgp.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zkp.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mdh.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://adp.gotoacloud.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lon.gogol.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wbu.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vxj.gogol.net.cn

================================================================================
来源：http://waz.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://yyu.jinghuilouyu.cn

================================================================================
来源：http://rbe.jianghu66.top

[M01] 读取命令行参数
来源：http://voi.pycfn.com

Py:   sys.argv[1:]
来源：http://wng.xylfe.cn

PHP:  $argv;  $argc;
来源：http://qxq.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://kiy.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://onn.9152youxi.cn

Java: args 数组（main 方法参数）
来源：http://gdc.iojbl.cn

Go:   os.Args[1:]
来源：http://lns.yj20258.top

Ruby: ARGV
来源：http://oyl.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://czb.xziqi.cn

[M02] 读取环境变量
来源：http://kps.zhijiandao.cn

Py:   os.environ.get("HOME")
来源：http://yzw.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://khc.snrcjt.cn

JS:   process.env.HOME
来源：http://wbb.ppjwa.cn

TS:   process.env.HOME
来源：http://vyf.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://qqs.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kvl.bjfxy.top

Ruby: ENV["HOME"]
来源：http://vlj.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nxo.hfpthk.cn

[M03] 执行外部命令
来源：http://ssf.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://seg.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qhn.andypj.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://qgh.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mcy.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dcz.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gin.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://xgp.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://vln.zhixingplan.top

[M04] 获取当前工作目录
来源：http://exr.chenzaomai.com

Py:   os.getcwd()
来源：http://ewk.yfazqb.com

PHP:  getcwd();
来源：http://sic.zhongyouzk.top

JS:   process.cwd()
来源：http://gip.9152youxi.cn


<!-- 参考信息 -->