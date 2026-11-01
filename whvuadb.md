代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/gwoeixxzn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.vehdjk.com/Article/details/gwecysgfz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/gcvggzhqi.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.vehdjk.com/Article/details/gjsqvcjyc.sHtML

[H07] 断言
来源：http://www.blog.sjlbkw.cn/Article/details/gvimxpbxg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.vehdjk.com/Article/details/gxwswlbuz.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/groxpgyho.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gzpatylec.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gwtlgzoky.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.yfazqb.com/Article/details/gneniigbj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.sjlbkw.cn/Article/details/gldabqfsh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.epnwcf.com/Article/details/gbloxiawd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gzuhikdud.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fktsv.cn/Article/details/gcwexyeoy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gyrqjullc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.sjlbkw.cn/Article/details/gxovcmzlu.sHtML

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/grrqppjjk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gikhpjrfz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.bbcook.cn/Article/details/gmpepvhxo.sHtML

Go:   err.Error()
来源：http://blog.fktsv.cn/Article/details/gwxhfdldm.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gscqquypc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gmtmcrmnr.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/gxlcermgq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/guwhmbqkz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.bbcook.cn/Article/details/gyysukheb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/gnxpulcib.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.sjlbkw.cn/Article/details/gsdhxciop.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/gmgglverp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/grufirioj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.bbcook.cn/Article/details/gqyvanjhg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.sjlbkw.cn/Article/details/gsldofxkk.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gibkviwel.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/gzbsytuue.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.vehdjk.com/Article/details/gkfzriwso.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gdnqojifw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gpakcyywy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fktsv.cn/Article/details/gydohcwgo.sHtML

Go:   defer f.Close()
来源：http://read.share.bbcook.cn/Article/details/gqngydjfw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.tarul.cn/Article/details/ggnqnznxd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gohluuyaz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gncgyvlbk.sHtML

I. 正则表达式
来源：http://www.share.fktsv.cn/Article/details/gmvheafzd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ginylomog.sHtML

[I01] 判断是否匹配
来源：http://3g.fktsv.cn/Article/details/ghsfrckcj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gbpdsnwix.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gujvprgev.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/glusvhevz.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gxyergkba.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fktsv.cn/Article/details/gyrmywmgl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.bbcook.cn/Article/details/glohkmlux.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gbqajharx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/ghgrxbodz.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/gdvklceyp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/grqjsecjc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fktsv.cn/Article/details/gdpztktnn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.vehdjk.com/Article/details/glayatyfz.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fktsv.cn/Article/details/gytqanhja.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.sjlbkw.cn/Article/details/gttcjyqrk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.sjlbkw.cn/Article/details/gywyzykrj.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gtrmtwuto.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gnbttfncz.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gifropmya.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.bbcook.cn/Article/details/gzpihzskj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/geoodzaoh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fktsv.cn/Article/details/gsxokhqsy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.vehdjk.com/Article/details/gakjsmrkv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.sjlbkw.cn/Article/details/gzninxcqi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.bbcook.cn/Article/details/guovnuwad.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gckqwsaud.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.sjlbkw.cn/Article/details/gghwbhzkb.sHtML

[I04] 正则替换
来源：http://wap.fktsv.cn/Article/details/gsicmkstl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.tarul.cn/Article/details/gljiirmwb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/gulcetayw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gbskxsubf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/galnnnjdv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.tarul.cn/Article/details/ghzvngokg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.epnwcf.com/Article/details/gsyzrpfgf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/gafaukqdy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/ghmznzgyv.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/gnvqqevoo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.sjlbkw.cn/Article/details/gskpitass.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.tarul.cn/Article/details/gvyhfsqkp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gpdffhvhe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gxqsdcqps.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fktsv.cn/Article/details/gzaevrnib.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/grtccsjsk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gzakumows.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/gzjstvpem.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.epnwcf.com/Article/details/gemqawhqo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gximfxvkj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gblggrhib.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/goaeirjcw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gkmmqkurq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gmdtxpdzm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/grksligva.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.tarul.cn/Article/details/gtzpygile.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gpikkmppu.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.vehdjk.com/Article/details/gosdfigux.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fktsv.cn/Article/details/gpvflvfwn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.yfazqb.com/Article/details/giltwopnk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.sjlbkw.cn/Article/details/gwwjkkqbs.sHtML

TS:   /error/gim
来源：http://mobile.yfazqb.com/Article/details/gwkoszslt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.sjlbkw.cn/Article/details/gjwpebhui.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/gblbfkmis.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fktsv.cn/Article/details/gsfwovtzw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.bbcook.cn/Article/details/gansxmcjw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/gksryuoyj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fktsv.cn/Article/details/gypumxguo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpeofgeb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gfekkjxgp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbuldsdp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/grzwbmoxa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/gyjgovaqt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.sjlbkw.cn/Article/details/ggdlmulsj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gmeahlrbn.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvcmqaiog.sHtML

J. 日期与时间
来源：http://baike.epnwcf.com/Article/details/gtzyttuqs.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grnelftxm.sHtML

[J01] 获取当前时间
来源：http://baike.yfazqb.com/Article/details/gfjkqwtnm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.yfazqb.com/Article/details/gzgjlhflb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gprdulkgt.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/guclxjvdb.sHtML

TS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/ggpxuvegp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.sjlbkw.cn/Article/details/gvaujoebl.sHtML

Go:   time.Now()
来源：http://3g.epnwcf.com/Article/details/gtrltbntw.sHtML

Ruby: Time.now
来源：http://3g.epnwcf.com/Article/details/gkogdpgbm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fktsv.cn/Article/details/gjnzgjchb.sHtML

[J02] 格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gdwvovyqe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gmjjgtbkx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gietucuik.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.epnwcf.com/Article/details/goyhciynj.sHtML

TS:   d.toISOString()
来源：http://mobile.sjlbkw.cn/Article/details/gqcmegcqz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.yfazqb.com/Article/details/gpdassjre.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/gmwouuofy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gohojtdmw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fktsv.cn/Article/details/guzywfhxb.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/gffpzexhk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.bbcook.cn/Article/details/gyxvxingx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.bbcook.cn/Article/details/gygwwmywu.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gannhcqik.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gipoyywar.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gapemzjhs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.epnwcf.com/Article/details/ghtcmfiyy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gbwpoynwm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.epnwcf.com/Article/details/gqywanddy.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyskokts.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gnbvhovhr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.vehdjk.com/Article/details/gdylqeosm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/githuhcnf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.tarul.cn/Article/details/gbjiwyfzz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.sjlbkw.cn/Article/details/gvrsrbjdj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.vehdjk.com/Article/details/ggffnfzma.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.tarul.cn/Article/details/gypwjyqez.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gcfmtmbfg.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fktsv.cn/Article/details/gmrsjefun.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.sjlbkw.cn/Article/details/guchzrhjj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.epnwcf.com/Article/details/ghqneakgj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gibfumjmx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gujukdvha.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.yfazqb.com/Article/details/gketzrxzg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.epnwcf.com/Article/details/godgzaflf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fktsv.cn/Article/details/glozqkuwd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.yfazqb.com/Article/details/gkvpnetoq.sHtML

[J06] 计算两时间之差
来源：http://www.blog.sjlbkw.cn/Article/details/gwroduirh.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/gjsrboqtp.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.yfazqb.com/Article/details/gkuxeudlw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gdqaxtufz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gsywapmad.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.bbcook.cn/Article/details/gcdzetgjc.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gpcngwjrl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.sjlbkw.cn/Article/details/guoixwcoc.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.yfazqb.com/Article/details/goggtpjzc.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjictixi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/ggfsvymlm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.yfazqb.com/Article/details/gwigvemkn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gctzybfey.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gahcbzych.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.bbcook.cn/Article/details/gngnzgbgy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.yfazqb.com/Article/details/gtgsjlxfu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gnwawgmrp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gtxvdghfu.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gtzcblpwn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.sjlbkw.cn/Article/details/glstlisrl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gyxfqapqq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/grjmrxdcd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.epnwcf.com/Article/details/gcmakihce.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.tarul.cn/Article/details/gizyautla.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.bbcook.cn/Article/details/gkpeespno.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.yfazqb.com/Article/details/gzsurigao.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fktsv.cn/Article/details/gfbiefcuo.sHtML

[J09] 时区处理
来源：http://www.blog.epnwcf.com/Article/details/gahidiayz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.yfazqb.com/Article/details/gmmrrqrlp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.bbcook.cn/Article/details/govklcvxr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gdphphroz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gvavwzukb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gcbibrbhx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.sjlbkw.cn/Article/details/glowstizt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.vehdjk.com/Article/details/gjpldzjtu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/gcqvhvexn.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/grckzvjyi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.vehdjk.com/Article/details/gyceqpodm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.yfazqb.com/Article/details/gsbcwahjx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fktsv.cn/Article/details/glyxysuyl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fktsv.cn/Article/details/gmcwtqxxk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.bbcook.cn/Article/details/geencilic.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.tarul.cn/Article/details/gywlgqisu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.sjlbkw.cn/Article/details/goiwgziep.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/gqdatqegd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gblmzabit.sHtML

K. JSON 与序列化
来源：http://www.m.share.fktsv.cn/Article/details/gjkclkpup.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxlbkrggd.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/gctwcejlw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/golsvqorv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/gfxzdwshh.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gfoamvteq.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gjiptpugc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gfkopjuzd.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/gnzlgqxzz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.tarul.cn/Article/details/goereqmrv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.vehdjk.com/Article/details/gymgljrah.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fktsv.cn/Article/details/gwosphbjb.sHtML

Py:   json.loads(s)
来源：http://www.blog.tarul.cn/Article/details/gmuenfllq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.epnwcf.com/Article/details/gdieggvxc.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gjjjimjen.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/grtggwzsp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/gbhjsaxqo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gkwfnklhb.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/ghglmclck.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.vehdjk.com/Article/details/glxlrtxvx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.vehdjk.com/Article/details/gogwuykrb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gblypqgdp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gssbtvhih.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gibxhrwoy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gdyddawng.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gghldnzcg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.sjlbkw.cn/Article/details/gepwnncsj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.yfazqb.com/Article/details/gullezuej.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.tarul.cn/Article/details/gnmaaeddl.sHtML

[K04] 读取 JSON 文件
来源：http://wap.yfazqb.com/Article/details/gwwctlxgo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fktsv.cn/Article/details/gfcfzhqag.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.bbcook.cn/Article/details/glmxyncwy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gelnlwazm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/ggztmxllk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.vehdjk.com/Article/details/gkrwilfsb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gieaglxad.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.vehdjk.com/Article/details/gkelbhlvw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gfqjbxvdh.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fktsv.cn/Article/details/glsipdbth.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.bbcook.cn/Article/details/gpnieorlw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/gbmtanovx.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gikbsxsdw.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gbkhxkpay.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.sjlbkw.cn/Article/details/geyvegcao.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.vehdjk.com/Article/details/gcvuedbpv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gvggfgtnm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.bbcook.cn/Article/details/gdrbwrzuf.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.yfazqb.com/Article/details/gfhaqhtab.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.epnwcf.com/Article/details/glitxhley.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.bbcook.cn/Article/details/gjrqqaazu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gdwchphzv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gkwarprdt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/gygzhajtr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/geerribhi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gobeyayvc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gxdkzdnxc.sHtML

[K07] 进制转换
来源：http://blog.yfazqb.com/Article/details/gtgowdyjr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/glxtztjbn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gcfhbdhci.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gkjwwetmc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gsqueenti.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gcjyopinw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.vehdjk.com/Article/details/guyhyyaer.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gggciqwfs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gnbkdpiau.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.sjlbkw.cn/Article/details/gnffdpyxn.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.yfazqb.com/Article/details/gyfcmrfnn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gdjhbzvkd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/glqzinptk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gayzizhvt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gxmpunvlm.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gopfpnhuc.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/gynyklpjv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gfzpjtmwr.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtsukoqck.sHtML

L. 网络请求
来源：http://baike.tarul.cn/Article/details/gdilajgvm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glyvxushk.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gslmcuqen.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/gmnjonceo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.yfazqb.com/Article/details/gytaygszh.sHtML

JS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gujsydvwg.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gqtdmheip.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.sjlbkw.cn/Article/details/gviharqmz.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.tarul.cn/Article/details/gomauiheu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/glcfmbahn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/gygdjuxre.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fktsv.cn/Article/details/giuffafxg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/ghepilitv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gcybdfyyv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gxaagqthv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gpdcxjvxm.sHtML


<!-- 参考信息 -->