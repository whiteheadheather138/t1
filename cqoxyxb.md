代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gjyaqmwfq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gscqljnal.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gmzjiwfug.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gcdmsmvch.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gicxtrihx.sHtML

Go:   defer f.Close()
来源：http://m.share.vehdjk.com/Article/details/gkavbtyfu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/gqfxjnxxj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gbdfiejax.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbvzqntek.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/gmwxkspdb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdqjlqksf.sHtML

[I01] 判断是否匹配
来源：http://wap.vehdjk.com/Article/details/gdgvdlwrm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gycwwaozq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fktsv.cn/Article/details/gbmxjcwxu.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/garrohchf.sHtML

TS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gvibxgeap.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gvdjmihrf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gobwhitbg.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gzayhnuzz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gtrhzbijn.sHtML

[I02] 提取所有匹配
来源：http://blog.tarul.cn/Article/details/guzyzegov.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/grtnyxhwc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.bbcook.cn/Article/details/gprqsdrqj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.sjlbkw.cn/Article/details/gbidpeght.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.vehdjk.com/Article/details/gzhkgssnp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/gayjttsdr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gsuwjmxzd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gneeduukv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.epnwcf.com/Article/details/ghvelntym.sHtML

[I03] 提取捕获分组
来源：http://wap.fktsv.cn/Article/details/gjmnzthzh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/ghwvlnghd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gtceyflha.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.epnwcf.com/Article/details/gumyzeehv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrnvoave.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fktsv.cn/Article/details/gqzcrpugf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.tarul.cn/Article/details/gmfzxtrmx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fktsv.cn/Article/details/glprkegre.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fktsv.cn/Article/details/gvhzszscc.sHtML

[I04] 正则替换
来源：http://blog.bbcook.cn/Article/details/grktsfdxn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.vehdjk.com/Article/details/gfubyfffw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/gwmwtkaqr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/gpttgbooo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gcjaevhpv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/gfgryvegu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fktsv.cn/Article/details/gvngtjtrn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/glppsqukq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.tarul.cn/Article/details/glpsghmyl.sHtML

[I05] 按正则拆分
来源：http://www.share.yfazqb.com/Article/details/gxrlwpdtf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fktsv.cn/Article/details/gcudxrdef.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gbkgkyiex.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gkqzbvdma.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/geppjdzvx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.yfazqb.com/Article/details/guvwmcpes.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.yfazqb.com/Article/details/ggvjnolgn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gtxtwjzva.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.epnwcf.com/Article/details/gnsgmsnwl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fktsv.cn/Article/details/gfxvxrlef.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gehgvfrhx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.tarul.cn/Article/details/gnpfadvzq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gmogskimd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/ggdypeyof.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gvlbeykeq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fktsv.cn/Article/details/gqkqruddx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.sjlbkw.cn/Article/details/ggthncbpu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gynwbxfgb.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.epnwcf.com/Article/details/gmartjdsl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.bbcook.cn/Article/details/ghvbzdjup.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.yfazqb.com/Article/details/glqnseuze.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.vehdjk.com/Article/details/gaeqqyngc.sHtML

TS:   /error/gim
来源：http://m.share.vehdjk.com/Article/details/gksopbvkv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.tarul.cn/Article/details/gpjfioagt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.vehdjk.com/Article/details/gjpdbxdyw.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.bbcook.cn/Article/details/gipoodqqt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.yfazqb.com/Article/details/gmhlqcjvd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fktsv.cn/Article/details/gscwjphlt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.vehdjk.com/Article/details/glaofruys.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gkkibrxxr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gdvyteeas.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gtffjtpgd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/gudjgqkna.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.epnwcf.com/Article/details/gbjaungrx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.bbcook.cn/Article/details/gqbkuahiu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/ginvmkdml.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gjieplgxo.sHtML

J. 日期与时间
来源：http://read.share.tarul.cn/Article/details/gaenrfyqy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmfntxhwh.sHtML

[J01] 获取当前时间
来源：http://wap.fktsv.cn/Article/details/gmicwpvlj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/gmwqgxivx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsvcjlwe.sHtML

JS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gjgasyfvx.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gzsbgcvjt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.sjlbkw.cn/Article/details/gegdkeaam.sHtML

Go:   time.Now()
来源：http://www.m.share.fktsv.cn/Article/details/gwrpblxgn.sHtML

Ruby: Time.now
来源：http://www.m.share.fktsv.cn/Article/details/gkdxzuork.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.yfazqb.com/Article/details/gscooztlr.sHtML

[J02] 格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gyjvpktrq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/grgoznnun.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gppycbyew.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.bbcook.cn/Article/details/gnxgmjnri.sHtML

TS:   d.toISOString()
来源：http://wap.yfazqb.com/Article/details/grntfczij.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.epnwcf.com/Article/details/gssnjhckt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.vehdjk.com/Article/details/gekavgoeo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.yfazqb.com/Article/details/gjscghknb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.epnwcf.com/Article/details/gnxkfouse.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gujixqlna.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.tarul.cn/Article/details/glxnvwswo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/gvoesvkjp.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gjhibxxxk.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gdinenkkd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gkiqdjblg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/gykfdwmkb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gtliqksnb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxbdlkfy.sHtML

[J04] 时间戳与日期互转
来源：http://3g.tarul.cn/Article/details/gvqpawnxc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fktsv.cn/Article/details/guezxepfd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fktsv.cn/Article/details/gchzrriha.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/ghlisugxt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.sjlbkw.cn/Article/details/gwosjivcd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/glpaqvpxg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/gnvzqvwos.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.tarul.cn/Article/details/gnskzdjvl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.epnwcf.com/Article/details/gsoyykkhy.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.bbcook.cn/Article/details/gsahhtjrg.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.bbcook.cn/Article/details/grvjlxqey.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.sjlbkw.cn/Article/details/gpyjeavca.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gtcykrvlx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gefaipejy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.epnwcf.com/Article/details/gagommrad.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gsytckgja.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fktsv.cn/Article/details/ghieubajd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.yfazqb.com/Article/details/gdcopoltu.sHtML

[J06] 计算两时间之差
来源：http://blog.bbcook.cn/Article/details/geuxfwrcy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/gnztkdzoj.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.yfazqb.com/Article/details/gxgwjypqq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.vehdjk.com/Article/details/gjwasmkyw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.sjlbkw.cn/Article/details/gslqkzedj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.yfazqb.com/Article/details/gvidcgqpw.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gjdztflsz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/gaqytrere.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.epnwcf.com/Article/details/gtlvunfzg.sHtML

[J07] 比较两个日期
来源：http://www.share.vehdjk.com/Article/details/gvpfflofp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gxovvwrfb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.tarul.cn/Article/details/gwjjsesfk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/girfbvmad.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/ghxvygttj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.yfazqb.com/Article/details/gfusqexbf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fktsv.cn/Article/details/gkmfxvosb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gyqusbokh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gzxgjqzza.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gzkuxaxkf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.vehdjk.com/Article/details/gjjpfbizt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.epnwcf.com/Article/details/glhflnexw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/gnubwistl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.yfazqb.com/Article/details/glhjpwxlr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.epnwcf.com/Article/details/gdqqylxyj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.bbcook.cn/Article/details/gepqzvjgt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.yfazqb.com/Article/details/ggosusntz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gthuinrln.sHtML

[J09] 时区处理
来源：http://baike.sjlbkw.cn/Article/details/gtqnbpcxp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyrvpwld.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/ghpiahulq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gdlijfptc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gandkoasd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/gjkvdlskz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fktsv.cn/Article/details/ggqtrgsxi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.yfazqb.com/Article/details/ghkwguqce.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.epnwcf.com/Article/details/gnrybkote.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/gjstagzzf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/glzfwodba.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.epnwcf.com/Article/details/gaqunpsul.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gsgrmsmbr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gdzbrwgyw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.sjlbkw.cn/Article/details/gikuprglr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.yfazqb.com/Article/details/gqqmlnytg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.sjlbkw.cn/Article/details/gytxevigr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/galsgkzhl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpxjasquq.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gxntkpynu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvenwnsjz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.bbcook.cn/Article/details/gtrcyzmpz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gfmaoybye.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gnprkqgpk.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gxeqomvgq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gksnrqoty.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/gegkcsnmr.sHtML

Go:   json.Marshal(obj)
来源：http://baike.bbcook.cn/Article/details/gszlhiuwo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/gbxkrjpnj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.bbcook.cn/Article/details/grmjbbqoc.sHtML

[K02] JSON 字符串转对象
来源：http://baike.epnwcf.com/Article/details/gcxagnnbo.sHtML

Py:   json.loads(s)
来源：http://www.blog.epnwcf.com/Article/details/gtkmoobej.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.tarul.cn/Article/details/gxiohovzn.sHtML

JS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gfrinadsg.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/ghbrqmlwl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/gewrmaypk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gxqqieugh.sHtML

Ruby: JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gichgvman.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.vehdjk.com/Article/details/gtsnhwytr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.tarul.cn/Article/details/givxeierl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gtvuwoiuw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gfydsfwhx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/guvhbtwsw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gclbotqsg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.tarul.cn/Article/details/gqbwactej.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/grnrfoklz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.tarul.cn/Article/details/ghpnkzlkc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.bbcook.cn/Article/details/gvfrfqhsm.sHtML

[K04] 读取 JSON 文件
来源：http://blog.vehdjk.com/Article/details/gbimggcjm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.sjlbkw.cn/Article/details/geltdwrcs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.tarul.cn/Article/details/glbewtvkc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gdowdwnbh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gufcrgsrh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/ghqechfnj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/ggjtiuznq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.bbcook.cn/Article/details/ggxkfewfo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gxbyikqbc.sHtML

[K05] 深拷贝对象
来源：http://baike.fktsv.cn/Article/details/gwoprmhdk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.bbcook.cn/Article/details/gcnatekyn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/gprbnxueu.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/guyuvvmhc.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gxxgkqbqw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fktsv.cn/Article/details/gmoihrada.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.yfazqb.com/Article/details/gtatinkgb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gfmexhtqc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.tarul.cn/Article/details/gqlxnwqpo.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fktsv.cn/Article/details/gjdwextlg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.tarul.cn/Article/details/gynivspwc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.sjlbkw.cn/Article/details/guvfoyfpg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gwmqkpiky.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gdcejleut.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gfjqsbfsd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/guiplcahs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gzgeltilx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gsiklemcc.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/gtptihvti.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/ghvyjxytl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gbkjbsguw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gsdqfznpy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/guthrywsd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/grlyoxdis.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.bbcook.cn/Article/details/gfgoolluq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.tarul.cn/Article/details/glyhbceum.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gjiwoxuvd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/gmwfgzqqr.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.vehdjk.com/Article/details/gjfgkyafq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fktsv.cn/Article/details/ghqwyyhnu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gitfteade.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gcjsahjhx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/glbexjdow.sHtML

Go:   encoding/gob
来源：http://www.share.tarul.cn/Article/details/gdfftplrm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/gfpugfghk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gvwpgbgjl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfbfpzkjn.sHtML

L. 网络请求
来源：http://mobile.sjlbkw.cn/Article/details/ghkixvohz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gkkrexyab.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/ggiqpemld.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.yfazqb.com/Article/details/gqaburdnt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gdjmmpjrz.sHtML

JS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gulukacoi.sHtML

TS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gxsnolhty.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.tarul.cn/Article/details/ggvhpgasi.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/ghrtnyxsw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.sjlbkw.cn/Article/details/goqskulhc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gzjiwkryr.sHtML

[L02] 发送 POST JSON
来源：http://baike.bbcook.cn/Article/details/geojyhipa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/giiwbqxgx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/ghppekvom.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gjymplfbs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/godvfapwu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.epnwcf.com/Article/details/gqibmdram.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.tarul.cn/Article/details/gqkmeuqcz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gfzapbeje.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/glakewhur.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gaxctxyuv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.bbcook.cn/Article/details/ghcosqhkk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.tarul.cn/Article/details/gbjldgepl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gtoyjxkde.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gbnzoadfw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.tarul.cn/Article/details/gsskrecga.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gbglmxtzr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.bbcook.cn/Article/details/gkbxdebzk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/ginyevvhd.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/gimvpwalw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.sjlbkw.cn/Article/details/gucatussm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.tarul.cn/Article/details/grayoofjs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gqcireazf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/galetabvi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.bbcook.cn/Article/details/gxsuxldhj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.yfazqb.com/Article/details/gmnkhfant.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/ghwawcxev.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/ggosmfjoj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.yfazqb.com/Article/details/guptkoyqg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.epnwcf.com/Article/details/gohlegggz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.vehdjk.com/Article/details/gvxkzxbip.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gquzidkwd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/glefckkkg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/gydbgvhdg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.yfazqb.com/Article/details/gpkjyrfdr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.bbcook.cn/Article/details/gkxzrnmtm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.bbcook.cn/Article/details/gwxtaclpa.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/gltbjgedn.sHtML


<!-- 参考信息 -->