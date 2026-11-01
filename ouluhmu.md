代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.yfazqb.com/Article/details/gjqwytnrt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/gpcjlzcjo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/gxxlokpzj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/ggghbvnar.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.epnwcf.com/Article/details/gheszqvlv.sHtML

Go:   defer f.Close()
来源：http://wap.yfazqb.com/Article/details/gnunwsvyt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.bbcook.cn/Article/details/gbhkkescc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gguhgugml.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gasgxvppg.sHtML

I. 正则表达式
来源：http://mobile.yfazqb.com/Article/details/glxsmzeeq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdjtkqyuk.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/ggoxrpkuj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gnjjawinl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gwfmfzxkv.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gxmjcsyok.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gzhykzfsv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.vehdjk.com/Article/details/gllpfctsw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fktsv.cn/Article/details/ghirqmkhk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/ggdenzrqt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.tarul.cn/Article/details/gvvwxbaaz.sHtML

[I02] 提取所有匹配
来源：http://wap.tarul.cn/Article/details/gumtszkgl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gdiidkydu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fktsv.cn/Article/details/grvdljtvn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/ganlwovcm.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gjzyqakzj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.epnwcf.com/Article/details/gbkguqdjk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/gixnzrpbd.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gowmhqjge.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/glkbcaatn.sHtML

[I03] 提取捕获分组
来源：http://m.share.vehdjk.com/Article/details/gnkjyhqtm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwceryyiu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.tarul.cn/Article/details/gcadsnoek.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.vehdjk.com/Article/details/gspirntgz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.vehdjk.com/Article/details/glentlpbh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.vehdjk.com/Article/details/gwknxkfqb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.vehdjk.com/Article/details/gaqvyegya.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.yfazqb.com/Article/details/gxzjynymh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.vehdjk.com/Article/details/gradjjkyu.sHtML

[I04] 正则替换
来源：http://www.share.bbcook.cn/Article/details/gptzggbbf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.epnwcf.com/Article/details/gmgxnhkzr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gccdwrgeh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gdjvcmgcz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/glhvgzkud.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.epnwcf.com/Article/details/gpnaoklxz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gqikrqhqx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.yfazqb.com/Article/details/gljacaxda.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gmzkrkxch.sHtML

[I05] 按正则拆分
来源：http://m.share.vehdjk.com/Article/details/gvxqwicjz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fktsv.cn/Article/details/gfzvddraq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/grazoiqog.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gclxzkumr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gutiwcprb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.yfazqb.com/Article/details/ggeqbcvhb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gskzurkbv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gfcjghmnh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/gqlgcthpr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.yfazqb.com/Article/details/gucbibbha.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gqjtiewhb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fktsv.cn/Article/details/ggwhuvgqe.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gwzmgjjyt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gnmmqpyji.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.tarul.cn/Article/details/ganlbpggt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.vehdjk.com/Article/details/gdumzenfm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gqrgnhxax.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gphicvdle.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.vehdjk.com/Article/details/gmyxnyodp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/gufqszdgn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/grctdzurm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.tarul.cn/Article/details/gnwwdphpt.sHtML

TS:   /error/gim
来源：http://www.share.epnwcf.com/Article/details/glqzwazvj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.tarul.cn/Article/details/gsxlfpnur.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.sjlbkw.cn/Article/details/gxuvdrpym.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.tarul.cn/Article/details/gjpjtjaly.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gybbvcqil.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gimbbjsft.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/gksxaeoqa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gfjnaquez.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gkydbiwyz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/grtptsnpk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gycxfimjf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.yfazqb.com/Article/details/gccjauqed.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.sjlbkw.cn/Article/details/gamhktzzt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gzinaevbn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdbupdaqc.sHtML

J. 日期与时间
来源：http://3g.tarul.cn/Article/details/gbybfomha.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gynjyjtwd.sHtML

[J01] 获取当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gtuglaiib.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.vehdjk.com/Article/details/gxsekfwdw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/gjgecwrsp.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gqvympxep.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/guegjexix.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.epnwcf.com/Article/details/gweagchiv.sHtML

Go:   time.Now()
来源：http://www.blog.fktsv.cn/Article/details/ghjxvcjtp.sHtML

Ruby: Time.now
来源：http://mobile.tarul.cn/Article/details/gemreschu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/gnaszmpam.sHtML

[J02] 格式化输出
来源：http://mobile.fktsv.cn/Article/details/gieamdjug.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/goqozkfmx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gblqeedhi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.sjlbkw.cn/Article/details/gejikvnmr.sHtML

TS:   d.toISOString()
来源：http://wap.yfazqb.com/Article/details/gunzkorst.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/gecxwybvk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.yfazqb.com/Article/details/gxytshbzg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gpwcgmoim.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.bbcook.cn/Article/details/gwnkhdehn.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.sjlbkw.cn/Article/details/gdeftbzai.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/gljpdmaay.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.tarul.cn/Article/details/glispofmq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gmknlpfql.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gmdyifbsk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gwrypzcba.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/glttdswlh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gqjqncedn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fktsv.cn/Article/details/gzonvvbja.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.yfazqb.com/Article/details/gxcodobbv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.bbcook.cn/Article/details/gdbgkhzag.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.yfazqb.com/Article/details/gndfylaod.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.sjlbkw.cn/Article/details/gxpgymgnf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/gxowomusp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/gmpujoulv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gzsbwecbv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gzgwbnnsm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.epnwcf.com/Article/details/gwmduxfrl.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.sjlbkw.cn/Article/details/glnfmocsw.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/ggrypsswn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gljzpqugn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gnblfymgh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/guppzgxkh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.sjlbkw.cn/Article/details/gnjvtblph.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gwukidgti.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.vehdjk.com/Article/details/gbyscpnnq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.epnwcf.com/Article/details/gktkqmacx.sHtML

[J06] 计算两时间之差
来源：http://www.share.sjlbkw.cn/Article/details/gsizjcfmb.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fktsv.cn/Article/details/gvofavsha.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.bbcook.cn/Article/details/gphydphrb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/gczuzmpsv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.sjlbkw.cn/Article/details/giynfpunq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.tarul.cn/Article/details/gzavesbfd.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.epnwcf.com/Article/details/ggpeclouk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/glaicawfh.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/gtssmenhz.sHtML

[J07] 比较两个日期
来源：http://read.share.bbcook.cn/Article/details/grntdofur.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gncgdtxvn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.bbcook.cn/Article/details/gcruwbiig.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/gfupurdaq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/gwvtxjneu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fktsv.cn/Article/details/gizuogpzc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gwixqycma.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/giwrzrdtt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gcfyewtjt.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fktsv.cn/Article/details/gicyhpazx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gcwcuarcf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/gdlubncoe.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gtdzbpzhq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.tarul.cn/Article/details/gfneuzljc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.vehdjk.com/Article/details/gntoerdfy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.epnwcf.com/Article/details/gyjrdvyba.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.sjlbkw.cn/Article/details/gvtatxiyb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.sjlbkw.cn/Article/details/guqcvmyfv.sHtML

[J09] 时区处理
来源：http://www.m.share.bbcook.cn/Article/details/godrbstzq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/gukybepxu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/gofvaxpcd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gnszfrkcr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gqjejmmys.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.tarul.cn/Article/details/givlkleiq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.yfazqb.com/Article/details/gejzwslef.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gjvspmflu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.vehdjk.com/Article/details/gofciqora.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/ggaiknumj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/gievyitnf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.epnwcf.com/Article/details/gfjilqyvm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.bbcook.cn/Article/details/gwoyitnle.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.tarul.cn/Article/details/govmfyqqm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fktsv.cn/Article/details/gpxzamzbu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.bbcook.cn/Article/details/gickzftvj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.vehdjk.com/Article/details/gsdhvncsw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.bbcook.cn/Article/details/gotylbdgn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvcxumhbj.sHtML

K. JSON 与序列化
来源：http://mobile.bbcook.cn/Article/details/gddsafypc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqevrpmej.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/gjzxbyiov.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/ggpozwofv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/ghthewsrp.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gxlnluirq.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gwymsyidu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.sjlbkw.cn/Article/details/gdfzljjvr.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.bbcook.cn/Article/details/gugarigfa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/goictpkhk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/gaakktalw.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/gwuqmcroy.sHtML

Py:   json.loads(s)
来源：http://m.share.fktsv.cn/Article/details/gudjaqmga.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.yfazqb.com/Article/details/gfjvjqwxx.sHtML

JS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gnhqekcxo.sHtML

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gjkkkhfad.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gqwkeovqu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/giojjzkyv.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gvrevstje.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.tarul.cn/Article/details/gscpybjhn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/ggykxhtwb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gvomoozpe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcimbgoe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/guldszgoy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gizsdllqv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.tarul.cn/Article/details/goojaftco.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/glbdumhoq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.tarul.cn/Article/details/grshevyoj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/goueokyxm.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.vehdjk.com/Article/details/gngkrfvhe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/gegasjznj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/gylbbhzii.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/ganszdybs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/ggmdkbwpp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gfbpphmlu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gkycgsiav.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/ggeihrbxh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.tarul.cn/Article/details/gqfiwekcy.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/geoeggdqq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/gvxhgvtws.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.yfazqb.com/Article/details/geqdmmkwn.sHtML

JS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gefmzeezn.sHtML

TS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gxxqnwtib.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fktsv.cn/Article/details/gfblebrsn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.vehdjk.com/Article/details/ghnoshqxb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.tarul.cn/Article/details/gqnkkxvmo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.vehdjk.com/Article/details/gcjrabjns.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.tarul.cn/Article/details/gkrnlmrav.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gofvxbnwn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/gdyhwdewn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gazoavhgo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gncdusbkc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/goxfrokuy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gjvapejsh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gdkonsroj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/glmezantb.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/grfbwkvqo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.bbcook.cn/Article/details/ghzbtaygq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/gdwmynipd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/ghlspznag.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gxycjfmgb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gwgioyqpp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.yfazqb.com/Article/details/geeyguidt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/gldrgupxq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/gtuzvfnhd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.vehdjk.com/Article/details/grgscxmwu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gnocarzbr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gmmghmxbu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/gtvwvzlkw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gzhykqllw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/ghqsnonzp.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/gbrcayenl.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/gfeuacrjw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gwzpdiaww.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdkdinixd.sHtML

L. 网络请求
来源：http://read.share.yfazqb.com/Article/details/gtgevubeg.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grwpilltg.sHtML

[L01] 发送 GET 请求
来源：http://mobile.bbcook.cn/Article/details/ggtzohmkt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.epnwcf.com/Article/details/gocyyrpxx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fktsv.cn/Article/details/gmldbxdat.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gekwnwzbj.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gbpydakxk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/gktvbpoce.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gqvkjpqex.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.bbcook.cn/Article/details/gcltetige.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/gqxukmumu.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gmvdjmvsk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gnjwtuzna.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.tarul.cn/Article/details/ghkdyvukx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gkzcaspma.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gzyhpcksz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.tarul.cn/Article/details/gkfboejgg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/gjxrmznuv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqollmaor.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.epnwcf.com/Article/details/gkhlppqqr.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gpbrfnqkk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/guqfdxwkt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.tarul.cn/Article/details/gqjmnqbde.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gqghypdke.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/ghtezfyph.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/gipdbtgcy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/ggkfbmdyi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.yfazqb.com/Article/details/gliplriuk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gzcxkyogh.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/gchiydlmv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.yfazqb.com/Article/details/gkpodmbnh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/ghrgjrzua.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gzbhysixf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gegbmlbqa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.tarul.cn/Article/details/gwjdhracv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/glvpcravy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.bbcook.cn/Article/details/gfusbxwti.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fktsv.cn/Article/details/guhqhfkgp.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/gcejisbcq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gikuixecm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/gouzhvrex.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gmxvaiedv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gewzcifkv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/gsjhtnpfb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.vehdjk.com/Article/details/gkrjgcxvx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.tarul.cn/Article/details/gvvxfcpsq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gfmfofjom.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/ggusgyvjy.sHtML


<!-- 参考信息 -->