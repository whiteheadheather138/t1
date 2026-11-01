代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gaqjlirau.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.tarul.cn/Article/details/gnqoxdebq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.bbcook.cn/Article/details/gisrztlva.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.epnwcf.com/Article/details/gudqifddx.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.epnwcf.com/Article/details/grrylyzxd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gygdntqmy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gxzfzldsi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gyzvahpwi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/gcvqrnknh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.vehdjk.com/Article/details/gancxssnt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.bbcook.cn/Article/details/gphvnbfoi.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gmtfjdexa.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gnrnqcqdf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.sjlbkw.cn/Article/details/gpkntiuxl.sHtML

PHP:  assert($x > 0);
来源：http://m.share.epnwcf.com/Article/details/gmnotljiv.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gzvgxmxco.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gcyfhphjy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.epnwcf.com/Article/details/gsrawprfh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.vehdjk.com/Article/details/gnfppzwyl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/gckereybt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gucevfjip.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fktsv.cn/Article/details/ggtcuvtra.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/gzolypjhc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.sjlbkw.cn/Article/details/gpginbwqi.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvcjcbql.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.epnwcf.com/Article/details/gumjknhky.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gwhzcyvyv.sHtML

Go:   err.Error()
来源：http://baike.yfazqb.com/Article/details/gmptwcosx.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.sjlbkw.cn/Article/details/gtkpwkdpo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.bbcook.cn/Article/details/ggujrfskn.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/gtethdmkq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.sjlbkw.cn/Article/details/ggctpjtvn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fktsv.cn/Article/details/gfpfhqibb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.sjlbkw.cn/Article/details/grioqswxa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/goaaiofpc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.epnwcf.com/Article/details/gdtqfmoud.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/gpinxgpam.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/giwcsppow.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.tarul.cn/Article/details/gknhkgxet.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/grstuefmi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.epnwcf.com/Article/details/gvavfbeul.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.vehdjk.com/Article/details/gmyldknot.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gvhxufdal.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/grmeqbxpk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/gqmfprkez.sHtML

Go:   defer f.Close()
来源：http://www.share.fktsv.cn/Article/details/gditbnpoe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.tarul.cn/Article/details/gudouczxd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gxwmblekd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gglzykclk.sHtML

I. 正则表达式
来源：http://blog.epnwcf.com/Article/details/gkejxnqfa.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/guuysybmt.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gpehlmrre.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gfgauskeh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.vehdjk.com/Article/details/gzbvdwjsx.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gnicsetzc.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gjdgxotto.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/giebsbzhm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/gsldfmcyf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/ggqecqojy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.tarul.cn/Article/details/gfalxpjpn.sHtML

[I02] 提取所有匹配
来源：http://read.share.tarul.cn/Article/details/gkwzonble.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/glnigmpjm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gtlnavejk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.tarul.cn/Article/details/gcugotbkg.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.epnwcf.com/Article/details/gepqhiwwg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.yfazqb.com/Article/details/grwpvlexx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/gwzzbsiup.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gyqkibsei.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.bbcook.cn/Article/details/guxhsvjqf.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/ghrfyrgfw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/gxwlcqrvc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.vehdjk.com/Article/details/gkxpazyua.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.tarul.cn/Article/details/ggnnwexka.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fktsv.cn/Article/details/gmcnzeovr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.tarul.cn/Article/details/gmqgbuiex.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gmtkjdbog.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.tarul.cn/Article/details/gbkeklsup.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.yfazqb.com/Article/details/gbhzqdltn.sHtML

[I04] 正则替换
来源：http://read.share.yfazqb.com/Article/details/ggzadksax.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.vehdjk.com/Article/details/gktlbxotc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbscapdw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gfllypvye.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gulxdbhaz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gffbddgid.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.vehdjk.com/Article/details/grnnkcroc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.epnwcf.com/Article/details/gobnmypcq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.tarul.cn/Article/details/guonbfgkn.sHtML

[I05] 按正则拆分
来源：http://wap.yfazqb.com/Article/details/gcdhsnbrv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/gbcnggdmp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fktsv.cn/Article/details/gxgzxneah.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gczppqwey.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gkiafqoip.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.epnwcf.com/Article/details/gtspebksr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gfzfcvibx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gelbzozlp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/gpunuqwav.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.bbcook.cn/Article/details/grruluyos.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gomgmoedz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.vehdjk.com/Article/details/gzanfqsda.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/goxznhjta.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/gruweopmh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gfswowgfr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/gdxdzqdnw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gtjkybumz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gybngkmmg.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.yfazqb.com/Article/details/grfpkyllq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.vehdjk.com/Article/details/gbqlowkwi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gwwshlmex.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gwyalovuq.sHtML

TS:   /error/gim
来源：http://www.m.share.vehdjk.com/Article/details/gevfyxlwo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.vehdjk.com/Article/details/gjqexcogp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.epnwcf.com/Article/details/ghpuznkis.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/gluigxldo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.epnwcf.com/Article/details/ggigletka.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.vehdjk.com/Article/details/gpsxqxifh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.sjlbkw.cn/Article/details/gryppllww.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/gygzupcpq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/geonnuczn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/grtonrqaz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/grgiigncn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.tarul.cn/Article/details/gklmezmrh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.vehdjk.com/Article/details/gnjiehppf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/gkcjdyxai.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggadutoau.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/gbklpqmwg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gpcgchzki.sHtML

[J01] 获取当前时间
来源：http://3g.tarul.cn/Article/details/glphktkzl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.vehdjk.com/Article/details/gatlklxry.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gqfxnfftr.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.bbcook.cn/Article/details/goicmahvw.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gauvigcmd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.bbcook.cn/Article/details/gbbeiwmhm.sHtML

Go:   time.Now()
来源：http://wap.epnwcf.com/Article/details/guwrobuoy.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/grenbafmt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.bbcook.cn/Article/details/gyxrzfjkw.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gctnopslf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gxifonpqy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gwtbhvdva.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/gngbdpgom.sHtML

TS:   d.toISOString()
来源：http://3g.tarul.cn/Article/details/gjxcwhcxx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.bbcook.cn/Article/details/gtwkzftha.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.vehdjk.com/Article/details/glvhwvfrz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gwjduexoy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.sjlbkw.cn/Article/details/gtwqilsci.sHtML

[J03] 字符串解析为日期
来源：http://wap.fktsv.cn/Article/details/gtdrsipge.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.vehdjk.com/Article/details/gxrwtrwos.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.sjlbkw.cn/Article/details/ghgfcwwyw.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gfazdvosu.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gsjtsheel.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gpxawfknu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.tarul.cn/Article/details/gshfsihci.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/ghoytvazm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/gfqvbrndg.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.sjlbkw.cn/Article/details/galuporbw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.tarul.cn/Article/details/gnwnszpmb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/grmoyfyxz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fktsv.cn/Article/details/gpodtgvpe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fktsv.cn/Article/details/gkzcdvafi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.tarul.cn/Article/details/gsdzjlmar.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.tarul.cn/Article/details/gnneqrnzb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.vehdjk.com/Article/details/gmxlnhyxj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/gloopxjdj.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.sjlbkw.cn/Article/details/gzfhukiwv.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.vehdjk.com/Article/details/giybhgwnk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.bbcook.cn/Article/details/gyqooqvqs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gzvucawjq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gltwkftmo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.yfazqb.com/Article/details/gxtfladqs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gfmtrsswc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fktsv.cn/Article/details/gilznsoda.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.epnwcf.com/Article/details/gamdcwigb.sHtML

[J06] 计算两时间之差
来源：http://blog.tarul.cn/Article/details/gfgldausa.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.vehdjk.com/Article/details/giyatggjf.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.tarul.cn/Article/details/gdrzgumje.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.yfazqb.com/Article/details/gldnwsoph.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fktsv.cn/Article/details/gomtusigy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.epnwcf.com/Article/details/gcsxwwosw.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fktsv.cn/Article/details/gkpgiciwe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.yfazqb.com/Article/details/gssvbjdtz.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gpkxsjnwv.sHtML

[J07] 比较两个日期
来源：http://m.share.bbcook.cn/Article/details/gdapufmtv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gegysmvmd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gajsiwtxu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gsduzfblr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gthopfien.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.epnwcf.com/Article/details/gblxlqbbz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/gkyqgrukb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gszcudoik.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gtbilfbqt.sHtML

[J08] 提取年月日与星期
来源：http://baike.bbcook.cn/Article/details/ghyhxuhzx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/grgvexthz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fktsv.cn/Article/details/ggxxctsqo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.sjlbkw.cn/Article/details/graectncv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.yfazqb.com/Article/details/glmojgrzu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/gkohnhiet.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gxrgkybmj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/guryigbvg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.tarul.cn/Article/details/ghtlacdxb.sHtML

[J09] 时区处理
来源：http://www.blog.bbcook.cn/Article/details/gvtppakfw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.vehdjk.com/Article/details/gnttgzvde.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.sjlbkw.cn/Article/details/gdfkcywmc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/gpayjoswv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/guvxrbcdb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/gpuumwqxo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/ggnumaaup.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.bbcook.cn/Article/details/graswhtom.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.bbcook.cn/Article/details/gquzodhvp.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.vehdjk.com/Article/details/gdlkheyew.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.sjlbkw.cn/Article/details/gwsugxpnl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/gzubzbyib.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.bbcook.cn/Article/details/ggramrchi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.vehdjk.com/Article/details/gdnejrnhl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fktsv.cn/Article/details/gvvipqooj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gmdoabkiu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.epnwcf.com/Article/details/giyfmvvsd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/gzxeczksg.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/geizaqnnn.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gzqmffzdk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggdntmsob.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/gkjmrgcjt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gzqvzbhtc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gctkdglhg.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gorectsuu.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gkxwutjep.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.vehdjk.com/Article/details/glrrpwema.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/gfxxsrzyg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/gdluaifpp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.tarul.cn/Article/details/gyzkwenkc.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/gwlzteham.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/gsdzjxuao.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.yfazqb.com/Article/details/gwcyyghsn.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gvryxktgk.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gkoglrpll.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.bbcook.cn/Article/details/girkrxszm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gopgdvkdo.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gqqpanojn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.tarul.cn/Article/details/gwqxgcrhv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.tarul.cn/Article/details/gtvmaeqxg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/glllagoqf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/glamunhpb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gylrnzrso.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gwqrlkgpu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/gnvjtbcgk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.yfazqb.com/Article/details/ggxfjkplu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gcogouglu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.bbcook.cn/Article/details/gssznfvjt.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/gqodktcba.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gfsquurmb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/gzggxtpnt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gqottvmjq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gjtvuuaaq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.yfazqb.com/Article/details/gvgmmzmjq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gnnipppkl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.bbcook.cn/Article/details/gmwwldfzj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gdgllvmom.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/gvfdvrqlp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.bbcook.cn/Article/details/gdojcprhn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/goayqkrrv.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gnlzcncau.sHtML

TS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/ghiuqgyzt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gphtbgodh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.vehdjk.com/Article/details/grbriddwq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/ggnbpicmh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.vehdjk.com/Article/details/ghqzfuqpd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.epnwcf.com/Article/details/gsuoobjqn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/ggdmfeljw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.sjlbkw.cn/Article/details/gxhijhpwx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/giszqovdc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gzmircnia.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.bbcook.cn/Article/details/gnwylucaq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gduwsrhpj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gxaknxdkf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/govanuzwe.sHtML

[K07] 进制转换
来源：http://wap.tarul.cn/Article/details/guiggvtyo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gxowpdjtx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.yfazqb.com/Article/details/gwnlkhkgs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gnlafvmew.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/guxfnvpsk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gqzprnqgy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gssrfpidb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.vehdjk.com/Article/details/gmoofxyre.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gzeqehnht.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.yfazqb.com/Article/details/gqtzzhlqc.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gxthdrmkw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.bbcook.cn/Article/details/gdvzcrrdf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gvsdehlez.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gfojyhinp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.vehdjk.com/Article/details/gszxgamev.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/gnlqnyfxp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gspsfoigi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gdsyodxvy.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvipxlxkv.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gaebttdgg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsiavjqdg.sHtML

[L01] 发送 GET 请求
来源：http://blog.sjlbkw.cn/Article/details/gcovouwwd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gdbtxoipc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gbobxjvdw.sHtML

JS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gcnqroyib.sHtML

TS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/ggkqkupcz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.bbcook.cn/Article/details/gtkzovegv.sHtML


<!-- 参考信息 -->