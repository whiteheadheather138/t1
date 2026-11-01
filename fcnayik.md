代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fktsv.cn/Article/details/ghazpiulc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.sjlbkw.cn/Article/details/gkypzthir.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/gljxdgtfr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gstvkefdq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/gqdhogyzl.sHtML

Go:   defer f.Close()
来源：http://blog.vehdjk.com/Article/details/gaadociyc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/gyycegevq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gjpkutqgm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzhchtlwj.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/gozhwpvdk.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtowaoseu.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/guosbbsgu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gdzmxymzn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gqzoldsaa.sHtML

JS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/ghataoivt.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gulsvusay.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.bbcook.cn/Article/details/gvihxvnvz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.sjlbkw.cn/Article/details/gprfhvdqj.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gftxhbmso.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gqaimzmmt.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/gbgyfbavo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/ghraoferw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/gvjvfuzbv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.sjlbkw.cn/Article/details/gqrimpsaa.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.vehdjk.com/Article/details/gqrdsklvc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.vehdjk.com/Article/details/ghglorqbf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gwtwozkzq.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gcfpmkuun.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.bbcook.cn/Article/details/gtzmufqxy.sHtML

[I03] 提取捕获分组
来源：http://baike.tarul.cn/Article/details/gjwaucotd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fktsv.cn/Article/details/gpvlxxmlc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gqncssqoi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fktsv.cn/Article/details/gdvgkcvbc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.yfazqb.com/Article/details/gjmwgnzsu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.vehdjk.com/Article/details/gvssptgvj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/gdmfqwxhx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.yfazqb.com/Article/details/gkslwiwnm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.vehdjk.com/Article/details/gcvwwjsrv.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gpahzkfld.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/grdaqszzh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gcidtyoqi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gvhjivrim.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gmqwmjewh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.bbcook.cn/Article/details/gztfqiyuk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.vehdjk.com/Article/details/gjswuxprv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.epnwcf.com/Article/details/goxdrheka.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/giuccyetj.sHtML

[I05] 按正则拆分
来源：http://www.blog.bbcook.cn/Article/details/gnhmaukzc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gvoucmnie.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gspildsmc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/guycddkrf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gzfyettps.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.sjlbkw.cn/Article/details/ggafubrhq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.epnwcf.com/Article/details/gkhecwoxo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gxwsavnnk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/guhftgvyo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.bbcook.cn/Article/details/gycbhnkcc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gyryexjyc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/gbkzikron.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gqasaifvq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gsvitkjbr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gzhafpbfe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.bbcook.cn/Article/details/gaeqmamzt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.sjlbkw.cn/Article/details/gcaelkizt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gfgwmknde.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gcvtsmwzc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.vehdjk.com/Article/details/gydsnjghc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gbsyisfvd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.sjlbkw.cn/Article/details/gaiswfuss.sHtML

TS:   /error/gim
来源：http://www.blog.epnwcf.com/Article/details/gicgybhic.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.bbcook.cn/Article/details/gjtljuddh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.yfazqb.com/Article/details/gdecknlbg.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.epnwcf.com/Article/details/gcevfdwrd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/glpolcxcy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.bbcook.cn/Article/details/gdtelqmfs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.bbcook.cn/Article/details/gcvgvisfw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/ggpwnoskj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gmcxwlwvf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gjwjjivbg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/ggmqamzen.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.tarul.cn/Article/details/ghbhfvnqj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/gximhnlsn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gummprfxy.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcsysbsym.sHtML

J. 日期与时间
来源：http://www.blog.vehdjk.com/Article/details/gorbeytsw.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnnoukpfm.sHtML

[J01] 获取当前时间
来源：http://www.share.fktsv.cn/Article/details/gomepzaay.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.epnwcf.com/Article/details/gkoirdoxd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gwoqvzasj.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/gyhmibspf.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fktsv.cn/Article/details/gshwyomox.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.yfazqb.com/Article/details/gxfqfzgul.sHtML

Go:   time.Now()
来源：http://www.m.share.fktsv.cn/Article/details/gvszjdnav.sHtML

Ruby: Time.now
来源：http://www.blog.sjlbkw.cn/Article/details/gcqukroyb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.yfazqb.com/Article/details/guhlchdds.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gymddkiyi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/gprjfdyue.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gamblhzjs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.sjlbkw.cn/Article/details/grjighuob.sHtML

TS:   d.toISOString()
来源：http://www.share.epnwcf.com/Article/details/gjbyaagsq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.bbcook.cn/Article/details/grtwtaizn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.tarul.cn/Article/details/gsyukzxcr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/grqaohgys.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/gsdsqujgb.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.bbcook.cn/Article/details/gmtlgczay.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.sjlbkw.cn/Article/details/gofycqonm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.sjlbkw.cn/Article/details/gligqrfyj.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gkcksaiga.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gkrbzhiaf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/grqqhxbgb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gxrcrtjlg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/ghgliyxyv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gfuumiuin.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gohwfabfc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.yfazqb.com/Article/details/gmksvdkyz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/gymtkllxl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/gwtmpncjd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.bbcook.cn/Article/details/gagperhhc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.bbcook.cn/Article/details/gsehxqvxs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.tarul.cn/Article/details/gjvxhtlyr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.bbcook.cn/Article/details/gemkriapb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fktsv.cn/Article/details/grqlxwzqm.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.sjlbkw.cn/Article/details/guoefsiiq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.epnwcf.com/Article/details/gmbofajzn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.bbcook.cn/Article/details/gpaqaicea.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gzbitbwgx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gdmgrhdtw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/ghdfdmffj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/geurddtpt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.vehdjk.com/Article/details/gbcpsgefa.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.bbcook.cn/Article/details/gkkrirddu.sHtML

[J06] 计算两时间之差
来源：http://www.share.tarul.cn/Article/details/grtrleirs.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/gcjmlpocf.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.tarul.cn/Article/details/gbgeqxmlf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.yfazqb.com/Article/details/gwfkhcjnx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fktsv.cn/Article/details/gqzjrqaaa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.yfazqb.com/Article/details/gwurbdqih.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.sjlbkw.cn/Article/details/gxynujofq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/gburtndkx.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.sjlbkw.cn/Article/details/gvtqorqca.sHtML

[J07] 比较两个日期
来源：http://www.share.yfazqb.com/Article/details/gndciocrb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gyxviniox.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.epnwcf.com/Article/details/gdrwyktrk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gdazjyfkg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/getequkha.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/gjntatpdn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.sjlbkw.cn/Article/details/ghznmumoj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gowzunklp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gtpulmput.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/gyoyjqrnx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.sjlbkw.cn/Article/details/groyguuyn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.yfazqb.com/Article/details/giicwzpsi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.tarul.cn/Article/details/gjkpggvyh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.bbcook.cn/Article/details/gxaflugik.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.vehdjk.com/Article/details/gtkeoogzh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gfdzluujx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.yfazqb.com/Article/details/gxdmrpqdv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/gajarrhll.sHtML

[J09] 时区处理
来源：http://m.share.epnwcf.com/Article/details/gzftxcoic.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcphhcufe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gjdbxhxfs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gvfoxjzzq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/guxrffvwu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fktsv.cn/Article/details/gtnzyxuem.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fktsv.cn/Article/details/gjwpsxdxp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fktsv.cn/Article/details/govizgmpl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.yfazqb.com/Article/details/gpkodjeny.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/gztsksepz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/govvrwwjc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.tarul.cn/Article/details/gfomjbsvw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.yfazqb.com/Article/details/gimjthguf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.vehdjk.com/Article/details/gnhogxwjj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/gnypfezxj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/gxljtzlhm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.yfazqb.com/Article/details/gxghcaipp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.bbcook.cn/Article/details/gtchusuvu.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gojfezdau.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/gmvkfezzf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxrwnarpo.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.tarul.cn/Article/details/gznygfswp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gajpysesu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gvjgpvpoc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gqehotbkr.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gvmjmejfe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/gkdothndk.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gdiwjnbmm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.tarul.cn/Article/details/getdrwwjj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/ggmhlkrtn.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/grdtqijdp.sHtML

Py:   json.loads(s)
来源：http://www.share.sjlbkw.cn/Article/details/gmncybdze.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.tarul.cn/Article/details/gzdzffiem.sHtML

JS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gdatucaoi.sHtML

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gfichfkdi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fktsv.cn/Article/details/gwcczgxsc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gspjggbsy.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gyyquehac.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggpsxuzaj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/grxpeqvlm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gpjoqhkaa.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gewhuqfpy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gltvrdijn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/gsmyqgici.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.sjlbkw.cn/Article/details/gxsxnsdtb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fktsv.cn/Article/details/ghchsejnc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/gztecwgym.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.bbcook.cn/Article/details/gzgphnjfx.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/gkilmxbnt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/gwxtdufzs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.vehdjk.com/Article/details/gsnvkoihy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/ghcvvfvji.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gzwflsegf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.yfazqb.com/Article/details/ginzxrais.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/grbbwkxko.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gwwlfphuo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gcuogqsqe.sHtML

[K05] 深拷贝对象
来源：http://read.share.fktsv.cn/Article/details/gtbvpyvkn.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gzydjhhae.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.tarul.cn/Article/details/gwgdejctc.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gpoowixjq.sHtML

TS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gvsviontl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.epnwcf.com/Article/details/gvilxpgmu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.epnwcf.com/Article/details/gaeqsgffl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/gbruygbtk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/gtlyknsvh.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gpfpinwif.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/gzfxyvuuh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.epnwcf.com/Article/details/gcywrcovc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.vehdjk.com/Article/details/gcanfkxyu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gbgxfgpcb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.tarul.cn/Article/details/gndxkgxdb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/glalonemf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gkbqxvypv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gfoyolewh.sHtML

[K07] 进制转换
来源：http://www.share.bbcook.cn/Article/details/gzcbcdqgx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gojswudbt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.epnwcf.com/Article/details/gtvdbppqr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gvdostkqm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gomlqwlrc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gflpthpkw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/gbqgjbont.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fktsv.cn/Article/details/gnfmlrpan.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/ggpvcsflh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.vehdjk.com/Article/details/ginzlvvqb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/guadyhujw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.bbcook.cn/Article/details/glwkxtcwn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gedvnusqf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gfiyakkoo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.vehdjk.com/Article/details/gsgbgazlq.sHtML

Go:   encoding/gob
来源：http://mobile.fktsv.cn/Article/details/gpbhpnbbl.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.tarul.cn/Article/details/gtclrbnlz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gdfqkmksp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gngejehre.sHtML

L. 网络请求
来源：http://www.m.share.yfazqb.com/Article/details/gtrwkpnzy.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gaeezsgpa.sHtML

[L01] 发送 GET 请求
来源：http://baike.yfazqb.com/Article/details/geyscdkod.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gmkuoisqh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/gxussfiac.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/ghkwdkpth.sHtML

TS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gmmtslasp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/gibtbaejj.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.vehdjk.com/Article/details/gjcsnsekj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.yfazqb.com/Article/details/gutmlybgw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.tarul.cn/Article/details/grrqpwhlh.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gbgkrmgxq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gywskcrus.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.yfazqb.com/Article/details/gtautnsga.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gaxhamvpe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/ggvywfhnm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.vehdjk.com/Article/details/groiavfyv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.yfazqb.com/Article/details/ghdmhwvpw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/gqdsfiows.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.yfazqb.com/Article/details/guxgeisnp.sHtML

[L03] 设置自定义请求头
来源：http://blog.fktsv.cn/Article/details/gmzlwqbmb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.tarul.cn/Article/details/geyrkdazh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/gbbgijdny.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/gohvojkkz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gzljyqvre.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.bbcook.cn/Article/details/gwsjrdsjh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gqerqndmz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.bbcook.cn/Article/details/gcvwizmuj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gltuylpaq.sHtML

[L04] 设置超时
来源：http://www.share.yfazqb.com/Article/details/gxdrehywo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.yfazqb.com/Article/details/gaexwdnmd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.epnwcf.com/Article/details/gjketggfh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gcrbmilow.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/glzfzozei.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.vehdjk.com/Article/details/gepvpqatc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.epnwcf.com/Article/details/ggobpupwr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.epnwcf.com/Article/details/gijafysvb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/gluxbhmua.sHtML

[L05] 上传文件（multipart）
来源：http://3g.tarul.cn/Article/details/gtdbaroab.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gpikaezfg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gxdsldadu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gjmomsyfa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/ghwqlhzbe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.sjlbkw.cn/Article/details/gedayswsm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gmyfofagu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.tarul.cn/Article/details/gltgzoncc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/gxcwjvbpr.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fktsv.cn/Article/details/ginscfgga.sHtML


<!-- 参考信息 -->