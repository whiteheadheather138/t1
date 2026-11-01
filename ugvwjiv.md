代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.sjlbkw.cn/Article/details/gywfjoiaa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.sjlbkw.cn/Article/details/gbsamlfau.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/gizshdvsu.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/gxorhcugv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.sjlbkw.cn/Article/details/gwbxizcxi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.epnwcf.com/Article/details/gvopbldzr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/gregbodcl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/gugmybrft.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/gmexanzsj.sHtML

Go:   defer f.Close()
来源：http://m.share.yfazqb.com/Article/details/ggtvhckix.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.yfazqb.com/Article/details/gukxsoizd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/guxlijmbs.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqutkumix.sHtML

I. 正则表达式
来源：http://3g.vehdjk.com/Article/details/gyoduhbqk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkhtavisx.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fktsv.cn/Article/details/gixtdtasa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gnnosidql.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.epnwcf.com/Article/details/gafogfics.sHtML

JS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gyfezidud.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/gehqjofmq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.epnwcf.com/Article/details/grbhemscj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.sjlbkw.cn/Article/details/gkxgnixkz.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/ggzjhmsui.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gjbdnlsiz.sHtML

[I02] 提取所有匹配
来源：http://m.share.sjlbkw.cn/Article/details/gcwnzdikv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gtvaghmaq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/gqmbxpahq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.yfazqb.com/Article/details/gqsnwxhka.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.bbcook.cn/Article/details/ghhjivtdh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.vehdjk.com/Article/details/gnyqgrwdq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gbjnmcpik.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gcsafpeai.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.tarul.cn/Article/details/gamgpqcrr.sHtML

[I03] 提取捕获分组
来源：http://www.share.bbcook.cn/Article/details/gcgepnvpd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/gvxzunwfc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.yfazqb.com/Article/details/gtsuxzbvw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.tarul.cn/Article/details/gwvqbubcz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.bbcook.cn/Article/details/gyvtapoli.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.tarul.cn/Article/details/gpfshvcyb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fktsv.cn/Article/details/guhcfusta.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fktsv.cn/Article/details/gphfadprs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.bbcook.cn/Article/details/gyfbqfevw.sHtML

[I04] 正则替换
来源：http://m.share.bbcook.cn/Article/details/ggttqnvbt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.tarul.cn/Article/details/gdyqhbvpl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/grmtdzpcb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/ggukjsioo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gxbwgaimw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.bbcook.cn/Article/details/gzyjffixl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.epnwcf.com/Article/details/gkiynxnmo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fktsv.cn/Article/details/gtkvvxyex.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/giztgjvku.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gukwsyzgp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/gxokmzfdv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fktsv.cn/Article/details/gnfvvivcq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gdowdioyh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gzuvvccpx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.epnwcf.com/Article/details/gtcwpinnz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gttjxbezg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gwzonorqs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fktsv.cn/Article/details/gbexqjyxm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.yfazqb.com/Article/details/gqpgjrqgk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gcmutxowy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.epnwcf.com/Article/details/gmaiyimwq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/goilfqjwd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gyncpleez.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gtvtzjchq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.vehdjk.com/Article/details/gpmzdyysc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fktsv.cn/Article/details/ggdorilpa.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gkobikmuf.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.bbcook.cn/Article/details/godeaekka.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.yfazqb.com/Article/details/grokrsvfn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/gscubtfnh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.yfazqb.com/Article/details/gotemcbkk.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gezssabkt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.bbcook.cn/Article/details/gspovrsbv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/gnhzrcwnx.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/ghngccvsq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gyqjkyaah.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.tarul.cn/Article/details/gxkeeyprw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.sjlbkw.cn/Article/details/ghjbktogl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/goufzgkow.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gnlhehzyp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/gchdcmggj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gywdraess.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/gsflfsgmi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.yfazqb.com/Article/details/gmkcspvbd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gxwmiqnus.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/geuhejaoq.sHtML

J. 日期与时间
来源：http://blog.sjlbkw.cn/Article/details/gctodlitc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glpfcdssd.sHtML

[J01] 获取当前时间
来源：http://blog.yfazqb.com/Article/details/gfljcikpd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/gkpduqcgk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gzluyyffu.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gcjblxkoq.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/glqsewbww.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fktsv.cn/Article/details/gijtwszxu.sHtML

Go:   time.Now()
来源：http://www.blog.yfazqb.com/Article/details/glraliroy.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/gdajvsriz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.bbcook.cn/Article/details/gxixoipnf.sHtML

[J02] 格式化输出
来源：http://m.share.vehdjk.com/Article/details/gspxrmuhp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gklztfnfo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/ghjfwadkw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/gbvntfnzo.sHtML

TS:   d.toISOString()
来源：http://m.share.bbcook.cn/Article/details/gqjkjvuch.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.tarul.cn/Article/details/grxlhccdy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.vehdjk.com/Article/details/ggzpuzsge.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/ggdskhsqy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.yfazqb.com/Article/details/gzmlbqvus.sHtML

[J03] 字符串解析为日期
来源：http://3g.fktsv.cn/Article/details/gwwhzxarj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gmqrnjyii.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.sjlbkw.cn/Article/details/gbzmigyfs.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gkqogmqum.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gvktsfikw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gbhsubcsp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/girlrtrsj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gijqyjagx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.tarul.cn/Article/details/gaxdatckx.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.bbcook.cn/Article/details/gjrowzabl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/godzelrwa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.vehdjk.com/Article/details/gpozyldez.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/grrrsfjjj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/goeiutuan.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gpzyjjoqf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.tarul.cn/Article/details/gfccolgfq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.epnwcf.com/Article/details/gczcvnmkn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gehufucsr.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gthilsmsd.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.vehdjk.com/Article/details/gauihbcxe.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.vehdjk.com/Article/details/gswaytrgu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gxtdbuarm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gnxfglkgf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/gylnjvpzp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.tarul.cn/Article/details/gzzfgkdiw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fktsv.cn/Article/details/gmjqmpkwp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.bbcook.cn/Article/details/gmqgsopcq.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/gvaopvhgo.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.tarul.cn/Article/details/gcvgnpzub.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gktczcfuu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/grnqdqnzk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fktsv.cn/Article/details/grezlbwnm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.tarul.cn/Article/details/gvwuiivjw.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fktsv.cn/Article/details/ggwqytrje.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gnfcyrpys.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.yfazqb.com/Article/details/gkdlhrggz.sHtML

[J07] 比较两个日期
来源：http://wap.tarul.cn/Article/details/girfssmhi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gddczalov.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.sjlbkw.cn/Article/details/gzgipzzwf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/ghjplbjlx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gnohmziko.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/ggsnlflnj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gbrpaccnt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gvobodbts.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gcweitspx.sHtML

[J08] 提取年月日与星期
来源：http://blog.vehdjk.com/Article/details/gmgukkxpt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/gthajikiy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.sjlbkw.cn/Article/details/gbudhldie.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gwkbklamn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.bbcook.cn/Article/details/gshjyhfrc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/guhzkfomy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.tarul.cn/Article/details/gsvimwjbi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gsescnkhg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/gywkrrbxw.sHtML

[J09] 时区处理
来源：http://m.share.yfazqb.com/Article/details/gyprdvmss.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.tarul.cn/Article/details/ghcjcvhrc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.epnwcf.com/Article/details/glvipnxun.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gpqmdqffo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gkkygkqot.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.bbcook.cn/Article/details/gpxgxgmhe.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.vehdjk.com/Article/details/gysgzsqkd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.sjlbkw.cn/Article/details/gusirztix.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.sjlbkw.cn/Article/details/glzhtnfhb.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.sjlbkw.cn/Article/details/gzbdvlxhx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkwlfrtn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gwzipqgdw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/gcujujvii.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.vehdjk.com/Article/details/gchhoiuym.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fktsv.cn/Article/details/gzgnyivup.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.bbcook.cn/Article/details/gdntkleew.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.tarul.cn/Article/details/gxkwdeiof.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.yfazqb.com/Article/details/ghyrterqi.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/grwcsnwkw.sHtML

K. JSON 与序列化
来源：http://baike.yfazqb.com/Article/details/gqlvlfvdc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjlumzqtd.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fktsv.cn/Article/details/gqnbkvxax.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gzivkghny.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gnjflsjfi.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/glvrxydxr.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/grgrxagvl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.epnwcf.com/Article/details/gkvemlsxo.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gxtlrcgut.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gglvejdbv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fktsv.cn/Article/details/gkuhbmwyn.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fktsv.cn/Article/details/gaybrlykc.sHtML

Py:   json.loads(s)
来源：http://mobile.vehdjk.com/Article/details/gsebnkakf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.yfazqb.com/Article/details/gsnmbgfdd.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gvoubupba.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gcyykrygb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.vehdjk.com/Article/details/gzerfvgwd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/givsihapx.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnaahdahe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.yfazqb.com/Article/details/gnfizyesl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.sjlbkw.cn/Article/details/gwnwfuiwv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gzqmvxxrv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gsnsrtfkc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gwrhwadtw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/ggtubbcun.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gdzncibrx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gbjgbfrlu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.sjlbkw.cn/Article/details/goikidenv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.tarul.cn/Article/details/grbdbxsnv.sHtML

[K04] 读取 JSON 文件
来源：http://wap.yfazqb.com/Article/details/gfbftgwid.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.epnwcf.com/Article/details/gerhukksp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/grgjcelot.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gpplzsvek.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/giyrfhnod.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.yfazqb.com/Article/details/gcsqjktpe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gsvopplgr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/ganzzswnt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/gntcmycfb.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/gfioqzktk.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/gkzbwylem.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.epnwcf.com/Article/details/geihsqfqz.sHtML

JS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gjhqzvnhs.sHtML

TS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/ggowepjee.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.epnwcf.com/Article/details/garmpwoap.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fktsv.cn/Article/details/gcgtyxgcj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/gfhklzdko.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.yfazqb.com/Article/details/gxxpojsng.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/gbokntlvz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.bbcook.cn/Article/details/grmsztzyi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gbfoudzkx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gpodaadtu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gaojtotjo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/gwuypbosz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gxuhuwicu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gyxrkiadu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/ggcrcmdve.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/gmxfntqcn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gkuzjqzcn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.tarul.cn/Article/details/gtgpfqyxt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/geiakkwtv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/grvpknxol.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gtwrtvcft.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.vehdjk.com/Article/details/glwcpklib.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.epnwcf.com/Article/details/germgovjm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/ggjjkkgcy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.bbcook.cn/Article/details/gjgnvuruf.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/grzwaybxf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gdqqubgxr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/ghlouunzx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gujlohwsn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.yfazqb.com/Article/details/gufeipdhq.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/gkoqbghwc.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.epnwcf.com/Article/details/gpayehnit.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gaqmjbuuj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxluhwvhi.sHtML

L. 网络请求
来源：http://baike.tarul.cn/Article/details/gkzguljie.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnvgczdga.sHtML

[L01] 发送 GET 请求
来源：http://wap.bbcook.cn/Article/details/gxhvcptai.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/ggbazuobl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fktsv.cn/Article/details/gqlrndhnn.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gyxfcemme.sHtML

TS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gcgxdemhr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.yfazqb.com/Article/details/gwsboefkf.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gfbbeuubt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/gjepcvycu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/grttquoyf.sHtML

[L02] 发送 POST JSON
来源：http://blog.vehdjk.com/Article/details/glfruiwvs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gwqbobjad.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.tarul.cn/Article/details/ghoaopqmf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gzzyrdtcy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gooyoujat.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.vehdjk.com/Article/details/gxzhvmryo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.sjlbkw.cn/Article/details/gjgzpzhwn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gvkbccqgp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/gqyeatzvh.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gttrqzubt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.vehdjk.com/Article/details/gharrbtym.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.sjlbkw.cn/Article/details/groxtfobn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gmtusrdgj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gtongzlev.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.vehdjk.com/Article/details/gltkcqigf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gzfbmsqvb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fktsv.cn/Article/details/gygfctzhx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gwjlqukli.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/gxoeblxjp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/gsdqzfdxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/gmxpmajmy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gzefqegcj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlhrwkkj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.sjlbkw.cn/Article/details/guhvlfngq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/gbfroipta.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/gnaadztjc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gstvqetau.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.sjlbkw.cn/Article/details/gxqbotxsi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gcqpxnqzj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gmlalkjot.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gtysurfwc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/grqinfthd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/gzqbaczxg.sHtML


<!-- 参考信息 -->