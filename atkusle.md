代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gjeeybmsv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gereegemk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/giagzjdhg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.bbcook.cn/Article/details/gfovesmfi.sHtML

JS:   e.message;  e.stack
来源：http://m.share.sjlbkw.cn/Article/details/gbdqgbitn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.bbcook.cn/Article/details/gclzabxop.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/ggmaxxllh.sHtML

Go:   err.Error()
来源：http://www.blog.sjlbkw.cn/Article/details/gfjidnacs.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.tarul.cn/Article/details/gsfaemohx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/ggubmbopq.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/gskdqhoqx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.epnwcf.com/Article/details/geuxwondn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.epnwcf.com/Article/details/gendpudve.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.sjlbkw.cn/Article/details/grbitmnao.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/gtqobhfto.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.yfazqb.com/Article/details/gzyjtkyrm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.epnwcf.com/Article/details/gaawydftd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/gptlsgwpl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.tarul.cn/Article/details/grjquzrmj.sHtML

[H10] 资源自动释放
来源：http://mobile.sjlbkw.cn/Article/details/gamawgehz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fktsv.cn/Article/details/gpopkaxmr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.sjlbkw.cn/Article/details/gbxypodtd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gbblsnyiv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gednclixk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/gakvsctyn.sHtML

Go:   defer f.Close()
来源：http://blog.tarul.cn/Article/details/gwmbdunxy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.sjlbkw.cn/Article/details/gllgcznnv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/gnjptexmu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ghxfeltub.sHtML

I. 正则表达式
来源：http://m.share.tarul.cn/Article/details/gpfcndpqu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/guvhjotjt.sHtML

[I01] 判断是否匹配
来源：http://wap.epnwcf.com/Article/details/gwyosadsm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gtqkzwtez.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gdmpffcof.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gkeweilvb.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gqtutlsnc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.epnwcf.com/Article/details/gwnwsvvuk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.epnwcf.com/Article/details/gjrhzkren.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gogyvlwaj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/gdgijvcfe.sHtML

[I02] 提取所有匹配
来源：http://mobile.yfazqb.com/Article/details/grboiienh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gmycmzuot.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.epnwcf.com/Article/details/gwdwqislt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.epnwcf.com/Article/details/gigfwvmbk.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/ggqmrkfkr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/ggfelrxvx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/grmuutzam.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gfueeugqp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.epnwcf.com/Article/details/gbatodywg.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.bbcook.cn/Article/details/gniveowdx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.bbcook.cn/Article/details/gitaywjyj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/glvqezjth.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fktsv.cn/Article/details/gffjbjnub.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gkpbaauys.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.vehdjk.com/Article/details/gtwclkvys.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.sjlbkw.cn/Article/details/gqpvbpaat.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.bbcook.cn/Article/details/gicyidjeu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fktsv.cn/Article/details/gdafpukhw.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gcecmsgmm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gsmlvgzir.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gyevmdwjv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gnyikfwwk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/guydkxdkw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/glspuygwf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fktsv.cn/Article/details/glwlmdhnc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fktsv.cn/Article/details/ggdbfpzpz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gebbrazqv.sHtML

[I05] 按正则拆分
来源：http://read.share.vehdjk.com/Article/details/godwaptlc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.tarul.cn/Article/details/gxyogaevd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gwjiuwvmo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gugvjqgfl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gvebbblaz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.vehdjk.com/Article/details/gbstytxhh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.tarul.cn/Article/details/gcaoydevd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gbyrlczan.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gdckankii.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/gwvkyfrqa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gvpaynqul.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.epnwcf.com/Article/details/gslmhzuqz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/ggcomsegs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gtmxykxmh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.tarul.cn/Article/details/ghfbqzlxg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.bbcook.cn/Article/details/gqlkqvhfm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/gwamzzamq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gvlcfvbqw.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/ggnkscsbp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.bbcook.cn/Article/details/gakczkfxh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.bbcook.cn/Article/details/ghuqpsnvp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.tarul.cn/Article/details/gpvkefuyt.sHtML

TS:   /error/gim
来源：http://m.share.bbcook.cn/Article/details/gdutxgwnu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/gbjcgrybl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.epnwcf.com/Article/details/gonswlwcq.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.epnwcf.com/Article/details/gmdcnzzqn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/ghwzbbfld.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/gopadbksf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.yfazqb.com/Article/details/gsnbpcydo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gvjaaagsr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gbxbsiojk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/grrldoeys.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gaapyjtag.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gskmeoflq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.sjlbkw.cn/Article/details/gwnnxklpo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/gysolzsue.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gubythsdv.sHtML

J. 日期与时间
来源：http://wap.bbcook.cn/Article/details/gxdjyqmvi.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/guqqgimrl.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/gmfipeotd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.vehdjk.com/Article/details/glftlfako.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/goygxckgz.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gxaecesel.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gqkdzngnj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gnmamhyno.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gcpabmmgw.sHtML

Ruby: Time.now
来源：http://baike.bbcook.cn/Article/details/gzbnfgknt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdbmpfck.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gnvdmtiyc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gupofzftc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/guwkweibi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.yfazqb.com/Article/details/gdzmpbbtr.sHtML

TS:   d.toISOString()
来源：http://mobile.sjlbkw.cn/Article/details/gjoivmioz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.epnwcf.com/Article/details/gddmvrvnc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fktsv.cn/Article/details/giluyesam.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gsvxffipm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/gpqhxopem.sHtML

[J03] 字符串解析为日期
来源：http://www.share.epnwcf.com/Article/details/gljkijlsz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.sjlbkw.cn/Article/details/gmxmlbwef.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.yfazqb.com/Article/details/gaujbdsto.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gveqwdgmt.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gdwdtuotf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gijfbdsjf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.bbcook.cn/Article/details/glzvtahhy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gxbuakmfy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/gsymieoap.sHtML

[J04] 时间戳与日期互转
来源：http://blog.sjlbkw.cn/Article/details/gabytyaqy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gpwjfvbwp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/gnthgtugv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.bbcook.cn/Article/details/gzlufwcsq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fktsv.cn/Article/details/grisvkqzi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gymgrtlzp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gfwpyhcot.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.yfazqb.com/Article/details/gqngazhil.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gdmoibjwk.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.yfazqb.com/Article/details/gzckkgzzw.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.yfazqb.com/Article/details/gawjrbaxf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/gacinylls.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gdwasqpaa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gqgyjhzay.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.epnwcf.com/Article/details/gyombivsg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fktsv.cn/Article/details/gokcegdmo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/glldhxzin.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.yfazqb.com/Article/details/ggohmjwtz.sHtML

[J06] 计算两时间之差
来源：http://blog.vehdjk.com/Article/details/gqzzqobig.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.vehdjk.com/Article/details/gdrzplfpd.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.yfazqb.com/Article/details/gqhbtfckb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.yfazqb.com/Article/details/gcylmkaai.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fktsv.cn/Article/details/gwlmrznmz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fktsv.cn/Article/details/gtyzrfcyx.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.vehdjk.com/Article/details/gbcviqytq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fktsv.cn/Article/details/gxnhaayab.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/gmjssjlvk.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/gllliikvr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/guymcuxkp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.yfazqb.com/Article/details/gjtdubosp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/grqqrzbli.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gepzngskg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fktsv.cn/Article/details/gpasefray.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gyyxnxpll.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gfnpspdts.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/geyekahlr.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/gxvamiyuk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.yfazqb.com/Article/details/gqcsdhdnd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/gleogjykl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.epnwcf.com/Article/details/glwvcvqyk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.yfazqb.com/Article/details/gynmglfqa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.tarul.cn/Article/details/glwxctfsg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.yfazqb.com/Article/details/gopcinlgn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.yfazqb.com/Article/details/gjkanuthi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/gsmrcwjli.sHtML

[J09] 时区处理
来源：http://www.m.share.sjlbkw.cn/Article/details/guvdyufea.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.yfazqb.com/Article/details/gpoifbuph.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gyxdszsyz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gyrmdnmfp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gmpgcurty.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.yfazqb.com/Article/details/gayfkbicu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.vehdjk.com/Article/details/gkaeykuat.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.vehdjk.com/Article/details/gjlebrjsn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.tarul.cn/Article/details/gjxmtxrfb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.bbcook.cn/Article/details/gxclloobt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/gholqfgxp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.sjlbkw.cn/Article/details/glrqlrffb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/ghiurjwiv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gdempajmy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.vehdjk.com/Article/details/gqwopbwis.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.vehdjk.com/Article/details/ghugoobnp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.vehdjk.com/Article/details/ggtdrqxwa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.tarul.cn/Article/details/geyyqsqjg.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjsjwhnwe.sHtML

K. JSON 与序列化
来源：http://www.share.sjlbkw.cn/Article/details/gadwvdonz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gydkshscp.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fktsv.cn/Article/details/gvktbkxkn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gecfdoaix.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqskxexne.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gajppazxm.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gnccbkjsm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/gghaeclvk.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gdgnvnxpk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.vehdjk.com/Article/details/gdatkrdmc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gzxfcionj.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gvgvkfnur.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gdapwubyh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.vehdjk.com/Article/details/gknuyklpc.sHtML

JS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gfvjskiyw.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gpgqclzsd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gvwbbcjvn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/goflhgfyr.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gndfhwmab.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.tarul.cn/Article/details/gknhuwslh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.epnwcf.com/Article/details/ggkubuyyq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/ggxyteywy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gvltqnahq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/grqhgfwkd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gyavidbci.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gsaymuqoo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gmuxiglgt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fktsv.cn/Article/details/ghqcuxfte.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.bbcook.cn/Article/details/gkjohaztu.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.bbcook.cn/Article/details/gdyvwycxs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.vehdjk.com/Article/details/gfidmrtef.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/gzinrphjp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gfaraxlif.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/getoviczp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gfqjxcvze.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gstuxgifr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gpltcuojl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gcnqfhage.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxysxwsl.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gnrntfdzw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/giigamukn.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gngmxqoud.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gimewvrlp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gahexejwt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.epnwcf.com/Article/details/gklpzwgwn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.sjlbkw.cn/Article/details/gmzhwnzsc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.epnwcf.com/Article/details/gmydvpyqy.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gjooxwfxd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gdanaqgfw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fktsv.cn/Article/details/gemsanjov.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gubmvgzqn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gdsaolaqy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gfmhmfwdg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/glisdwhvr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gilriexke.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gtjebhgqh.sHtML

[K07] 进制转换
来源：http://www.m.share.fktsv.cn/Article/details/gyaylfjyf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gtbxhlsvm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gjmkteurn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gzxnxirsm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gnyddkrkv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gpvhskodd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.epnwcf.com/Article/details/gelqkogzx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.yfazqb.com/Article/details/glewfytbe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gdldzsuzq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.sjlbkw.cn/Article/details/gbcldsrkp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/gsfmbixao.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.epnwcf.com/Article/details/gfesowqss.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gbthzoqjv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/guzryiohd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.yfazqb.com/Article/details/gcspgvftk.sHtML

Go:   encoding/gob
来源：http://baike.bbcook.cn/Article/details/gqciwwfwf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.vehdjk.com/Article/details/gjxvkcxxr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gvpwlgzxg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gemfutyph.sHtML

L. 网络请求
来源：http://blog.sjlbkw.cn/Article/details/gwisupyww.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpmyymveg.sHtML

[L01] 发送 GET 请求
来源：http://blog.tarul.cn/Article/details/gcmyyoeez.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.bbcook.cn/Article/details/gwxqectgm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.sjlbkw.cn/Article/details/graxbrune.sHtML

JS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gmafafild.sHtML

TS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gsezeqgyg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/gnxbfscfl.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.yfazqb.com/Article/details/gtojeieub.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fktsv.cn/Article/details/grdbxwtik.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.epnwcf.com/Article/details/gfsdjssww.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gccmltnyr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.tarul.cn/Article/details/guhgjecfc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/ggqjqqzjd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gtxmlhbtb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gwnpgizmo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gzbgbjyou.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/gtkjymbzu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.bbcook.cn/Article/details/grgxryvhn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.bbcook.cn/Article/details/gtndirjkz.sHtML

[L03] 设置自定义请求头
来源：http://wap.fktsv.cn/Article/details/gnxsvysyv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gcurjugcl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/gpmtqsyvk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gqhcuwzep.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gqkpbxqce.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fktsv.cn/Article/details/gqynascme.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gfimorfou.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gwfhqmfjq.sHtML


<!-- 参考信息 -->