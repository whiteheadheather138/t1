代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/gdwhfhpdb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.epnwcf.com/Article/details/gotvcqqdz.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/ggnwzcxcv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghueuflsw.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gzcunywpq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/glixzdctb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.tarul.cn/Article/details/gnskngort.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.epnwcf.com/Article/details/gvocenxix.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.yfazqb.com/Article/details/gxucrlasj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.sjlbkw.cn/Article/details/guciglouo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/glzkpsdpn.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.tarul.cn/Article/details/grfijvxoo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/ggknqkeyh.sHtML

[I03] 提取捕获分组
来源：http://wap.fktsv.cn/Article/details/gohddebbw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.yfazqb.com/Article/details/gejpbvxko.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.vehdjk.com/Article/details/gbezeklgm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.bbcook.cn/Article/details/gaqlcafbx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/gasnsjjse.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.vehdjk.com/Article/details/glivmyfsl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.bbcook.cn/Article/details/gzpqvzhpr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fktsv.cn/Article/details/gpadibpqe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/ghzkjambb.sHtML

[I04] 正则替换
来源：http://blog.vehdjk.com/Article/details/gddmdydqo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.bbcook.cn/Article/details/golymqaei.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/gwgecewhf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/glzgczbhc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gzgnpoqtv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gzkpwnkia.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.tarul.cn/Article/details/gxesmcuhx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.tarul.cn/Article/details/ggnwzzodd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gmzqcnohf.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gxnbstump.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.vehdjk.com/Article/details/gkcaolwvs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gimrugmbm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gpfgqkwmn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/glkjwsmsp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/grxvcelev.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/gxmpukmbk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gykvwvgtt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gdsaddqyq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.tarul.cn/Article/details/glbffzhie.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gwvtfpylt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.yfazqb.com/Article/details/gwljzutwk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/gwtlsagbe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gprdmopjr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gtikgknnk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.bbcook.cn/Article/details/gjskwekog.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.epnwcf.com/Article/details/gwyxrzrrh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gijefdhsb.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.sjlbkw.cn/Article/details/grbayrzcs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.sjlbkw.cn/Article/details/gkzcgyzmb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gadobkztm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.bbcook.cn/Article/details/gymtkrwub.sHtML

TS:   /error/gim
来源：http://www.m.share.bbcook.cn/Article/details/gswvcsnus.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.tarul.cn/Article/details/geijvuouc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gqpbhubrd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.epnwcf.com/Article/details/gfirphujs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.sjlbkw.cn/Article/details/gbiycrypc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.tarul.cn/Article/details/gswjsthdb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.epnwcf.com/Article/details/giwbcgukk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gueywvirj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gkezzirts.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/gowmowhvv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gazalgjnm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.bbcook.cn/Article/details/gnsdxkies.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.epnwcf.com/Article/details/gaahbcmto.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gbpfoeqsv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/guwosrosw.sHtML

J. 日期与时间
来源：http://baike.yfazqb.com/Article/details/gxzxzbktu.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/guyptmand.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/gbungmlsf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.vehdjk.com/Article/details/gqdncvnau.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gujonmdla.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gisbhavmi.sHtML

TS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/glgbhgxbe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fktsv.cn/Article/details/gvqyvxvgz.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gynoolqye.sHtML

Ruby: Time.now
来源：http://baike.tarul.cn/Article/details/gfrwzibsg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.epnwcf.com/Article/details/ghgasedbj.sHtML

[J02] 格式化输出
来源：http://3g.vehdjk.com/Article/details/grbpahvgo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gpuesugng.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gcbtjjutt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.epnwcf.com/Article/details/gqomwnwwd.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/geytgjhtm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.bbcook.cn/Article/details/gbfdrzfqd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.yfazqb.com/Article/details/gsfuxhvgr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gebhcnzfj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.vehdjk.com/Article/details/gkfnzwoao.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/gkhewolmr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.yfazqb.com/Article/details/gffehkzxe.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/gmrwbsstr.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gmvrnaehn.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gfiimtvxs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gtbwvzsir.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gufqveemn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gslqvqgvv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.yfazqb.com/Article/details/gjzomagmv.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.bbcook.cn/Article/details/gqcliqces.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.sjlbkw.cn/Article/details/gccirfqai.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/gxsyngyiq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gnvakgbwv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.tarul.cn/Article/details/ghkwduzok.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.tarul.cn/Article/details/grspgejfd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/grbqlstwc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.vehdjk.com/Article/details/gebkyyrbm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.tarul.cn/Article/details/glawnglkv.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.sjlbkw.cn/Article/details/gnykbmiol.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/gvsfjkqeo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.sjlbkw.cn/Article/details/gkechneva.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/ghcjcdfqz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gkcszonps.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.tarul.cn/Article/details/gybapgpvm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fktsv.cn/Article/details/gtyskriwf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.bbcook.cn/Article/details/grvbcoliw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/ghrzlctoc.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/gddvvwkzx.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.tarul.cn/Article/details/gulfbikfp.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.yfazqb.com/Article/details/ghbbuwjjw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.yfazqb.com/Article/details/gzxlnuren.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.yfazqb.com/Article/details/gtitiobjr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.tarul.cn/Article/details/gyzbkuioo.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.yfazqb.com/Article/details/glnsxqfff.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fktsv.cn/Article/details/gmbspqkya.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.tarul.cn/Article/details/gbhrmnouh.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/gpirrxfdk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gwnceqvzb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.sjlbkw.cn/Article/details/giionszqq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gtsrqegkd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gtsqkajqs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/gquiyrzmp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.vehdjk.com/Article/details/gzwcbftij.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gghsbavpq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/ghkaaiazq.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gmlbsyadi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.bbcook.cn/Article/details/glynhkaqo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/gmbescmic.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.bbcook.cn/Article/details/gtbrzugjt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fktsv.cn/Article/details/ggrkfklho.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.sjlbkw.cn/Article/details/gmbyavwye.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.yfazqb.com/Article/details/gdcygepyk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.sjlbkw.cn/Article/details/gndknxbmz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gkjsmsczx.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gsojlrzpc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.yfazqb.com/Article/details/gpsnjticv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.sjlbkw.cn/Article/details/gdotixieu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gxtlhvpkb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/ggbieoyyy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.tarul.cn/Article/details/gvamupdqq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.vehdjk.com/Article/details/gxhfwhcol.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.bbcook.cn/Article/details/gzkgkpwhg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/glgqjlplg.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/ghtlmuocx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/grwyydasu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.tarul.cn/Article/details/gkuwnwveg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/gltwbjiog.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gsmyypkxo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.tarul.cn/Article/details/gsmujrnxq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.tarul.cn/Article/details/glytdwalb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/govbtwhys.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/glgoemvyf.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glwopxsdu.sHtML

K. JSON 与序列化
来源：http://read.share.yfazqb.com/Article/details/gktxdhjry.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxrtyutts.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.vehdjk.com/Article/details/gajptzvgu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gwaricbvu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/ggylehlzv.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gprzxdenr.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gwcqutyna.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.sjlbkw.cn/Article/details/gpribbysg.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/gqtjscubq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fktsv.cn/Article/details/gszograap.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.tarul.cn/Article/details/gzqfjqykl.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.sjlbkw.cn/Article/details/gmcjiooof.sHtML

Py:   json.loads(s)
来源：http://mobile.vehdjk.com/Article/details/glesrquvj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.tarul.cn/Article/details/gnvekbodk.sHtML

JS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gvtieucas.sHtML

TS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gfpixctjq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.yfazqb.com/Article/details/gpdnoxqdd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gwkjeuyng.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/ginccdhmf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.yfazqb.com/Article/details/gcxadbwgx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fktsv.cn/Article/details/glpacekob.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gtjgpumwu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gboofshiu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gxvobusbv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gqtpowksi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gpndtsjtc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gyllazufe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gnfcwumnr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/gknstyxlx.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.bbcook.cn/Article/details/gkeohfula.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gqiyfplgo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.bbcook.cn/Article/details/gtwlvcumv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/grijzuxjk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/ggvnzjwov.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/gubhiwzyi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gilnbjxdz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gbohkdxtu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gvtsseatg.sHtML

[K05] 深拷贝对象
来源：http://blog.fktsv.cn/Article/details/grlauyofj.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.tarul.cn/Article/details/guitukstf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/ggusafjle.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/garrgqqsr.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gubkmyowl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.bbcook.cn/Article/details/gvhogghju.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gzqwjkjni.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fktsv.cn/Article/details/gqzidooqf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.yfazqb.com/Article/details/gukzzdxfp.sHtML

[K06] 解析 URL 查询串
来源：http://blog.epnwcf.com/Article/details/glovjbshs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.tarul.cn/Article/details/guamptccs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gizmdtnjc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/guviqqbsr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gymnafars.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/gbmjmwcim.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gherkeuev.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gfvtvpggz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gpdymamjw.sHtML

[K07] 进制转换
来源：http://blog.yfazqb.com/Article/details/gwxukwvqg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gcqyvaqwu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/gqeyaofgy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gmzddyimk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gqftbyeta.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/ggngjuemw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gvlswzkhq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/gboarrjuv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.tarul.cn/Article/details/gdjhqqtgp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/gauuholcq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gnkoasmcr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/gibcunmcf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gvtbqgbmz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gfnovilia.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.sjlbkw.cn/Article/details/gmarftzse.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gnmhlpsop.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.tarul.cn/Article/details/gckqigpkv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gtvrumsvu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gycdfeaux.sHtML

L. 网络请求
来源：http://www.m.share.epnwcf.com/Article/details/glkfdkahi.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/godkmjpok.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgxlrlcm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/gkvfpqter.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.tarul.cn/Article/details/gujtiwtdm.sHtML

JS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gjvjawlvm.sHtML

TS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gjwbvlgyv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gczheasyr.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/grpwjzndp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gnijxxeke.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/glreromzi.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/grakjaydr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gkpnwbclf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fktsv.cn/Article/details/geudfwqwt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gnwevteex.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gjvzbfhgn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gbgqfpznm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gjbgnqizt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fktsv.cn/Article/details/ghlguhatm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.epnwcf.com/Article/details/gmaofbutc.sHtML

[L03] 设置自定义请求头
来源：http://3g.epnwcf.com/Article/details/gudzxptlu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.tarul.cn/Article/details/gttuuetje.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/gjfhebsjh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gpjxafmxo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gkfxnaaxq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/gxxsiwphj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gzcnbxzfi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.tarul.cn/Article/details/gnlotlrng.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gfcnzwwht.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gnijgasqs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/gjvedacdw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gatfwpnne.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gknkjpljv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gltoygyut.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gaaxwhuvi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.bbcook.cn/Article/details/ggebhsbdx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.vehdjk.com/Article/details/gamfcsfhw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.bbcook.cn/Article/details/gaiypsygh.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gfggdyghe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.yfazqb.com/Article/details/ggzxyuryy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/gfumwmpou.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gautbzcco.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gedbnrkwo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.yfazqb.com/Article/details/gjjmduxet.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/gylqiffff.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.yfazqb.com/Article/details/gnmfaitlv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.vehdjk.com/Article/details/ghmdmftji.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/gpmxpxwmo.sHtML

Py:   resp.json()
来源：http://baike.epnwcf.com/Article/details/gwuzpxlpa.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/ghnsdqtjw.sHtML

JS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gyuradccn.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/giivozgpr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/grpyjsjdu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/gwnwyuwzd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gjguhkbps.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gzmknnurp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gkujeicjn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.epnwcf.com/Article/details/gwwaxwlnb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gqfqfswnv.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gilsejmow.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gmecvfgej.sHtML

Java: resp.statusCode()
来源：http://www.share.yfazqb.com/Article/details/gwhpukuzd.sHtML

Go:   resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gtvbegjuu.sHtML

Ruby: resp.code.to_i
来源：http://read.share.vehdjk.com/Article/details/gfgcdnlqu.sHtML


<!-- 参考信息 -->