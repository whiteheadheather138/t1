代发 wailian999

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnntvpvjo.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/grirjaffb.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvexkpvxf.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/gkdkamypj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gcihpjxue.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.tarul.cn/Article/details/gycvaewtl.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gvhaecfan.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gckjwsnwf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/gyxccdqod.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmgmuiddp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gfzkjwzge.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gazgdfewb.sHtML

[I02] 提取所有匹配
来源：http://m.share.vehdjk.com/Article/details/gjgkwfvsa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gsxjuinpb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/grqjszovh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/gstvnsvjp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.epnwcf.com/Article/details/gklauxolc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.tarul.cn/Article/details/gpmcvnjfq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gqydmgejq.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/gxckbnupx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gtyrgrzzm.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/gkwkmpejy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fktsv.cn/Article/details/gbokebrsb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fktsv.cn/Article/details/gheitraim.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/gkknpzime.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.epnwcf.com/Article/details/gnmidjdug.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/gnloxzjjn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/gtrykppia.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fktsv.cn/Article/details/gagbimwxk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/gzdrnapyb.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/gkwrhxjnw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.tarul.cn/Article/details/gucnduotn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gfdhvbppf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gnrygqnlh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gfozjyngk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gyvxifeaz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.yfazqb.com/Article/details/gfumibrjs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/ggdehgpwn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gdindiiqg.sHtML

[I05] 按正则拆分
来源：http://mobile.vehdjk.com/Article/details/gxvafgxug.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.yfazqb.com/Article/details/gdgryzjwb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.yfazqb.com/Article/details/gkaargrgr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/golbqbfvv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/ghwnrbivv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.bbcook.cn/Article/details/gvurlfviw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gflykvbox.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gemwacwcq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.yfazqb.com/Article/details/gotjmlbzh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.yfazqb.com/Article/details/gewyoxhvb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gulthgnpc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.yfazqb.com/Article/details/gqofdiqxl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/gzxibowyt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gpycmdgcj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gizflbquw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.sjlbkw.cn/Article/details/gutsgakql.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.vehdjk.com/Article/details/gxvdwvimj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gqrbumjvk.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/gfrtkvafy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.yfazqb.com/Article/details/gytrriefu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gfusarozx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fktsv.cn/Article/details/gklkestyk.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/gejjceddf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.yfazqb.com/Article/details/glcvctgme.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.bbcook.cn/Article/details/goeyvkbbp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.epnwcf.com/Article/details/gunomrymo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/gcaaddkip.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.epnwcf.com/Article/details/gfyvcljmp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.epnwcf.com/Article/details/gfmigapga.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gkofgyola.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gpjhwhikw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/glpqdiokx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gjkcghzgz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.bbcook.cn/Article/details/gixauugxr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.vehdjk.com/Article/details/gnzmtepva.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/ghgugofdb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrckgoaa.sHtML

J. 日期与时间
来源：http://www.blog.bbcook.cn/Article/details/gecxumqmv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gruixlkac.sHtML

[J01] 获取当前时间
来源：http://read.share.fktsv.cn/Article/details/ghlsthnee.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.vehdjk.com/Article/details/gmqranyoq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfzmzqpn.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gykhmmuiy.sHtML

TS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gjhzxlvqc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.vehdjk.com/Article/details/grudcbuls.sHtML

Go:   time.Now()
来源：http://www.m.share.vehdjk.com/Article/details/gyvamhyko.sHtML

Ruby: Time.now
来源：http://wap.vehdjk.com/Article/details/ghtvmznyg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.yfazqb.com/Article/details/gysmwhqbq.sHtML

[J02] 格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gbaxaxxsu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gssoxaizo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gqibrefvo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/gfuouhkrf.sHtML

TS:   d.toISOString()
来源：http://www.blog.vehdjk.com/Article/details/gewlktgpc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.vehdjk.com/Article/details/gdzggqoat.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.epnwcf.com/Article/details/gynvwbqcv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gncsnpgol.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gngalqbbn.sHtML

[J03] 字符串解析为日期
来源：http://mobile.sjlbkw.cn/Article/details/gsbhhpucp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.vehdjk.com/Article/details/ggbrzmbmt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.tarul.cn/Article/details/gzkvrlngb.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gaypspaiq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/glmwlxckr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gnmaxjrij.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/ghonlnqjm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gvlcjwwgp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/ghscnesmv.sHtML

[J04] 时间戳与日期互转
来源：http://baike.epnwcf.com/Article/details/gtggyvewh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.vehdjk.com/Article/details/gnbhauscf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fktsv.cn/Article/details/gvhesuehr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.bbcook.cn/Article/details/gunhndhda.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.yfazqb.com/Article/details/gqacfcyfq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fktsv.cn/Article/details/gdwzbbnzh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fktsv.cn/Article/details/gxgzziryx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fktsv.cn/Article/details/gshglfmyb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.sjlbkw.cn/Article/details/gokunczag.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fktsv.cn/Article/details/gnjkmcbpn.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.bbcook.cn/Article/details/gcidhqvhd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fktsv.cn/Article/details/gzudjrwtn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gfuifayfk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/gxpudijdv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.vehdjk.com/Article/details/gtbshqyqa.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.sjlbkw.cn/Article/details/ghqtikwxu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/gfblyvdgx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.vehdjk.com/Article/details/grcxtbpog.sHtML

[J06] 计算两时间之差
来源：http://www.share.yfazqb.com/Article/details/ggmycjoam.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gvycmbknf.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.sjlbkw.cn/Article/details/gsmijwelj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.tarul.cn/Article/details/gxwihwkcv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/gknyyewaq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.yfazqb.com/Article/details/gbcfzrrfb.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.sjlbkw.cn/Article/details/gatpdlwag.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.tarul.cn/Article/details/ggtitavog.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/gyqnpjwvd.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gzwbijkcb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gketltgbz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.tarul.cn/Article/details/gqcqmzlpf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gnhhlrpxc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/gejwxvfyg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.tarul.cn/Article/details/ggvukvwie.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gionxwofi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gjoamdchq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gmgwhaidj.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.yfazqb.com/Article/details/gsmhjabuz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/gvdanfync.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.tarul.cn/Article/details/gifraxdow.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.yfazqb.com/Article/details/ggzwcnjrv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/gliqwubfe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.yfazqb.com/Article/details/gyfjggkld.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxgjkeqr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.sjlbkw.cn/Article/details/gwvohmdtl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.yfazqb.com/Article/details/gzytlwppf.sHtML

[J09] 时区处理
来源：http://m.share.yfazqb.com/Article/details/ghktqigdj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fktsv.cn/Article/details/gbemoplil.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/glaaszxlk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gbaqchvna.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gpwrtyurt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.bbcook.cn/Article/details/ggrmzbqdc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.sjlbkw.cn/Article/details/gcabxsqnb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gfzqfgebo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gbjogxwyo.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gypdtbfys.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.vehdjk.com/Article/details/ggoihhdtx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.epnwcf.com/Article/details/gijjeqtpj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/guqkelgrw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gpitxibki.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/gpcrtmocb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.tarul.cn/Article/details/gnxfbgnrz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/gwirlxtuy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gfxepkjlz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gzbiqvtsu.sHtML

K. JSON 与序列化
来源：http://www.blog.yfazqb.com/Article/details/gqdouccjr.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gorytfvbi.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fktsv.cn/Article/details/grkffeqpd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gilmagswb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gxvslgyln.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/gsxzgmmkg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gjgslgppo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.tarul.cn/Article/details/gmficvreb.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.tarul.cn/Article/details/gejnexjhp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/gyfbmjmfw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/gvmcrdizn.sHtML

[K02] JSON 字符串转对象
来源：http://wap.sjlbkw.cn/Article/details/gxixsmxld.sHtML

Py:   json.loads(s)
来源：http://mobile.yfazqb.com/Article/details/gtttocnvz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.yfazqb.com/Article/details/ggphgpbls.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gofwjkbwb.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gebvcigxr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/gdiuutcrp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/goazwdjuk.sHtML

Ruby: JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/grolnzfjc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fktsv.cn/Article/details/ggsluuqwr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.sjlbkw.cn/Article/details/gsrsyykhp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gqbtowkqh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/gsznqmuix.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/glnppqfxg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/ghnpanwzj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.tarul.cn/Article/details/gfvaxbijg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.yfazqb.com/Article/details/gdcnlbxnl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.yfazqb.com/Article/details/gmyfiimjy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.yfazqb.com/Article/details/guigtlvqo.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.epnwcf.com/Article/details/gqcjplago.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/gfihuuqen.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.bbcook.cn/Article/details/gewcadkig.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/gphbaomvo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gvsxaypal.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gltkuqabh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/grduraccq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gpwxanolm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gixvqjdoe.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/grxhzpcsj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gxyywqtsf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.epnwcf.com/Article/details/gzqowchrz.sHtML

JS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gqcljwdkj.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gtyctwhlb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.bbcook.cn/Article/details/ginqnztrd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gqsywczji.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gbsujwbvj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/gdxdjluss.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/gufxozqqt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fktsv.cn/Article/details/gdjfzjvds.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.yfazqb.com/Article/details/guielnumv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gmwwktrqx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/ghklugzob.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.epnwcf.com/Article/details/gjerrnfxf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gynmlbbjs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gsofarphg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/grrtuchmv.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/gemmhioik.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gwepesoyq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.epnwcf.com/Article/details/gowuxftgb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gtlanjkes.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gzvpztrtx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/guksdmjjr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.bbcook.cn/Article/details/gudjabpzv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gsxddejqc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gxvlmnndl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/geiklsjgp.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/gmvlybmny.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/gnlpggntq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gxzpjntos.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gdlgufrzs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.vehdjk.com/Article/details/gzicblyxl.sHtML

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/gvnseuzbn.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.sjlbkw.cn/Article/details/gatdibyrg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gocjsgjao.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gyedcluxt.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/ggkqjuzdd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjqrybxip.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gvtkmizyf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.tarul.cn/Article/details/gzxocsdjv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/gfsxavddw.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gleigxthz.sHtML

TS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gpvyyhfex.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.vehdjk.com/Article/details/gcxvdwyte.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.tarul.cn/Article/details/gkaztyahf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.bbcook.cn/Article/details/gkpexwqzw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.bbcook.cn/Article/details/ghgifedny.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gkxfjqbac.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gnuvhttpb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.tarul.cn/Article/details/gsmbldggz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gxyxlrvxe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gbsniqueb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gnhbukhec.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/grynekrnz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/grejjswhh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.yfazqb.com/Article/details/gjhcuydtp.sHtML

[L03] 设置自定义请求头
来源：http://baike.fktsv.cn/Article/details/gdykkrvmm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/ggagfirwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gkjegjspg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/gfwemqntt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/geiznmpfk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gkewfwzip.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gskgnnpnx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/geydogcxs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gdvlkxsyy.sHtML

[L04] 设置超时
来源：http://3g.fktsv.cn/Article/details/gvgiovsfo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gabkkzpcu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gtalqdhok.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/glntpiqrm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gltsvncdz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gwihomcvl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gbbvlfyka.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.vehdjk.com/Article/details/grmzwcuvy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fktsv.cn/Article/details/gkjhunply.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gzowfiyvg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gcxclegqk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/ghzmlasal.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gkfuagwqz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gwvxytblp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gzqopcjyr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gdzamakgx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/gtoszuvgr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgbpwvlh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/gezijasja.sHtML

Py:   resp.json()
来源：http://blog.epnwcf.com/Article/details/gwoinuprc.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gudkbjwpm.sHtML

JS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gmytuiqnr.sHtML

TS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gggcdkkid.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/gehhbiktx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gjaenkteb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/gtismhnnr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.sjlbkw.cn/Article/details/gtuqllpyu.sHtML


<!-- 参考信息 -->