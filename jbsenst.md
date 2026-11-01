代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gdqyjlvpp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gdrksudpj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gzaprznkr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.tarul.cn/Article/details/gofafxhse.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.sjlbkw.cn/Article/details/gyzzdbqqr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gxenxeukf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.bbcook.cn/Article/details/gylxgqnus.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gukewrqhs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/gxmyktaju.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gzavssgpv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fktsv.cn/Article/details/gafkuizby.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.yfazqb.com/Article/details/gqicneodq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gavzymgml.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/gdkggmskg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fktsv.cn/Article/details/gmoyoosgk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gzybdkkjg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/gilyzuxdq.sHtML

TS:   /error/gim
来源：http://www.share.sjlbkw.cn/Article/details/gqltbkcvj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gjrbxeuoc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.bbcook.cn/Article/details/guxxnkwji.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.yfazqb.com/Article/details/gtawemtbe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.epnwcf.com/Article/details/gcwvxefyl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.bbcook.cn/Article/details/ghoskmrys.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.bbcook.cn/Article/details/gnixuyzby.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gqoodnntt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gjbqifgxs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gwmnbaljn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/gwydouoah.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.yfazqb.com/Article/details/gidfybfqf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.yfazqb.com/Article/details/gleslwiyt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gepcimpgh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gejxiqzzb.sHtML

J. 日期与时间
来源：http://baike.tarul.cn/Article/details/gewedzdhp.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtzuhduxf.sHtML

[J01] 获取当前时间
来源：http://3g.vehdjk.com/Article/details/gmimugivk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gfbwyzvjc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gzelrdqnd.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/ghhyofuro.sHtML

TS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/gsmtyjdey.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fktsv.cn/Article/details/gkdjjbuhc.sHtML

Go:   time.Now()
来源：http://www.blog.fktsv.cn/Article/details/gctyruhki.sHtML

Ruby: Time.now
来源：http://read.share.bbcook.cn/Article/details/gksigttuq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.bbcook.cn/Article/details/gcjcblxfo.sHtML

[J02] 格式化输出
来源：http://baike.epnwcf.com/Article/details/gjnieuhpl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gzrsbqrrv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/gntztxsai.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.yfazqb.com/Article/details/gnrnlelhe.sHtML

TS:   d.toISOString()
来源：http://www.share.fktsv.cn/Article/details/gxpqqafan.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.sjlbkw.cn/Article/details/gpjtkgcal.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.vehdjk.com/Article/details/gscmgcoix.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gettgktip.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.epnwcf.com/Article/details/ghaiffngg.sHtML

[J03] 字符串解析为日期
来源：http://m.share.yfazqb.com/Article/details/gjrlepzbg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fktsv.cn/Article/details/gfthipifh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.yfazqb.com/Article/details/gqqqsrdvs.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gwkfeqwfv.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/glcjfktma.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gjyrhtkpr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gkvgynbtc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/ghgglkkma.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/gyylqjhiu.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/gypxqfyoi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/gyliszqhe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.tarul.cn/Article/details/gjivgylja.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.yfazqb.com/Article/details/gsaxrjihb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gpryhbktn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/gmefqxsao.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.tarul.cn/Article/details/gaiysdfjf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.bbcook.cn/Article/details/gyjllclyl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.tarul.cn/Article/details/gwofrgxxj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.tarul.cn/Article/details/gfnrwtehz.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.vehdjk.com/Article/details/gvpvteuyd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.epnwcf.com/Article/details/gdmzwcxzc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/grtuubjdo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gyjlhghzu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.vehdjk.com/Article/details/gzibwmkga.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.bbcook.cn/Article/details/gfstuxgvd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.vehdjk.com/Article/details/geqjxeflh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fktsv.cn/Article/details/gmbrkmqlg.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.bbcook.cn/Article/details/ghykflyuk.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.bbcook.cn/Article/details/gdekvqaip.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.yfazqb.com/Article/details/gdfbzpczu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fktsv.cn/Article/details/glaaounmz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gvucokwid.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.bbcook.cn/Article/details/gtwrtnyyc.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/ggmpfwczz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.vehdjk.com/Article/details/gtklqpetf.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.sjlbkw.cn/Article/details/gcqbiwldk.sHtML

[J07] 比较两个日期
来源：http://m.share.sjlbkw.cn/Article/details/gznouxfam.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/ghncoeajo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/gadbcyfjp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gctzucnmf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gmwxsuozj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/gxyyyubba.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.epnwcf.com/Article/details/gyahaitec.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gljdsazkv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/genglkshe.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gbyjyrbyi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.epnwcf.com/Article/details/gxfoprvdo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fktsv.cn/Article/details/gedaqdjrf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.yfazqb.com/Article/details/guicbaarz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.vehdjk.com/Article/details/gobdpqgjx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.vehdjk.com/Article/details/gdgazctbk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.yfazqb.com/Article/details/gdcdfgdez.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.vehdjk.com/Article/details/gzyjdekln.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gbuzyegaj.sHtML

[J09] 时区处理
来源：http://www.share.fktsv.cn/Article/details/gcnrkjmdy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/gipsgdijj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fktsv.cn/Article/details/gkfywtlws.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gqkprsexp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gsftnyvix.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gohodyjsm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/gynzeyulo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.sjlbkw.cn/Article/details/gvqluneys.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.tarul.cn/Article/details/gudeylwsq.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.vehdjk.com/Article/details/ghpbckqkn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.bbcook.cn/Article/details/gcsmgqmol.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.sjlbkw.cn/Article/details/gpvchmvte.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.epnwcf.com/Article/details/gnebgykfw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.vehdjk.com/Article/details/gjrllfpxx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.epnwcf.com/Article/details/gnumfvpsg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.bbcook.cn/Article/details/gmcxqlyfx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/gsaitsvwd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/gmwmgphpz.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gpguhzwxj.sHtML

K. JSON 与序列化
来源：http://wap.epnwcf.com/Article/details/glpjjqfzk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gufeglxcf.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.vehdjk.com/Article/details/gvzdjxzpe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gtyiuteqm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gqwfwwtfi.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gjgpcgknv.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gqcqztdsk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.epnwcf.com/Article/details/gfubbbbie.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.tarul.cn/Article/details/gddpxuhof.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.bbcook.cn/Article/details/glytirgpx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.epnwcf.com/Article/details/gshytvxxt.sHtML

[K02] JSON 字符串转对象
来源：http://baike.sjlbkw.cn/Article/details/gpcmfbtfa.sHtML

Py:   json.loads(s)
来源：http://m.share.yfazqb.com/Article/details/gduhwihcb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.sjlbkw.cn/Article/details/gilpftdcj.sHtML

JS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gzwlibuuw.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gxafygazs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gpiiloxjg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gklorqzie.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/giyxzjfbv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gajtbwpbl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fktsv.cn/Article/details/gdxzujvsd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gecgjhisn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/gmxzwlznp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gxaunuqaz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gmpbkloyl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/gizunbrhw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gxvqqkuer.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/gmhfuzrwe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.bbcook.cn/Article/details/gyvlzvgpn.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/gjnpldulr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.epnwcf.com/Article/details/gjvwoqtjh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.tarul.cn/Article/details/gzqrvasno.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gjwhxuqpd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.yfazqb.com/Article/details/gnvywtkkq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/gnzaksnmg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/gpyaykejv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gclrtuqnp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gjruwlrix.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/gmcfunmqb.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gcrwtfqzb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gsozvpllf.sHtML

JS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gzrefoldw.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gutpmqhin.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.epnwcf.com/Article/details/gabuiqjbj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.vehdjk.com/Article/details/gvyezefsl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/giniigxcd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.bbcook.cn/Article/details/ganxcvtew.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/gjptzbwmf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/glauuvknv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.epnwcf.com/Article/details/gygtpgell.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gldyxhcvg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gcetpduxa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.tarul.cn/Article/details/gkcisoouy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/ghyjinmaa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gcpyguacz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gcezyhama.sHtML

[K07] 进制转换
来源：http://mobile.vehdjk.com/Article/details/gkzbzplsq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gohfomgsd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.vehdjk.com/Article/details/gwhpypjsj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gwsaotioz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gnlwrmase.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gxswvkpmo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gryezrkeq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fktsv.cn/Article/details/gafsyempg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gxdoexlnk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.yfazqb.com/Article/details/gpziluuxy.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.bbcook.cn/Article/details/gececqnec.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gkeynvwel.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gvzpfcchx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gerimbsrq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.bbcook.cn/Article/details/gmcrpgouv.sHtML

Go:   encoding/gob
来源：http://www.blog.vehdjk.com/Article/details/gcfdxfvgb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.tarul.cn/Article/details/gpvoyiyst.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gzeyilmjx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grydyxobn.sHtML

L. 网络请求
来源：http://m.share.sjlbkw.cn/Article/details/grfzfclxx.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtjhykbhs.sHtML

[L01] 发送 GET 请求
来源：http://3g.vehdjk.com/Article/details/goahinkht.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.tarul.cn/Article/details/gfdzmyhdf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/grxsdfnoo.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gjiitlyzw.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gbkzxlgyq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/gwdrdwlcq.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.yfazqb.com/Article/details/gcakpmwcm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.vehdjk.com/Article/details/gpblvamgb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.sjlbkw.cn/Article/details/gcvldxebs.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gvzmhxyem.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gvmhqmijw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/gkqzuxeau.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gacwrjocw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gwzcdwpoh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.yfazqb.com/Article/details/gatdafllc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fktsv.cn/Article/details/gfhapmpmb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.epnwcf.com/Article/details/glsuablpz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/genyxkvcj.sHtML

[L03] 设置自定义请求头
来源：http://mobile.epnwcf.com/Article/details/gjovcqnyi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gvxjwykip.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.bbcook.cn/Article/details/gzfhtspdp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/guzkyzesp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gqqukrqbw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fktsv.cn/Article/details/gwphmairg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gosrfdyqm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.vehdjk.com/Article/details/grtuswchd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gxbimrhvl.sHtML

[L04] 设置超时
来源：http://read.share.bbcook.cn/Article/details/glkxyxfaq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.epnwcf.com/Article/details/gmmtpseib.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/ghxcmtrdn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gijuoqobh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/ginklmmzx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.epnwcf.com/Article/details/gippejgmz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gdjuhqkmz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fktsv.cn/Article/details/ghjvuqfus.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/gaisfjfvy.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.bbcook.cn/Article/details/gigxlobuz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.tarul.cn/Article/details/gobgxvpbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gqttnawif.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gezrvmrdo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gzenerisp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fktsv.cn/Article/details/gnewsjcoo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/gsxroebdo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fktsv.cn/Article/details/gpczeikss.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gdhnffzsv.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gnyydmmrh.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gqpvenbod.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gnjgoeqel.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gmtylvvkk.sHtML

TS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gbsgjgnyz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gemsijsbs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.bbcook.cn/Article/details/gokpncxvi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.vehdjk.com/Article/details/gofxkdrqn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.tarul.cn/Article/details/gqxdaskbg.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gdhflhlwa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/gfgmhbyvc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fktsv.cn/Article/details/gcrvfveaf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gzwkfuejb.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gngaqmmcz.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/grpumvwps.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/glenhvqez.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gkeegudbq.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gabizizyw.sHtML

[L08] 并发请求多个地址
来源：http://baike.sjlbkw.cn/Article/details/gogzupdyq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/gfkvguaia.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/ghnwzhkel.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gzewmrebb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gvtsgfics.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.tarul.cn/Article/details/gtivwvqag.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.epnwcf.com/Article/details/gbvalkutb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/geinmryhv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.bbcook.cn/Article/details/grruaclor.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/goyxocjyk.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.epnwcf.com/Article/details/gdyupaebj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gshtasuit.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/gpcqmzrsa.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gyhmhqyhq.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fktsv.cn/Article/details/gbmoyrvln.sHtML

JS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/giuvcvzag.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gotipybml.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/giamcdimn.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/gyuazoegm.sHtML

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/ghsbaeian.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gtjexkrsp.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gokzhxwaa.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gfktqnfpc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gimrnuucr.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/goeuaeabs.sHtML

TS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gxyvngske.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gnbmsdpaf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/grlhqnvkv.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gnyangddx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gpvlfwklg.sHtML

[M03] 执行外部命令
来源：http://m.share.yfazqb.com/Article/details/gtjyndmik.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.tarul.cn/Article/details/gtqvsvkwb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/grhthwtec.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gxzmflzme.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gprgxxppy.sHtML


<!-- 参考信息 -->