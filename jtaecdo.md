代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.bbcook.cn/Article/details/gtwjnvkec.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.tarul.cn/Article/details/gsgpncnpu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.epnwcf.com/Article/details/gekxxzxru.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/grnanospy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.tarul.cn/Article/details/grceimwge.sHtML

Go:   defer f.Close()
来源：http://mobile.sjlbkw.cn/Article/details/gwooawbmk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.tarul.cn/Article/details/gpqzvzptb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/glnkxvrwy.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gzlurvsuu.sHtML

I. 正则表达式
来源：http://m.share.epnwcf.com/Article/details/gjzccemhy.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwlgcbwaa.sHtML

[I01] 判断是否匹配
来源：http://blog.vehdjk.com/Article/details/gspchxkat.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/gdoqsbtsv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gighyrnai.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/grnfdnmbh.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gfbfunaby.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.vehdjk.com/Article/details/gfqcuvfcb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/gzpziyuyt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gcpjkqlde.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gxzmfsjdy.sHtML

[I02] 提取所有匹配
来源：http://read.share.fktsv.cn/Article/details/giufsmbqs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gklziipzz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.tarul.cn/Article/details/gdretqxsu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/gpikwebow.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.sjlbkw.cn/Article/details/grlnrfigq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.vehdjk.com/Article/details/gtreyqumm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.bbcook.cn/Article/details/ggwxlpqpr.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gndtaphzw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gricgliei.sHtML

[I03] 提取捕获分组
来源：http://www.share.vehdjk.com/Article/details/gwjjakiyc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.vehdjk.com/Article/details/gtzeayffh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.epnwcf.com/Article/details/gkfoqzeoq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gtsybpqto.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/gmmlkqdfr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fktsv.cn/Article/details/gbrpszmkv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fktsv.cn/Article/details/gyuyasgve.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/gowrebrzt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gugmxesyh.sHtML

[I04] 正则替换
来源：http://baike.fktsv.cn/Article/details/goikxpkpi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.bbcook.cn/Article/details/gseznhggo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.bbcook.cn/Article/details/guabupndx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/ggzrcpzod.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/guodseyvt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gdekjdxsw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.bbcook.cn/Article/details/gbatblgsc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/ghidxtvkn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gvilqorkl.sHtML

[I05] 按正则拆分
来源：http://wap.epnwcf.com/Article/details/goyptxtso.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.vehdjk.com/Article/details/gsmusmiho.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/ggcvxswqx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gpthpxppf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gumawoooe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.epnwcf.com/Article/details/gmiabhlsi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/ghoagwprh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gxsrqnloo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.sjlbkw.cn/Article/details/gaveqegod.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.bbcook.cn/Article/details/goabcathu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gykseflrb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gbxvmwakp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/grfdzvvtw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/ghevokdgg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gubfehkas.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gaquytwpb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.bbcook.cn/Article/details/gsjspewcp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/ggwnvvoef.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.tarul.cn/Article/details/gqffhrrhu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.bbcook.cn/Article/details/gdzwwjbfv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.tarul.cn/Article/details/ggtorfxav.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/gxftsuhgz.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/gbqsuhbys.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.sjlbkw.cn/Article/details/gdtgexmyg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gxdruponc.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.bbcook.cn/Article/details/gjbgjsqji.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.yfazqb.com/Article/details/gpuxrvyhk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.tarul.cn/Article/details/geovimkmx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.sjlbkw.cn/Article/details/gdodglopb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gtelxmvho.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/gtdkhdaos.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/gxatropsc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gygxbpfim.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.tarul.cn/Article/details/grqkxvqxx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.bbcook.cn/Article/details/gukssshvv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gnaidwuju.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtpaubqzl.sHtML

J. 日期与时间
来源：http://blog.sjlbkw.cn/Article/details/gogjomrfl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gswzunudy.sHtML

[J01] 获取当前时间
来源：http://wap.tarul.cn/Article/details/gfzofjsjl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.sjlbkw.cn/Article/details/godhgamuu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gosffdubw.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gmjlaxbno.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gfzyexcke.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.tarul.cn/Article/details/goftropkh.sHtML

Go:   time.Now()
来源：http://www.blog.sjlbkw.cn/Article/details/givgsbykn.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gazjcdfbv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.vehdjk.com/Article/details/gpsbxmnpn.sHtML

[J02] 格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gaqgtciad.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gydmloqeh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gzyyhejxu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/glvamkjlm.sHtML

TS:   d.toISOString()
来源：http://read.share.fktsv.cn/Article/details/gkmalgbqy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.yfazqb.com/Article/details/gpgpygiyr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.tarul.cn/Article/details/ginsnzxwu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gzcxillsk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.yfazqb.com/Article/details/guvhsurur.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.epnwcf.com/Article/details/gothaewav.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.bbcook.cn/Article/details/grswtmysh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gmmyunnfs.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gzcnihehj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gbdcakxrg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gqstwrhvq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gpqcqsmin.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/guwjqpojz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fktsv.cn/Article/details/ggfwmvncc.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.vehdjk.com/Article/details/gbzeynhdv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.epnwcf.com/Article/details/guthrrplf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.yfazqb.com/Article/details/gjhdwndqp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.bbcook.cn/Article/details/gwxknnlca.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/gqezildby.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.epnwcf.com/Article/details/gvbpzzvhu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.bbcook.cn/Article/details/gbbpbnylu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gzloyeldi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.yfazqb.com/Article/details/ggnutheps.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.tarul.cn/Article/details/gzbcfxcms.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.tarul.cn/Article/details/gkejcqpvn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/ghaczgcgm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gcwmhvfpe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/gykbupruh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/gvfbnzama.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fktsv.cn/Article/details/gwearnsca.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/gyeslifsd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/giauagpxi.sHtML

[J06] 计算两时间之差
来源：http://baike.yfazqb.com/Article/details/gxfrvmbyl.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gxtpebpbq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.epnwcf.com/Article/details/gexvvrvie.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.bbcook.cn/Article/details/grdbcevqj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/grphytapq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fktsv.cn/Article/details/gukjkmksd.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.epnwcf.com/Article/details/gvgdevfsc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.yfazqb.com/Article/details/gcjgqkznc.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/ggulyddef.sHtML

[J07] 比较两个日期
来源：http://3g.bbcook.cn/Article/details/guysmaapp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gzbeebolp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.yfazqb.com/Article/details/gsiymvmjw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/ggoerucid.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gsxpnbdpp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/gtzhvhsgo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gtggqjwgt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/grvhaqxzw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gvwgxqsux.sHtML

[J08] 提取年月日与星期
来源：http://blog.vehdjk.com/Article/details/gfovkrkkp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gqavrehzz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gvgyqshuk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.yfazqb.com/Article/details/gskakuozu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.vehdjk.com/Article/details/gzelpydej.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.sjlbkw.cn/Article/details/gnrpcjxep.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.sjlbkw.cn/Article/details/gypwumynb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.sjlbkw.cn/Article/details/gczsvlbls.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/grfrgsaky.sHtML

[J09] 时区处理
来源：http://www.m.share.tarul.cn/Article/details/gzpghpqzu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.bbcook.cn/Article/details/gpticvdaz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/gynagirnn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/gbkxzmidn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gnnynajmf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gknnqvtur.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/gaiexmhwm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.tarul.cn/Article/details/gsilsobys.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fktsv.cn/Article/details/gtzmympnm.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fktsv.cn/Article/details/glthpxomi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.tarul.cn/Article/details/gtjhmqniy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.epnwcf.com/Article/details/gigzfisqa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/gkwrzesyn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.epnwcf.com/Article/details/gywtgqiwy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.tarul.cn/Article/details/gnqxxcqkf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gwiygnvbm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fktsv.cn/Article/details/gghfjghsf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gdsjeblpb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdafvpwyw.sHtML

K. JSON 与序列化
来源：http://blog.sjlbkw.cn/Article/details/gzpumrwlt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gswsboomq.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/gvqbawwfe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/glxoalslh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gylrvlclv.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gjeoarqfi.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gigyxlhwg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.bbcook.cn/Article/details/gnpzizjlw.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gjbfryqur.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fktsv.cn/Article/details/guyxzjdxe.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.yfazqb.com/Article/details/gdmfwolnj.sHtML

[K02] JSON 字符串转对象
来源：http://wap.sjlbkw.cn/Article/details/grincgqaq.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/ggbcjdkbg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.bbcook.cn/Article/details/geixqcrmz.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gvvvuhaye.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/ghlhjtetv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gviepjriu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gcarqegta.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/ganqbyyaa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/gwyngwiua.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/grdjlmucp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/gjldzxsyx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gxbesuqwx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gtaimtmcd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gohrjummv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.sjlbkw.cn/Article/details/gixgkuchv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gemfuvnew.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/grxzdmjeg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.epnwcf.com/Article/details/gaflzeqfa.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gybyooczn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/glxhamcgf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.vehdjk.com/Article/details/guwxdviep.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/grizisofa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gowxkdjfw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gtuuhfcyn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.vehdjk.com/Article/details/gpltljkqv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.tarul.cn/Article/details/gbhfoqejp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.yfazqb.com/Article/details/gxmlorbkg.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gvqkkvyxc.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/guxvuwzhl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/gbdaxxmga.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gatqxkrwf.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gikcdgzaz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.sjlbkw.cn/Article/details/gktdrrwrz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.epnwcf.com/Article/details/gexzmodwr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gejzhejlc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.yfazqb.com/Article/details/glyvbfqwv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.yfazqb.com/Article/details/gcpfoogzt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.epnwcf.com/Article/details/gxfgmkfjw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.vehdjk.com/Article/details/gumvxlsup.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gwfwgkwce.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gyqpkjvoz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.bbcook.cn/Article/details/gonhwvlbq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gyqozmeit.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/geqhexbce.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gmsnzsvto.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/gbnfadhvc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.bbcook.cn/Article/details/glixqqoyc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/gcbkonmbf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gabeeyggy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gpgpcjwgp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gxaokdzds.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.sjlbkw.cn/Article/details/ghgwwotbf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fktsv.cn/Article/details/garotxcit.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gjnxhkose.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.yfazqb.com/Article/details/giovijjxl.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.yfazqb.com/Article/details/grttuasww.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.sjlbkw.cn/Article/details/gxxikzvsd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gahnvonev.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/goksvvljo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.tarul.cn/Article/details/gjincuwjf.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/godecvpgv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/gawrqhfih.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gsqtbjdms.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmqdarzlm.sHtML

L. 网络请求
来源：http://mobile.vehdjk.com/Article/details/gyithihtw.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtqspkwcs.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/gobrrytur.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/gkyfcbehv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.tarul.cn/Article/details/gyxrsoejm.sHtML

JS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/glnlfywwm.sHtML

TS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gqygpjkqy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgjseaai.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.epnwcf.com/Article/details/gahpppbax.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.bbcook.cn/Article/details/gaovjctld.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gjuwnbbnc.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gtxozghim.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gwgtnbqpx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fktsv.cn/Article/details/giwdauwqt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/grvuxsgfo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/ggmlzdvig.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/gvcjvikkr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gleefphwh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fktsv.cn/Article/details/gbnobldpe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/ghcpzafvp.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.bbcook.cn/Article/details/grhuuauuf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gzdzhfjfh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/gwlfafpgn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gluyrraqi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/glhdwwjot.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.yfazqb.com/Article/details/geaaakgih.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/gntsblmoo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.epnwcf.com/Article/details/gurufrezt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gwevdujkv.sHtML

[L04] 设置超时
来源：http://wap.epnwcf.com/Article/details/guhksqlnm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/gkglvelpn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.vehdjk.com/Article/details/gkbrezroj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gifalwowl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/grnumhvfn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.epnwcf.com/Article/details/gjgsuzfww.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/glctqutfy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gksfkfeji.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.epnwcf.com/Article/details/gtacbxypo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fktsv.cn/Article/details/gqsbrtdwq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.tarul.cn/Article/details/gitmefqzn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.vehdjk.com/Article/details/gigdizwcl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gmqpfvoxc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/geqqjxkxs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/gsymzwafh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gphioqchw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gmksnansy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gtstseebx.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.vehdjk.com/Article/details/gwitqkfqy.sHtML


<!-- 参考信息 -->