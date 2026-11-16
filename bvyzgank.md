代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ara.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://caf.cheryme.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kbl.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hti.svipenyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hyy.aizwys.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gsw.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rml.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ggt.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wpn.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://axi.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cjb.xylfe.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zvr.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dtw.jiagoushi.top

TS:   /error/gim
来源：http://qis.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sop.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rmt.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://cpx.cheryme.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://viv.iojbl.cn

[I08] 贪婪与非贪婪匹配
来源：http://zoi.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eir.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ntg.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wce.zhiwuduotai.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cmf.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lmm.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://png.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://srj.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vsn.bjfxy.top

================================================================================
来源：http://fxq.jqgfzy.top

J. 日期与时间
来源：http://dpj.jinghuilouyu.cn

================================================================================
来源：http://ars.ydjk.org.cn

[J01] 获取当前时间
来源：http://ijf.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pko.iojbl.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xua.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://zwz.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://ptp.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gxe.zhijiandao.cn

Go:   time.Now()
来源：http://eqf.cqqwz.cn

Ruby: Time.now
来源：http://esl.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tiv.fanxiaobao.xyz

[J02] 格式化输出
来源：http://mmu.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yae.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://seo.tanke756.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nfy.hnxiangtu.top

TS:   d.toISOString()
来源：http://wgl.ydjk.org.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fhl.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oua.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hmq.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zyn.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://ocq.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fhz.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://soo.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://tym.cheryme.top

TS:   new Date("2024-01-02")
来源：http://afr.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yze.xingfuxueyuan.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nkh.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://wtq.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ckj.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://njp.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tig.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ouw.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qjn.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://frb.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uee.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bbk.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bnc.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://geh.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://stv.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://icu.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dcc.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://khl.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cfm.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://dpm.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zbq.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://nxd.nwbrower.top

C#:   DateTime.Now.AddDays(7)
来源：http://rkm.yueranfly.top

[J06] 计算两时间之差
来源：http://bxf.cucudq.cn

Py:   (end - start).total_seconds()
来源：http://joz.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://csp.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sos.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mcp.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zjw.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://tvk.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://plf.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://ueh.andypj.xyz

[J07] 比较两个日期
来源：http://vgt.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://iad.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dsc.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://lpz.yonumen.top

TS:   d1.getTime() < d2.getTime()
来源：http://ldg.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wqb.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://esf.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hds.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://qlx.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://adb.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zox.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vjz.sweek.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rov.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dct.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://grr.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://efv.bjfxy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kjr.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jjr.zdbjq.cn

[J09] 时区处理
来源：http://sef.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uel.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hqh.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rqd.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qlk.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hpm.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bkl.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cmm.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vlv.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://ncp.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lez.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fdn.sufxvd.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rvz.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dum.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ago.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ukh.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zee.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://duf.yonumen.top

================================================================================
来源：http://vfd.zycfv.cn

K. JSON 与序列化
来源：http://eod.chenlongwang.top

================================================================================
来源：http://uki.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://hjq.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jic.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hjp.cheryme.top

JS:   JSON.stringify(obj)
来源：http://ome.yuxming.cn

TS:   JSON.stringify(obj)
来源：http://osl.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lwp.sweek.top

Go:   json.Marshal(obj)
来源：http://apx.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://aqm.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ggg.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://hvy.ybcxt.top

Py:   json.loads(s)
来源：http://qqj.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qph.9152youxi.cn

JS:   JSON.parse(s)
来源：http://gjd.wangdashe.top

TS:   JSON.parse(s)
来源：http://fpx.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gwt.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://odg.xziqi.cn

Ruby: JSON.parse(s)
来源：http://ndc.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fld.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://hss.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hao.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ugh.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://erd.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cvg.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cay.ybcxt.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://crc.jyoumei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gza.xziqi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ewp.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://rjy.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gbg.chenzaomai.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://shv.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ihk.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zkm.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qgk.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://snz.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ilj.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://moy.hfpthk.cn

[K05] 深拷贝对象
来源：http://slv.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://lep.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://ybn.fengsongda.top

JS:   structuredClone(obj)
来源：http://itd.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://szw.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://iba.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://evx.52xcode.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hqx.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lnv.sxryk.cn

[K06] 解析 URL 查询串
来源：http://tyt.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jyp.redwolf501.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cfw.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bbi.shuidangran.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gcb.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jfw.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zea.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gvd.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://glr.pycfn.com

[K07] 进制转换
来源：http://fey.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nfo.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nby.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lzu.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rkc.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wxe.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://urc.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cce.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eah.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://ylh.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://kut.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hvk.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://ych.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://bql.nwbrower.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://erj.jlsjyb.cn

Go:   encoding/gob
来源：http://laz.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://xcc.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qcs.nwbrower.top

================================================================================
来源：http://jkz.nanxinkj.top

L. 网络请求
来源：http://dvh.zhixingplan.top

================================================================================
来源：http://sfp.daxiang520.top

[L01] 发送 GET 请求
来源：http://rgn.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://siu.daria6918.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dxg.hcnkem.com

JS:   await fetch(url)
来源：http://xza.jqgfzy.top

TS:   await fetch(url)
来源：http://hcj.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sxc.ydjk.org.cn

Go:   resp, err := http.Get(url)
来源：http://yda.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pfv.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wie.tanke756.top

[L02] 发送 POST JSON
来源：http://iwa.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pnw.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kqq.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wqr.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://igd.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fqq.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uim.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://txu.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://znx.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://aah.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bsf.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rpg.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lhs.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vvc.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lkw.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hks.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://doy.xuetiantiany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ish.hysaishi.cn

[L04] 设置超时
来源：http://lya.shanyushiyangtech.top

Py:   requests.get(url, timeout=5)
来源：http://mcr.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://roc.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zwl.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ptm.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ybe.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ngd.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iom.nanxuanxn.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rkq.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://syn.zhoulong.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://emj.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mzb.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uzz.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gsq.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://siz.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rag.nanxinkj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bwg.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://roe.gogol.net.cn

[L06] 解析响应为 JSON
来源：http://tsw.hesvh.cn

Py:   resp.json()
来源：http://nfe.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://sbg.chenlongwang.top

JS:   await resp.json()
来源：http://mba.hywenlv.cn

TS:   await resp.json()
来源：http://cob.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zpr.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wqu.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://znq.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pch.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://qbd.jianghu66.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gkg.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vrp.cashguo.top

JS:   resp.ok;  resp.status
来源：http://yxt.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://tgh.gaohongyu789.top

Java: resp.statusCode()
来源：http://ljp.guowangkeji.top

Go:   resp.StatusCode
来源：http://irf.zhengqikj.top

Ruby: resp.code.to_i
来源：http://idd.cashguo.top

C#:   (int)resp.StatusCode
来源：http://lqk.shzxlz.cn

[L08] 并发请求多个地址
来源：http://ted.tianlin.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zfs.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://tev.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gur.jqgfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fmo.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zmo.xuanzx.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cgd.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yvn.guannengcc.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wip.zdqjudy.top

================================================================================
来源：http://hyv.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://ppr.hesvh.cn

================================================================================
来源：http://usr.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://dkg.hysaishi.cn

Py:   sys.argv[1:]
来源：http://atv.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://dyu.52xcode.cn

JS:   process.argv.slice(2)
来源：http://jxr.meibo888.top

TS:   process.argv.slice(2)
来源：http://biz.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://hph.gogol.net.cn

Go:   os.Args[1:]
来源：http://oja.shuidangran.top

Ruby: ARGV
来源：http://sps.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://kmm.ybcxt.top

[M02] 读取环境变量
来源：http://ndm.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://rlf.ydjk.org.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cgo.cheryme.top

JS:   process.env.HOME
来源：http://mmr.ppjwa.cn

TS:   process.env.HOME
来源：http://mis.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://roz.fehbvm.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ufh.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://wxi.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ksz.shuidangran.top

[M03] 执行外部命令
来源：http://mqy.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xfl.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mcb.zdqjudy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kge.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://mzz.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wos.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://upx.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://bfj.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://wqd.vqdsnc.cn


<!-- 参考信息 -->