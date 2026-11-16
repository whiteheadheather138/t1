代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://caj.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mlh.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qmw.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://asf.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mjo.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://mrs.yongpay.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jpt.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://amr.birdmap.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jzf.c1oappe.top

TS:   /error/gim
来源：http://ziy.hnxiangtu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yqr.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wjj.meibo888.top

Ruby: s.scan(/error/i)
来源：http://wrq.jqgufenzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qoh.uphjek.com

[I08] 贪婪与非贪婪匹配
来源：http://qic.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://glu.jqgufenzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kky.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yrw.shanyushiyangtech.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ptn.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kcu.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zde.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qgv.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://seg.birdmap.top

================================================================================
来源：http://xqi.cheryme.top

J. 日期与时间
来源：http://nye.tarul.cn

================================================================================
来源：http://uax.zhiwuduotai.top

[J01] 获取当前时间
来源：http://krk.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ulm.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hff.yfazqb.com

JS:   new Date();  Date.now()
来源：http://evj.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://ovi.jinqigfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rlw.ywan-chungtsiang.top

Go:   time.Now()
来源：http://ikc.yongpay.top

Ruby: Time.now
来源：http://pzc.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vdr.hammf.cn

[J02] 格式化输出
来源：http://bbs.chenzaomai.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ddx.jianghu66.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bko.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qmc.9152youxi.cn

TS:   d.toISOString()
来源：http://cmh.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zki.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hen.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cao.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jjo.hammf.cn

[J03] 字符串解析为日期
来源：http://bin.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ips.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nwk.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://jzv.yj20258.top

TS:   new Date("2024-01-02")
来源：http://amw.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jtb.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iik.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://wgz.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bwj.feifeiyinyue.top

[J04] 时间戳与日期互转
来源：http://cxf.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cek.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yuz.meibo888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uum.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bsz.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dwg.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rdu.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://phu.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ydf.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://xtp.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://hes.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://uey.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zgl.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xih.xinyue.icu

Java: LocalDate.now().plusDays(7)
来源：http://xyd.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://das.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://tdc.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://vwx.hysaishi.cn

[J06] 计算两时间之差
来源：http://fbm.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://tff.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://nks.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ifn.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tbc.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ouq.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://fot.xuetiantiany.cn

Ruby: end - start                 # 返回秒数
来源：http://ftz.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://chy.yuanzhike.top

[J07] 比较两个日期
来源：http://yaw.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://hkf.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uxh.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dux.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://ohb.jyoumei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zlp.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eto.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://kiw.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://mod.zycfv.cn

[J08] 提取年月日与星期
来源：http://wxi.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://thr.yangfankeji.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aet.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fes.jianghu66.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xen.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xpv.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ots.shanyushiyangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zyx.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pcf.gaohongyu789.top

[J09] 时区处理
来源：http://vch.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tra.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tfq.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jud.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vbu.zdqjudy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wde.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cfk.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hxz.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eij.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://nks.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ckg.cqqwz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wzv.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rjy.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nkd.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zrl.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://glk.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zpz.c1oappe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xhn.birdmap.top

================================================================================
来源：http://fzq.ydjk.org.cn

K. JSON 与序列化
来源：http://xbc.yangfankeji.com

================================================================================
来源：http://oae.cucudq.cn

[K01] 对象转 JSON 字符串
来源：http://pcb.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cvr.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://etb.yj20258.top

JS:   JSON.stringify(obj)
来源：http://rqh.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://vyi.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://icy.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://opl.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nmi.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://znc.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://wgh.andypj.xyz

Py:   json.loads(s)
来源：http://ius.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rdo.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://kkm.tian-w.cn

TS:   JSON.parse(s)
来源：http://jtu.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kjw.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://kyn.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://kau.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jsr.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://fpo.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uma.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zec.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uqa.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://syz.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jso.snrcjt.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xcq.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://eli.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rky.fktsv.cn

[K04] 读取 JSON 文件
来源：http://ssa.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hov.xinyue.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vcx.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nsg.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nta.yanxiufei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dqn.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://evt.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zjn.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qye.hammf.cn

[K05] 深拷贝对象
来源：http://sdb.sysykeji.top

Py:   copy.deepcopy(obj)
来源：http://jmz.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://riw.havefunace.top

JS:   structuredClone(obj)
来源：http://yqx.jqgfzy.top

TS:   structuredClone(obj)
来源：http://osb.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ufs.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zdn.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rfq.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kbg.andypj.xyz

[K06] 解析 URL 查询串
来源：http://nky.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vgo.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nrd.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lgt.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://whf.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jpu.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mat.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kee.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yaf.0kj1m.cn

[K07] 进制转换
来源：http://xps.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hmd.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bpa.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://auj.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://djz.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jst.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bee.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ojs.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fil.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://lir.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://rzl.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://meq.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://xjo.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://nee.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://unf.hesvh.cn

Go:   encoding/gob
来源：http://jzp.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://igv.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qlc.cashguo.top

================================================================================
来源：http://vob.feifeiyinyue.top

L. 网络请求
来源：http://cdr.haohaochexian.top

================================================================================
来源：http://bsu.shuidangran.top

[L01] 发送 GET 请求
来源：http://fmk.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uhe.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vyh.yongpay.top

JS:   await fetch(url)
来源：http://kkx.meibo888.top

TS:   await fetch(url)
来源：http://swz.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lag.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://wyk.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pym.sxryk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://phg.sufxvd.cn

[L02] 发送 POST JSON
来源：http://ppv.jlsjyb.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cja.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://afl.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bef.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://txc.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gra.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mtl.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ozp.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://etp.chenzaomai.com

[L03] 设置自定义请求头
来源：http://cvo.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dyz.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ihu.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bpm.fzhhl.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hox.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cia.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eil.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pjy.andypj.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nps.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://zlt.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://jxx.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ifu.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://glp.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mca.snrcjt.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vgd.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ljx.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kmq.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ymb.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://gkj.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wkv.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oeo.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gdo.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dkl.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://snh.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dtz.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zji.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aym.tanke756.top

[L06] 解析响应为 JSON
来源：http://azr.feifeiyinyue.top

Py:   resp.json()
来源：http://uim.hesvh.cn

PHP:  json_decode($body, true);
来源：http://vhw.vehdjk.com

JS:   await resp.json()
来源：http://owl.wangdashe.top

TS:   await resp.json()
来源：http://tvw.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://udl.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hxe.fktsv.cn

Ruby: JSON.parse(resp.body)
来源：http://bye.shangyingyoupin.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gkv.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://qdr.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ddp.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bso.sufxvd.cn

JS:   resp.ok;  resp.status
来源：http://htg.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://cvx.yfazqb.com

Java: resp.statusCode()
来源：http://hhx.hongshengwenyu.top

Go:   resp.StatusCode
来源：http://sys.hywenlv.cn

Ruby: resp.code.to_i
来源：http://wco.yj202588.top

C#:   (int)resp.StatusCode
来源：http://pte.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://czl.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dms.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://sfw.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tzf.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sfm.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pei.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ggy.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mto.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yll.guannengcc.top

================================================================================
来源：http://zww.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://skt.zhijiandao.cn

================================================================================
来源：http://kcz.tanke756.top

[M01] 读取命令行参数
来源：http://jck.andypj.xyz

Py:   sys.argv[1:]
来源：http://dyz.shuidangran.top

PHP:  $argv;  $argc;
来源：http://rfa.xinyue.icu

JS:   process.argv.slice(2)
来源：http://qam.ybcxt.top

TS:   process.argv.slice(2)
来源：http://asy.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://lcx.ppjwa.cn

Go:   os.Args[1:]
来源：http://chb.chenlongwang.top

Ruby: ARGV
来源：http://eyz.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://bdy.daxiang520.top

[M02] 读取环境变量
来源：http://mcw.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://xoh.jqgfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jll.0kj1m.cn

JS:   process.env.HOME
来源：http://vbe.ehwqpu.com

TS:   process.env.HOME
来源：http://cuz.fzhhl.top

Java: System.getenv("HOME")
来源：http://ojx.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mef.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://gcu.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dmn.chenjidiqi.icu

[M03] 执行外部命令
来源：http://age.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ifs.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ubz.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hth.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://deh.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aua.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lfy.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://hpu.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://cnk.xinyue.icu

[M04] 获取当前工作目录
来源：http://goq.yanxiufei.cn

Py:   os.getcwd()
来源：http://uww.zhiwuduotai.top

PHP:  getcwd();
来源：http://ocu.jiagoushi.top

JS:   process.cwd()
来源：http://gbu.hcnkem.com


<!-- 参考信息 -->