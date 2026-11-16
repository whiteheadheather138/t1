代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://zvo.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vdx.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://pqp.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hdt.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xei.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xmb.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eiq.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://etx.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vro.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rrc.shanyushiyangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bqe.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xfs.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ewb.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://dpz.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://anr.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zpq.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hbt.zdqjudy.top

TS:   /error/gim
来源：http://peu.cheryme.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hus.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qyj.jqgfzy.top

Ruby: s.scan(/error/i)
来源：http://pxj.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tly.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://xvq.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ofk.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wtv.jyoumei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pur.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://flk.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cct.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ysh.nanxinkj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ccc.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nrh.zhixingplan.top

================================================================================
来源：http://wzm.ehwqpu.com

J. 日期与时间
来源：http://afa.zhongyouzk.top

================================================================================
来源：http://kyz.epnwcf.com

[J01] 获取当前时间
来源：http://zry.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://cgf.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vbw.yangfankeji.com

JS:   new Date();  Date.now()
来源：http://lkz.jinyuanbaomall.cn

TS:   new Date();  Date.now()
来源：http://xjc.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lwa.jinqigufen.top

Go:   time.Now()
来源：http://byz.tianlin.xyz

Ruby: Time.now
来源：http://scr.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ekk.yueranfly.top

[J02] 格式化输出
来源：http://ott.bjfxy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xjr.smart0.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qth.316326.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://icx.yueranfly.top

TS:   d.toISOString()
来源：http://hnw.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oeb.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hdx.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cti.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hlb.tianlin.xyz

[J03] 字符串解析为日期
来源：http://grb.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gev.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gmc.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://syb.birdmap.top

TS:   new Date("2024-01-02")
来源：http://ynh.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://srl.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pzs.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://bjx.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://efk.yvedp.cn

[J04] 时间戳与日期互转
来源：http://lqn.aizwys.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zky.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pad.svipenyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://msb.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hjn.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ukq.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qbd.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cxp.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qjc.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://ean.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://gbt.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wwo.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mnn.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dln.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://gli.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dyp.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://ome.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cip.guannengcc.top

[J06] 计算两时间之差
来源：http://nox.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://ttb.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://ntu.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vfr.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xry.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://xif.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://qlc.cheryme.top

Ruby: end - start                 # 返回秒数
来源：http://pux.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://wgv.ywan-chungtsiang.top

[J07] 比较两个日期
来源：http://wvd.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://apr.zdqjudy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zen.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://ssi.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://sex.tarul.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xkh.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://scn.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://bot.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://mrc.316326.xyz

[J08] 提取年月日与星期
来源：http://fwa.tarul.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://air.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yyb.yonumen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qxo.sysykeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fjb.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://icc.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dkx.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yab.shanyushiyangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://amj.cdnleiting.top

[J09] 时区处理
来源：http://mob.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rse.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qga.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://umj.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zqr.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oqc.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jyt.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bct.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fha.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://qmm.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tdz.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qhp.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xgx.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mbf.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zcu.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zer.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://agp.tanke756.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://djv.tarul.cn

================================================================================
来源：http://hel.shangyingyoupin.top

K. JSON 与序列化
来源：http://imw.shuidangran.top

================================================================================
来源：http://gny.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://kjg.bjfxy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://naf.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kwr.redwolf501.top

JS:   JSON.stringify(obj)
来源：http://dvd.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://dxc.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://myw.zhongyouzk.top

Go:   json.Marshal(obj)
来源：http://zxr.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kjm.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nwi.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://uzp.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://otu.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pzl.dashuyun.cn

JS:   JSON.parse(s)
来源：http://rop.chenlongwang.top

TS:   JSON.parse(s)
来源：http://ase.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pzb.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://bpu.daxiang520.top

Ruby: JSON.parse(s)
来源：http://hmw.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gne.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://qdl.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://djy.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cfl.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wrf.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wfs.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hwp.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uyi.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://czz.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pwz.cashguo.top

[K04] 读取 JSON 文件
来源：http://aks.jiagoushi.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mgt.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dyn.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jbq.zycfv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tyl.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yhl.epnwcf.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ovp.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mmk.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qwq.yongpay.top

[K05] 深拷贝对象
来源：http://hfd.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://ass.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://kpe.havefunace.top

JS:   structuredClone(obj)
来源：http://fef.cqqwz.cn

TS:   structuredClone(obj)
来源：http://tuj.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://rxj.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://urs.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yog.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://zvm.daxiang520.top

[K06] 解析 URL 查询串
来源：http://gqx.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qrt.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bde.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zrx.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tvm.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://imp.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://axa.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ufv.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ufo.wangdashe.top

[K07] 进制转换
来源：http://eig.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://juy.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cjd.316326.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kyk.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vve.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mud.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lha.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://raz.nanxinkj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://onf.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://psr.havefunace.top

Py:   pickle.dumps(obj)
来源：http://jpk.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://qmq.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://zrt.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://sph.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nxm.gotoacloud.top

Go:   encoding/gob
来源：http://fab.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://eqd.hammf.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tsk.chenlongwang.top

================================================================================
来源：http://vif.nanxuanxn.top

L. 网络请求
来源：http://qmo.svipenyu.cn

================================================================================
来源：http://mac.cheryme.top

[L01] 发送 GET 请求
来源：http://vzp.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eev.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://buu.nanxuanxn.top

JS:   await fetch(url)
来源：http://rxz.yj202588.top

TS:   await fetch(url)
来源：http://xxf.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hca.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://plk.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tny.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fbm.chenjidiqi.icu

[L02] 发送 POST JSON
来源：http://qrr.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://wle.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dea.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://isa.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://prg.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hum.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cdg.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wym.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jge.cashguo.top

[L03] 设置自定义请求头
来源：http://gng.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mrj.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cha.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xmn.ydjk.org.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lxa.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xpi.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nil.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ldf.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mcv.zhijiandao.cn

[L04] 设置超时
来源：http://soq.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://rxr.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kpf.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qvs.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vxt.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://flr.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hsf.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fgy.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ddl.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://blu.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xan.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oes.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://txb.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zjg.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kse.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vqv.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jfl.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tbf.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://son.yongpay.top

Py:   resp.json()
来源：http://rmp.ybcxt.top

PHP:  json_decode($body, true);
来源：http://rjy.0kj1m.cn

JS:   await resp.json()
来源：http://lfb.hnqzz.top

TS:   await resp.json()
来源：http://omj.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vab.haohaochexian.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pkr.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://yae.jinqigufen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xdl.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://myk.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ppu.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eqx.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://bon.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://jxq.tarul.cn

Java: resp.statusCode()
来源：http://rmn.hnxiangtu.top

Go:   resp.StatusCode
来源：http://jnj.jyoumei.cn

Ruby: resp.code.to_i
来源：http://syb.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://nqn.chenzaomai.com

[L08] 并发请求多个地址
来源：http://aqs.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ylk.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://fac.zhaomingkeji.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jgz.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hqn.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ruu.yuxming.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://juo.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mat.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://niq.vehdjk.com

================================================================================
来源：http://ils.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://lvn.fehbvm.com

================================================================================
来源：http://dvw.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://wsk.yj20258.top

Py:   sys.argv[1:]
来源：http://hyd.yueranfly.top

PHP:  $argv;  $argc;
来源：http://tnb.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://rcu.hcnkem.com

TS:   process.argv.slice(2)
来源：http://zga.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://dje.shzxlz.cn

Go:   os.Args[1:]
来源：http://foz.vqdsnc.cn

Ruby: ARGV
来源：http://rwa.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://lqt.vehdjk.com

[M02] 读取环境变量
来源：http://zal.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://evv.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ltj.zhoulong.xyz

JS:   process.env.HOME
来源：http://qnx.cashguo.top

TS:   process.env.HOME
来源：http://fpl.havefunace.top

Java: System.getenv("HOME")
来源：http://jdv.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tpe.jinqigufen.top

Ruby: ENV["HOME"]
来源：http://khf.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://slo.zdqjudy.top

[M03] 执行外部命令
来源：http://vfw.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bes.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kwx.sweek.top

JS:   child_process.execSync("ls -l").toString()
来源：http://oem.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pmn.xinyue.icu


<!-- 参考信息 -->