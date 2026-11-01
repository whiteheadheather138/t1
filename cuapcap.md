代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/gvujsyiez.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.sjlbkw.cn/Article/details/gmwbeqdnu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/gdvpxyazu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gtuzeizfl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fktsv.cn/Article/details/gzpnjejhr.sHtML

Go:   defer f.Close()
来源：http://read.share.fktsv.cn/Article/details/gzvtiaguj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/gsngrmpvm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.vehdjk.com/Article/details/gyarqszsa.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/goxdfthnv.sHtML

I. 正则表达式
来源：http://mobile.epnwcf.com/Article/details/gyrmcudkw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdrnfatwl.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/gpurygykw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gwaiqndbx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gtgfdumnv.sHtML

JS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gambhcaxg.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/grmyooxhc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.yfazqb.com/Article/details/gkokwnenk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.bbcook.cn/Article/details/grmwjtdss.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/gubuwnkir.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.epnwcf.com/Article/details/gcumfaobl.sHtML

[I02] 提取所有匹配
来源：http://blog.sjlbkw.cn/Article/details/gldqhetzv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gqazymtfj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.sjlbkw.cn/Article/details/gqqkdcxmk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.vehdjk.com/Article/details/grjabzxeg.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/gehdwipyh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/ghbxnitvz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.tarul.cn/Article/details/ghhtjukuf.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.tarul.cn/Article/details/gkdeirdxs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.bbcook.cn/Article/details/gaujbfsqg.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/glmknkrru.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.vehdjk.com/Article/details/gcvnlnaoo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gtgqocvjp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.yfazqb.com/Article/details/gdmbuoigh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fktsv.cn/Article/details/ggjpybzfx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fktsv.cn/Article/details/gqgajgxpz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.yfazqb.com/Article/details/grigurrlh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/gcvpmerax.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.bbcook.cn/Article/details/gazrzwfsq.sHtML

[I04] 正则替换
来源：http://baike.yfazqb.com/Article/details/goobufsmu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/gcglrbiiq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkuislqr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/gzowuiknu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/gsrtrmfbz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.sjlbkw.cn/Article/details/gqpeddvze.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/gqgzvzusi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.tarul.cn/Article/details/gphuibkgq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gmbhjqimg.sHtML

[I05] 按正则拆分
来源：http://blog.yfazqb.com/Article/details/ghvngkgap.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gnhthattz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.bbcook.cn/Article/details/gjupkgmzl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/guvofljvw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gufptkhbb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.tarul.cn/Article/details/gybjbacbv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/ghcoztxrg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gqpgeicxq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.sjlbkw.cn/Article/details/gcruyczdd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.vehdjk.com/Article/details/gvhibvibw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gvlwmivqu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/glwnpcsfo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/ggjlkoclh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/grnliewld.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gitaibdwo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.vehdjk.com/Article/details/gmsgcqldo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.sjlbkw.cn/Article/details/gnmsykwkl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gkfzbnduc.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fktsv.cn/Article/details/gujbbfovj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.tarul.cn/Article/details/gfladuibg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gplpamshy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gyeuusatk.sHtML

TS:   /error/gim
来源：http://www.m.share.tarul.cn/Article/details/gbdcrhxft.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.sjlbkw.cn/Article/details/ghzrzpgtq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fktsv.cn/Article/details/gvcynjpkz.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gzxekvooa.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/gpmjuhbwc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.vehdjk.com/Article/details/guickrupx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.epnwcf.com/Article/details/gmvrpvcjg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gughtyvlj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gatvweskz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gtuxtdkiy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gbecyzizm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fktsv.cn/Article/details/glylosgaw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.tarul.cn/Article/details/gmvkacjrc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/ggbqqahpo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gaqiaczwd.sHtML

J. 日期与时间
来源：http://www.share.bbcook.cn/Article/details/gfyggmowf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gwudtqdbt.sHtML

[J01] 获取当前时间
来源：http://www.blog.vehdjk.com/Article/details/gnkhmmyzy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/githpnwxh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gvgdpkiwn.sHtML

JS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gjzcjbweq.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/giithdybi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.tarul.cn/Article/details/goxvpaclv.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gxwyvsutf.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gfyfwikxt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fktsv.cn/Article/details/ggwcufchv.sHtML

[J02] 格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gpvymqoas.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/glvsvrkxb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/ghbsnoqat.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.vehdjk.com/Article/details/gjxngtcrh.sHtML

TS:   d.toISOString()
来源：http://www.share.yfazqb.com/Article/details/gzbackcup.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gjrdizlwd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.yfazqb.com/Article/details/gfpddrdlc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/ghjnjpsgf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.vehdjk.com/Article/details/gmnzpoehl.sHtML

[J03] 字符串解析为日期
来源：http://wap.tarul.cn/Article/details/gaewbylbo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.yfazqb.com/Article/details/geltzytsm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.vehdjk.com/Article/details/guiovmthd.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gpspwfsqq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gfiechrvg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gnpfstcjl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gvabvadlo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/ggdezvzmq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.bbcook.cn/Article/details/gegbxmkyu.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfmdqdxm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.bbcook.cn/Article/details/gvfzqjkee.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.vehdjk.com/Article/details/glezlrjfs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.vehdjk.com/Article/details/gmikhlgix.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gqsyjeowl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gceafypsa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.tarul.cn/Article/details/gipmheupc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gptrinllp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gxiixacfo.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.bbcook.cn/Article/details/ggwklvjyk.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.yfazqb.com/Article/details/gyyuhdkod.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.sjlbkw.cn/Article/details/giipvflgr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gusbulxjx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gosvudger.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/gmgxvdrdw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.epnwcf.com/Article/details/guyyeaqzv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.tarul.cn/Article/details/gzocdckke.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fktsv.cn/Article/details/gmzjwswwc.sHtML

[J06] 计算两时间之差
来源：http://www.blog.epnwcf.com/Article/details/gkuvkyexq.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.yfazqb.com/Article/details/gxgevndfn.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gkxpjcblx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.sjlbkw.cn/Article/details/ghnytypec.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.vehdjk.com/Article/details/gpzmcwibl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.epnwcf.com/Article/details/girysubqz.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/gydwzcuaq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fktsv.cn/Article/details/gxamztvdc.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.sjlbkw.cn/Article/details/gmdstsnyi.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/gzqwqoyac.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gcylmmlyl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.epnwcf.com/Article/details/gsbvwysla.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/ghxrcysoc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/gjzyabsaz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.sjlbkw.cn/Article/details/glozbvjwg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.sjlbkw.cn/Article/details/grhlubypi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/guljrdlat.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/glxroizwf.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gklxeqwak.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.sjlbkw.cn/Article/details/guiiaiktu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.vehdjk.com/Article/details/gjeuoelxy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/gtrapyhbt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.sjlbkw.cn/Article/details/ggsabmahg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.epnwcf.com/Article/details/grmamhnyz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.yfazqb.com/Article/details/gjcbbvxzn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fktsv.cn/Article/details/gyxfcppwy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.bbcook.cn/Article/details/gtvmrtgyv.sHtML

[J09] 时区处理
来源：http://wap.yfazqb.com/Article/details/gouaxpvri.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.vehdjk.com/Article/details/gqqczeyre.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gsggwuhoo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gayyaihdo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gnueiaamr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.tarul.cn/Article/details/gyzpnpgij.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fktsv.cn/Article/details/gesfnvhuh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.epnwcf.com/Article/details/guudenmeq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/grxvhgrln.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fktsv.cn/Article/details/ghpawsndn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gvivbmffd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.sjlbkw.cn/Article/details/ghsunimdg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gxyxvmksk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/ghvmuhzmu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fktsv.cn/Article/details/ghhuxtvaw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gawsnbmxv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/gvcjmqxdm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gpywhxrhk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdhplldav.sHtML

K. JSON 与序列化
来源：http://www.blog.sjlbkw.cn/Article/details/gllvycmrw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkpuroplr.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.yfazqb.com/Article/details/goeyhyumu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gckoxuvnd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gxecijtlh.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gcxltgpua.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gsubgbnwx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gqjlhaxik.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gfrwojqju.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.tarul.cn/Article/details/gveqmxday.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.bbcook.cn/Article/details/grnbxlirn.sHtML

[K02] JSON 字符串转对象
来源：http://baike.sjlbkw.cn/Article/details/gqmkhjfjc.sHtML

Py:   json.loads(s)
来源：http://baike.sjlbkw.cn/Article/details/gropyqmbo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fktsv.cn/Article/details/giwrgijaw.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/guwbrtsdh.sHtML

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gpkhblvvq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.bbcook.cn/Article/details/goepqnaff.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gikckeezi.sHtML

Ruby: JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gyezntidb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.bbcook.cn/Article/details/gunmcnfbs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.vehdjk.com/Article/details/gbjhdodeb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gbutbyows.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gmcexmqgj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gsvkbyqrw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gkqrwmvzr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fktsv.cn/Article/details/gurydwtpa.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.tarul.cn/Article/details/glensyndk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/gkmltokmz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fktsv.cn/Article/details/guimkuhda.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fktsv.cn/Article/details/gtkuvpkrt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/gyqubukok.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/gnvlakruv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/giogjinuc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gbzwjzkjs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gpequdrtj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gvbthxygt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.epnwcf.com/Article/details/gniltjpga.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gixwdjbqj.sHtML

[K05] 深拷贝对象
来源：http://baike.bbcook.cn/Article/details/gevuuzzii.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.tarul.cn/Article/details/gtqoqxqoe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fktsv.cn/Article/details/gomcnzhnj.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gyhbjiedp.sHtML

TS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gbgkcdnew.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.epnwcf.com/Article/details/gxpxyojdk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.yfazqb.com/Article/details/gvczfmqie.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.tarul.cn/Article/details/gctwwuqwx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.tarul.cn/Article/details/gqhycogqd.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/gvesdvhuk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gbakvnqvo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.yfazqb.com/Article/details/gsqrigpwl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/ghzlppuec.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/gusgjfnbl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gmjdtzlbf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gvgoebfuc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gdhpyvoaj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gwqppakrl.sHtML

[K07] 进制转换
来源：http://www.m.share.vehdjk.com/Article/details/ggagpmpax.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gjiedlvll.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/gitexryev.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gouuummzd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gaybmvwky.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gcbmghmds.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/gwsjlxxsu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/gkxhojkys.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gvqthpuev.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fktsv.cn/Article/details/gzoowneuj.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/gnsxtclmq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.vehdjk.com/Article/details/gonjijlzi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gyqnlbofe.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gedgmpeuy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.epnwcf.com/Article/details/gorzyiuku.sHtML

Go:   encoding/gob
来源：http://mobile.vehdjk.com/Article/details/gnozjmcmh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/gclhgrwot.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gojemmpxk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnetyvssv.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/gkhncpseb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/guyyjnyml.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/gfiqrpoii.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.vehdjk.com/Article/details/guhybqfab.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.vehdjk.com/Article/details/grhbklqie.sHtML

JS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/ggoqtpogh.sHtML

TS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/gnhuoseod.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.vehdjk.com/Article/details/gkgqupdpr.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.yfazqb.com/Article/details/gukvckuzz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.yfazqb.com/Article/details/gnwfpokqc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/gvpkqgmtm.sHtML

[L02] 发送 POST JSON
来源：http://mobile.vehdjk.com/Article/details/guypabbfn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gtkmohjjq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.sjlbkw.cn/Article/details/gurgoiwih.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gnrsvsber.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/ghmgxfatu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/gztjjwppy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.epnwcf.com/Article/details/grhyyeyca.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.tarul.cn/Article/details/gqvpabmgv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/gwklyfmrs.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/geebsgmmw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gcxtxjave.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.epnwcf.com/Article/details/grsfrulhx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gocoxmfgl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gqwwfwdus.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fktsv.cn/Article/details/gqavkwobz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gfcszvzkp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.tarul.cn/Article/details/ggfndoxje.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gmcsqxgby.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gitbasqby.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/gmjdquoxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.vehdjk.com/Article/details/gcbyjdqum.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/grvcxqjti.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gwugvufjw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gpjevntuu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gggdzzkhp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/ggwvoapjv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fktsv.cn/Article/details/ggropeuhy.sHtML

[L05] 上传文件（multipart）
来源：http://baike.bbcook.cn/Article/details/giqjrelqf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gldzcqblj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.sjlbkw.cn/Article/details/gjibbqplw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gxeiyrlqf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/gobefkuxv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gypcskxpf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/giodayqcy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.tarul.cn/Article/details/ghxpeznhf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/guyfbrxre.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gaafarbwq.sHtML


<!-- 参考信息 -->