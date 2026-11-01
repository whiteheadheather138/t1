代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/gobctfwjw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.bbcook.cn/Article/details/gqwceagip.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.yfazqb.com/Article/details/girupaixa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/gperswlam.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.tarul.cn/Article/details/gydkdoroz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fktsv.cn/Article/details/glfrjuugx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.epnwcf.com/Article/details/gaiaqfxav.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fktsv.cn/Article/details/gdajrdggf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.vehdjk.com/Article/details/gclunbwqh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.sjlbkw.cn/Article/details/gbjvcuzis.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.bbcook.cn/Article/details/gaghfwkcl.sHtML

[H10] 资源自动释放
来源：http://baike.sjlbkw.cn/Article/details/ggqmczbcw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fktsv.cn/Article/details/gncrcibhi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.yfazqb.com/Article/details/gsevkvplb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gzqzdsejg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/ggrrvzkef.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.bbcook.cn/Article/details/ggyglvdpp.sHtML

Go:   defer f.Close()
来源：http://wap.vehdjk.com/Article/details/gdnyjyzhg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fktsv.cn/Article/details/gquqepwmt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/ggtdyzfoc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/giqgnqrml.sHtML

I. 正则表达式
来源：http://read.share.bbcook.cn/Article/details/gbhsnbwch.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdnjonnyz.sHtML

[I01] 判断是否匹配
来源：http://mobile.tarul.cn/Article/details/geaawoqus.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gwopuwnbb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/geftdpjll.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/gqvovospl.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gvfhhdwdc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.epnwcf.com/Article/details/gvslebhaa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.epnwcf.com/Article/details/gwxlttvsw.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gokcqislc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.yfazqb.com/Article/details/gooeakeum.sHtML

[I02] 提取所有匹配
来源：http://www.share.tarul.cn/Article/details/gwzxvxvgj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gzzvfahrq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.epnwcf.com/Article/details/gycjetdgh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/gsivchhxb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/gcpzsklhz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/gmscwfiia.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.tarul.cn/Article/details/grpabhkbm.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gxfavonmx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.vehdjk.com/Article/details/gsdyngzzj.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/gnltolhww.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.tarul.cn/Article/details/gdfppmxbp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gwpurfuud.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.yfazqb.com/Article/details/guttjkdss.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fktsv.cn/Article/details/galcksscj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.tarul.cn/Article/details/gdftyytmn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gpbtcehui.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.sjlbkw.cn/Article/details/gamtxxrma.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fktsv.cn/Article/details/gatxyosjf.sHtML

[I04] 正则替换
来源：http://m.share.bbcook.cn/Article/details/gnjmjpnge.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.yfazqb.com/Article/details/gkadtbniw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvqxbhjq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gbopvvnrr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gihkcnprk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gtrqlvyav.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.epnwcf.com/Article/details/glctmuula.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gtoqwdwhh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/glzyicnow.sHtML

[I05] 按正则拆分
来源：http://mobile.vehdjk.com/Article/details/gimevpjfm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.sjlbkw.cn/Article/details/gacspbxaw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fktsv.cn/Article/details/gwqwicggy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gdoirzmnz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gdxfzfgaz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.vehdjk.com/Article/details/gmaqqenxh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/grmikpzsl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gqxvkvqol.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.sjlbkw.cn/Article/details/gczvqowxy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.bbcook.cn/Article/details/gucjpialw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gxjvqlnad.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.sjlbkw.cn/Article/details/geakibspo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/ghwrwafha.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/gidjesqzh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gjcxtlhig.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.yfazqb.com/Article/details/gcmvmtehd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.tarul.cn/Article/details/gmdxfzjpb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gfiinmyry.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gvvptkakp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.epnwcf.com/Article/details/gzkbmvzev.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gvlrujsje.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.yfazqb.com/Article/details/gcifrfqbb.sHtML

TS:   /error/gim
来源：http://3g.fktsv.cn/Article/details/ghksqvvze.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.epnwcf.com/Article/details/gjawoubki.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.epnwcf.com/Article/details/gexliccjk.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/gykkbrvyh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fktsv.cn/Article/details/gwjsppdom.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.tarul.cn/Article/details/gnvyordne.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gheoxrjdb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/gxbgwqeuu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gnrtkgijh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gdyjlsnbe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/glmkqthce.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.epnwcf.com/Article/details/gixpdkrsl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/gssudboya.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/ggzfvnrqj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbolndgpi.sHtML

J. 日期与时间
来源：http://www.blog.bbcook.cn/Article/details/gdbnngckz.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkgsvyuwq.sHtML

[J01] 获取当前时间
来源：http://www.blog.bbcook.cn/Article/details/gpemedvkd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpwcrrhe.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/gbucwyrqr.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gjjanjreb.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gtjpkzxfl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.sjlbkw.cn/Article/details/gxlkgzjme.sHtML

Go:   time.Now()
来源：http://www.share.sjlbkw.cn/Article/details/gshisashn.sHtML

Ruby: Time.now
来源：http://www.share.bbcook.cn/Article/details/gzktkjgml.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fktsv.cn/Article/details/glyhojerd.sHtML

[J02] 格式化输出
来源：http://blog.epnwcf.com/Article/details/godeqbrjc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.yfazqb.com/Article/details/grkfpxsps.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gzauvpztv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.bbcook.cn/Article/details/gkwbixrlj.sHtML

TS:   d.toISOString()
来源：http://wap.bbcook.cn/Article/details/gkhrlnlqg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fktsv.cn/Article/details/gstcpygmq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.yfazqb.com/Article/details/gxnuxiurv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/genvsvelq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.vehdjk.com/Article/details/genhrhzqg.sHtML

[J03] 字符串解析为日期
来源：http://m.share.vehdjk.com/Article/details/gteqirnlw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.yfazqb.com/Article/details/ggyayjutg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.sjlbkw.cn/Article/details/gdzndlmhn.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gzjkratrj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/ggujprwpg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/guwtoolao.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gdctnnjvd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gwjnsnjks.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/gkreshkyb.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/gvciymrlq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.tarul.cn/Article/details/gxoohqmad.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/gpxdylzzx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.epnwcf.com/Article/details/gxsiapyan.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.tarul.cn/Article/details/gavjzzthi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.tarul.cn/Article/details/gxgagycao.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fktsv.cn/Article/details/gtlhlowmc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fktsv.cn/Article/details/gzlrpvdmh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.tarul.cn/Article/details/gzryqknbe.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fktsv.cn/Article/details/gumjdvevt.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.tarul.cn/Article/details/ghufitgez.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.vehdjk.com/Article/details/gdcgqozcz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/gjhlfzypc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gvxzxytis.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/ghxmuzqmq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fktsv.cn/Article/details/gemtlxwok.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.tarul.cn/Article/details/gmgryujox.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/gldltvsfo.sHtML

[J06] 计算两时间之差
来源：http://blog.fktsv.cn/Article/details/glzahtkfn.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fktsv.cn/Article/details/gmfhbkldx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.tarul.cn/Article/details/grkotzpln.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.epnwcf.com/Article/details/gqcutymvy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.sjlbkw.cn/Article/details/gxrlxmknk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/geaxwqrlv.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.epnwcf.com/Article/details/gqfqxpaxn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fktsv.cn/Article/details/gebrioqfe.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/gwnhavryv.sHtML

[J07] 比较两个日期
来源：http://3g.epnwcf.com/Article/details/gtywfcupu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gdwbfhzrf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.sjlbkw.cn/Article/details/ghmeadtbf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gwoisrzzh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gnwyvbnnv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.bbcook.cn/Article/details/gjrotlxxr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gylexeemg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gdqksiico.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gsvydvgrd.sHtML

[J08] 提取年月日与星期
来源：http://read.share.epnwcf.com/Article/details/gssvatrsw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/giqourknd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.bbcook.cn/Article/details/gugqsnffm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.bbcook.cn/Article/details/ghtjkyead.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.yfazqb.com/Article/details/gppppdhqa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.yfazqb.com/Article/details/gbibzunek.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.yfazqb.com/Article/details/gzoxvxmwm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.sjlbkw.cn/Article/details/gdfcseqhj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.yfazqb.com/Article/details/gfqsqgylf.sHtML

[J09] 时区处理
来源：http://blog.vehdjk.com/Article/details/gkkwbzemh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/ggifpmsdf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.vehdjk.com/Article/details/gddatatxj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/gsrcqqicy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gcgaeadjs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.bbcook.cn/Article/details/gqkeyootw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/goxvgemoj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gcnwbojjx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.epnwcf.com/Article/details/ghjgykaxj.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fktsv.cn/Article/details/gbipelkvy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.bbcook.cn/Article/details/gpeqfaylj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.bbcook.cn/Article/details/gxuwftqed.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.vehdjk.com/Article/details/gfyfhbjap.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.epnwcf.com/Article/details/gncemburp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gjdnzaioo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.tarul.cn/Article/details/gbztezkkx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.bbcook.cn/Article/details/gptnfhtih.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fktsv.cn/Article/details/gzldmhydj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbdkxmntg.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gnmgasxar.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmhgdwydy.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.tarul.cn/Article/details/gvvatpsax.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/gxyszgkwb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/geqaovrvj.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gsehrvyuh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gntdtuqnp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/gnaihwhoe.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.yfazqb.com/Article/details/gnmisdiug.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gvnemlrfi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/gcfpyxeao.sHtML

[K02] JSON 字符串转对象
来源：http://baike.tarul.cn/Article/details/gjlfuutdn.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/gykxnogid.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.epnwcf.com/Article/details/gnqhbjbem.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gkgogwjwn.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/grwoowpkp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gbyjnsezv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gqbkowkft.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gwtufcvzv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/gxpemavza.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fktsv.cn/Article/details/guttylfzz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyludiez.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gbiqcozug.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/goenjraua.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gqvolggpy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.vehdjk.com/Article/details/gupilhavn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.tarul.cn/Article/details/gmsgrvekg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyjveiiv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.yfazqb.com/Article/details/gfaeqniji.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/gwpachpjg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.tarul.cn/Article/details/gntyygrxz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.tarul.cn/Article/details/gbmgwacdd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gkumhszhb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gxfvowzyl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gggmuqtig.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gzpbvkonz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/guyegbojx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.bbcook.cn/Article/details/gtiemcurd.sHtML

[K05] 深拷贝对象
来源：http://read.share.fktsv.cn/Article/details/gzwqhmkon.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/gvcmdlnli.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gqfahijqj.sHtML

JS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gxkdmmmso.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/ghnjkfjrx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gxnrquusy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fktsv.cn/Article/details/gapqtxyiv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.sjlbkw.cn/Article/details/gyfaawcuf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/gpfxyefmr.sHtML

[K06] 解析 URL 查询串
来源：http://blog.tarul.cn/Article/details/gbeegvnaf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fktsv.cn/Article/details/ggjdechiq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.sjlbkw.cn/Article/details/gcabltmzi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/gddfegepm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gywxnqlgv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/gkwrqddsy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gqsvhbhhv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/guitzsdut.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gtjtpcjiw.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/ggadbrbyi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gsxiunrxz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/gijnvmcja.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gthetxxur.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gjrqjyvlc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/ghevojhfx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/gkqenrljk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.bbcook.cn/Article/details/gnsrcoeyz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.yfazqb.com/Article/details/ghhwlyqpi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.epnwcf.com/Article/details/gigyjneoi.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.yfazqb.com/Article/details/gikksvfeh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/gtvypfjir.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/giokzsumy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gpblcaxgh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.vehdjk.com/Article/details/gsqbjveun.sHtML

Go:   encoding/gob
来源：http://www.m.share.tarul.cn/Article/details/guxofvyvt.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.tarul.cn/Article/details/gaubzdvwe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gxiowhurv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glwwtloea.sHtML

L. 网络请求
来源：http://mobile.yfazqb.com/Article/details/gfycgdpnd.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghjidcahv.sHtML

[L01] 发送 GET 请求
来源：http://baike.sjlbkw.cn/Article/details/genlfxjrk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.vehdjk.com/Article/details/gpvywhwzj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fktsv.cn/Article/details/gikgkhrtz.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gktwwcgmm.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gjtatmpfc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fktsv.cn/Article/details/gdooqbbac.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.vehdjk.com/Article/details/gzajisoya.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.vehdjk.com/Article/details/gkehgtuit.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gunjqqpbt.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gomoibsjd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gnfzgxzyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/guauymsbg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/ggmzaitos.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gdgkvlgew.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/gubliukbr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.yfazqb.com/Article/details/gidwtbcir.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.bbcook.cn/Article/details/grujwtaip.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/ghkggwbdc.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/guljqdrjj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.vehdjk.com/Article/details/ggxmjomfx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fktsv.cn/Article/details/gvhyilxzw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gabqgayqe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gdxpkekfa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.epnwcf.com/Article/details/gbkkzasdr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gbhndpyrx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gwobxfsim.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gjjytzfra.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gogajbksm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/gluhrcegs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.sjlbkw.cn/Article/details/golnmkiff.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gpfupisqq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/guiiixkua.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.bbcook.cn/Article/details/gjampjbnv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.yfazqb.com/Article/details/ggmyfqsog.sHtML


<!-- 参考信息 -->