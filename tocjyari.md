代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ptz.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sim.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://doq.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mkp.birdmap.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rpr.shanyushiyangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zpf.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://knk.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bbh.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ekx.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://aoq.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ssn.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bli.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lki.sufxvd.cn

TS:   /error/gim
来源：http://kgw.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fgn.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rrh.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://clr.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sgv.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://otj.yueranfly.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://skk.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pyo.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zyg.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cmi.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qan.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kez.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bea.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://voy.hywenlv.cn

================================================================================
来源：http://trm.hnxiangtu.top

J. 日期与时间
来源：http://pjv.zycfv.cn

================================================================================
来源：http://vaf.hammf.cn

[J01] 获取当前时间
来源：http://xkm.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kaa.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kom.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://kiv.hammf.cn

TS:   new Date();  Date.now()
来源：http://yke.jiagoushi.top

Java: LocalDateTime.now();  Instant.now()
来源：http://njv.hammf.cn

Go:   time.Now()
来源：http://den.sjlbkw.cn

Ruby: Time.now
来源：http://dit.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cad.jinghuilouyu.cn

[J02] 格式化输出
来源：http://yvs.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tme.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ieg.316326.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sre.hammf.cn

TS:   d.toISOString()
来源：http://sml.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dul.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://irb.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://atn.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://prj.ctjpmb.com

[J03] 字符串解析为日期
来源：http://jdf.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://huy.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yvl.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://yax.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://zvj.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://xsb.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eqc.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://ulr.zhongyouzk.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hyn.wangdashe.top

[J04] 时间戳与日期互转
来源：http://nlb.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://joz.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gsa.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bxc.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rqh.bbcook.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zpt.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wci.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xgp.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gaa.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://vlh.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://xrh.fzhhl.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://put.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xfy.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ufg.xuetiantiany.cn

Java: LocalDate.now().plusDays(7)
来源：http://rfp.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jwn.pycfn.com

Ruby: Time.now + 7 * 86400
来源：http://opg.zhongyouzk.top

C#:   DateTime.Now.AddDays(7)
来源：http://ctu.andypj.xyz

[J06] 计算两时间之差
来源：http://ars.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://xuu.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://zat.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qio.dianchejie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xbv.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://asn.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://nnk.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://eqh.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://dom.dashuyun.cn

[J07] 比较两个日期
来源：http://iqv.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://zhy.ybcxt.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wmn.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hre.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fyb.sufxvd.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ito.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://esi.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://hce.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://mzs.xylfe.cn

[J08] 提取年月日与星期
来源：http://gvy.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rxl.cucudq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bpf.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sui.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wuk.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yxe.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fkf.snrcjt.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://opd.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fmb.sweek.top

[J09] 时区处理
来源：http://tgn.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lfv.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://akl.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yjl.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ktw.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xqa.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://meq.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ldu.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oqc.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://myy.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pms.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vha.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ehg.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nbq.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wcg.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wsr.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qhh.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://btn.zhiwuduotai.top

================================================================================
来源：http://kxi.ydzc1.top

K. JSON 与序列化
来源：http://ntn.epnwcf.com

================================================================================
来源：http://pwq.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://uwv.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hrb.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hmz.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://ghk.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://brs.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xfv.birdmap.top

Go:   json.Marshal(obj)
来源：http://cki.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hae.hammf.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ulq.yueranfly.top

[K02] JSON 字符串转对象
来源：http://gdg.jyoumei.cn

Py:   json.loads(s)
来源：http://jef.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://spy.chenzaomai.com

JS:   JSON.parse(s)
来源：http://ayx.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://dkv.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aeh.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://kpx.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://urg.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://plo.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://aji.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ypk.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xdc.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ktl.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://win.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tdu.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vrz.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://vpe.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gem.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://rvz.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vid.havefunace.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tpc.tarul.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kqq.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pfx.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://liq.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wom.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kxm.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qsz.cucudq.cn

[K05] 深拷贝对象
来源：http://bcu.zdbjq.cn

Py:   copy.deepcopy(obj)
来源：http://env.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://kci.shzxlz.cn

JS:   structuredClone(obj)
来源：http://yep.havefunace.top

TS:   structuredClone(obj)
来源：http://ecv.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://icq.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ybm.zycfv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bog.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eyo.svipenyu.cn

[K06] 解析 URL 查询串
来源：http://coz.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://smc.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ehw.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tjg.pengpengdd.cyou

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dru.pengpengdd.cyou

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://egw.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://tzq.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uqg.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lqy.bbcook.cn

[K07] 进制转换
来源：http://xlx.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lwv.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vfw.snrcjt.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://erx.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wti.fengsongda.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ekt.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lfk.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yze.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yzh.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://ncm.andypj.xyz

Py:   pickle.dumps(obj)
来源：http://aua.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ojs.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://ezn.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://tyb.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zuf.ivvv.top

Go:   encoding/gob
来源：http://vkj.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://mjs.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://quc.chenjidiqi.icu

================================================================================
来源：http://cto.yvedp.cn

L. 网络请求
来源：http://mvz.0kj1m.cn

================================================================================
来源：http://sks.guannengcc.top

[L01] 发送 GET 请求
来源：http://cya.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wuw.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fio.fehbvm.com

JS:   await fetch(url)
来源：http://zve.xziqi.cn

TS:   await fetch(url)
来源：http://kxx.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zoj.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://saz.pycfn.com

Ruby: Net::HTTP.get(URI(url))
来源：http://phz.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lsd.uphjek.com

[L02] 发送 POST JSON
来源：http://nkb.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://vpf.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ixf.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kkw.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://obw.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cst.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cce.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lvz.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ixb.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://ety.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oto.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fsd.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cxn.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qei.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://evx.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uqv.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ewv.bjfxy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cse.hnxiangtu.top

[L04] 设置超时
来源：http://xod.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://bib.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ysj.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://frc.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zqf.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://awo.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://huz.hongshengwenyu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zcr.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zfm.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://olo.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jei.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://egi.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://guy.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jvx.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bom.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://clq.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qld.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zdp.tian-w.cn

[L06] 解析响应为 JSON
来源：http://cpp.havefunace.top

Py:   resp.json()
来源：http://yot.zhengqikj.top

PHP:  json_decode($body, true);
来源：http://raj.dianchejie.cn

JS:   await resp.json()
来源：http://mgb.cashguo.top

TS:   await resp.json()
来源：http://sre.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lfv.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://awr.fengsongda.top

Ruby: JSON.parse(resp.body)
来源：http://dql.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uhn.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://ija.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kmz.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dek.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://hhp.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://abx.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://fcu.ivvv.top

Go:   resp.StatusCode
来源：http://ayn.pycfn.com

Ruby: resp.code.to_i
来源：http://szh.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://jor.sxryk.cn

[L08] 并发请求多个地址
来源：http://olq.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qri.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://yxz.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zpr.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bbx.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://err.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vzp.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cfy.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mer.shangyingyoupin.top

================================================================================
来源：http://vqv.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://tqv.gotoacloud.top

================================================================================
来源：http://pib.dashuyun.cn

[M01] 读取命令行参数
来源：http://xcn.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://uun.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://ucv.cheryme.top

JS:   process.argv.slice(2)
来源：http://qgn.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://gwn.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://ycb.316326.xyz

Go:   os.Args[1:]
来源：http://xaa.wangdashe.top

Ruby: ARGV
来源：http://goh.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://djf.tianlin.xyz

[M02] 读取环境变量
来源：http://dhb.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://dkh.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fmx.aibaodan.cn

JS:   process.env.HOME
来源：http://fqp.wangshuangyany.cn

TS:   process.env.HOME
来源：http://ytd.wangdashe.top

Java: System.getenv("HOME")
来源：http://khi.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bcs.epnwcf.com

Ruby: ENV["HOME"]
来源：http://ktr.jinghuilouyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://get.guowangkeji.top

[M03] 执行外部命令
来源：http://ymm.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://llv.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rll.andypj.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://fmo.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://zjk.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aym.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://lwm.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qqi.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://tbj.shzxlz.cn


<!-- 参考信息 -->