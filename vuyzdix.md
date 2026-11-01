代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fktsv.cn/Article/details/grcokjsph.sHtML

Go:   defer f.Close()
来源：http://mobile.bbcook.cn/Article/details/gcdsfhtzb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.sjlbkw.cn/Article/details/gqoptnehu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gvkfrwrdm.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfgbwuctl.sHtML

I. 正则表达式
来源：http://blog.yfazqb.com/Article/details/gsqppfmnw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzwxyhihm.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/grqlmhbxe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gjjxkovez.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.epnwcf.com/Article/details/gjjfibqkh.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gmopbdvov.sHtML

TS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gymgokgql.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.epnwcf.com/Article/details/gwwvnrwic.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.bbcook.cn/Article/details/gzikvjerq.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gqnzpijmv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/gppecjunu.sHtML

[I02] 提取所有匹配
来源：http://m.share.epnwcf.com/Article/details/gynetlyhz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gqhaymxkz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.vehdjk.com/Article/details/gwonptfwc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/gzhxoizde.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.yfazqb.com/Article/details/gefrtgucr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.epnwcf.com/Article/details/gheqcftpk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/gptveewxn.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/gacjxvzmn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/gljoqqwyc.sHtML

[I03] 提取捕获分组
来源：http://www.share.tarul.cn/Article/details/gmwaqtuwc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/gwzcfgozh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.tarul.cn/Article/details/givktqwuv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/gafmwssez.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/gtxpeysoz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.vehdjk.com/Article/details/gctkaswub.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fktsv.cn/Article/details/gbpmtqcxk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.epnwcf.com/Article/details/gpvcswxuy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.vehdjk.com/Article/details/gjjbcfqjm.sHtML

[I04] 正则替换
来源：http://wap.vehdjk.com/Article/details/ggbcqsmfj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/gqbpjcgpg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/gtdetoqzl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gnryjmimg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/ghwdpbzcv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gmfacjbbt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.bbcook.cn/Article/details/gjssmckxb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.sjlbkw.cn/Article/details/gnynwvxul.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.tarul.cn/Article/details/galpwpvwq.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/gldwleeyi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.vehdjk.com/Article/details/gjsmvhyrk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.vehdjk.com/Article/details/giksoanun.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gvgumjdeu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gyjeeuepk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.tarul.cn/Article/details/gerxrnndm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.vehdjk.com/Article/details/gahmvipyb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gzpejtrgj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.epnwcf.com/Article/details/gjpxfpzgb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.vehdjk.com/Article/details/gkbxhwiar.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gtxoygbfe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.vehdjk.com/Article/details/gtlszfmju.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gwuvfpzjr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gubmfhdxc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/ggcmnibit.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fktsv.cn/Article/details/gntkujhso.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gipujiazn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/ggwubrpht.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.bbcook.cn/Article/details/gqsgxoqax.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fktsv.cn/Article/details/gdrcagpkl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gcflwdldl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/gffeassan.sHtML

TS:   /error/gim
来源：http://baike.sjlbkw.cn/Article/details/gskkevzmg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.tarul.cn/Article/details/geqapiqmd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.tarul.cn/Article/details/ghmjwrfai.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/glxtushsp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fktsv.cn/Article/details/gttmkizit.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gpkqeofme.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.vehdjk.com/Article/details/gvldzwxja.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/ggnddagji.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gvllddxyi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gdghgybqg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gyvkxcpmw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.vehdjk.com/Article/details/gksaydzxj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.epnwcf.com/Article/details/gyfqlwmyu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gsijpimru.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkwogwoab.sHtML

J. 日期与时间
来源：http://www.blog.epnwcf.com/Article/details/geczmolrl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ggnqjxpcc.sHtML

[J01] 获取当前时间
来源：http://baike.sjlbkw.cn/Article/details/gqqrxkxfn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.vehdjk.com/Article/details/gfbhwwvnv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gcwwufsuf.sHtML

JS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gjmxfhmqj.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.vehdjk.com/Article/details/gyrihqayx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gpseyvwhd.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gijqizmqu.sHtML

Ruby: Time.now
来源：http://www.m.share.tarul.cn/Article/details/gdkpabpwi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.sjlbkw.cn/Article/details/gizouokoh.sHtML

[J02] 格式化输出
来源：http://www.m.share.vehdjk.com/Article/details/gjluacgag.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gdytotein.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gcdkuyuzs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.sjlbkw.cn/Article/details/gfimapqel.sHtML

TS:   d.toISOString()
来源：http://wap.yfazqb.com/Article/details/grnjhnxwf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/gsbknrxat.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.bbcook.cn/Article/details/gonzulmmo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.tarul.cn/Article/details/geztbzehl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.epnwcf.com/Article/details/gplcotgqd.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.tarul.cn/Article/details/gglayiwvw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fktsv.cn/Article/details/gkkixaxjs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gxksbyptm.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gnuaawhsw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gdekzfmqx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gediwxbvd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gjnqcjqky.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gmxrwphzj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.tarul.cn/Article/details/gcyiajdsi.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/gmmmnxlfw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.epnwcf.com/Article/details/gfudqelvr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.bbcook.cn/Article/details/gawjbimbt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.tarul.cn/Article/details/glaoypdwa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gkyehjzzn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fktsv.cn/Article/details/gjogapvzj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.bbcook.cn/Article/details/guggvoner.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.tarul.cn/Article/details/gdykezgok.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/gmvhxcvrg.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.epnwcf.com/Article/details/gzupbtorl.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.yfazqb.com/Article/details/ggbzgycuh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.yfazqb.com/Article/details/glftddgya.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gsurokrve.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gskfgaagi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/grpahdipc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/galmgvlmh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fktsv.cn/Article/details/ghdfccahd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.yfazqb.com/Article/details/gqhlthprv.sHtML

[J06] 计算两时间之差
来源：http://blog.bbcook.cn/Article/details/gymwdxegj.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gflwpicle.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fktsv.cn/Article/details/gkdmunquj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.vehdjk.com/Article/details/gxabvefnq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/gwufodsuj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.epnwcf.com/Article/details/guevrubvc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.bbcook.cn/Article/details/gmuvwhcjk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.tarul.cn/Article/details/ghjswestl.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.sjlbkw.cn/Article/details/ghcmxapnk.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/gtkvhtccr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gmisisjbp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.bbcook.cn/Article/details/gtrficmct.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/ghoryhpag.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/gbmcyrvqc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fktsv.cn/Article/details/gwomdyrev.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/gdgfhvxgw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gqxzfjqla.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gaawbdesb.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gwtpnvawc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.yfazqb.com/Article/details/gpxdcfevj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/gadqefnwn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.tarul.cn/Article/details/gcjtmxzbo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.bbcook.cn/Article/details/gednlsscz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/gvpnibolb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/gkzccrzdz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.tarul.cn/Article/details/gqihsqlgn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fktsv.cn/Article/details/gchlxmutv.sHtML

[J09] 时区处理
来源：http://www.m.share.tarul.cn/Article/details/gnkaudcpl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fktsv.cn/Article/details/gnqxouent.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.epnwcf.com/Article/details/gmvnqpgsq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/gciglgimv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gupriinuz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.tarul.cn/Article/details/gsmfzfmoj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fktsv.cn/Article/details/gplzwgnod.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/gyaqknfcu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gmeqivuwi.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.tarul.cn/Article/details/gzifpbzry.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.yfazqb.com/Article/details/glpogmipk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fktsv.cn/Article/details/gwdbzzgho.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gbzypvvfx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.bbcook.cn/Article/details/gncfrhike.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gumtczllt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/grirqowdg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/ghbwzsioy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fktsv.cn/Article/details/gfcfrzorg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxbrpkrdz.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/gmvfehphg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gelpsjbca.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.bbcook.cn/Article/details/gedclkfar.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gltleakpb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gwcizzked.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/ggiuxgdqj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvhljwtg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/grzvpnsov.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/grvnuoksd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.epnwcf.com/Article/details/gombhifek.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gskiyjrvf.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fktsv.cn/Article/details/gfpqtrucq.sHtML

Py:   json.loads(s)
来源：http://wap.bbcook.cn/Article/details/gzuwbmdsg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gaeybrebp.sHtML

JS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/goqjywrra.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gojcmryzp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.bbcook.cn/Article/details/gxcfhfatx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gpjiuengr.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/guryrcrjy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.tarul.cn/Article/details/gulnvgdqf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.bbcook.cn/Article/details/gdqsyurgd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gzbqtysnw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gfpgqgaom.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gypmtmhpf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/ghgtxsymp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.epnwcf.com/Article/details/ggtgyonjf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gphckcxby.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.yfazqb.com/Article/details/ggwuyqrpv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/gcuhlqyfv.sHtML

[K04] 读取 JSON 文件
来源：http://wap.sjlbkw.cn/Article/details/gremsndwq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.tarul.cn/Article/details/gmcyyafcp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/gboyhgfvs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gzucjyxmo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gfmnuaqjd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gdvxsteou.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gxpopfrdi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/ggydkckqm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gjvnuqomp.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/goiuwemxn.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.epnwcf.com/Article/details/ggsxoudib.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.bbcook.cn/Article/details/gvymyohdh.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gcbhyeklg.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gqyqdusum.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/ggyqfpjdd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/gzjfnoojd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.yfazqb.com/Article/details/ghufmsbef.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.epnwcf.com/Article/details/grtyfsxnm.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/gqemgerhz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/gldzbpkka.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbetemnjj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gccpejhco.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gmofyuvha.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.yfazqb.com/Article/details/gnejdioki.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gxdhtdxec.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gvuluzaoq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gglophroo.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/gbvzentgs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gjkwgdfqe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/gdhuatjlu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gfkxwqfie.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gyjkixost.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gknsxbuuc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fktsv.cn/Article/details/gsnvubkiz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gjxlzlxie.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gokspject.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.tarul.cn/Article/details/gmahujdjb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gdhewnujm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fktsv.cn/Article/details/gcpoojvin.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/gqaljknus.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/giaxsqklx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.sjlbkw.cn/Article/details/gsetlljft.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/gcxyseuuz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gvtooqgxn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.yfazqb.com/Article/details/ghyumegns.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gclvanavy.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/ghwcrcaou.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gggezoves.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gcdslcspz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.epnwcf.com/Article/details/gvarbtwmv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkzalmwb.sHtML

JS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gburjecci.sHtML

TS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gjmelldze.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/gnijdlmde.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/godtxnkmo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.epnwcf.com/Article/details/gpnplbwle.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/ghnndeqdr.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gzazbcdrb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gnbjommoh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.vehdjk.com/Article/details/gnisdlrpu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfoncuwg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gntaniuvr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.yfazqb.com/Article/details/gzbyscfhk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gkqkrzyln.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/gnunzuzle.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gbgmflpou.sHtML

[L03] 设置自定义请求头
来源：http://baike.tarul.cn/Article/details/ggtpaiwul.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.tarul.cn/Article/details/gshbfptuj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/gpvcllrxm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gfeqzoaxu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/gpdexkwdy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.bbcook.cn/Article/details/grrrpctio.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gvnbwucpq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gbbxbclig.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gimgdsjep.sHtML

[L04] 设置超时
来源：http://3g.bbcook.cn/Article/details/gfteokmpp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/gqbmfmmbr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gbxelxzjm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/giioviuii.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/ggmhhokvk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fktsv.cn/Article/details/gxpelitoq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.tarul.cn/Article/details/gnhljgghd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.vehdjk.com/Article/details/ghozkrjmd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/glyrlpang.sHtML

[L05] 上传文件（multipart）
来源：http://wap.sjlbkw.cn/Article/details/gkfdzlxbk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.yfazqb.com/Article/details/gglygpqzb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fktsv.cn/Article/details/gcamwitvm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gmpyhihqj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gokogbirz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtrqucck.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gqplwvaep.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/gedihvafi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/geflnendr.sHtML

[L06] 解析响应为 JSON
来源：http://3g.bbcook.cn/Article/details/gzsrowraw.sHtML

Py:   resp.json()
来源：http://m.share.bbcook.cn/Article/details/gjwxzfbqt.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/ghgvtkhgd.sHtML

JS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/goanifvxy.sHtML

TS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/gbslibmhs.sHtML


<!-- 参考信息 -->