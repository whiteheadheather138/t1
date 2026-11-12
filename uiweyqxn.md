代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://qcs.fengsongda.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xhc.c1oappe.top

JS:   s.split(/\s*,\s*/)
来源：http://ppr.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://bff.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://hzn.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://byc.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://cyz.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wrg.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ecv.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xxr.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bmd.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lvh.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://api.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mjx.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qut.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aqq.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xrs.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://dau.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dmr.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vex.shuidangran.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bra.ctjpmb.com

TS:   /error/gim
来源：http://axb.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ghh.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aji.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://dnt.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tpi.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://pdw.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ymh.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://acx.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pzb.yvedp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pzf.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gel.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gog.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fos.dashuyun.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://agt.tarul.cn

================================================================================
来源：http://vhp.wangdashe.top

J. 日期与时间
来源：http://qya.wangdashe.top

================================================================================
来源：http://uqz.wangdashe.top

[J01] 获取当前时间
来源：http://mys.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://piz.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iut.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://aae.vehdjk.com

TS:   new Date();  Date.now()
来源：http://zcz.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hgw.chenlongwang.top

Go:   time.Now()
来源：http://zyp.aizwys.cn

Ruby: Time.now
来源：http://bqi.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bdh.zhiwuduotai.top

[J02] 格式化输出
来源：http://ubq.bbcook.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://inz.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ecm.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yna.cucudq.cn

TS:   d.toISOString()
来源：http://xjx.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gig.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zey.ybcxt.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nzg.sufxvd.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rsn.nanxuanxn.top

[J03] 字符串解析为日期
来源：http://yzg.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ljs.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sib.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://nox.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://ggi.aizwys.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sny.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://spz.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://gxd.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://quh.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://dgn.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uao.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tuf.aibaodan.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dww.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://feo.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rly.gogol.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://srq.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jzw.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://slr.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://qcj.ctjpmb.com

Py:   now + timedelta(days=7)
来源：http://yex.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dta.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lcf.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eor.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://efu.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hdd.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://qya.svipenyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vhs.tanke756.top

[J06] 计算两时间之差
来源：http://wvy.ivvv.top

Py:   (end - start).total_seconds()
来源：http://hck.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://gjr.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jaa.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://toa.zhongyouzk.top

Java: Duration.between(start, end).toSeconds()
来源：http://rjd.cdnleiting.top

Go:   end.Sub(start).Hours()
来源：http://eom.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://lmi.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://bdb.shanyushiyangtech.top

[J07] 比较两个日期
来源：http://sxs.hnxiangtu.top

Py:   d1 < d2;  d1 == d2
来源：http://hbj.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rff.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ldu.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://oup.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ucu.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jjb.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://fsm.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://xka.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://rat.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zka.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oxy.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cou.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uep.jinyuanbaomall.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mmb.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yoo.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iml.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rrm.xylfe.cn

[J09] 时区处理
来源：http://mqd.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nlq.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lvs.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oly.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://omj.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gkm.zhongyouzk.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://woj.hcnkem.com

Ruby: Time.now.getlocal("+08:00")
来源：http://czh.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sax.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://aha.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ftz.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lnv.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fbg.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aqn.hesvh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zza.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hbe.nwbrower.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zwu.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vln.kuanghao11.cn

================================================================================
来源：http://cac.xylfe.cn

K. JSON 与序列化
来源：http://ytw.sysykeji.top

================================================================================
来源：http://uyp.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://aar.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://epu.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lph.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://zdj.cheryme.top

TS:   JSON.stringify(obj)
来源：http://nsw.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://chv.hnqzz.top

Go:   json.Marshal(obj)
来源：http://hev.aibaodan.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mah.zdbjq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://omh.c1oappe.top

[K02] JSON 字符串转对象
来源：http://vgq.dashuyun.cn

Py:   json.loads(s)
来源：http://jez.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fij.shuidangran.top

JS:   JSON.parse(s)
来源：http://gtp.sxryk.cn

TS:   JSON.parse(s)
来源：http://buc.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ncn.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://fui.sysykeji.top

Ruby: JSON.parse(s)
来源：http://nxr.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fmo.xziqi.cn

[K03] JSON 美化输出（带缩进）
来源：http://tbs.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yga.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tcq.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yhn.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vuf.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sxz.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ifo.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://zah.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qcz.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://gme.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dih.dashuyun.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hrr.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://msi.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wjh.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jqn.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ffg.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://frx.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wcs.svipenyu.cn

[K05] 深拷贝对象
来源：http://kqm.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://lvu.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://htr.wangdashe.top

JS:   structuredClone(obj)
来源：http://yfy.smart0.xyz

TS:   structuredClone(obj)
来源：http://baq.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://woe.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kkq.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hrh.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tam.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://ccs.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yih.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ncm.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xjg.nwbrower.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://glc.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gbn.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ycp.hnxiangtu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aek.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://phg.hesvh.cn

[K07] 进制转换
来源：http://pdf.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uec.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xpg.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iuy.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wej.sysykeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bgj.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vgl.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xpw.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iox.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://lqq.daria6918.cn

Py:   pickle.dumps(obj)
来源：http://jyk.zhongyouzk.top

PHP:  serialize($obj);  unserialize($s);
来源：http://znb.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://rod.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://pnl.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ipb.shzxlz.cn

Go:   encoding/gob
来源：http://qfx.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://rgu.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pwa.tarul.cn

================================================================================
来源：http://tlx.zycfv.cn

L. 网络请求
来源：http://fpk.ydjk.org.cn

================================================================================
来源：http://arr.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://gik.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xnn.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rqf.birdmap.top

JS:   await fetch(url)
来源：http://epp.havefunace.top

TS:   await fetch(url)
来源：http://kyk.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://srx.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://hks.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jim.smart0.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://puu.yueranfly.top

[L02] 发送 POST JSON
来源：http://rjh.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://siq.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xml.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jge.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jmf.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oub.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ccb.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xhk.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://psa.xinyue.icu

[L03] 设置自定义请求头
来源：http://njs.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qhm.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jph.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ebf.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bty.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xfm.cheryme.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://neh.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qdg.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qbe.guowangkeji.top

[L04] 设置超时
来源：http://zhs.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://gvv.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://doq.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tst.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyh.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://msu.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bmg.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lye.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lmv.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://kfs.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tap.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://umc.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tuo.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tax.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://spk.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dos.uphjek.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wll.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://glh.bjfxy.top

[L06] 解析响应为 JSON
来源：http://btb.hfpthk.cn

Py:   resp.json()
来源：http://wrh.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://ijw.nanxuanxn.top

JS:   await resp.json()
来源：http://sfw.gotoacloud.top

TS:   await resp.json()
来源：http://wjq.gotoacloud.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mag.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tup.snrcjt.cn

Ruby: JSON.parse(resp.body)
来源：http://tzj.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rze.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://wwx.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fdq.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wvm.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://hsm.yj202588.top

TS:   resp.ok;  resp.status
来源：http://mrn.ydjk.org.cn

Java: resp.statusCode()
来源：http://fgk.gogol.net.cn

Go:   resp.StatusCode
来源：http://enr.dianchejie.cn

Ruby: resp.code.to_i
来源：http://ejr.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://hxx.ydzc1.top

[L08] 并发请求多个地址
来源：http://dqe.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lsn.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://fto.xziqi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sig.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gcq.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nxt.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pcx.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vmu.shzxlz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dhn.snrcjt.cn

================================================================================
来源：http://ncg.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://vms.jqgfzy.top

================================================================================
来源：http://wnh.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://fso.hywenlv.cn

Py:   sys.argv[1:]
来源：http://eue.pycfn.com

PHP:  $argv;  $argc;
来源：http://vmr.yvedp.cn

JS:   process.argv.slice(2)
来源：http://zwl.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://ote.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://pzv.havefunace.top

Go:   os.Args[1:]
来源：http://ihp.fanxiaobao.xyz

Ruby: ARGV
来源：http://vmz.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://flc.xuanzx.com

[M02] 读取环境变量
来源：http://irs.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://crw.hesvh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ehm.hesvh.cn

JS:   process.env.HOME
来源：http://tus.wangshuangyany.cn

TS:   process.env.HOME
来源：http://grq.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://ezn.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gie.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://vkm.hfpthk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ozc.andypj.xyz

[M03] 执行外部命令
来源：http://xgm.dianchejie.cn


<!-- 参考信息 -->