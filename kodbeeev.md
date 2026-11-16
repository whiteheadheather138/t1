代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hvh.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wqb.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://qer.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fmo.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://twg.yfazqb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bdf.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qgn.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ies.fzhhl.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://enr.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://swf.yj20258888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aga.chenzaomai.com

================================================================================
来源：http://nyd.wangshuangyany.cn

J. 日期与时间
来源：http://yxm.kuanghao11.cn

================================================================================
来源：http://tdi.shuidangran.top

[J01] 获取当前时间
来源：http://tpa.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fyf.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vqi.yueranfly.top

JS:   new Date();  Date.now()
来源：http://jjd.shangyingyoupin.top

TS:   new Date();  Date.now()
来源：http://xtq.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yqq.ehwqpu.com

Go:   time.Now()
来源：http://bcb.9152youxi.cn

Ruby: Time.now
来源：http://els.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cdp.yj20258888.top

[J02] 格式化输出
来源：http://cdt.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nso.ywan-chungtsiang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://afa.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hfj.jlsjyb.cn

TS:   d.toISOString()
来源：http://abb.nanxuanxn.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tkj.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ftw.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qaf.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jra.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://zse.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ogz.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xyx.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://lkf.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://ltz.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vwe.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fuw.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://dkd.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://arv.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://cdk.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zcq.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qcp.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qdm.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://aou.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lcf.haohaochexian.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zqd.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zdk.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oki.zhixingplan.top

[J05] 时间加减（加 7 天）
来源：http://xww.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://bfn.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rwf.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://trm.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ypy.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://roh.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cwt.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://fgg.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://cms.fengsongda.top

[J06] 计算两时间之差
来源：http://nte.zycfv.cn

Py:   (end - start).total_seconds()
来源：http://loa.yj20258888.top

PHP:  $end->diff($start)->days;
来源：http://uhn.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dte.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xpm.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://kqi.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://ikl.guowangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://srq.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://rzw.nwbrower.top

[J07] 比较两个日期
来源：http://cwo.hywenlv.cn

Py:   d1 < d2;  d1 == d2
来源：http://zdw.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aic.tian-w.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xhy.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fdm.xinyue.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mct.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wil.iojbl.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sic.zdbjq.cn

C#:   d1 < d2;  d1 == d2
来源：http://kdt.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://fjr.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vyy.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qgb.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mne.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vfo.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aus.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gmt.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://odt.sxryk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ori.fktsv.cn

[J09] 时区处理
来源：http://auu.shanyushiyangtech.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://idh.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qkq.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xba.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kuf.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nqw.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://obh.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://djf.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ezm.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://lkm.gaohongyu789.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dvs.wangshuangyany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xhy.yangfankeji.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://liz.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rmj.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://skq.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qjs.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tiu.gotoacloud.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zci.hysaishi.cn

================================================================================
来源：http://xql.yonumen.top

K. JSON 与序列化
来源：http://hnt.c1oappe.top

================================================================================
来源：http://ahf.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://aqg.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://irv.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vwh.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://vdm.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://uhq.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://puz.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://wxp.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://map.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gir.xuanzx.com

[K02] JSON 字符串转对象
来源：http://qbm.mhx1999.top

Py:   json.loads(s)
来源：http://bnv.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://chy.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://joj.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://awn.bbcook.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nir.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://odn.epnwcf.com

Ruby: JSON.parse(s)
来源：http://tlg.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fbb.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://jof.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qer.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://exr.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tgu.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tzu.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jlr.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://clf.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fol.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://szt.yongpay.top

[K04] 读取 JSON 文件
来源：http://xme.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jsu.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dzr.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gnr.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wtm.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bcl.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gak.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://kmz.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tos.sufxvd.cn

[K05] 深拷贝对象
来源：http://xmr.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://ztv.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://pbb.mhx1999.top

JS:   structuredClone(obj)
来源：http://fix.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://ces.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://stt.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eqo.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://adv.gaohongyu789.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tyo.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://iys.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jfb.52xcode.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://shl.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qmx.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ise.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dpj.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qjx.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jwl.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sgy.jyoumei.cn

[K07] 进制转换
来源：http://siy.sweek.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://plo.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cgi.hesvh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fcj.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://spg.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fme.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://riw.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vfv.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://akd.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://uel.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://vij.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://spd.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://rtn.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://por.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vaa.9152youxi.cn

Go:   encoding/gob
来源：http://awd.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://qdv.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rgg.cucudq.cn

================================================================================
来源：http://hrt.hnqzz.top

L. 网络请求
来源：http://nvt.zhiwuduotai.top

================================================================================
来源：http://pcv.hnqzz.top

[L01] 发送 GET 请求
来源：http://rmy.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ews.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bjl.aizwys.cn

JS:   await fetch(url)
来源：http://uza.tian-w.cn

TS:   await fetch(url)
来源：http://rce.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nsc.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://eca.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wey.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kes.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://ojv.zdbjq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sut.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://npk.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://atc.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pqh.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fzx.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://caw.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mkg.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mhs.gotoacloud.top

[L03] 设置自定义请求头
来源：http://ner.yanxiufei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eeo.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://snu.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ceg.birdmap.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bag.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gar.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jdd.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cnp.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jtf.yj20258.top

[L04] 设置超时
来源：http://qqd.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://vmx.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vta.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://war.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nat.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qqt.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://amg.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://emh.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vww.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://woi.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cpk.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jal.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ebi.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qjb.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lly.iojbl.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rzo.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://are.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://duu.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://lpx.0kj1m.cn

Py:   resp.json()
来源：http://gdn.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://lnu.cqqwz.cn

JS:   await resp.json()
来源：http://ihw.sxryk.cn

TS:   await resp.json()
来源：http://plv.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oca.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fbe.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://ktt.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rdv.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://dgp.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fqp.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dpe.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://efr.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://idf.hcnkem.com

Java: resp.statusCode()
来源：http://ouq.gotoacloud.top

Go:   resp.StatusCode
来源：http://phc.jianghu66.top

Ruby: resp.code.to_i
来源：http://fxu.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://wqj.sweek.top

[L08] 并发请求多个地址
来源：http://wrb.xziqi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ygw.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://vke.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jsw.tian-w.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uxr.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://flz.kuanghao11.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aby.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://umy.zhengqikj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qpl.daxiang520.top

================================================================================
来源：http://oeg.jinqigfzy.top

M. 命令行 / 进程 / 环境
来源：http://mtt.zhongyouzk.top

================================================================================
来源：http://ayz.jinqigfzy.top

[M01] 读取命令行参数
来源：http://yim.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://kic.xziqi.cn

PHP:  $argv;  $argc;
来源：http://qjd.sweek.top

JS:   process.argv.slice(2)
来源：http://scs.andypj.xyz

TS:   process.argv.slice(2)
来源：http://afk.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://cei.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://lck.hfpthk.cn

Ruby: ARGV
来源：http://ndp.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://nak.zhoulong.xyz

[M02] 读取环境变量
来源：http://oul.cheryme.top

Py:   os.environ.get("HOME")
来源：http://dwd.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nky.wangshuangyany.cn

JS:   process.env.HOME
来源：http://nip.jianghu66.top

TS:   process.env.HOME
来源：http://ehf.hcnkem.com

Java: System.getenv("HOME")
来源：http://byk.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fra.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://mea.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bby.xinyue.icu

[M03] 执行外部命令
来源：http://dfr.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zhw.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xxv.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qpe.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sog.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fvo.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jtt.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://nmg.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://zos.gotoacloud.top

[M04] 获取当前工作目录
来源：http://fpe.mhx1999.top

Py:   os.getcwd()
来源：http://ojj.chenzaomai.com

PHP:  getcwd();
来源：http://ubx.yueranfly.top

JS:   process.cwd()
来源：http://xbu.zhengqikj.top

TS:   process.cwd()
来源：http://jfo.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://nzc.tarul.cn

Go:   os.Getwd()
来源：http://qes.jlsjyb.cn

Ruby: Dir.pwd
来源：http://bpk.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://esz.ivvv.top

[M05] 设置退出码
来源：http://pgn.yanxiufei.cn

Py:   sys.exit(1)
来源：http://twq.ydjk.org.cn

PHP:  exit(1);
来源：http://jwk.jyoumei.cn

JS:   process.exit(1)
来源：http://pyg.yuxming.cn

TS:   process.exit(1)
来源：http://kpb.zhixingplan.top

Java: System.exit(1)
来源：http://elb.hnxiangtu.top

Go:   os.Exit(1)
来源：http://dnj.ywan-chungtsiang.top


<!-- 参考信息 -->