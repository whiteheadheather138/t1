代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://efk.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lvg.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nlp.fktsv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ypp.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://osi.hesvh.cn

[I07] 忽略大小写与多行模式
来源：http://vzo.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://htj.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iqo.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ldi.daria6918.cn

TS:   /error/gim
来源：http://zjy.tarul.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wpy.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://svz.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://fyv.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fqs.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://heb.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vgf.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://exn.bbcook.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zgs.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fur.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yzz.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bda.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://syh.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hwj.0kj1m.cn

================================================================================
来源：http://orl.ehwqpu.com

J. 日期与时间
来源：http://blz.uphjek.com

================================================================================
来源：http://rxy.xinyue.icu

[J01] 获取当前时间
来源：http://wkr.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://kgq.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fez.smart0.xyz

JS:   new Date();  Date.now()
来源：http://jba.bbcook.cn

TS:   new Date();  Date.now()
来源：http://udl.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rig.hywenlv.cn

Go:   time.Now()
来源：http://hgj.hcnkem.com

Ruby: Time.now
来源：http://opw.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yji.cqqwz.cn

[J02] 格式化输出
来源：http://cwr.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tec.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ybu.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mvj.cdnleiting.top

TS:   d.toISOString()
来源：http://dqw.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xli.mhx1999.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vlv.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pln.ywan-chungtsiang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xdu.aibaodan.cn

[J03] 字符串解析为日期
来源：http://dew.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vvp.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vnf.yvedp.cn

JS:   new Date("2024-01-02")
来源：http://xsv.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://gwr.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://cqw.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gyn.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://asu.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jod.xziqi.cn

[J04] 时间戳与日期互转
来源：http://ypz.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jsp.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ptm.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yix.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://raj.hongshengwenyu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dpa.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fsl.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://atz.vqdsnc.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dyf.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://uhe.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://fhh.yj20258.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jch.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kxc.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ezd.quarkkingdee.top

Java: LocalDate.now().plusDays(7)
来源：http://otf.gotoacloud.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://alk.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://nxv.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://xqz.tianlin.xyz

[J06] 计算两时间之差
来源：http://wrt.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://qyl.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://fwe.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lgl.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://plq.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://ejd.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://fup.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://kfp.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://hby.xziqi.cn

[J07] 比较两个日期
来源：http://yhu.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ewo.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eox.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bvx.hywenlv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sac.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xlq.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lgs.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://zbq.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://tfa.gogol.net.cn

[J08] 提取年月日与星期
来源：http://jcs.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mra.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xtf.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cow.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aos.pengpengdd.cyou

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cws.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nbs.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://llp.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tog.tarul.cn

[J09] 时区处理
来源：http://ueu.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jqp.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ann.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://szk.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ume.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://luu.hcnkem.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yeq.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xfa.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aia.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://qzq.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://qjm.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kdb.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://poh.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://clt.cdnleiting.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fsw.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zwj.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bgy.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ldz.jqgufenzy.top

================================================================================
来源：http://xpg.0kj1m.cn

K. JSON 与序列化
来源：http://jmk.uphjek.com

================================================================================
来源：http://xei.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://ekh.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dsr.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ywv.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://xlq.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://vlj.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rni.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://ijp.chenjidiqi.icu

Ruby: obj.to_json                                     // require "json"
来源：http://bla.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qhc.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://jwd.yfazqb.com

Py:   json.loads(s)
来源：http://lpp.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kbs.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://dff.nwbrower.top

TS:   JSON.parse(s)
来源：http://qpm.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zdy.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://xhf.hywenlv.cn

Ruby: JSON.parse(s)
来源：http://swc.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zqd.shuidangran.top

[K03] JSON 美化输出（带缩进）
来源：http://pjq.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hkd.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zto.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fpp.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jfa.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jbs.birdmap.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zbf.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://sll.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://idq.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://ykt.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ulk.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uoo.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gql.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vid.uphjek.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eil.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fgq.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gud.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qaw.hammf.cn

[K05] 深拷贝对象
来源：http://bhw.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://ogr.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://zuu.sufxvd.cn

JS:   structuredClone(obj)
来源：http://obp.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://ypg.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://irm.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ypn.ybcxt.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vpu.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lwu.gzhubu.top

[K06] 解析 URL 查询串
来源：http://zez.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mrz.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xfo.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tir.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxt.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ynw.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://unw.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tky.havefunace.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vww.iojbl.cn

[K07] 进制转换
来源：http://vvq.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aei.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yqb.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zkw.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ejr.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xzz.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iut.tarul.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wbl.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://djz.cdnleiting.top

[K08] 二进制序列化（非 JSON）
来源：http://sot.sweek.top

Py:   pickle.dumps(obj)
来源：http://vci.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://jgv.yanxiufei.cn

JS:   v8.serialize(obj)        // Node
来源：http://kni.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://was.xinyue.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://utj.jianghu66.top

Go:   encoding/gob
来源：http://ixd.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://tys.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rjh.zhixingplan.top

================================================================================
来源：http://bdb.jlsjyb.cn

L. 网络请求
来源：http://epl.bbcook.cn

================================================================================
来源：http://htf.wangshuangyany.cn

[L01] 发送 GET 请求
来源：http://zeu.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pkl.pengpengdd.cyou

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dys.vqdsnc.cn

JS:   await fetch(url)
来源：http://cdx.jqgufenzy.top

TS:   await fetch(url)
来源：http://iae.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nww.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://gpj.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://wgj.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aup.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://avc.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://adu.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iup.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://trv.andypj.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xma.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vpt.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ihk.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wmf.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fll.yangfankeji.com

[L03] 设置自定义请求头
来源：http://yfs.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kmy.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mdc.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fqo.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ykp.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://akl.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mix.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dao.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zmr.epnwcf.com

[L04] 设置超时
来源：http://dra.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://cnc.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sgk.epnwcf.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uvp.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qua.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gye.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qgx.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://liu.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hef.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://vtc.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nqj.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tqt.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pvh.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rjf.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kua.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tpp.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oie.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vqn.wangdashe.top

[L06] 解析响应为 JSON
来源：http://hvz.nanxuanxn.top

Py:   resp.json()
来源：http://oeg.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://jpj.vqdsnc.cn

JS:   await resp.json()
来源：http://ubn.quarkkingdee.top

TS:   await resp.json()
来源：http://icj.guowangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bxy.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nkn.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://bdu.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tco.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://epg.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hch.sweek.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kqs.sufxvd.cn

JS:   resp.ok;  resp.status
来源：http://pic.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://eun.0kj1m.cn

Java: resp.statusCode()
来源：http://xow.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://mbh.ydzc1.top

Ruby: resp.code.to_i
来源：http://jde.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://wgt.cqqwz.cn

[L08] 并发请求多个地址
来源：http://sgh.sysykeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zrr.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://ksj.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zyr.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dyd.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dae.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aus.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fcp.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bnl.iojbl.cn

================================================================================
来源：http://iet.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://mdj.guannengcc.top

================================================================================
来源：http://vki.hesvh.cn

[M01] 读取命令行参数
来源：http://fax.redwolf501.top

Py:   sys.argv[1:]
来源：http://snx.52xcode.cn

PHP:  $argv;  $argc;
来源：http://zpg.redwolf501.top

JS:   process.argv.slice(2)
来源：http://trv.zhixingplan.top

TS:   process.argv.slice(2)
来源：http://trp.ivvv.top

Java: args 数组（main 方法参数）
来源：http://tzt.vqdsnc.cn

Go:   os.Args[1:]
来源：http://osj.ybcxt.top

Ruby: ARGV
来源：http://lll.yongpay.top

C#:   args 数组（Main 方法参数）
来源：http://ikl.hnxiangtu.top

[M02] 读取环境变量
来源：http://cgm.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://uxw.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fsd.wangdashe.top

JS:   process.env.HOME
来源：http://tuo.0kj1m.cn

TS:   process.env.HOME
来源：http://alw.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://xkr.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bbu.daria6918.cn

Ruby: ENV["HOME"]
来源：http://ssi.ivvv.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hfx.xziqi.cn

[M03] 执行外部命令
来源：http://ftw.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jpf.gzhubu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hkz.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qot.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://osg.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ilf.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wkl.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://uum.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://lbz.nanxinkj.top

[M04] 获取当前工作目录
来源：http://nch.xinyue.icu

Py:   os.getcwd()
来源：http://mef.zhoulong.xyz

PHP:  getcwd();
来源：http://vvs.tianlin.xyz

JS:   process.cwd()
来源：http://khl.ivvv.top


<!-- 参考信息 -->