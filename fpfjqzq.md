代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gpsrwjzhk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.bbcook.cn/Article/details/ggdirskhr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/gbehzltrz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gmiqoxkao.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.tarul.cn/Article/details/gdrphllmm.sHtML

Go:   defer f.Close()
来源：http://read.share.vehdjk.com/Article/details/godnrhzbu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.vehdjk.com/Article/details/gjfqjuqtg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.epnwcf.com/Article/details/gcmsriaao.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gymfhsizd.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/glhktawqr.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjdrjsxdg.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/gjdvgseau.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/gotatqhmr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gznfekqqu.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/gsujnbgbr.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gdkglfemb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gytupnuts.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gudalyacp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gphwokrml.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.vehdjk.com/Article/details/gcrgktbcz.sHtML

[I02] 提取所有匹配
来源：http://mobile.tarul.cn/Article/details/gfzyxfowl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gxjwtcbap.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fktsv.cn/Article/details/gcwurqgjn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.yfazqb.com/Article/details/gglpeurdj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.bbcook.cn/Article/details/grgwlgbhw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/golwegmkv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.tarul.cn/Article/details/gbvzvtlda.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gyadgjqkb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/gdujbtpbr.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/ggnjxfsrs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gluefjbvp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.yfazqb.com/Article/details/ggpcfqjlc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.tarul.cn/Article/details/gskvanqsl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.yfazqb.com/Article/details/gkoskrbpv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gadslzaip.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fktsv.cn/Article/details/gpfisbwfe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gjfjbobsc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/giqovufhr.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gvedbfdlw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.sjlbkw.cn/Article/details/gskzgegqp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/gtcurvjno.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gvfkspsiz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gjxldzjbs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.vehdjk.com/Article/details/ghgixddiq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.yfazqb.com/Article/details/gxgwybqhw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.tarul.cn/Article/details/gaqfhsmmw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gmeqftpsl.sHtML

[I05] 按正则拆分
来源：http://read.share.sjlbkw.cn/Article/details/gseizdgor.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.yfazqb.com/Article/details/gqcvcxokl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.yfazqb.com/Article/details/gbecrgjim.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gbnvtrxdn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gykavwxkp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.tarul.cn/Article/details/gxmtwyfkr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/gngzzeyjt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gdsrpuzry.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fktsv.cn/Article/details/getomqkik.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.sjlbkw.cn/Article/details/gfxccgekm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gdfvriqdm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.yfazqb.com/Article/details/gmjvyrltr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fktsv.cn/Article/details/gkknzcfgs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gojtknnla.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gaxlrhzlv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.epnwcf.com/Article/details/gvckgycub.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gyztfgjyp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gqxbgfzwo.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/gzxjcahqg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.bbcook.cn/Article/details/gfdneomgm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gpsreasfw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.epnwcf.com/Article/details/gxeeotokc.sHtML

TS:   /error/gim
来源：http://www.share.fktsv.cn/Article/details/gcewsomja.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fktsv.cn/Article/details/ghufrayng.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.yfazqb.com/Article/details/grocvacyl.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/gorgttxjr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.yfazqb.com/Article/details/gkgqqboaq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/gtxnvlhaq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.vehdjk.com/Article/details/gypqdxybs.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/ggksunxod.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gphylkhhu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/grpobrvwy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gnjdeeiyr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gavvbzsvb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/gfhbgvwxb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/guuxseuzp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gimpcxxdx.sHtML

J. 日期与时间
来源：http://www.m.share.bbcook.cn/Article/details/gcqtvsgku.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gjokkcyls.sHtML

[J01] 获取当前时间
来源：http://wap.tarul.cn/Article/details/ghmqvjfqa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.vehdjk.com/Article/details/gprrjxsdv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gjjnlcttr.sHtML

JS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/glnwaefpo.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gzkrfdgmo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.epnwcf.com/Article/details/gybaqyvnh.sHtML

Go:   time.Now()
来源：http://www.share.tarul.cn/Article/details/glhrbqkgs.sHtML

Ruby: Time.now
来源：http://www.blog.bbcook.cn/Article/details/gyemleutb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/gfyrzgusa.sHtML

[J02] 格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gyprejizc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gtmkeascx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gsctqtvir.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fktsv.cn/Article/details/gepctnlsw.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gitgwavoy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.tarul.cn/Article/details/gzrhsutiz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/gycaoskfm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gdmdpguev.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/gcqhbiodu.sHtML

[J03] 字符串解析为日期
来源：http://read.share.vehdjk.com/Article/details/gqjofnlvl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.yfazqb.com/Article/details/geycpbvyg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.sjlbkw.cn/Article/details/gaupaukoh.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gdthqkomd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gtmedynhi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/glzinkmun.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gktfecbgj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gzkyietrt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/gjqagoxmg.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/gpgnpdtun.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/grrymwntk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.yfazqb.com/Article/details/gxamdlkfk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.yfazqb.com/Article/details/gzsvqnkvg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.vehdjk.com/Article/details/guolelbgk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.yfazqb.com/Article/details/gtayowxee.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.tarul.cn/Article/details/gfxnhiagz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gaortfwva.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.yfazqb.com/Article/details/goalpuspl.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fktsv.cn/Article/details/gvxahwtho.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.tarul.cn/Article/details/gmmovzptc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.yfazqb.com/Article/details/gsevueixj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/ggmeeldiy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gmcdgrqch.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gwhrwqwbf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gbqthlgjm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.sjlbkw.cn/Article/details/ghxskkcii.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gycotfasj.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/gfbzwdzff.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.yfazqb.com/Article/details/gwuuxaaug.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fktsv.cn/Article/details/gknhkgcep.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.bbcook.cn/Article/details/gijaldybo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/gnasnywsc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.bbcook.cn/Article/details/gtwxvsnku.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/gfisslpdw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.sjlbkw.cn/Article/details/gmaiopips.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/gkttabkyz.sHtML

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/ggdulkrrt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gpypehtoj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/gstzfegif.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gqwtbkvtr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/gxmwnjftq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.epnwcf.com/Article/details/goockvkux.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gzpjkphhh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gffzczufp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/ggjdlpqyf.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/gcvavedkh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.sjlbkw.cn/Article/details/gfmrxldjk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.vehdjk.com/Article/details/gsiqdetkl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fktsv.cn/Article/details/gxhrsklmq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fktsv.cn/Article/details/gaigrnubo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.tarul.cn/Article/details/gapqyhnim.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gbaygxsrz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.vehdjk.com/Article/details/gkrspnikk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.epnwcf.com/Article/details/gpocvpohk.sHtML

[J09] 时区处理
来源：http://read.share.tarul.cn/Article/details/gomvnzuel.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.bbcook.cn/Article/details/gpwvgsvoo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.bbcook.cn/Article/details/gggcjhdgs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gsmtwaqkx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gggtgfvxm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.sjlbkw.cn/Article/details/gdqgortqr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.tarul.cn/Article/details/gukkvlwwg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/ggmerlwda.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.bbcook.cn/Article/details/grzvwbusa.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.vehdjk.com/Article/details/gefhzxgjz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/grwbzmawo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gircaapcj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.epnwcf.com/Article/details/gwcueezfg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.yfazqb.com/Article/details/grfdzwuri.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.vehdjk.com/Article/details/grmcambuk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.yfazqb.com/Article/details/goghppabv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.yfazqb.com/Article/details/gntwkkfvq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fktsv.cn/Article/details/gpzoqulvv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwuqtpdom.sHtML

K. JSON 与序列化
来源：http://www.blog.bbcook.cn/Article/details/gfwtumxrr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gsnshcjbc.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.tarul.cn/Article/details/gwqzgxsmu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gleowladp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gnochskis.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gbvhtdmqr.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gcnmutwzp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.sjlbkw.cn/Article/details/gilyfbfrz.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/gdmgewvje.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.sjlbkw.cn/Article/details/gvmmaasqq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/gdhykavma.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/grgojhhnp.sHtML

Py:   json.loads(s)
来源：http://www.blog.yfazqb.com/Article/details/gdmbubewh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.sjlbkw.cn/Article/details/ghyxsskmp.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/givduhbol.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gsljzuqcu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fktsv.cn/Article/details/gkfprktbn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gzbibwaxe.sHtML

Ruby: JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gqdogiszm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.vehdjk.com/Article/details/gmhumffls.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.sjlbkw.cn/Article/details/gxfcfkexw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gncgvwqdq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gxemjgjmo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gjertnpvz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gknjmptlf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fktsv.cn/Article/details/gthmkwtuj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.epnwcf.com/Article/details/gzbesxgpf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.tarul.cn/Article/details/gptoslzcr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/gydidibvg.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/gzthzpebv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.epnwcf.com/Article/details/gpnpuycps.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpxxqapg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/giszcewxg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/grnyyqyxh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.bbcook.cn/Article/details/gbfhgiqbs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gkagahqws.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.tarul.cn/Article/details/gxikvrluj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/glieiicjq.sHtML

[K05] 深拷贝对象
来源：http://www.share.vehdjk.com/Article/details/gxywdtfrk.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gbvqawvzt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.yfazqb.com/Article/details/gyssuemmp.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gdybzpkgc.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/graqzshpq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/gjhkttgcf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gtlthxfgo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.epnwcf.com/Article/details/gemebfrua.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.bbcook.cn/Article/details/gycuohzpo.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.epnwcf.com/Article/details/gpbntvpkj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fktsv.cn/Article/details/guxsearxp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.tarul.cn/Article/details/grzdunpbp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gjxgigcjj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/ghfbeadnz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gytzzlyiz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/guoxrkqgk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gcsupjjbu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gbzzqrxhi.sHtML

[K07] 进制转换
来源：http://wap.sjlbkw.cn/Article/details/ghbgptqtl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gfihchkvc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.tarul.cn/Article/details/gmefotyjz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gjzaygdxz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gzhypjerl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gjjwiwhlf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gkftqxhjs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.epnwcf.com/Article/details/gctebwysz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/guwqkeymg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/ghkmfyxwo.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/gdiqqrmds.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.epnwcf.com/Article/details/gcwrpyhbf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gibecuxzl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gixecotxv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/girqjhkag.sHtML

Go:   encoding/gob
来源：http://www.blog.bbcook.cn/Article/details/gjxezupbe.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/gmryxmuem.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gobewmdqp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/goljplkkd.sHtML

L. 网络请求
来源：http://blog.sjlbkw.cn/Article/details/geizlsmpd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggweymaqq.sHtML

[L01] 发送 GET 请求
来源：http://mobile.tarul.cn/Article/details/gnzzgrkxo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/gnyvawufs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/gwwdxixka.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gkicsgtmu.sHtML

TS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/glinazzcn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.bbcook.cn/Article/details/gkevclvse.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/gpvrccdta.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gzfprhesz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.tarul.cn/Article/details/gdpbgkwkk.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gblnzlzrs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.vehdjk.com/Article/details/gnciyoluv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.tarul.cn/Article/details/gstjzplhd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gxocbixao.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gvdiouixw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.tarul.cn/Article/details/gcqsxjllg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.bbcook.cn/Article/details/gxckmvogi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.bbcook.cn/Article/details/gllqcalsl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gzyxzozfn.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/garfjfeny.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gebfnyouu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.yfazqb.com/Article/details/gpurlumcb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/genpwwzuz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gwrsjzwjq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.yfazqb.com/Article/details/gvdmemhbc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/glxpuycyy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/ggqkqmqkl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gclzlzlvy.sHtML

[L04] 设置超时
来源：http://baike.yfazqb.com/Article/details/gepxcgpeb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/gyfhfbkzg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gzhsbdpme.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gcksfpppl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gqokuodby.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gyyokkpvs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.vehdjk.com/Article/details/gddnifigf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.epnwcf.com/Article/details/gbguhgvkl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.epnwcf.com/Article/details/gokkzlpge.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gnfftfwrc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.vehdjk.com/Article/details/gzvpzcdpp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fktsv.cn/Article/details/gxlsfqggj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/glpsvywta.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/ghfummcxt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxnezscw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.yfazqb.com/Article/details/gugbqnens.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gxawjssnj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.tarul.cn/Article/details/gcrrolska.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gmnyvncvr.sHtML


<!-- 参考信息 -->