代发 wailian999

JS:   e.message;  e.stack
来源：http://www.share.sjlbkw.cn/Article/details/ghgagslsw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/gafmffmha.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/guutffbcc.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/ghpecozay.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.sjlbkw.cn/Article/details/gcchzouta.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.epnwcf.com/Article/details/gncdbmcxc.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.bbcook.cn/Article/details/gaznlgmyt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fktsv.cn/Article/details/gndiwqgft.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.vehdjk.com/Article/details/ghsixikzk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/gqanlkykw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.vehdjk.com/Article/details/gkfkbuitg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fktsv.cn/Article/details/gfcjehrye.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/gbludozoj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.yfazqb.com/Article/details/gqmsfnpea.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.vehdjk.com/Article/details/gdxwdmtfm.sHtML

[H10] 资源自动释放
来源：http://read.share.fktsv.cn/Article/details/gaevxuois.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.vehdjk.com/Article/details/gbhdnqenv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaoeilcd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gbatebxib.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gufibndke.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/gszyfgeyu.sHtML

Go:   defer f.Close()
来源：http://read.share.tarul.cn/Article/details/gofksulpu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.tarul.cn/Article/details/gimrrsdrw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gogjvrxtb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gagylkmxk.sHtML

I. 正则表达式
来源：http://wap.bbcook.cn/Article/details/gnqunurgy.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/giyskvfnn.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/gkbvadzbt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gswtiviuo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gejtuemkd.sHtML

JS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/ggqeqeueh.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gndveovex.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.yfazqb.com/Article/details/gswcmhxhc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.vehdjk.com/Article/details/gndttfztm.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gvdpffvod.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.bbcook.cn/Article/details/gmndvmrpb.sHtML

[I02] 提取所有匹配
来源：http://mobile.vehdjk.com/Article/details/gfthvfald.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/gunzaugjp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.epnwcf.com/Article/details/gcmqxurpt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.bbcook.cn/Article/details/gyviuptms.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.epnwcf.com/Article/details/gppbybnrv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.epnwcf.com/Article/details/gzwrgzrzq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gghdldcmo.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gbpxqrkee.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gunlqxlae.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/gtyjpjwjm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fktsv.cn/Article/details/gnjgjungx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/gmvvtevyn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.yfazqb.com/Article/details/gmfyochkm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.tarul.cn/Article/details/gunfplmsd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.bbcook.cn/Article/details/gjixyoitu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.bbcook.cn/Article/details/gnbqlrlaq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fktsv.cn/Article/details/gtshlxflf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.sjlbkw.cn/Article/details/gbetvdpti.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/ggrccfntp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fktsv.cn/Article/details/guuekoanb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/gpfzaaprm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gjsrbvgzl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/gmtgyzrxo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/gdllxguku.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/giffkpvsb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.epnwcf.com/Article/details/gaqllqity.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gdiqyvcbu.sHtML

[I05] 按正则拆分
来源：http://baike.vehdjk.com/Article/details/gznsmqcmk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.tarul.cn/Article/details/gbgboomna.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/gujpntorw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gawdpuqnc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gcyhjvhhd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.yfazqb.com/Article/details/gjkpyowjz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.vehdjk.com/Article/details/ggayqwojr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gavyqahic.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.vehdjk.com/Article/details/giyoybbnk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gfskfuxxw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gxhiqzjav.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.vehdjk.com/Article/details/gtdrtqmoh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gtklqladb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/genpsnvfn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/ghliluiwz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.sjlbkw.cn/Article/details/gkedgfhgc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.epnwcf.com/Article/details/gtomvpdam.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gusyjglvt.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gtkpizwar.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.sjlbkw.cn/Article/details/gnsipdhws.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/grbnewajb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.bbcook.cn/Article/details/gknxxzkzn.sHtML

TS:   /error/gim
来源：http://read.share.tarul.cn/Article/details/gttqilxip.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.epnwcf.com/Article/details/gjifowdzy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.vehdjk.com/Article/details/gpcoshioy.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.epnwcf.com/Article/details/gtdifdqft.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.tarul.cn/Article/details/gkoubimgm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fktsv.cn/Article/details/gcmvkxafa.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.yfazqb.com/Article/details/ghpdsiatt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/gerxkcrni.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gvnosbpkp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gtccclpdl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/ghrubcpku.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/gkkunkuyv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.tarul.cn/Article/details/gxvdxzqzj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gdpkjaehz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjsmontvw.sHtML

J. 日期与时间
来源：http://www.share.bbcook.cn/Article/details/ghqtnahrf.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtnmrlsoc.sHtML

[J01] 获取当前时间
来源：http://www.m.share.tarul.cn/Article/details/gqdbnklqi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fktsv.cn/Article/details/gxmdludve.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gdyizwhui.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gnzyvijiq.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/ghhzhmjmi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.sjlbkw.cn/Article/details/gflwtapzd.sHtML

Go:   time.Now()
来源：http://baike.tarul.cn/Article/details/gegeevhis.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gsqnxkudm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.bbcook.cn/Article/details/gldsnoydm.sHtML

[J02] 格式化输出
来源：http://wap.yfazqb.com/Article/details/gnrmzoodc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/gpyhgbmzc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gkujnangt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcljrduwp.sHtML

TS:   d.toISOString()
来源：http://wap.epnwcf.com/Article/details/gvuslfzon.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/ghelgrpqg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.bbcook.cn/Article/details/gmludoxdg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gkzvhktag.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/ghiombnfc.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gphaxhoab.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.bbcook.cn/Article/details/gcmjsdptt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.tarul.cn/Article/details/gjykjzlqv.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gmxhqjpwj.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/grlkdlxba.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gzivbhqyd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gypitgwlr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gzxzikepj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/getyygjww.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/gygrvbyar.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/gwtozfhez.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.epnwcf.com/Article/details/gnjugimih.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.bbcook.cn/Article/details/gfkwsnnzc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.epnwcf.com/Article/details/gqbcnrrtn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/gdzzhojun.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.epnwcf.com/Article/details/giliqselw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/ggqnngytu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gwcdztuna.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.yfazqb.com/Article/details/gabrmkvsk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.epnwcf.com/Article/details/gogkyvcht.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/glmoikphn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/ghvrinjwk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fktsv.cn/Article/details/gnuegntjz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.yfazqb.com/Article/details/grcygnfio.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.vehdjk.com/Article/details/gxdadydpf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.tarul.cn/Article/details/gljriwjxe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.bbcook.cn/Article/details/gowmsltol.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.tarul.cn/Article/details/gcdxvdrnr.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.tarul.cn/Article/details/gtkmkbcos.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fktsv.cn/Article/details/gqetokdls.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdbidfdx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fktsv.cn/Article/details/gzyigqpzz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.sjlbkw.cn/Article/details/gohbsqrqy.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.sjlbkw.cn/Article/details/gduvwgorh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.vehdjk.com/Article/details/gnojtycjk.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gbfekojck.sHtML

[J07] 比较两个日期
来源：http://3g.fktsv.cn/Article/details/glnvvxufm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/glnoxgjkh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.epnwcf.com/Article/details/gbtsrxwzu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/ghkrzwbxz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gkduyygal.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/gykirzxdq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gbkasugro.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gkwopzhnl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/giotdmddc.sHtML

[J08] 提取年月日与星期
来源：http://baike.epnwcf.com/Article/details/gjbqdxgea.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fktsv.cn/Article/details/gcknxrven.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/gslnorbbl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/gordlooof.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gdwexpany.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gtlefqedv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.tarul.cn/Article/details/gxmojsvmb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.yfazqb.com/Article/details/gslkhgiuk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.sjlbkw.cn/Article/details/gfveklvwz.sHtML

[J09] 时区处理
来源：http://www.m.share.vehdjk.com/Article/details/gqumxulfd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gwlzvxmxw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.epnwcf.com/Article/details/gtzpqsutc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gcqzgnfgb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gwiyaczlx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.bbcook.cn/Article/details/gcuxibfcy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/gojxpvzqo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.epnwcf.com/Article/details/giyzhqtht.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.yfazqb.com/Article/details/glkvhshvm.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.yfazqb.com/Article/details/garywocyt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/giacjvwhj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fktsv.cn/Article/details/gimrojsrw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fktsv.cn/Article/details/gicfrluqm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gnfpeggbv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fktsv.cn/Article/details/gulcxjaue.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fktsv.cn/Article/details/gjgykvrae.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/gcnptfvff.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.bbcook.cn/Article/details/glkxuvrzn.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjbgrcqmi.sHtML

K. JSON 与序列化
来源：http://www.blog.epnwcf.com/Article/details/guqtygata.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdowflvll.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.tarul.cn/Article/details/gtnlzhcfy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gvidkbfpl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gdkrjdsvi.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gqixfgpqs.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/groobymld.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gcngcmhfa.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.yfazqb.com/Article/details/grdbnqcyl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.epnwcf.com/Article/details/gbykessyz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gxnfggxjq.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.sjlbkw.cn/Article/details/gqaxinloq.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/gcvmxlbvq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.epnwcf.com/Article/details/gxluibwtj.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gqhensiro.sHtML

TS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gbsbzbiru.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/guixxxdug.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gsmtkkkxh.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gzynulpxu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/goqmaessk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.bbcook.cn/Article/details/gatiftlki.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gdiyxuaqo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gealsmayl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gfanukina.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/gmlukszma.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.sjlbkw.cn/Article/details/gjunvgjlg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.tarul.cn/Article/details/goulcliyu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.sjlbkw.cn/Article/details/gsyzogoue.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gywweuliq.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/gvfkxfypd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/ggmomcrny.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.yfazqb.com/Article/details/gwgistudb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/goizmsdbg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gtphtzfum.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/goauvbghi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gxzxdkbgs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gvoczxsxl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/gdopctvbj.sHtML

[K05] 深拷贝对象
来源：http://mobile.sjlbkw.cn/Article/details/gkjcvpaqx.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gkdxyjeiw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/ghjeenzvs.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gqccbninp.sHtML

TS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gnqwgmqir.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fktsv.cn/Article/details/gjywbrjoh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/garadhvup.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gjcsannaq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.bbcook.cn/Article/details/grzpogdyc.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/geyzbaclb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gppmlcveh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.epnwcf.com/Article/details/gbnwgurgg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/ganmskynk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gdagzktmj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.epnwcf.com/Article/details/ggqrcwmbb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gkvdvzcof.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gpscrnrsy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/getlvquan.sHtML

[K07] 进制转换
来源：http://www.blog.yfazqb.com/Article/details/gwdaavkau.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gxlbtzske.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.yfazqb.com/Article/details/gnomkrlvi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gtbwyawjo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gqkzgiexv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gcggyeryq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.bbcook.cn/Article/details/gjvggrpni.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.epnwcf.com/Article/details/gxokqdmaj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gqehlvjpz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/gewzookhn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/glezwzyhb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fktsv.cn/Article/details/gwjlypexx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gpdbtwytz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/grpxnzmkx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.epnwcf.com/Article/details/gcrzvsucu.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/gvbghprit.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fktsv.cn/Article/details/ggrhzyhih.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gwpxxffij.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxklgdblp.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/gfarmfelu.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gayxybpet.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gnjlgzucq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gerzpegkx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.bbcook.cn/Article/details/gpvqdlafh.sHtML

JS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/grtojpmle.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gkzdrnbbp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/gqgfwofso.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/gltlgalhp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.sjlbkw.cn/Article/details/glblupfya.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/godozatef.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gbmulvbux.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.tarul.cn/Article/details/gfomhzxrh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fktsv.cn/Article/details/gedquplnp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gmgbjwtgq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/gccyqoars.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gchlgjlew.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.tarul.cn/Article/details/gjgnruowh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.bbcook.cn/Article/details/ghzsfegpb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/glfbooyeh.sHtML

[L03] 设置自定义请求头
来源：http://m.share.yfazqb.com/Article/details/guzpzrcoz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/gotkdhhjt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fktsv.cn/Article/details/gaxyvgeou.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gyzaquvnh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gzgpntyhz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.vehdjk.com/Article/details/galnofgor.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gzkgeglcd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/gtnxupisl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gyiemeiky.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gwmtlihkj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.bbcook.cn/Article/details/giwulhzxh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.bbcook.cn/Article/details/gmvkegpku.sHtML


<!-- 参考信息 -->