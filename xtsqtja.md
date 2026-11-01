代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/gezljziqd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gaiztgujm.sHtML

JS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gngkztpjf.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gmjwkxnwy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/giaheurjn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fktsv.cn/Article/details/gjnzuivnb.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/gturvbhip.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.vehdjk.com/Article/details/gzyyodgaw.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.epnwcf.com/Article/details/ghypquina.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gyfanqced.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwfduvgz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fktsv.cn/Article/details/gqyskhazc.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.yfazqb.com/Article/details/goiuifpqz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/gybzcjoae.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.yfazqb.com/Article/details/gfjzozjfl.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.tarul.cn/Article/details/guxbalnyc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.bbcook.cn/Article/details/gkerauhzb.sHtML

[I03] 提取捕获分组
来源：http://m.share.vehdjk.com/Article/details/gxeeqqnzl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.sjlbkw.cn/Article/details/gvdrrqjzd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gnwujcofl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/grqdwpmrd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.vehdjk.com/Article/details/gnhojagsy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/goouusgah.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fktsv.cn/Article/details/gcqzbfcod.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.vehdjk.com/Article/details/gqmhbrlpc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.bbcook.cn/Article/details/gwiburzfz.sHtML

[I04] 正则替换
来源：http://baike.tarul.cn/Article/details/gkdypcrlf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.yfazqb.com/Article/details/grggkaacp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/grvyjztvn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gyztljbcz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/girqfxerg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gaazdwosx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.vehdjk.com/Article/details/gkxmybpxc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gojnojbnv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.vehdjk.com/Article/details/ghqivjtai.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gfokxtlcd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fktsv.cn/Article/details/giwjtcpkg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/gjorydeec.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gdcownrqk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gnhomyixq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/greqjfapt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.tarul.cn/Article/details/gtvbfiudr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gtmtzckiv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.vehdjk.com/Article/details/gdubsrpcj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/ghvawszef.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gxbiamrwz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.bbcook.cn/Article/details/gurjwqkob.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/ghlyumdnf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/gecufokan.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gkkdzpbno.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.yfazqb.com/Article/details/grkcuvime.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gznbyudgx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/ggkewhxfc.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.vehdjk.com/Article/details/gwicddmtj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.yfazqb.com/Article/details/ghcvmvzbr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.epnwcf.com/Article/details/ggfbfjqla.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.sjlbkw.cn/Article/details/gkhrlufuf.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/gcqrlsuqn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.epnwcf.com/Article/details/gdjwmdtcx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.vehdjk.com/Article/details/gplnutlis.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.yfazqb.com/Article/details/gygulgjxy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/glbmfgbor.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.vehdjk.com/Article/details/gaiysdsuu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/ghcfvoylo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/ggqfidsiu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gvobytdrh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/glvbxaqxy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gbhceaahd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/gjabbhyct.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fktsv.cn/Article/details/gerjplqxo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/gtqarhanp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glyjcvnaq.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gpylcfmns.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxiuedayb.sHtML

[J01] 获取当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gcekrhogm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.sjlbkw.cn/Article/details/ggkpfrqfu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/guraunkfo.sHtML

JS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/gumbrcncn.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/gnxdtukdq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpjpkkdv.sHtML

Go:   time.Now()
来源：http://mobile.bbcook.cn/Article/details/gvapkdsar.sHtML

Ruby: Time.now
来源：http://m.share.sjlbkw.cn/Article/details/gkazqpmjr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.epnwcf.com/Article/details/gecayufeu.sHtML

[J02] 格式化输出
来源：http://baike.epnwcf.com/Article/details/gufacngzh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gxnkzodnq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gfbtgwpal.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.epnwcf.com/Article/details/gbjcbbtmz.sHtML

TS:   d.toISOString()
来源：http://wap.epnwcf.com/Article/details/gzmmxmzed.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.vehdjk.com/Article/details/ghvpsrtfi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.bbcook.cn/Article/details/gxxasmdhv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/ggjwmtktn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fktsv.cn/Article/details/guvhejbds.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gvtaqrpui.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/gnlceqayd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.yfazqb.com/Article/details/geoukjxry.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gwvcnwgjt.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gqinghjcp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gnakaovjf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gevdqxwho.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gozdmonvn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/gokdclqdh.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.sjlbkw.cn/Article/details/gzmfhprmc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.bbcook.cn/Article/details/gqewqvpug.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.tarul.cn/Article/details/gpcjtjevm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gxpwjtxed.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.sjlbkw.cn/Article/details/gizidosmo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.epnwcf.com/Article/details/gskjlfner.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gdrzriibe.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.vehdjk.com/Article/details/ggmxjpwif.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fktsv.cn/Article/details/gqpqstaky.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.epnwcf.com/Article/details/gpliubzmj.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fktsv.cn/Article/details/gqgqojmyy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/gvzfjzzxm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gqjlhdmyv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gjjtqwcrb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gyllvgczy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fktsv.cn/Article/details/gbjryefww.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/gzqlavmyc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.vehdjk.com/Article/details/gitbjsbba.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gtrywcarx.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fktsv.cn/Article/details/gqgwuokqz.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.tarul.cn/Article/details/gkqaxqzlm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.epnwcf.com/Article/details/glcsgdbdx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.epnwcf.com/Article/details/gphsdvgvb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/gilmhhmtu.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/ggdsrltcf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.epnwcf.com/Article/details/gwvugqjyf.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gsvrggplq.sHtML

[J07] 比较两个日期
来源：http://3g.fktsv.cn/Article/details/grrdeywhx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gobqrlhop.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.tarul.cn/Article/details/grusrzfva.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gsfhjfyep.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/grjdadbkr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/gvocwgjjl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gpyhupriz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gfctnvxzo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gjeuiqpmz.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/ggwjvamgg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/ggwjuxnqa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/goglaozks.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/gwtbksqtf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.vehdjk.com/Article/details/gycbxphko.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/ghixlftwy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.bbcook.cn/Article/details/gxnqonrzk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.yfazqb.com/Article/details/geokmitig.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/gusvtsghf.sHtML

[J09] 时区处理
来源：http://www.blog.yfazqb.com/Article/details/gskggnife.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.tarul.cn/Article/details/gcdovxlkb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.sjlbkw.cn/Article/details/gblxilaiq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gpkcixnvq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gxinhpyhp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.bbcook.cn/Article/details/gqtaeelzq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gwcfbyxzz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/ggvupnjix.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.epnwcf.com/Article/details/gpxlwgubk.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.tarul.cn/Article/details/gmyafoeae.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.bbcook.cn/Article/details/giicpncjz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.epnwcf.com/Article/details/gdlsukoyn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.sjlbkw.cn/Article/details/ggmlcdfsi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gdoumyykl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.epnwcf.com/Article/details/gcatfzhln.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.yfazqb.com/Article/details/gjgrdlsxm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.bbcook.cn/Article/details/gkvgjmnxs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/gkvvgbesz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtxqsgkvt.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/gitdmmrzj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxlrwsgrl.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fktsv.cn/Article/details/gbhmervuf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gzkwncqkt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gervmwezm.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gajokoamv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gpummyfug.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/gtaozrhho.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gxsrnuueg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/ghxawqdnx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gvrievfdh.sHtML

[K02] JSON 字符串转对象
来源：http://3g.epnwcf.com/Article/details/ggjtsctmh.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/glxqtyttg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.epnwcf.com/Article/details/gmkysatlq.sHtML

JS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gnsganlzq.sHtML

TS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gepccadmw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gobfrfwdo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gmariswxf.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gjoesoyej.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/gpupyepyg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.bbcook.cn/Article/details/gialjdcer.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/gqklepzlt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/gfdesbrqh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gbjywcbsb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gkyiglxez.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlrsjvgv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.sjlbkw.cn/Article/details/gtwtrbjzu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.tarul.cn/Article/details/gzwvhwjve.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.tarul.cn/Article/details/gmeodgpqg.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.bbcook.cn/Article/details/goswnmbkk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/gfbubawiz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/gusrgrmfb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/giwpbnbui.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gavkorrfz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.epnwcf.com/Article/details/garyfgjfn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gzcntlloj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.tarul.cn/Article/details/gxvoxkuxh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/gsauznsxl.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gimtbggti.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.epnwcf.com/Article/details/gqfoagpsf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fktsv.cn/Article/details/gcrwafhem.sHtML

JS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gsbhmgmkr.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/ggwlwmumh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.epnwcf.com/Article/details/ggdrsmqzx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gipftcaij.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.yfazqb.com/Article/details/gpnqbrbhw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fktsv.cn/Article/details/gancgxjld.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gvlqkwjmy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gitgkepcp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/gudekawah.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gyttcpsut.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/ghwfbwfld.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/gupwwsmhk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/guepsblnt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gqwpcgovg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gmgcxhszy.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/gqzzvcfaz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gwzrsrnqa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.yfazqb.com/Article/details/gnhrpiorz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gjnxyngag.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gsmaoqgqm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gxonxevry.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gbgdeclju.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/gisgmqfzq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gastnklcu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fktsv.cn/Article/details/gbyrbxtdj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gougzjprl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/gecwgffbq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gsxqwfarb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gqpsdqayv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/gruegcber.sHtML

Go:   encoding/gob
来源：http://www.m.share.bbcook.cn/Article/details/grtddfnfb.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.vehdjk.com/Article/details/gybmnxyrk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.tarul.cn/Article/details/gvajhrmfi.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggdtvrygk.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/goagajxxm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfdomggnt.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/gzsdzwmht.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.vehdjk.com/Article/details/gugptrqdz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.sjlbkw.cn/Article/details/gipuzfxgh.sHtML

JS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gowqctead.sHtML

TS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gikfbyjst.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fktsv.cn/Article/details/gonkbctvl.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gexwlatqs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/gcqnxkmsf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.tarul.cn/Article/details/gqpzlognf.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gexrmvskh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gcrghmcho.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fktsv.cn/Article/details/guyqilqcg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gryidiopr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gbhefllta.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/glckfapdi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fktsv.cn/Article/details/gwbqqtfjw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gtuvxyqgq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.epnwcf.com/Article/details/gwatikxjn.sHtML

[L03] 设置自定义请求头
来源：http://baike.fktsv.cn/Article/details/gfdvxviku.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.sjlbkw.cn/Article/details/gajthoqiz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.yfazqb.com/Article/details/gfgrhplfz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/ggcmpjuzc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gqazxlxmb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fktsv.cn/Article/details/gucyilwvf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/gnorfctvr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/guwyqwsaq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gvupkzixu.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gtjoqteza.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.vehdjk.com/Article/details/gorwaegup.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.vehdjk.com/Article/details/gbqlalncb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/ggaplbclo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gfnxmstxg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/glyboegkg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/gukggijgz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.epnwcf.com/Article/details/gqyqyihan.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.tarul.cn/Article/details/ghzadguny.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/gsngnfkzg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.bbcook.cn/Article/details/girpkwoin.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gkxjopkzt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gulvapgke.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gxcxtlaxb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/gmkyqbpao.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.yfazqb.com/Article/details/gmqnzsocf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/gewyhxchx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fktsv.cn/Article/details/gjgnmsvdf.sHtML

[L06] 解析响应为 JSON
来源：http://blog.tarul.cn/Article/details/ghdkgjayg.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gdrndujka.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/gjgztqvzl.sHtML

JS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/ginlcymai.sHtML

TS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gesgokbie.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gotgtwtuq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.epnwcf.com/Article/details/gogxarnzy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fktsv.cn/Article/details/gtohcfkti.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gzpwcxfoy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/grhjfqvii.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fktsv.cn/Article/details/gygojvahe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gkqiqwvwt.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gimvjitbq.sHtML


<!-- 参考信息 -->