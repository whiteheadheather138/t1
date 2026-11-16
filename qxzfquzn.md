代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://zno.fehbvm.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://npz.smart0.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://hiy.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cby.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ckx.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://umo.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cgu.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qef.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rbq.jqgfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ffr.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zrc.fehbvm.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://acz.fzhhl.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zav.jinyuanbaomall.cn

[I07] 忽略大小写与多行模式
来源：http://fzx.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bxn.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ycq.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://djj.birdmap.top

TS:   /error/gim
来源：http://moa.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://axt.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vgr.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://aia.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uka.gogol.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://ktm.gaohongyu789.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ybk.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hqc.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ris.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zec.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ehy.ctjpmb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bsh.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ije.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tui.guowangkeji.top

================================================================================
来源：http://vum.hongshengwenyu.top

J. 日期与时间
来源：http://fiq.jinqigufen.top

================================================================================
来源：http://seu.andypj.xyz

[J01] 获取当前时间
来源：http://ric.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://voc.hcnkem.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gve.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://zdc.zycfv.cn

TS:   new Date();  Date.now()
来源：http://izx.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://jgb.xuetiantiany.cn

Go:   time.Now()
来源：http://rwg.yj202588.top

Ruby: Time.now
来源：http://jch.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cfm.jianghu66.top

[J02] 格式化输出
来源：http://eow.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ana.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uwi.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://orj.xuanzx.com

TS:   d.toISOString()
来源：http://qeg.haohaochexian.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mkh.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://raz.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://khh.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ric.tianlin.xyz

[J03] 字符串解析为日期
来源：http://qmn.andypj.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hgv.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://isc.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://xrg.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://jwl.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iie.zdbjq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://toq.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://dcy.zhengqikj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://irz.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://baf.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pbg.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dpz.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hhx.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://abv.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aiz.sufxvd.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kdc.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uxh.pengpengdd.cyou

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tpq.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://mkl.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://tlz.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xor.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dgl.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cyk.ydjk.org.cn

Java: LocalDate.now().plusDays(7)
来源：http://eyb.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ifu.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://yzk.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://hsc.sweek.top

[J06] 计算两时间之差
来源：http://hfp.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://rmv.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://eou.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://stj.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://czr.yuxming.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rrb.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://llg.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://zhf.shanyushiyangtech.top

C#:   (end - start).TotalSeconds
来源：http://qvm.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://wpq.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://ela.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sdk.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fiu.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://huc.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kvc.cdnleiting.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hwa.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://hed.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://dax.zhaomingkeji.xyz

[J08] 提取年月日与星期
来源：http://hqm.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wkf.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jsk.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hsu.xinyue.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ols.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iqz.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mcq.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ist.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qlr.yueranfly.top

[J09] 时区处理
来源：http://mwf.0kj1m.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zws.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://buh.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://umz.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zge.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sjf.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kkd.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xsi.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aun.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://yop.nanxinkj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uwi.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://itx.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://quv.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yqa.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://efm.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://imq.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oji.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jyd.yangfankeji.com

================================================================================
来源：http://put.jianghu66.top

K. JSON 与序列化
来源：http://pah.shzxlz.cn

================================================================================
来源：http://zbl.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://bec.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bri.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://olq.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://cvp.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://yih.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oar.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://qzp.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://qzt.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sgt.vehdjk.com

[K02] JSON 字符串转对象
来源：http://hul.hfpthk.cn

Py:   json.loads(s)
来源：http://csb.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jwi.yangfankeji.com

JS:   JSON.parse(s)
来源：http://xxg.hysaishi.cn

TS:   JSON.parse(s)
来源：http://yiy.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oqe.jlsjyb.cn

Go:   json.Unmarshal(data, &v)
来源：http://bkq.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://bvg.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lob.vehdjk.com

[K03] JSON 美化输出（带缩进）
来源：http://wnf.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://faq.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vro.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dyk.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qli.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sqt.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cfu.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://dky.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hql.tarul.cn

[K04] 读取 JSON 文件
来源：http://nsx.zdqjudy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gmd.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mak.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ehw.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jpj.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kax.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uqt.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://liu.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aof.yonumen.top

[K05] 深拷贝对象
来源：http://zcl.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://eel.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://fky.xylfe.cn

JS:   structuredClone(obj)
来源：http://sog.birdmap.top

TS:   structuredClone(obj)
来源：http://wjw.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nva.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://epm.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xnh.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://iuq.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://ckc.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uzh.smart0.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aqm.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vcw.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iym.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aam.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://feb.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wja.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tlk.tian-w.cn

[K07] 进制转换
来源：http://ceq.jqgfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xgy.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://etq.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rlb.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zpl.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zxi.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wfk.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nab.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://roo.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://yyr.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://jhl.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wrh.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://mtl.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://cri.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://djb.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://vvh.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://ybu.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yzq.52xcode.cn

================================================================================
来源：http://lqb.yueranfly.top

L. 网络请求
来源：http://wsx.ppjwa.cn

================================================================================
来源：http://fbv.sxryk.cn

[L01] 发送 GET 请求
来源：http://vdc.sysykeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jve.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wgy.xuetiantiany.cn

JS:   await fetch(url)
来源：http://lll.guannengcc.top

TS:   await fetch(url)
来源：http://jpt.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rjn.316326.xyz

Go:   resp, err := http.Get(url)
来源：http://ixc.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://btz.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://abl.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://oob.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wht.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lbh.redwolf501.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://alt.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rde.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qal.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gbx.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bae.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vgn.yj202588.top

[L03] 设置自定义请求头
来源：http://bfz.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gta.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pcj.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kxn.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ncl.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tmc.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qot.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kby.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://icx.xylfe.cn

[L04] 设置超时
来源：http://hvv.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://hdr.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rpk.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tbx.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://juw.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zuk.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uyt.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jlt.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yfk.hywenlv.cn

[L05] 上传文件（multipart）
来源：http://htw.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rwh.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://emd.shzxlz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://moh.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nhy.ehwqpu.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://inq.kuanghao11.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jfk.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vdc.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lte.yongpay.top

[L06] 解析响应为 JSON
来源：http://rde.zycfv.cn

Py:   resp.json()
来源：http://awp.daxiang520.top

PHP:  json_decode($body, true);
来源：http://cgv.jinghuilouyu.cn

JS:   await resp.json()
来源：http://wfb.shanyushiyangkeji.top

TS:   await resp.json()
来源：http://nzj.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zvx.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ncn.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://jcg.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lab.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://efr.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nxb.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iwe.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://syt.xingfuxueyuan.xyz

TS:   resp.ok;  resp.status
来源：http://rlx.xuanzx.com

Java: resp.statusCode()
来源：http://fhv.jlsjyb.cn

Go:   resp.StatusCode
来源：http://qbn.hcnkem.com

Ruby: resp.code.to_i
来源：http://zdc.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://gdg.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://hfz.guowangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://erg.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://rey.sweek.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zdr.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://urc.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gpy.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fyt.yj20258888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dtv.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cys.shangyingyoupin.top

================================================================================
来源：http://hol.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://ywa.svipenyu.cn

================================================================================
来源：http://olf.ivvv.top

[M01] 读取命令行参数
来源：http://orm.yfazqb.com

Py:   sys.argv[1:]
来源：http://aeu.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://jmo.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://jnj.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://iur.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://tti.yanxiufei.cn

Go:   os.Args[1:]
来源：http://ngv.sysykeji.top

Ruby: ARGV
来源：http://ulu.guannengcc.top

C#:   args 数组（Main 方法参数）
来源：http://jvd.hnxiangtu.top

[M02] 读取环境变量
来源：http://slt.tarul.cn

Py:   os.environ.get("HOME")
来源：http://fqh.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kzd.ivvv.top

JS:   process.env.HOME
来源：http://ueg.yuxming.cn

TS:   process.env.HOME
来源：http://ypv.ivvv.top

Java: System.getenv("HOME")
来源：http://nly.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iti.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://rme.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wcs.fzhhl.top

[M03] 执行外部命令
来源：http://mhg.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gkr.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fys.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://iwm.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gut.hfpthk.cn


<!-- 参考信息 -->