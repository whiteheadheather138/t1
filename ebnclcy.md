代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gvmpmskcy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.tarul.cn/Article/details/gspvdnarr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gdlusctli.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.vehdjk.com/Article/details/gzfkxgloz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.yfazqb.com/Article/details/gfaiyypni.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gvlevycmd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/gagkfsrdr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/geidqqhpg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gfauhyxgc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/ghrddefpc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.epnwcf.com/Article/details/gzypelzyv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fktsv.cn/Article/details/gowyjvbps.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gevsspjnr.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.vehdjk.com/Article/details/gpntpguht.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.bbcook.cn/Article/details/gbjyonpwa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gwlcfuozi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.yfazqb.com/Article/details/ggeoqydqd.sHtML

TS:   /error/gim
来源：http://blog.epnwcf.com/Article/details/gcfervygv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fktsv.cn/Article/details/gkxvgolih.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.epnwcf.com/Article/details/gdjmpmeqs.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.tarul.cn/Article/details/gipflhyst.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/gqnkhmrut.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.yfazqb.com/Article/details/gpprhgcor.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fktsv.cn/Article/details/gtkyjjttl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gfqjzwlar.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gbmjixekw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gjoipyyiw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gwoobmeuq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/gfisjqwbl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.sjlbkw.cn/Article/details/gakwmsihd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/gxurmmrtc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grkcjkwyz.sHtML

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gyxbdbcxt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glwyvzaqj.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/gshsmzkjw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.tarul.cn/Article/details/gxdyhkpke.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gktjnulhl.sHtML

JS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gsuurcpiw.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.vehdjk.com/Article/details/gktsqjddh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.yfazqb.com/Article/details/givfejqdd.sHtML

Go:   time.Now()
来源：http://www.share.vehdjk.com/Article/details/gvqyngkew.sHtML

Ruby: Time.now
来源：http://3g.vehdjk.com/Article/details/guttqolxy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.yfazqb.com/Article/details/gkfytjrre.sHtML

[J02] 格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gdkpfwrvk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gfldfzynh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gnxnuegxg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.tarul.cn/Article/details/gvccbxmnd.sHtML

TS:   d.toISOString()
来源：http://mobile.bbcook.cn/Article/details/gsdevxzgp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.bbcook.cn/Article/details/gipywwjhx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.vehdjk.com/Article/details/gqjofgabi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gyybhpjxh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.sjlbkw.cn/Article/details/gvulgvhjf.sHtML

[J03] 字符串解析为日期
来源：http://blog.epnwcf.com/Article/details/gvtmxmsic.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fktsv.cn/Article/details/gulpxrapg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fktsv.cn/Article/details/gvtfkjgfv.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/giqoaaaso.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gaejxbbhq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gejzxmzlh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/ghcyvhxpz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gvyhynmqq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.bbcook.cn/Article/details/gnkxcglnj.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gelvlbopa.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.yfazqb.com/Article/details/gtfetkhtp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.epnwcf.com/Article/details/gkaickixk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.tarul.cn/Article/details/gdekvhnxw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.epnwcf.com/Article/details/gxdmmwwff.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fktsv.cn/Article/details/giwmmvzsk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fktsv.cn/Article/details/gmxdiqntg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gwwfrpkzk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fktsv.cn/Article/details/gavasitif.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.epnwcf.com/Article/details/gsnflzttt.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.epnwcf.com/Article/details/gdwkekxsl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.vehdjk.com/Article/details/gjkzdqgmj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gxuytreht.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gcsuzkvsp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fktsv.cn/Article/details/gcsrjsbff.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.sjlbkw.cn/Article/details/gedbrgkey.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.tarul.cn/Article/details/gaistcshw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/gfaxoossb.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gdcyxouzb.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fktsv.cn/Article/details/grxzoxhbw.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fktsv.cn/Article/details/gclffbtfp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.yfazqb.com/Article/details/gqrleymrj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gzgesrspp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gcpwesjct.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.tarul.cn/Article/details/gqnzbiqyr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.bbcook.cn/Article/details/guybansfo.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/gceymphxw.sHtML

[J07] 比较两个日期
来源：http://3g.epnwcf.com/Article/details/gpiojasha.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gtascntfm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gqgpxqkja.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gnbgstvvk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gpjkqyxgf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/ginibgjko.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/gfgfekmob.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gpnadtdlj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gjglfrhzy.sHtML

[J08] 提取年月日与星期
来源：http://baike.tarul.cn/Article/details/gullzawev.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.tarul.cn/Article/details/gyswnhjhf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.yfazqb.com/Article/details/grdmabwlr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/gshmsmdma.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.vehdjk.com/Article/details/gdlxvlvdr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/gbkjzvcss.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gpfufztst.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.bbcook.cn/Article/details/gnsbxbbcr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.vehdjk.com/Article/details/gbapawyjf.sHtML

[J09] 时区处理
来源：http://3g.bbcook.cn/Article/details/gudnjcjtq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.epnwcf.com/Article/details/gngskgsss.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fktsv.cn/Article/details/goipnnsvg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gyrrjorue.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/grtcmlvgv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/gevpufasc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gvljphisi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.vehdjk.com/Article/details/gjzcpjped.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/gmsxwuyah.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/gudqlkxue.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fktsv.cn/Article/details/grtipfhce.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/gumbqakhe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gpienvwfx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.tarul.cn/Article/details/gvgqymkci.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.vehdjk.com/Article/details/giudrbuie.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.bbcook.cn/Article/details/govdwexxn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.sjlbkw.cn/Article/details/gaxtqfotc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.epnwcf.com/Article/details/gmpovemzv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gimgzkykc.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/gkbyrhobp.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxjedebpe.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.epnwcf.com/Article/details/gehkqpczn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/geuaptwfr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gigxvatwq.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gadwignuc.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gdfyftssb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fktsv.cn/Article/details/gekffxpud.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.vehdjk.com/Article/details/geqlycuuu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/gbipfzcoe.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.epnwcf.com/Article/details/gzrbmmcrt.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gbhvcsfkj.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gixwxozyi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.bbcook.cn/Article/details/gofyfhnso.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gthtxvuid.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gvbkyjhhb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gtzydmnat.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gvqgommkr.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gkmvrykro.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/grycwqltc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/goanzwkob.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/gkbxdyyhp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/ggzldgpei.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/gyzdiihyq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gncekkvzp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.tarul.cn/Article/details/gzermfpfm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/gakqoxyif.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gyedjsjqw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.vehdjk.com/Article/details/gmwknemyz.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/goizedpgp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/ghznzlrkc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.vehdjk.com/Article/details/glbmsgnpw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gfswhwssd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/glsgcxfdr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlhlfrba.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gwwdjuams.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.yfazqb.com/Article/details/gwfcpcsnl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.vehdjk.com/Article/details/guheafqrr.sHtML

[K05] 深拷贝对象
来源：http://mobile.tarul.cn/Article/details/gcblijcyj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gkducdqby.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gsepuqmja.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gjmzoxtiq.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gzkwuhrrg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gshhyxyet.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gjmjhnfzf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gsseyvzra.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.epnwcf.com/Article/details/gomvznevd.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.sjlbkw.cn/Article/details/gavpplkcu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/grfzixhhy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/ghxvcpqmp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gdqhoelff.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gdkvvpfey.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fktsv.cn/Article/details/gkydgnxrx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gjcyxnqzi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/guxrauwaj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gdbreltom.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/ggcpvlgvp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gsiedhofm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gndgigqrk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gaioqsxvv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gtnbmpfso.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gjqnyqcru.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/gmllsogqa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.yfazqb.com/Article/details/gxgafheie.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gekvevxma.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/gsqufznkt.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fktsv.cn/Article/details/gklggawfg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.tarul.cn/Article/details/gmexnakun.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gthzytmdm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/guhhzbsza.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.vehdjk.com/Article/details/gjtycsniq.sHtML

Go:   encoding/gob
来源：http://3g.fktsv.cn/Article/details/gkastbqlb.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.bbcook.cn/Article/details/ghzaaztvk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gwqgdgyqi.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gizxcychg.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/ghmdvpuhf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gfnqbuxmn.sHtML

[L01] 发送 GET 请求
来源：http://read.share.vehdjk.com/Article/details/gwecgtvbi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/ggmoavpcr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/gvezjkvki.sHtML

JS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/grnxjwjue.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/ggvrxzirq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.tarul.cn/Article/details/gkpvmflpa.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.vehdjk.com/Article/details/gourrizws.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.tarul.cn/Article/details/gbbgzmvgd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.epnwcf.com/Article/details/gawazofjp.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gvgksdrua.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.bbcook.cn/Article/details/galqlqony.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fktsv.cn/Article/details/gscasroot.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gituoiuwk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gmdsqmwno.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/gusnetnev.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.tarul.cn/Article/details/gafstmjpe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/gsvggvple.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.epnwcf.com/Article/details/guavdbxxx.sHtML

[L03] 设置自定义请求头
来源：http://www.share.vehdjk.com/Article/details/gwicxplfr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.yfazqb.com/Article/details/gaqfsclvp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.bbcook.cn/Article/details/ggtmtbycx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/gxwgldofz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/grvjsrjsc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.bbcook.cn/Article/details/glwpftlam.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/guskrbwxj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.tarul.cn/Article/details/gjjoehesb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/ghhulpxly.sHtML

[L04] 设置超时
来源：http://read.share.fktsv.cn/Article/details/gkbwqpogz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.tarul.cn/Article/details/gosrxjbtf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gewsbspgq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gngxxtidk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/glprtzaeh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.tarul.cn/Article/details/gzarokwse.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gboehdsuq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.sjlbkw.cn/Article/details/gsfttnlji.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.epnwcf.com/Article/details/gefwrmvwp.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gmqrqqlky.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gzvfvycdw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/gdedgxjbb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gbjsakrdh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gcrlavwep.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.yfazqb.com/Article/details/gvjcucnaf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/glshquwos.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.epnwcf.com/Article/details/gqmontypr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gndaploxa.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmiqzftn.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/gxehkxqjl.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/gptgtmsgg.sHtML

JS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gcnbzorat.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gjxstgkis.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gqypyiodc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/gquebelqy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.yfazqb.com/Article/details/gawcyjdng.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.yfazqb.com/Article/details/gqedenzzt.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gkacbwyry.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gucnwjbcm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/gaydpyzvo.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/glogwlpwp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gomzowtdi.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/gzrxdtcor.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gzcnvaeew.sHtML

Ruby: resp.code.to_i
来源：http://www.share.vehdjk.com/Article/details/gbctuywnp.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gixgbrvqv.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/gkzhnthns.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.tarul.cn/Article/details/gdigmjfxr.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.vehdjk.com/Article/details/gfupddulh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gtgwgrojd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/ghvqfmufv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fktsv.cn/Article/details/gylemkkzc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.epnwcf.com/Article/details/gqvjpojqy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/giffnxtxk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gnntopici.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gogenpgpw.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fktsv.cn/Article/details/gyuahwnec.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gryzcohwj.sHtML

[M01] 读取命令行参数
来源：http://mobile.fktsv.cn/Article/details/gvtssioyg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/gryphzjth.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/ghrrecdqu.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gcioxwqbv.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gddhtwhtf.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gpsocmgnx.sHtML

Go:   os.Args[1:]
来源：http://read.share.vehdjk.com/Article/details/gmyunoxfw.sHtML

Ruby: ARGV
来源：http://www.blog.bbcook.cn/Article/details/gkweeagih.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gwfuewwvs.sHtML

[M02] 读取环境变量
来源：http://mobile.epnwcf.com/Article/details/gnrsmqpmo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gdwtkihhq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gnxrxjitx.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gkdkfvkxa.sHtML

TS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gvsipsnan.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gwikngexc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gdwttyzie.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gmmmzthwf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/guaqtukqa.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/gekyddezx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fktsv.cn/Article/details/gidqcgeiy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/gaguedhwt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gpiholrhk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/grlewkvwe.sHtML


<!-- 参考信息 -->