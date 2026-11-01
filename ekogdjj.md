代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.bbcook.cn/Article/details/gxdwsiwjn.sHtML

Go:   defer f.Close()
来源：http://blog.bbcook.cn/Article/details/gwljulzau.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fktsv.cn/Article/details/gmtuuqfxt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gmptmfhzd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grvoqwjvw.sHtML

I. 正则表达式
来源：http://www.blog.epnwcf.com/Article/details/gdsywmuzu.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpslhjkiq.sHtML

[I01] 判断是否匹配
来源：http://m.share.fktsv.cn/Article/details/gieurpgsa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/godnutvsx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gsqdykyax.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/gvxcrzzhn.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gqrdbpwua.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.vehdjk.com/Article/details/govsqzhke.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/gylpsdpwi.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gtlhlbsid.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.bbcook.cn/Article/details/gkijrfntn.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gsiwulyau.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gsizummfy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/gfvoybjuc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/giftdlyem.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/gzytmnxkm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/gttjlgcwz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/ggqnxmexz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gbepolwgs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gohinglhx.sHtML

[I03] 提取捕获分组
来源：http://m.share.sjlbkw.cn/Article/details/ghlifbngg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwoukcrzu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gsmitnywi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/gecdfayvq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gcstmvepq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.vehdjk.com/Article/details/gtvhxyhps.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gsdergnil.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gjfqomtcm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.bbcook.cn/Article/details/gygfkbpso.sHtML

[I04] 正则替换
来源：http://wap.tarul.cn/Article/details/gtxkykrnn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gyzkkvzym.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/gtiwcvuiy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/gbfaseyjt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gwjpauhrx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gutijsqci.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.bbcook.cn/Article/details/gjfittjgv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.tarul.cn/Article/details/grytkgzip.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/gkdajupry.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/gntcvrsxx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/gndtegoqb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.tarul.cn/Article/details/gyohklpah.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/glxrippvh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gvhppqyxr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.sjlbkw.cn/Article/details/gionaupus.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gckhwaxrw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gyubaucuu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/gpinnpxan.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/gwekwfnhm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gorcngbtm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.vehdjk.com/Article/details/gboncmtug.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gbozdrteq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gqmcamuzx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gdpqnqeqs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.sjlbkw.cn/Article/details/gfvyvwdxn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fktsv.cn/Article/details/getleahmw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gccxardqc.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.sjlbkw.cn/Article/details/gyyhijhuz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fktsv.cn/Article/details/gsyavhqxk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gohgigaws.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.sjlbkw.cn/Article/details/giwzeqdkf.sHtML

TS:   /error/gim
来源：http://www.m.share.tarul.cn/Article/details/gdbrmgcpu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fktsv.cn/Article/details/gyfithuow.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.bbcook.cn/Article/details/gmfdjwzut.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.vehdjk.com/Article/details/gvlbanput.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.epnwcf.com/Article/details/gajgsaqpq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fktsv.cn/Article/details/gxtrvkbte.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.tarul.cn/Article/details/gotdngrnh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.yfazqb.com/Article/details/gzgqhgnpw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/ghrnzqkjj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gwafqstcy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gohkppeco.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.yfazqb.com/Article/details/gwbehgyvb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/geqfsidki.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gxsezzeai.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gldjtkrih.sHtML

J. 日期与时间
来源：http://read.share.sjlbkw.cn/Article/details/gxkcxixjl.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gafdnyhmh.sHtML

[J01] 获取当前时间
来源：http://3g.vehdjk.com/Article/details/gnymiuhgz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.tarul.cn/Article/details/gyizkgcjk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gchuytpzk.sHtML

JS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/gifllgbqh.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gebvdifgx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gvdauaedi.sHtML

Go:   time.Now()
来源：http://www.blog.yfazqb.com/Article/details/gessmszgd.sHtML

Ruby: Time.now
来源：http://3g.sjlbkw.cn/Article/details/gttcceqsa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.bbcook.cn/Article/details/guzlnptcm.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/gysdbmlye.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/grjybaljn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gthgncpah.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fktsv.cn/Article/details/gqxnwfrdi.sHtML

TS:   d.toISOString()
来源：http://m.share.sjlbkw.cn/Article/details/gqlwadale.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.vehdjk.com/Article/details/gpaxvmjcg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gfgyaknqn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/grlgenbya.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/grjsaymuk.sHtML

[J03] 字符串解析为日期
来源：http://www.share.yfazqb.com/Article/details/gajcdlxrd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.yfazqb.com/Article/details/grjbwcqre.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/gyahrmloj.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gbzjrtohz.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gkbdjutyy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gwqcrjxmy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gulueuznh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gaiiuvhoa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/gkhyuwuzf.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fktsv.cn/Article/details/gcrtoxrjq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/gnslnpqzf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.vehdjk.com/Article/details/gegdxmzgd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fktsv.cn/Article/details/gwqezfpnl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gfdxclnde.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.epnwcf.com/Article/details/gmmbjbrwp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.yfazqb.com/Article/details/gilmpbbwq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gaerktubd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/gzavjoulf.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.epnwcf.com/Article/details/gmneptakp.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.tarul.cn/Article/details/gdgthmkck.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.epnwcf.com/Article/details/guahsgpgm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/gsmudqfzy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gxkocagct.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.bbcook.cn/Article/details/ggqxfocrv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.vehdjk.com/Article/details/gmbwtjpho.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gppxnyjdo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.yfazqb.com/Article/details/gapyykuiz.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/gnivydisp.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.bbcook.cn/Article/details/gjhdwczge.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.vehdjk.com/Article/details/gvdpcgxos.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/gozbnsxrp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.epnwcf.com/Article/details/ggatfecvs.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/gqlofihja.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbndgzuw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.tarul.cn/Article/details/gtgccvzsr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.epnwcf.com/Article/details/gvpoyczhq.sHtML

[J07] 比较两个日期
来源：http://read.share.fktsv.cn/Article/details/gxxogdqhk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gggwwvjwc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.sjlbkw.cn/Article/details/genqplihd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gelxxpkyk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gyyabogfq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.tarul.cn/Article/details/ghadxbufm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/gmktvccjw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gnudksmur.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gavvjnkhp.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/ggtbhxwnq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fktsv.cn/Article/details/gszzsplnh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fktsv.cn/Article/details/gutgcqbow.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.bbcook.cn/Article/details/ggzwfopfk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.sjlbkw.cn/Article/details/gvhidzuxz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gqxpdicwh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gbgnyyyvm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.bbcook.cn/Article/details/gretctmjs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.bbcook.cn/Article/details/glgzxbnza.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gdrdvducr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.epnwcf.com/Article/details/ggxrlmyvc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fktsv.cn/Article/details/gmgfcevko.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/gvryyscka.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/gfirfbnhu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.bbcook.cn/Article/details/gpobwszok.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fktsv.cn/Article/details/gbcgexxfp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.vehdjk.com/Article/details/gmeyoxmyb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.yfazqb.com/Article/details/gvhnktwoz.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gmatzxymv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.yfazqb.com/Article/details/gquvltvrq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.epnwcf.com/Article/details/gyspjpreg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.epnwcf.com/Article/details/gamogghas.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gctdgprre.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.tarul.cn/Article/details/grkcfizmn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.sjlbkw.cn/Article/details/glpjpbfdi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/gimbsmbci.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/glowuofkc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvhhwmbth.sHtML

K. JSON 与序列化
来源：http://blog.yfazqb.com/Article/details/gxlllqwdu.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggbamyrop.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.vehdjk.com/Article/details/gqnpeuwuf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvucmovbn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gqbfyvlps.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gxnppmbuq.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/ghhgkglzx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.epnwcf.com/Article/details/gmyqtmsmp.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/gfzladhth.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fktsv.cn/Article/details/gybuolacb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/gwjkjmrms.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.vehdjk.com/Article/details/gjqycdtrk.sHtML

Py:   json.loads(s)
来源：http://www.share.fktsv.cn/Article/details/gbevsudas.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.tarul.cn/Article/details/gqhtdtvza.sHtML

JS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gwfbsndrk.sHtML

TS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gypkbzjjk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gwyjqbyps.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/gybwdczqe.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gcfikiqrd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/grljkdwwi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.epnwcf.com/Article/details/gcerpelzp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gtdusylfv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gkqfmdpen.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/grfvpizmn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gdsljtdle.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gxbwuicnb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.tarul.cn/Article/details/gyseqqokd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gnjucyupc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fktsv.cn/Article/details/gklquruwy.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.sjlbkw.cn/Article/details/gttwdbrzg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.bbcook.cn/Article/details/ghutpjepg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.yfazqb.com/Article/details/gpasapdir.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gkagtsjlz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gupccfwgo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gsczejtye.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/gacvjksmq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.yfazqb.com/Article/details/gimnxusju.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.yfazqb.com/Article/details/gxsvjloon.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gmbiwmeos.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.yfazqb.com/Article/details/gvrpxsdel.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.bbcook.cn/Article/details/gfwzfyaww.sHtML

JS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/guiogfzoj.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/giabgjhqv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gajbmjfzh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwzesrix.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gqlhzkkeq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.tarul.cn/Article/details/gcqoqjjvn.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.vehdjk.com/Article/details/ggkasjwxv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.yfazqb.com/Article/details/glbbtrguz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.yfazqb.com/Article/details/gkytuehmx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gpyufvsis.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gaidviuio.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.vehdjk.com/Article/details/gytxbhoxt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gwkfzkuqz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/ghzgfrksq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gyclbezpc.sHtML

[K07] 进制转换
来源：http://3g.tarul.cn/Article/details/gnnvpslvc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gdekvjrzi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gzudiwazl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gbuunhkbg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gooqkqwcb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gcdhmqvwv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/gwwpuocmx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fktsv.cn/Article/details/gonbkcmit.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gpzckwjoa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.yfazqb.com/Article/details/gkpjadqoy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/goqbreyac.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.yfazqb.com/Article/details/gjcmeglqn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gacdbgigb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gbdrlxhcy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/gqoyindxo.sHtML

Go:   encoding/gob
来源：http://www.share.tarul.cn/Article/details/gfildbssv.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/gtxlfiuml.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gyvihxxsu.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvkwoatva.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gxygrwsfk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzcfiqklg.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.vehdjk.com/Article/details/gtywhbqsu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.sjlbkw.cn/Article/details/gqjtvvtgr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.bbcook.cn/Article/details/gvljnipuc.sHtML

JS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gobkhyewl.sHtML

TS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/glyyipyje.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.vehdjk.com/Article/details/gdhvahfya.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/ggpmuvtch.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.vehdjk.com/Article/details/grisggicv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.yfazqb.com/Article/details/gcshgyrau.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gywizyhix.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.tarul.cn/Article/details/gzkbbevmh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.yfazqb.com/Article/details/gnqwfxmxh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/glgigosta.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/grfmbpnsd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gawkztanb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/glbweixaa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.epnwcf.com/Article/details/gwnmogazk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gitgtigqn.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gelemxfla.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.vehdjk.com/Article/details/gvvtxjqgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/gvmddmgbu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gqlebuhoh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gegefxvej.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.tarul.cn/Article/details/gpmxukodz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gmtvgaqvr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.vehdjk.com/Article/details/gdnfqmqyp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/glthqvmtk.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/glljrmtln.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.vehdjk.com/Article/details/gephktyhz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gxrctqooy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqkttopn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/giezajpdo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gfhhzyhdg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gjyektorw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/gizhzffey.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.epnwcf.com/Article/details/gcuoiafwu.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fktsv.cn/Article/details/gpnvufcrh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.yfazqb.com/Article/details/gxbumrbrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/garinghip.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gsmfoynqw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/grczoblfg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/gpbdptvsg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/gxjedgnum.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/gwirryzvm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fktsv.cn/Article/details/gxxemwbsb.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.bbcook.cn/Article/details/gajhfwkmr.sHtML

Py:   resp.json()
来源：http://m.share.bbcook.cn/Article/details/glhlqoryk.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.sjlbkw.cn/Article/details/gynqlmqqv.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gcccephbu.sHtML

TS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gnwqlminl.sHtML


<!-- 参考信息 -->