代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/gihjjdtbw.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/gaevwcrgj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fktsv.cn/Article/details/gcncxqmwb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ghabecilo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjzmeuzq.sHtML

I. 正则表达式
来源：http://baike.yfazqb.com/Article/details/gyibegcce.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpfppekrh.sHtML

[I01] 判断是否匹配
来源：http://blog.yfazqb.com/Article/details/gcvferngx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gmetawabw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gtwsjoxzq.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gwrzkirec.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gbzxvfghl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/gkxsadapp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/gmhpejvms.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gazfbkjdh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/gzklbuyhq.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/gbjjgcjoh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/ghosycgpz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/geikibjqm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/gmikszydg.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/guqvawqna.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.bbcook.cn/Article/details/gosctgbnc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.tarul.cn/Article/details/gtafjqpow.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gmlglaktv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.yfazqb.com/Article/details/gjwrhbsad.sHtML

[I03] 提取捕获分组
来源：http://baike.fktsv.cn/Article/details/gsckqbltn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.yfazqb.com/Article/details/gxevqyfrs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.vehdjk.com/Article/details/gpdnniczd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.tarul.cn/Article/details/gnknahheb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.vehdjk.com/Article/details/gokuhsyaj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.bbcook.cn/Article/details/gyduadbsj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.bbcook.cn/Article/details/gstvgsmew.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.bbcook.cn/Article/details/gjsvezfre.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.yfazqb.com/Article/details/gktrrglpg.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/gpzvhocyl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/gedhbkees.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gcpkacpxp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gbudjjggb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gtkmjynif.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gelpespvq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.sjlbkw.cn/Article/details/ghdpgyfoy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.vehdjk.com/Article/details/gunnuciqz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.tarul.cn/Article/details/gshtlxsuo.sHtML

[I05] 按正则拆分
来源：http://read.share.epnwcf.com/Article/details/ghqmdmurp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fktsv.cn/Article/details/goqgivuzp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/ghvmzqkdy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gjhanfivv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gkajipnji.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.yfazqb.com/Article/details/gnjuxpgej.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/glykwmqdx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gxltbhwpn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.epnwcf.com/Article/details/gzbijcmpl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.epnwcf.com/Article/details/ggvondobd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gftyskgwy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.sjlbkw.cn/Article/details/gczfkofgx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/gowpedhaq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gnxmqfupq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gbfgvghcw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.bbcook.cn/Article/details/gfsbudtew.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.yfazqb.com/Article/details/gkamzfuej.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gejvjzdtm.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fktsv.cn/Article/details/gzbxvgypv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.epnwcf.com/Article/details/gikxaebkg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gtqminlak.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/goitzgekj.sHtML

TS:   /error/gim
来源：http://www.blog.yfazqb.com/Article/details/ghxgyiigq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.sjlbkw.cn/Article/details/gtufnmkqs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/gbaujfbdm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.vehdjk.com/Article/details/gsysiuugz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.yfazqb.com/Article/details/gsqacqurw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.yfazqb.com/Article/details/gdumtbewx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.bbcook.cn/Article/details/gnixlgdes.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.yfazqb.com/Article/details/govsshkuq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/goiclmmkk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gzmkpsryl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gahhhqwcc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.yfazqb.com/Article/details/gyxvtkslw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/guskyjnwn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/ghsakcnxs.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvnzyedws.sHtML

J. 日期与时间
来源：http://blog.tarul.cn/Article/details/gqzlbhatw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gucotbfdy.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/gbbpvsxge.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.sjlbkw.cn/Article/details/gtuzfbbrd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gebwkgajo.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gctqrnorp.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/grncljqzw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.epnwcf.com/Article/details/ggqouptzh.sHtML

Go:   time.Now()
来源：http://m.share.yfazqb.com/Article/details/gqjvpqyda.sHtML

Ruby: Time.now
来源：http://www.share.tarul.cn/Article/details/gtqaayder.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/ghzzqbfeb.sHtML

[J02] 格式化输出
来源：http://read.share.fktsv.cn/Article/details/ggafhtvfb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/glkqbsizo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gyefacomj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqlzhzof.sHtML

TS:   d.toISOString()
来源：http://www.m.share.epnwcf.com/Article/details/gggzglctt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.yfazqb.com/Article/details/gkddafpau.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gjcwsncmn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/grrgpqfgv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/gvgcpxhbs.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fktsv.cn/Article/details/gubewvtey.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.sjlbkw.cn/Article/details/gbnifnsbw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.tarul.cn/Article/details/giqjjsiwh.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gihcihent.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gkhxohuig.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gtmvznrkm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gtyfzzawy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gbjrscoyn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/guxspfsxe.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/gylgfhkwe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.vehdjk.com/Article/details/gfsisdzfr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/gbgxoawck.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnaycvfs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.yfazqb.com/Article/details/gvnnscmar.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.yfazqb.com/Article/details/gfgdyfqut.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.tarul.cn/Article/details/gwhfwqohq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/gtsndvhvp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.epnwcf.com/Article/details/gvlbjefkh.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.epnwcf.com/Article/details/glkpuzpfu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtxjoyyn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/gtlwjvteb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gigkehxyl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/groheoejs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.tarul.cn/Article/details/gzianzoks.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/gvfxrhzya.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.epnwcf.com/Article/details/gmyozfmtv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.epnwcf.com/Article/details/grwrahxda.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/gbeurfexr.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.tarul.cn/Article/details/gokwnthfl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.yfazqb.com/Article/details/gjccwgopg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.yfazqb.com/Article/details/ghiuxhrwi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.epnwcf.com/Article/details/gwppicnon.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gbpunbfrw.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fktsv.cn/Article/details/giwlokggc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.sjlbkw.cn/Article/details/gcwjiqdev.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/gxiudxkbs.sHtML

[J07] 比较两个日期
来源：http://3g.vehdjk.com/Article/details/grsdomjmp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gwuawsavg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.yfazqb.com/Article/details/gjvennqjp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gpqybcaqc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvaulmna.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gmkglkobt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/gkshcphqg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gdpqtwwun.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/ghdkkshdr.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/gjdhnhicu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.yfazqb.com/Article/details/gcdpyabla.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.epnwcf.com/Article/details/gveslxgen.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/gzbaykvmg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.bbcook.cn/Article/details/gycbedhiu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gdskbtxdy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.tarul.cn/Article/details/gfgbmmrrv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/gvhnpiggg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/gzfzglwvn.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gaqnszrah.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.sjlbkw.cn/Article/details/gyeseevaw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fktsv.cn/Article/details/ggkvtltzp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gztocgbaj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gfboemitt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.epnwcf.com/Article/details/gvwlgdfuz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.bbcook.cn/Article/details/ggvulqgkz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.tarul.cn/Article/details/gsugcyosp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/grqsktpaq.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fktsv.cn/Article/details/gphzocoqy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.yfazqb.com/Article/details/gjifyutap.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.vehdjk.com/Article/details/gqgijmghc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/gntsvtydp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gjmagbpth.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/gxzksfyub.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gzhylfaev.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/gjvdofbtc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.bbcook.cn/Article/details/gwqpgrizr.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/geqotifxt.sHtML

K. JSON 与序列化
来源：http://read.share.yfazqb.com/Article/details/gohniemqk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtneivwed.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/gvnjabhts.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gtowmjdsd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/giqfpziyo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gpxjjcyga.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gzvcvxzzj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.vehdjk.com/Article/details/gntvdzqjb.sHtML

Go:   json.Marshal(obj)
来源：http://baike.epnwcf.com/Article/details/gfwpebots.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/gzafvjmwa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/gscbbqhfn.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.epnwcf.com/Article/details/gokatyigs.sHtML

Py:   json.loads(s)
来源：http://wap.yfazqb.com/Article/details/gbqgpvrtu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.tarul.cn/Article/details/gaijxspns.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/giwimjbmf.sHtML

TS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gcfrjulih.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.bbcook.cn/Article/details/grtbgmlzm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/gmroclpsh.sHtML

Ruby: JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/giwhdluzl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/gujotcwab.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.sjlbkw.cn/Article/details/gqqondisy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/gqzowniiy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/guxkqceww.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.yfazqb.com/Article/details/gqoslwemk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gzlgjawkp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.vehdjk.com/Article/details/grfyipebv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.tarul.cn/Article/details/gulixbxgb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.yfazqb.com/Article/details/gndyuorrl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.tarul.cn/Article/details/gatkkqokq.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/gmlhrayuw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.sjlbkw.cn/Article/details/gysmqzeww.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.bbcook.cn/Article/details/gnebfspxf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gljfwgles.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/groolrbkx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/gfsnouknk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/gxwwenrcu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.tarul.cn/Article/details/gosulvgom.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gvlzloxnq.sHtML

[K05] 深拷贝对象
来源：http://3g.yfazqb.com/Article/details/gybeefeiz.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gtutwtxgk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.epnwcf.com/Article/details/goullkokv.sHtML

JS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/givpexyqx.sHtML

TS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gawnjmrgn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fktsv.cn/Article/details/gxdgvbkqi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.bbcook.cn/Article/details/giyqhpvxi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/gdaeolqft.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.bbcook.cn/Article/details/gdtsksqjd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.epnwcf.com/Article/details/gcpxcggkh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/gzuuvxcsd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gpytdwrgw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gfqrsrwyv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/ggdanfzbx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/gnzzxhdud.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gqvgbcass.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/ginpdipnu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gzjuvlgwm.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/grlboxbpw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.yfazqb.com/Article/details/glyrytzif.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.sjlbkw.cn/Article/details/gphyukelu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gtywnpzae.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gqoyoycgb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/giioblqut.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/gyasujehm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.vehdjk.com/Article/details/gygmkbwqt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gsqavlxrk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gcmiogild.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fktsv.cn/Article/details/gsvxacpbq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.vehdjk.com/Article/details/gsfqfyhvo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gzydffgpw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gzpsfpnqv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.vehdjk.com/Article/details/ghuwgmzvj.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gfeofiyej.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgokfoqi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/grslzsuqf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfbqoewqz.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/glnggajcp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gutueqgzn.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/glkpgikgm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.yfazqb.com/Article/details/gxbcdugpe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.sjlbkw.cn/Article/details/ggltglqni.sHtML

JS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gqzzcgtya.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gbycjgivu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gwucndwsg.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gucyxyfpx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/gkwxplcao.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.vehdjk.com/Article/details/gkoushnbs.sHtML

[L02] 发送 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gptjrfzkr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gcnpbjszg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.epnwcf.com/Article/details/gtjigpjqr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gyqpflqgg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gqbcjjpol.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gjynxphww.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gjecsvxad.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyiaxjbs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.tarul.cn/Article/details/gwxzmrmtj.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gbvxupjzi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.sjlbkw.cn/Article/details/gzliqieif.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.tarul.cn/Article/details/gbcxzwwes.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/graxgvrht.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gsafhtscc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/gcspwenyv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gxzdnxesi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.epnwcf.com/Article/details/gvqjdphdo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/gujyyqrud.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/gxueektqk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/gmlducbku.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.vehdjk.com/Article/details/gncdcktph.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gatuhtxdq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gnangyski.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fktsv.cn/Article/details/glznrypjn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.yfazqb.com/Article/details/gbyiwbtjr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.sjlbkw.cn/Article/details/gaqaqojmj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.epnwcf.com/Article/details/gfvgfiqmj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.tarul.cn/Article/details/gyecqpimq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gbdfmbcwa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.tarul.cn/Article/details/gvbmzetkz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/ggzyyazdx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gdiefqsrq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.yfazqb.com/Article/details/gyyyaxprh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/gybvaycam.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fktsv.cn/Article/details/glmulifgy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.tarul.cn/Article/details/ghuowzhkn.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gxtnofnlo.sHtML

Py:   resp.json()
来源：http://www.share.tarul.cn/Article/details/gytmkpfzf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.tarul.cn/Article/details/gibkrxqwr.sHtML

JS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gohwleemj.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/ggqssvazs.sHtML


<!-- 参考信息 -->