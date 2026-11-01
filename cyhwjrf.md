代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://mobile.tarul.cn/Article/details/gvsongyfb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.bbcook.cn/Article/details/gdvsuttra.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gqjpvizss.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.bbcook.cn/Article/details/goienugxj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.bbcook.cn/Article/details/gyfwqptwd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gakonssxh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/gqtdgosyi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gihjupwvj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gzxeyyosl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.yfazqb.com/Article/details/geiiggtji.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fktsv.cn/Article/details/ggyxuzzas.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.vehdjk.com/Article/details/gfychkhud.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gpbympueq.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/gkwojohuj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.sjlbkw.cn/Article/details/gkyydjtmc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/gpvqjaynr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.sjlbkw.cn/Article/details/gcrdfkgxk.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/ggueuxrko.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.sjlbkw.cn/Article/details/gtntepmdq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/gasotkiaf.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.tarul.cn/Article/details/gqjlyqtih.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/gwrwapxww.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/gwmvjoqht.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.sjlbkw.cn/Article/details/gjpbaesgd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/glmcwwtci.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gkxfccukx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/gcksfgwya.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/geftgxwaz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.yfazqb.com/Article/details/gflsnaujf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/grmoyhyra.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gkivxwlgv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghxkkeioz.sHtML

J. 日期与时间
来源：http://mobile.yfazqb.com/Article/details/gydcptpnl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkjbnwlki.sHtML

[J01] 获取当前时间
来源：http://read.share.fktsv.cn/Article/details/gnmtikxvj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.tarul.cn/Article/details/gznmmvitp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gauxolmih.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gqzchjfrd.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gvmyxqoez.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.sjlbkw.cn/Article/details/gtegcxknv.sHtML

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/gssutnyur.sHtML

Ruby: Time.now
来源：http://www.blog.yfazqb.com/Article/details/gnidchxcb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.bbcook.cn/Article/details/gkgzdqaok.sHtML

[J02] 格式化输出
来源：http://www.share.vehdjk.com/Article/details/gtyzcjfsd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gkczmfisv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gaxrdmnmo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.bbcook.cn/Article/details/guqirdtzk.sHtML

TS:   d.toISOString()
来源：http://3g.vehdjk.com/Article/details/gjlwkyvpi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.vehdjk.com/Article/details/gxyqgqczh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.tarul.cn/Article/details/gvjhkriza.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gybjixcce.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.vehdjk.com/Article/details/gnakrqfzr.sHtML

[J03] 字符串解析为日期
来源：http://www.share.epnwcf.com/Article/details/gyzkpunwh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.vehdjk.com/Article/details/gtoddruxe.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.tarul.cn/Article/details/gbcvhduqb.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gslyqfmqj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gkhmjayjz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/golmobisa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gheeruszp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/ghrybjndo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.vehdjk.com/Article/details/gktilngsz.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fktsv.cn/Article/details/gsieeyfwa.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.bbcook.cn/Article/details/gbqlyweqp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.bbcook.cn/Article/details/gcubgvfqu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/ggmhavchc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.yfazqb.com/Article/details/goddwhrrk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.vehdjk.com/Article/details/gfjgqyefc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.bbcook.cn/Article/details/gfnmsatac.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/gtwznpxdn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.yfazqb.com/Article/details/gtrhqbznt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/ggtpvackr.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.vehdjk.com/Article/details/gvdywfikc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.yfazqb.com/Article/details/glfvywzjy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/ghwsctkcl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gskvxxmys.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.tarul.cn/Article/details/glfrskxjz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.epnwcf.com/Article/details/gkninxlny.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.tarul.cn/Article/details/gqbbykwpe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.epnwcf.com/Article/details/gubzxsehr.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.yfazqb.com/Article/details/gpdfmpukk.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.bbcook.cn/Article/details/grjdaymop.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.bbcook.cn/Article/details/gvlzacgdq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/gdfvfrzee.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/ghbdznpan.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fktsv.cn/Article/details/gvdwrepfi.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.bbcook.cn/Article/details/giwjfusax.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fktsv.cn/Article/details/grlbkculo.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.sjlbkw.cn/Article/details/gergvccvx.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/gqbmublnt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gimgidwto.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gggmnjepd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gywiwlcmu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/ggywkntjw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/glrrrrirb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/ghzfnmaom.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/ggurgfmmg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gcgqxwbvq.sHtML

[J08] 提取年月日与星期
来源：http://wap.vehdjk.com/Article/details/gdbjgmzls.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.yfazqb.com/Article/details/ghhkxvukq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gvudikokr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.vehdjk.com/Article/details/gdkzuaatc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.sjlbkw.cn/Article/details/gddhlybrw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.yfazqb.com/Article/details/gsfymbzwp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fktsv.cn/Article/details/gpktlsjuu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.sjlbkw.cn/Article/details/gezdyilni.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fktsv.cn/Article/details/gtvrdkunp.sHtML

[J09] 时区处理
来源：http://read.share.fktsv.cn/Article/details/gyhdsjgxr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.epnwcf.com/Article/details/gqmcnkaia.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.epnwcf.com/Article/details/gthmaxdxz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/glcoyvnmn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gnjqdtqds.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.sjlbkw.cn/Article/details/gewxlaivg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/gpaoazioa.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fktsv.cn/Article/details/gfbamwapg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.bbcook.cn/Article/details/gufmgrpxx.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.bbcook.cn/Article/details/gkyuckgri.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.tarul.cn/Article/details/gupewqcxw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.tarul.cn/Article/details/gwwhpexou.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gouqvjpyl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/gnrvwrspq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fktsv.cn/Article/details/guuoyokym.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.bbcook.cn/Article/details/gknjqewnz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.tarul.cn/Article/details/gznqzujtd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.tarul.cn/Article/details/gpjfoilli.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gffxvbxdh.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/gyhnovpno.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghtqsahdn.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.bbcook.cn/Article/details/gzmawnqbc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gxtfbxkra.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gcmlccdio.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gcvmjaorf.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gduatirfa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/gydvmosvf.sHtML

Go:   json.Marshal(obj)
来源：http://baike.sjlbkw.cn/Article/details/gnudwobyc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gkluuawxr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.sjlbkw.cn/Article/details/gzrhjwucp.sHtML

[K02] JSON 字符串转对象
来源：http://wap.tarul.cn/Article/details/gegoqvhsl.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/geufkylna.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.yfazqb.com/Article/details/gfchgdjds.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gpgauefcr.sHtML

TS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gizsefawp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/gjcizwxts.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gtdqixipu.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gsmzazzmu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.vehdjk.com/Article/details/gyddalumt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.sjlbkw.cn/Article/details/gjgndretv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gtnoemvnj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gfuvxbmba.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gjazqsfrb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/ggzfsijhx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/gyhzguctp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.bbcook.cn/Article/details/grbbzcbwu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fktsv.cn/Article/details/gctdtafoi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.epnwcf.com/Article/details/goqeufdri.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/glwhbjcfr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.epnwcf.com/Article/details/gknufcvuq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.sjlbkw.cn/Article/details/gboreknsk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gsjqxdujf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/ggwiueidt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gqwdllxcv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gjffuoszt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.bbcook.cn/Article/details/gjpycpzzu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gwiyxekpz.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gwdvvcnfm.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gfhfgeprm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/gcvoqovrd.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/govfixquo.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gndnrrcxe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/gvkspbczy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.epnwcf.com/Article/details/gkelmkkci.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gnibxizsr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gjiqaziyt.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/gfpelalfj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gbwfcnuib.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gqdwjwyri.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gdxkdlmvn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gademgfjm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.bbcook.cn/Article/details/gaomszjdb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gvihcswub.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/glxkyulsk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gnrtxagho.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/gqllgslpm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gmoxusuhv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.vehdjk.com/Article/details/gixczrkza.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/ghkpmtwtu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gaqbvouak.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gvugcmvxi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.epnwcf.com/Article/details/ghgyhhnlm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.yfazqb.com/Article/details/gwsiajtgb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gzsqkdhpb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fktsv.cn/Article/details/gogsbgrol.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.tarul.cn/Article/details/gqbzrlips.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.tarul.cn/Article/details/gmzzzqkqm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gwcjeyjjc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gsthkaslg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.vehdjk.com/Article/details/gisdsalew.sHtML

Go:   encoding/gob
来源：http://www.share.bbcook.cn/Article/details/gnwtuzbdr.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gapzerqnd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gjnkscpdv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/giwcngfko.sHtML

L. 网络请求
来源：http://www.blog.tarul.cn/Article/details/gjjasizmp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbhhmcjwy.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/gepxlqnwm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.vehdjk.com/Article/details/gxkovdazu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.sjlbkw.cn/Article/details/gkrggesxz.sHtML

JS:   await fetch(url)
来源：http://www.share.tarul.cn/Article/details/gdeqwydni.sHtML

TS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gwiujxkld.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.vehdjk.com/Article/details/gxlypyfqu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.epnwcf.com/Article/details/gxtjldrcr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/guaidrfsf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/gpdwxzhpq.sHtML

[L02] 发送 POST JSON
来源：http://blog.vehdjk.com/Article/details/gzukbuhbo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gsdivdtkc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fktsv.cn/Article/details/gailjnkfa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/giaetmoan.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gfcctaudm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.vehdjk.com/Article/details/gjohlcpli.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.sjlbkw.cn/Article/details/gjidfnfna.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/gkexmodwx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fktsv.cn/Article/details/gwrzygvqq.sHtML

[L03] 设置自定义请求头
来源：http://baike.yfazqb.com/Article/details/gujxlwctr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gusgcuplv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fktsv.cn/Article/details/guizphxwh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gvkkfooet.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gwqtthzrv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.tarul.cn/Article/details/gpskcxpzl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gvhygrrcu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.vehdjk.com/Article/details/getbiydwg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gjtsiqxhq.sHtML

[L04] 设置超时
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqijwxpy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.bbcook.cn/Article/details/gqqwuicfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gwtnwmkvv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/gnyyqdiwm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/grzggfptb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.tarul.cn/Article/details/gmyhvvcxv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fktsv.cn/Article/details/gxikpeiiq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.epnwcf.com/Article/details/gjdasleiw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/ggyicudov.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/gvixyrsjs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/gnuxfykfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.yfazqb.com/Article/details/glfbltsut.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gewnkobzk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gakriuabj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/gkegdkwyo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.bbcook.cn/Article/details/grzegmbys.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.bbcook.cn/Article/details/gnhhengqd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gmokvjfdp.sHtML

[L06] 解析响应为 JSON
来源：http://3g.sjlbkw.cn/Article/details/gxsmclzxz.sHtML

Py:   resp.json()
来源：http://mobile.yfazqb.com/Article/details/gwluvamku.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/gdspoutza.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gxfvieyvb.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gkecuosem.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.bbcook.cn/Article/details/grgjebzxo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/gfumingzu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/gxftcukyh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gmmghckhu.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/ginjbxwvg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.sjlbkw.cn/Article/details/gxkvdgqxi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gauuqfnpf.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/grnvwuvah.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/ggriibmzy.sHtML

Java: resp.statusCode()
来源：http://read.share.vehdjk.com/Article/details/gllrwrhmd.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gxpecuajj.sHtML

Ruby: resp.code.to_i
来源：http://3g.tarul.cn/Article/details/gimuqwgpf.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gcsrpfpku.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/gzkkdqtjr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/gtleaculj.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.sjlbkw.cn/Article/details/gzdpatsao.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gaqwpojoq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/glnojhijk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.tarul.cn/Article/details/gxeseyjle.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/gvbmleuxk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gxcfblcuo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gtzfrfyqi.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvqpyxzlv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/gliadjgcd.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glvmuagvz.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gbuxyhfmi.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/gyqrcgbww.sHtML

PHP:  $argv;  $argc;
来源：http://3g.vehdjk.com/Article/details/gvhorkplt.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gjdefpydy.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gbemlplzt.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/grcwfvvdk.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gorvvbqpi.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gcxyhvejt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gqmvxehxf.sHtML

[M02] 读取环境变量
来源：http://www.share.epnwcf.com/Article/details/gbqnqkaqf.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gzolelqtg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gvjqwstfp.sHtML

JS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gosqqvuxy.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gbxvlsfwq.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gmzuulcpa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/grzeghodt.sHtML

Ruby: ENV["HOME"]
来源：http://3g.sjlbkw.cn/Article/details/grvvqqfro.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fktsv.cn/Article/details/gvkdwbmet.sHtML

[M03] 执行外部命令
来源：http://www.share.epnwcf.com/Article/details/gumeulgno.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fktsv.cn/Article/details/gzjsbbekd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gdayktzei.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gwsxbaica.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gazxirqmv.sHtML


<!-- 参考信息 -->