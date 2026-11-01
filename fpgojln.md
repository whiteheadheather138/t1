代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gzvlbsmos.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/glgwiyrbs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.tarul.cn/Article/details/gweyvqzxx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.yfazqb.com/Article/details/gozdurweo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gyisrpxfv.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.yfazqb.com/Article/details/gswhzjcms.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gntmqqtiw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.vehdjk.com/Article/details/ggzbtttuc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fktsv.cn/Article/details/gwfcvzopy.sHtML

TS:   /error/gim
来源：http://m.share.yfazqb.com/Article/details/gisnfonxl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fktsv.cn/Article/details/golebjwan.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.bbcook.cn/Article/details/gpfbzmeeo.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.sjlbkw.cn/Article/details/gigaxigqw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.epnwcf.com/Article/details/gadqhvjje.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fktsv.cn/Article/details/gvptyyrel.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.bbcook.cn/Article/details/guzyyxfoe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/gclkmionv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gxhviavnc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gndxrdpcm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/gqpwthmzz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/guvbfhvoz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.sjlbkw.cn/Article/details/ghifxjlky.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gbjmplddk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbumtixkx.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gesymktei.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqjavciif.sHtML

[J01] 获取当前时间
来源：http://read.share.fktsv.cn/Article/details/ganfsiggd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/gfsuludlb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gwhaxbbch.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/gshbomvaw.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gfmnzmrtp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.bbcook.cn/Article/details/ggersvnkb.sHtML

Go:   time.Now()
来源：http://mobile.vehdjk.com/Article/details/gqsvfdgqb.sHtML

Ruby: Time.now
来源：http://mobile.sjlbkw.cn/Article/details/gfftvdrmx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/gjtvebkgu.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/geuomudzu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/gyklzpzyw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/ghoengqrq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.epnwcf.com/Article/details/gxodbawwn.sHtML

TS:   d.toISOString()
来源：http://baike.tarul.cn/Article/details/gmiuxlsvf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gsithnpvj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.sjlbkw.cn/Article/details/grmfgagop.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/grrnfiozq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/giwireaks.sHtML

[J03] 字符串解析为日期
来源：http://m.share.tarul.cn/Article/details/gcnfqjmpd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.epnwcf.com/Article/details/gbpsihbbf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.tarul.cn/Article/details/gqdrvvkut.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gumvepyfz.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/glkmoupyv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/glwacrmek.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gheaxfinr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/ggfvztcew.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/gjizbxwyi.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gcnjpxozl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fktsv.cn/Article/details/gdsfemkht.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.epnwcf.com/Article/details/gigwseoyb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/ggyjsybnz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.tarul.cn/Article/details/grjygflrw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gkbsrwgwg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fktsv.cn/Article/details/gwpedkcsf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.yfazqb.com/Article/details/guojzhrsv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gxaswlkmy.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fktsv.cn/Article/details/gbmmmqfxu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/gwdzyahro.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/ggontbsjt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gprsvqprf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/grbqgxryz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.epnwcf.com/Article/details/gkorsqcmq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/gntpvmbqb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.epnwcf.com/Article/details/gbcjhvuxp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gmyciyejg.sHtML

[J06] 计算两时间之差
来源：http://read.share.yfazqb.com/Article/details/gaattkiuu.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.tarul.cn/Article/details/gxveqhtzq.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.sjlbkw.cn/Article/details/gijcnprdy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.tarul.cn/Article/details/gecfxhcwx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.vehdjk.com/Article/details/gzomfbeaj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.bbcook.cn/Article/details/gzgkhhhup.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.sjlbkw.cn/Article/details/gqshhrsqv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.bbcook.cn/Article/details/gcxdprfsw.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.bbcook.cn/Article/details/gnytjtfyg.sHtML

[J07] 比较两个日期
来源：http://wap.tarul.cn/Article/details/gxizkopju.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gfbrbtpaf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gkpyosbpg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gixznblxi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gfykhqisp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gnhycekcg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.vehdjk.com/Article/details/gbtedzukd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/ggkdthacx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/ggbjmfwpf.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gmzeppfoi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.vehdjk.com/Article/details/glxfegsmo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.yfazqb.com/Article/details/gggccqsjo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.bbcook.cn/Article/details/grzwnbvyi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fktsv.cn/Article/details/gvtshhhus.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/gthnzliaz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.sjlbkw.cn/Article/details/gzmpsvvoz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fktsv.cn/Article/details/gilsobpfl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.epnwcf.com/Article/details/gaznuuusp.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gbojlrkpg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.epnwcf.com/Article/details/gvlibdzcg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.vehdjk.com/Article/details/gdmbwoojl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gelwevjop.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gvrujgvte.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/glmvbcqws.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.yfazqb.com/Article/details/gejfffixr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fktsv.cn/Article/details/gatkmfomg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.vehdjk.com/Article/details/gwqgscsjk.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.bbcook.cn/Article/details/gjqpdagqj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/gmmtzxjyn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gafkvsozr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.epnwcf.com/Article/details/gdkbfkgis.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/goegoqzlq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gpokemvza.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.bbcook.cn/Article/details/giypqazea.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.bbcook.cn/Article/details/gpvohuqah.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/ggakkyzye.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/glnjbltqv.sHtML

K. JSON 与序列化
来源：http://read.share.sjlbkw.cn/Article/details/gwpryrcoj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gptntbjce.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.yfazqb.com/Article/details/ghqkigdht.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/ginhavoth.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gygzsufom.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdepnzgkz.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/ghxmzfcwo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.vehdjk.com/Article/details/gvxhqchig.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/glaonqhnd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.sjlbkw.cn/Article/details/gxizrjmfn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gvtglgzyu.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.tarul.cn/Article/details/guxmhhpke.sHtML

Py:   json.loads(s)
来源：http://www.blog.epnwcf.com/Article/details/gxjosioho.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.vehdjk.com/Article/details/gdubugxah.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gsunadrpl.sHtML

TS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/ghvrqwmix.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.bbcook.cn/Article/details/gtntwecxi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gjdzlvkbr.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gcrwoxczi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/gxrpyebow.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.bbcook.cn/Article/details/gybybvwlf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gxhtijncd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gaymufkbc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gfkdxfvrn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gxvplegrm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fktsv.cn/Article/details/gsvmridjn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.sjlbkw.cn/Article/details/gevjafuhf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fktsv.cn/Article/details/gkqbhjrxm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.bbcook.cn/Article/details/gjijjxhfi.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fktsv.cn/Article/details/ggcodcnhn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/geikkwrdx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.bbcook.cn/Article/details/gchchpnkq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gkvslwfmi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gjgusrjoe.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmpixxmr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gcvlhozsz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.vehdjk.com/Article/details/gjwixcokw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.tarul.cn/Article/details/gcnnvunrg.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/gefmulplo.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gcpdxpzof.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.tarul.cn/Article/details/geclcegol.sHtML

JS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gbhqixeii.sHtML

TS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/grqcthjgt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.sjlbkw.cn/Article/details/gnpogpvli.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.tarul.cn/Article/details/gfdhhnedt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.vehdjk.com/Article/details/gsmzodbkh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fktsv.cn/Article/details/gpkdhqhcd.sHtML

[K06] 解析 URL 查询串
来源：http://3g.bbcook.cn/Article/details/gheruuikb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/gsnzitlcv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/gzzryuwxi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gmexnnijq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gleulktnp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gxjwbjukj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gdxcdhnei.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gdbhwdaac.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gvrbazzzz.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/gtsekaqcn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyowsonn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gcjitpvtu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gbbdnxxem.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gqjsuctpo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gegjzmekx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gulezuhzs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.epnwcf.com/Article/details/ghnjjifyk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/goglepujy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gundjdwyo.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gguuutdmg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/grfrktzty.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gphuknvjt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gcjenwdzk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gbzawsytz.sHtML

Go:   encoding/gob
来源：http://www.m.share.fktsv.cn/Article/details/glldletoz.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/girxmuwab.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gwojlakxv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqifmafdq.sHtML

L. 网络请求
来源：http://blog.epnwcf.com/Article/details/gpmnetuqp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/geqhqtqjq.sHtML

[L01] 发送 GET 请求
来源：http://read.share.tarul.cn/Article/details/gdspckpyn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fktsv.cn/Article/details/gpnmhqgfw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.bbcook.cn/Article/details/gwmsfuvul.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/golrqudbh.sHtML

TS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gnapibdqq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.bbcook.cn/Article/details/giejnybue.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/glypynifb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.epnwcf.com/Article/details/gwznvhshn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/gqmfpeoos.sHtML

[L02] 发送 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gywqerttb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/goswaxuyv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/gmevtapaz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gnwquclqm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gnkuowasw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/gjnldomga.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/gjfaqhamu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/gghhutnxt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gsxllmobt.sHtML

[L03] 设置自定义请求头
来源：http://mobile.yfazqb.com/Article/details/guhccjitq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.tarul.cn/Article/details/gkqrrkfbh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fktsv.cn/Article/details/gwqfsugub.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gxkvrbfks.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/ghdzhqfyz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/gntuakxks.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gvbpvcoor.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/gppgpxwck.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gfcssjtzb.sHtML

[L04] 设置超时
来源：http://3g.vehdjk.com/Article/details/grpcwqssw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/gswbkstvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gtgqsagzg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/ggeemeape.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gdugvnyvw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.epnwcf.com/Article/details/gwbcunrxd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.epnwcf.com/Article/details/gxckjxoqp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/gcgdqsmar.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/ggzwyzrwt.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.vehdjk.com/Article/details/ggxxpdbdk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gokonezjv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.vehdjk.com/Article/details/gjnbauxkc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gugiqakzn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gfosvpdxu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gehvftkme.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/glllttiiw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.yfazqb.com/Article/details/gtsvdfida.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gqusonyvt.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gbbohrmre.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gdykxumbo.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.yfazqb.com/Article/details/gdyqclttd.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/glayyyrdj.sHtML

TS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gfzsovyln.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gvwgutmjf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gbmiyydfk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gjlyvolhr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gdrijulmn.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gtsorbxlz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gilklviiy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gplnorcjj.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gvhhrddrl.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gdaitlswt.sHtML

Java: resp.statusCode()
来源：http://mobile.bbcook.cn/Article/details/geygtzhad.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gmfokmvul.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gazpncbzh.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fktsv.cn/Article/details/gdyxmldqj.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/gcesdocyk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fktsv.cn/Article/details/gzgyywbkw.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.tarul.cn/Article/details/gigvafqgw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gygllgvsu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gqdjccigc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.epnwcf.com/Article/details/gwsxfglfd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.yfazqb.com/Article/details/gqrcbwpwz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gonkvbrxw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gfymhdmmg.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glhzuofop.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.sjlbkw.cn/Article/details/gjrndxcqf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmwvkemvs.sHtML

[M01] 读取命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gguwmnpbi.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/gfgziwgji.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/gxfjbwmeg.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gsspaxqpq.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gyyptkhco.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gogmlxljz.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gfcciclml.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/glqrrqxlb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gehztspnf.sHtML

[M02] 读取环境变量
来源：http://wap.vehdjk.com/Article/details/gjgghuinr.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/gbiyrnhit.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gmredveby.sHtML

JS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/geoutuzep.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/guwfcormq.sHtML

Java: System.getenv("HOME")
来源：http://baike.yfazqb.com/Article/details/gqxtcwjcs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gbhzypveo.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.bbcook.cn/Article/details/gqzsdtfzg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/giqesivku.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/gmlioqkpx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fktsv.cn/Article/details/gttvbevjg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/gqjugwjdu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gzcshnezp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gvaizccbz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/guzltodxo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.tarul.cn/Article/details/ggixsddmy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.epnwcf.com/Article/details/godwletwr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fktsv.cn/Article/details/gibbipdan.sHtML

[M04] 获取当前工作目录
来源：http://mobile.epnwcf.com/Article/details/gbejdsnis.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/gtxpajygp.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/giizpfmrv.sHtML

JS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/grijscxqz.sHtML


<!-- 参考信息 -->