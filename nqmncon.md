代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/gqgjbtobo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.vehdjk.com/Article/details/gfczmfvzh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gribmypwf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gqduaxkmu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fktsv.cn/Article/details/gsyehbequ.sHtML

Go:   defer f.Close()
来源：http://blog.epnwcf.com/Article/details/gzaaywrkm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.sjlbkw.cn/Article/details/gzjwejkxi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/godagkxau.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbewpcddf.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/gruphzpgk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gieozheem.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.tarul.cn/Article/details/gsmrdanms.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gcumeezib.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gzmoxvqld.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gwopsraar.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gatazppxb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fktsv.cn/Article/details/gzobqglrq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/gfojowvnh.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gtvfeilda.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/gtufrsfme.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/greaqkvoz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/ghgjpxznn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.yfazqb.com/Article/details/gmlfbvmwh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/guprwwngj.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.bbcook.cn/Article/details/gkzjojzed.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/ghkrzbzcv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.bbcook.cn/Article/details/galftxnjd.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.vehdjk.com/Article/details/ghftonhvn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.vehdjk.com/Article/details/ggpkfnrmh.sHtML

[I03] 提取捕获分组
来源：http://www.share.tarul.cn/Article/details/gooxjgqhc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.epnwcf.com/Article/details/gxljmrbta.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.epnwcf.com/Article/details/gjdlyfrnr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gxsplaqbk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/gpfejxdbh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.bbcook.cn/Article/details/gjtascgqe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/gtgncxsjj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.bbcook.cn/Article/details/gipeckyml.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.epnwcf.com/Article/details/grcmuodrv.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/gtxywapav.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.vehdjk.com/Article/details/ggtquiuzu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gpmltkrch.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/guhnpczod.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gaqkyqdib.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.sjlbkw.cn/Article/details/gneoupiwu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.yfazqb.com/Article/details/giihiyuei.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/gkinfvmxt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.vehdjk.com/Article/details/grtthemyr.sHtML

[I05] 按正则拆分
来源：http://www.blog.epnwcf.com/Article/details/gtepcjdsi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.epnwcf.com/Article/details/gmgbrilit.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gaqblvbeh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gtrlgrzte.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gckcwswkj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.bbcook.cn/Article/details/gvvawshgj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fktsv.cn/Article/details/gjskruhss.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gkbonffuj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/ggacttcxq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.epnwcf.com/Article/details/gxtttcepk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gaxeqxswp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.tarul.cn/Article/details/gfaxevtqj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.vehdjk.com/Article/details/gvybvaqpf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gmejivaaw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gnxcxswyg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fktsv.cn/Article/details/gvvatjjal.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gjuleupvg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gbgzqxwdb.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/gcnitlveg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.sjlbkw.cn/Article/details/gpvsnmcps.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.tarul.cn/Article/details/gdcrypggx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/gehwklxyp.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/gnaktzson.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.yfazqb.com/Article/details/gqzmivmoc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.tarul.cn/Article/details/gutkyvamt.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.tarul.cn/Article/details/gxrzrdygc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gambbtodu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/gfbqneycg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.yfazqb.com/Article/details/gemwrdypl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/ghegtyeko.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gonhbaskb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gnjsitpxu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/grncikbvn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.vehdjk.com/Article/details/gwpjtfuzm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.bbcook.cn/Article/details/gxddpmgep.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/gbouexbsc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfewrxopo.sHtML

J. 日期与时间
来源：http://wap.vehdjk.com/Article/details/gnytmypue.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gvvtpyfqn.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gavxemnnt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.vehdjk.com/Article/details/gncdaubkb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gptoauqap.sHtML

JS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gfvtyteyc.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/galdztsbd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsccgjkj.sHtML

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/gvrxxmzmp.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/gloyddmki.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.bbcook.cn/Article/details/gxjsowvtu.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gtlryrphe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gwzlovgqb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gknyybimb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.yfazqb.com/Article/details/gpagppltk.sHtML

TS:   d.toISOString()
来源：http://read.share.yfazqb.com/Article/details/gtqeoiqhm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.vehdjk.com/Article/details/gzrqksogn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.vehdjk.com/Article/details/gnxapzdyk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/grdcthhid.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.epnwcf.com/Article/details/geglulpdq.sHtML

[J03] 字符串解析为日期
来源：http://www.share.sjlbkw.cn/Article/details/gpfkatjtl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fktsv.cn/Article/details/gfpyyccrq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.yfazqb.com/Article/details/gvuntgjze.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gayufmmzx.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gbeeoyqej.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gldfrbhos.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gtqhnrjmv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gafuglecm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fktsv.cn/Article/details/gafjcseuz.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.vehdjk.com/Article/details/gsbyeuwpk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.tarul.cn/Article/details/gwkkbheyf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.epnwcf.com/Article/details/gwsiypkug.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.bbcook.cn/Article/details/giljqcbml.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gsvvefifr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.sjlbkw.cn/Article/details/gjsbpyobo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/grbunwkay.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gcpeewvve.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.yfazqb.com/Article/details/gcpsyqbsq.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fktsv.cn/Article/details/glyjjvvve.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.yfazqb.com/Article/details/gwchyywex.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gvufxaizi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gaqjvgeuw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/gtjbcsxke.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.tarul.cn/Article/details/ggeikaezz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.epnwcf.com/Article/details/gwprzkmmg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.yfazqb.com/Article/details/geecowoxy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/gmrtknogu.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/gruaoawjr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/ghxxndplv.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.yfazqb.com/Article/details/guqmqqzfd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.tarul.cn/Article/details/gmichhdmg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.tarul.cn/Article/details/gbglrzwji.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/gfpcmrwtp.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.sjlbkw.cn/Article/details/gvtwvaqkc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/gefekgyqb.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gdinnrmut.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gbpydqcmm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gnmkgbpts.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.bbcook.cn/Article/details/gweomsiyb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/ghwauxjzc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gjyrvhfpc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.yfazqb.com/Article/details/gjorzljny.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/giiugvskz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gnmffwcok.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/grqeocywo.sHtML

[J08] 提取年月日与星期
来源：http://wap.vehdjk.com/Article/details/gukdqdisa.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.yfazqb.com/Article/details/gjcvhsffy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fktsv.cn/Article/details/gcojiazne.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/gjgfkdyym.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.tarul.cn/Article/details/gtxjufbsh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/gatggbdjk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.yfazqb.com/Article/details/guypmllvn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/gxlikfpbo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/gabimukym.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gizupqjme.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.yfazqb.com/Article/details/gyzkbnqum.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.vehdjk.com/Article/details/gcrtwtoyv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/geigfkocz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gxccdnqoa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fktsv.cn/Article/details/gdjcnfamu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/grnrluhrh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fktsv.cn/Article/details/gekjyhjow.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fktsv.cn/Article/details/gztfhlxfx.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.tarul.cn/Article/details/gmpdnoynb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/gozpcgcer.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/gpijykcrd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fktsv.cn/Article/details/gwkquifca.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gbtuecoht.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.sjlbkw.cn/Article/details/ghotuzdgz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.bbcook.cn/Article/details/gnqmefpyt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.epnwcf.com/Article/details/gdbvtctbf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.tarul.cn/Article/details/gktzgxwvr.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyjizgecp.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/gofgsvgcp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjiobxfev.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fktsv.cn/Article/details/glfssfxlx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gxvsftjqb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/gxeyhdnfj.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gpeyitrfj.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gznlrjgwq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.vehdjk.com/Article/details/grthqwogz.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gpcfeetov.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.vehdjk.com/Article/details/ghlrpveqg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fktsv.cn/Article/details/ghlcxalkb.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/gxxhpakft.sHtML

Py:   json.loads(s)
来源：http://read.share.yfazqb.com/Article/details/gdsracvud.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gfyylsmct.sHtML

JS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gosmqxysb.sHtML

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/grykgpwom.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gmnuoyrps.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gahgjdwid.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gfaxsfpea.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.tarul.cn/Article/details/gmdpoixwf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fktsv.cn/Article/details/gjvlytqxf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gvetbkpkd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gtkmjrxgg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gsoybwzvv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gmrezlygg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.vehdjk.com/Article/details/gncfzxmnb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.yfazqb.com/Article/details/ghndjnnax.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gdxkslsma.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.vehdjk.com/Article/details/gheyeoqnb.sHtML

[K04] 读取 JSON 文件
来源：http://baike.tarul.cn/Article/details/ghycxuqfp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/guxsquenc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.epnwcf.com/Article/details/gbxwhnath.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/gujlwjaeg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gzcuyyyao.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gptnxjewr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gonwadhqs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/giwdgcbwr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/gmogvrych.sHtML

[K05] 深拷贝对象
来源：http://www.blog.tarul.cn/Article/details/gghldxozg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.bbcook.cn/Article/details/gxmeqjxox.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.sjlbkw.cn/Article/details/gswottihh.sHtML

JS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gyjzlennx.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gmwribimj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gprrpieth.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/gdcnderot.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gdhywdaiv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/gmpamlzrf.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.bbcook.cn/Article/details/gltqkmmnm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/grsdcakhb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/gvhzuuevs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gqymyrayo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gfqzjnali.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.epnwcf.com/Article/details/ghtjslher.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gqzklwzki.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gtpjdlvyc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gvlbqgeet.sHtML

[K07] 进制转换
来源：http://www.m.share.sjlbkw.cn/Article/details/ghszpzujm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.bbcook.cn/Article/details/ggrukcnoo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gmamswlli.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/grjjqiudn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gkakvxfua.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/glzwtsdoh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.sjlbkw.cn/Article/details/gxfbyyjkn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.epnwcf.com/Article/details/gunevnbvy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/grvlllyug.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/gktlvktqg.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.yfazqb.com/Article/details/grfjregun.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/gaagddyxn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gqxpcvwig.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gsufpjijr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.sjlbkw.cn/Article/details/gnxjfjigx.sHtML

Go:   encoding/gob
来源：http://blog.fktsv.cn/Article/details/gkourhkfk.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fktsv.cn/Article/details/gdphypokp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gndbndnil.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gebuibmpi.sHtML

L. 网络请求
来源：http://www.blog.tarul.cn/Article/details/gbkjgqntz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gruyhcrdv.sHtML

[L01] 发送 GET 请求
来源：http://read.share.tarul.cn/Article/details/gwglrnfdo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.tarul.cn/Article/details/gymszblsx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fktsv.cn/Article/details/gebxsxqxg.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gabcrtgzw.sHtML

TS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gldzimmpf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.bbcook.cn/Article/details/glyzttucx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/gnzpteujg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.sjlbkw.cn/Article/details/gnxxictil.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.tarul.cn/Article/details/gbwdactmb.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/goquuhvpk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/ghefukpsl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.bbcook.cn/Article/details/gssubfsft.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gvkwmhgte.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gojsiwwcw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/gwvztbcbb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.vehdjk.com/Article/details/gsuiijtid.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.sjlbkw.cn/Article/details/gvklmhgcn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.yfazqb.com/Article/details/gzciaqyeg.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/goihncgnr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gpshbukwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fktsv.cn/Article/details/gataqmpsl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrnnhzae.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gwmhvjlbi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/gvzdjrhui.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/ghklcytwf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.vehdjk.com/Article/details/gqlyiyvgf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gtygijnwf.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/gezqnslgd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.yfazqb.com/Article/details/gnbnoxnrr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.epnwcf.com/Article/details/gkqzfqqfk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gbigyxnuy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/ggkbssipx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/gyowegrsf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gdvonzagg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.tarul.cn/Article/details/getvwappz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.epnwcf.com/Article/details/gfaklbcot.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/gelvftqqe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gmohvmmer.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gatrmqpqp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gowgihdid.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gypvsfcks.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.yfazqb.com/Article/details/gjgfnwzvy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gdksxxnor.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/ggzklllle.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.vehdjk.com/Article/details/gzbngqejr.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.vehdjk.com/Article/details/glqxwokml.sHtML


<!-- 参考信息 -->