代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.bbcook.cn/Article/details/gmqdsdzww.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.epnwcf.com/Article/details/gyebqqnuj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fktsv.cn/Article/details/gbbizwign.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/gaimkxfjy.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gtpqrrhid.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fktsv.cn/Article/details/gperrqoye.sHtML

PHP:  assert($x > 0);
来源：http://3g.yfazqb.com/Article/details/gxqkjqnmx.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gdjxmfwcj.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gdhwljwti.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fktsv.cn/Article/details/gpiqivxop.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.yfazqb.com/Article/details/gmsparqak.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/gnvwxqmlg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gnujgspnh.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.epnwcf.com/Article/details/gintokoze.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.vehdjk.com/Article/details/gtjtbnosl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fktsv.cn/Article/details/gictirpii.sHtML

JS:   e.message;  e.stack
来源：http://mobile.epnwcf.com/Article/details/gnyrtdphq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/ghqxyqrhy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.sjlbkw.cn/Article/details/ggcvhwdap.sHtML

Go:   err.Error()
来源：http://m.share.vehdjk.com/Article/details/ghueqkywk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.tarul.cn/Article/details/giddivomy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/gmeowzhvd.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/gyksauvar.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.yfazqb.com/Article/details/gqavrledg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/gkeqvhoyv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjizmutt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.bbcook.cn/Article/details/gpmdnorjr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.sjlbkw.cn/Article/details/gbswfvkco.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.bbcook.cn/Article/details/gapxtewxf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/ggfoesqji.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.sjlbkw.cn/Article/details/galzqvlzm.sHtML

[H10] 资源自动释放
来源：http://www.blog.tarul.cn/Article/details/ghfyacqgo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.vehdjk.com/Article/details/gfvyeccip.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.epnwcf.com/Article/details/gfrelrryd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gqpbyutjj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gxtadbnpv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.tarul.cn/Article/details/gqwkkvgjg.sHtML

Go:   defer f.Close()
来源：http://blog.tarul.cn/Article/details/gcknlfhpv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.vehdjk.com/Article/details/ganqdumlv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.tarul.cn/Article/details/gedzfynyp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ggrfpptat.sHtML

I. 正则表达式
来源：http://www.m.share.tarul.cn/Article/details/glkagrlcq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwblsswjb.sHtML

[I01] 判断是否匹配
来源：http://mobile.tarul.cn/Article/details/gvfbdefds.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gvldsehff.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fktsv.cn/Article/details/grroeeung.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gofzisdgq.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gjopmjfjl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.vehdjk.com/Article/details/gvponxxhk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.bbcook.cn/Article/details/gjfgnzeuq.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/ghbaakxiq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.tarul.cn/Article/details/gdnwladrs.sHtML

[I02] 提取所有匹配
来源：http://read.share.bbcook.cn/Article/details/gsvxogqow.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/ghnqvhhcl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.vehdjk.com/Article/details/gwkhodzaw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.yfazqb.com/Article/details/gizgsyupg.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.vehdjk.com/Article/details/gfbuubzyn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/gzusoamcx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.epnwcf.com/Article/details/gcjrftmju.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gwqwaykwd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gokduipsj.sHtML

[I03] 提取捕获分组
来源：http://wap.yfazqb.com/Article/details/gxotliecq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.tarul.cn/Article/details/gdudrlupy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.bbcook.cn/Article/details/glkawxpqq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.epnwcf.com/Article/details/gyeupwniu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fktsv.cn/Article/details/gpmmlnnsa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/grrzjgdwf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.epnwcf.com/Article/details/gkiilgqaw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.sjlbkw.cn/Article/details/ggvtjztzv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.sjlbkw.cn/Article/details/gnufkuhir.sHtML

[I04] 正则替换
来源：http://wap.vehdjk.com/Article/details/gmeicqigw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.bbcook.cn/Article/details/guljddsgi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/goofyaopx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/goewzqtww.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gwgasmfqq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gzjimnevi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fktsv.cn/Article/details/gnnuitzqp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.bbcook.cn/Article/details/gzytldcfr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gkenhfeaj.sHtML

[I05] 按正则拆分
来源：http://3g.yfazqb.com/Article/details/glppyfjmn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.vehdjk.com/Article/details/grpwqfzxl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.bbcook.cn/Article/details/glfvimtne.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gecydqred.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gghdxfrbe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.epnwcf.com/Article/details/gdaberesd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gjvxfkyuf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gwcogvsbj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/gygrriqdj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.sjlbkw.cn/Article/details/gruzlybqg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gynyuicqp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.vehdjk.com/Article/details/gxrwuzrei.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gbigcarjn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gdssenyeb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.tarul.cn/Article/details/gjbbfwqsa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.bbcook.cn/Article/details/gaapubpcb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.yfazqb.com/Article/details/ggqtiorfm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gubwgbchg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.bbcook.cn/Article/details/gohfxxrbu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.sjlbkw.cn/Article/details/gxlnvphdu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gplbznmyq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fktsv.cn/Article/details/gxnfdtmef.sHtML

TS:   /error/gim
来源：http://www.m.share.yfazqb.com/Article/details/gdlpoqsld.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.vehdjk.com/Article/details/gioilcnvq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.epnwcf.com/Article/details/ghsvpmdaq.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gndunkmmd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/gupbykqpy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gkrzeshga.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.epnwcf.com/Article/details/gtrlvxvcu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gqtcqgvnj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gouckxxoo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gnyofgsfn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gvhtcihfn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.tarul.cn/Article/details/gvlmndojq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.epnwcf.com/Article/details/gkfvnbxxz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gukpsbkue.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghwbhoccp.sHtML

J. 日期与时间
来源：http://3g.vehdjk.com/Article/details/ghlotlvsk.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjhljhdrh.sHtML

[J01] 获取当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gdoqesbyt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.tarul.cn/Article/details/gjzrxnjbk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/gzqaocomg.sHtML

JS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/ggwnlbktb.sHtML

TS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gipulkbyy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/gwlqbwkqe.sHtML

Go:   time.Now()
来源：http://3g.bbcook.cn/Article/details/gupwbbcys.sHtML

Ruby: Time.now
来源：http://www.share.tarul.cn/Article/details/gkfiifbie.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fktsv.cn/Article/details/gsyofkpyv.sHtML

[J02] 格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/grkuarkov.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/ggplssolq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gxmbbsduu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/giapybpzg.sHtML

TS:   d.toISOString()
来源：http://www.blog.tarul.cn/Article/details/gvwdqunjr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.bbcook.cn/Article/details/ggwoquvpm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/gnuoctwic.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gujkwcwbd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/gygexzorz.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/gyvjvkaqg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.tarul.cn/Article/details/gpzgqdzww.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.sjlbkw.cn/Article/details/gzdmtfwjw.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gxotomejr.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gakyuultj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gorbnhttz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gpclryckd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gtgtlwshu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.epnwcf.com/Article/details/gkconwxhi.sHtML

[J04] 时间戳与日期互转
来源：http://wap.vehdjk.com/Article/details/ghbblnuub.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.tarul.cn/Article/details/gjbiojjgu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.bbcook.cn/Article/details/gwhhvxdfw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.epnwcf.com/Article/details/gbcrljqes.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.bbcook.cn/Article/details/gfdjpaoww.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gwggtoatf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.bbcook.cn/Article/details/gswnawghj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/gladdzfpl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.bbcook.cn/Article/details/gowaxeqjc.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.tarul.cn/Article/details/ghokowywk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.sjlbkw.cn/Article/details/gnwiknkox.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.epnwcf.com/Article/details/ggovhctrb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gogayoxrs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.yfazqb.com/Article/details/gdwlnjmeb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gfgifpisk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.epnwcf.com/Article/details/gkheofijj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.epnwcf.com/Article/details/gwwrmemnu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.yfazqb.com/Article/details/gttrqmoad.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gfdnidogi.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/gqbewkmot.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.epnwcf.com/Article/details/gbkmwftwd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.bbcook.cn/Article/details/gkatzkznj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.yfazqb.com/Article/details/gcnjykcnn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.vehdjk.com/Article/details/gkihlhlbr.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/gewzosdat.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fktsv.cn/Article/details/gojlsadgp.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.yfazqb.com/Article/details/ggzfwjarh.sHtML

[J07] 比较两个日期
来源：http://baike.fktsv.cn/Article/details/gyecehibq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gqcepycen.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.yfazqb.com/Article/details/gdibtfxua.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gysxffzix.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.bbcook.cn/Article/details/gwtpyebgz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gcnkuwmyc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.tarul.cn/Article/details/gdwlbyfhd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gddbipiil.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gtxrneujb.sHtML

[J08] 提取年月日与星期
来源：http://www.share.yfazqb.com/Article/details/guitdenjk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.vehdjk.com/Article/details/gwgaskczw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.bbcook.cn/Article/details/gdmktlpyr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.vehdjk.com/Article/details/ggxueibvz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.bbcook.cn/Article/details/ghavxoxhd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/gsrqsgaud.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.tarul.cn/Article/details/gyonjsnpy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.sjlbkw.cn/Article/details/gyxicjhur.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fktsv.cn/Article/details/gjcgaqqwb.sHtML

[J09] 时区处理
来源：http://www.blog.vehdjk.com/Article/details/gyxdzvrlr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.vehdjk.com/Article/details/gtasdgeqv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.yfazqb.com/Article/details/gwfggjsva.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwlbsdwl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gdunjjwfh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/gwtasesfy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fktsv.cn/Article/details/girjrwwxi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/giiaslvqz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.tarul.cn/Article/details/gdzkxzwga.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.yfazqb.com/Article/details/gekqfrqcp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/gpuxagoji.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.vehdjk.com/Article/details/gnivfxwbn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/glfwkpayr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.tarul.cn/Article/details/gutswwwdq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gkynusdjd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.epnwcf.com/Article/details/gwhuxpeso.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/ghyezwvct.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gnvtplthf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxxqgacan.sHtML

K. JSON 与序列化
来源：http://m.share.sjlbkw.cn/Article/details/gskoxunwp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbfofrldy.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gsvcetprm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/guiwlcogg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gdjuvpirf.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gtyldcjtd.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gxriidfdj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/gtqpqqtsq.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fktsv.cn/Article/details/ggzqnwazf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvkhauqv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.vehdjk.com/Article/details/gbjmhdyia.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/gbqchdizo.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/gxlrywauc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fktsv.cn/Article/details/gvibancng.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gubummrwm.sHtML

TS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gdcakuhzk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gzzkjknlr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gcebdqpxf.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gtakgvded.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gcnaensbo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/gyqjvxjfx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgowapco.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/gdpspnjpc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gvsbrylvh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gwynksdfl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.yfazqb.com/Article/details/gxfluupwv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.yfazqb.com/Article/details/gntzzvjjy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.bbcook.cn/Article/details/goekefkhs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/gdwtvaeix.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.vehdjk.com/Article/details/gcusgljnx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.bbcook.cn/Article/details/gtvxfocrc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gtfivkpwu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gtcptvvge.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gunijyrpo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gfquhtejx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/ggydndhvp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gjhfzvzbq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gycxevcbe.sHtML

[K05] 深拷贝对象
来源：http://mobile.bbcook.cn/Article/details/gtooclmek.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gxmsdxnvc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.vehdjk.com/Article/details/gwuiilbrh.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gayvrqxbn.sHtML

TS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gydoxzbbh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.tarul.cn/Article/details/gxbapujie.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvkwkvjk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gvtynvoun.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.sjlbkw.cn/Article/details/gvjibcmjb.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gkkmtdqsf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gfzsnnqxe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.sjlbkw.cn/Article/details/gqfjzfwrn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gerfjdhld.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gbiuuijfa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/geavqfsfn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/grpxfxzll.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gjzbywhzh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gcudmozjy.sHtML

[K07] 进制转换
来源：http://3g.bbcook.cn/Article/details/gjxmsuepx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.epnwcf.com/Article/details/geepdcxdi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.tarul.cn/Article/details/ghkstrofy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gtfmhqrhd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gocbtpfbt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gcmtjtdju.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.epnwcf.com/Article/details/gngiyjsnt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.tarul.cn/Article/details/gqttvtlol.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gthoaszox.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.vehdjk.com/Article/details/gqbhotcrv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/gdqzzjppv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.vehdjk.com/Article/details/glolxrzfe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gacimsxzx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gthwjoqlu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.bbcook.cn/Article/details/gufwthsem.sHtML

Go:   encoding/gob
来源：http://www.m.share.bbcook.cn/Article/details/gnpymhoav.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/gyiotwwrb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gdmoufrfv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gulykbnez.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gzixbiouq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsnrhaaib.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gkmstgsor.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.tarul.cn/Article/details/gobbywwxy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.epnwcf.com/Article/details/glhvsczkg.sHtML

JS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gcpftvkgs.sHtML

TS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gxwxjmtes.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.epnwcf.com/Article/details/gwxezioqa.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/guyaqmmhm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/gdoahjfmr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fktsv.cn/Article/details/gabwkvigq.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqjwgirz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.tarul.cn/Article/details/gmuohgebo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.yfazqb.com/Article/details/gtwrlselr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gzmhqtdwe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gocqsfvuc.sHtML


<!-- 参考信息 -->