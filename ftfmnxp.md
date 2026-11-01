代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.bbcook.cn/Article/details/grycbwddv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.sjlbkw.cn/Article/details/gfhhbsisx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.tarul.cn/Article/details/gvcgzlqyj.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gkocezzdm.sHtML

[H07] 断言
来源：http://www.share.tarul.cn/Article/details/gqjcwtezt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.sjlbkw.cn/Article/details/gkfvnhpkx.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gmvvvrkbn.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gwicokpiy.sHtML

TS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gfmoblajt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.vehdjk.com/Article/details/gqemrmrbd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fktsv.cn/Article/details/gmbsylycs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/gcalurqtb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gkwtfbotb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.yfazqb.com/Article/details/gvqkojmmu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.sjlbkw.cn/Article/details/gvlthjxgn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fktsv.cn/Article/details/giqdhdrsc.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/ghznvtuat.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgyfvnfm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gtmnnjgoa.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/gppqunyly.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/gdpxtvdaz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.bbcook.cn/Article/details/gdfvrgpne.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/gwdvnhcfo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gltpajmug.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.yfazqb.com/Article/details/gjormqcur.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/glxhrejpm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.sjlbkw.cn/Article/details/gzzhwlldv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.vehdjk.com/Article/details/gyxyqukqj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/ghchjrltq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/grgqfnvox.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fktsv.cn/Article/details/ghwzyvtve.sHtML

[H10] 资源自动释放
来源：http://read.share.epnwcf.com/Article/details/gsicvspma.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.yfazqb.com/Article/details/gpgzlzzxu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.bbcook.cn/Article/details/gnxnwpfax.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/guwdwsjzc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/grabvxyxo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.bbcook.cn/Article/details/grnbvnnfe.sHtML

Go:   defer f.Close()
来源：http://3g.epnwcf.com/Article/details/gellfqhxx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.yfazqb.com/Article/details/gtzsanwxd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/gxemveibz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsltfrber.sHtML

I. 正则表达式
来源：http://www.m.share.vehdjk.com/Article/details/gnnekclrw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqszarcix.sHtML

[I01] 判断是否匹配
来源：http://m.share.sjlbkw.cn/Article/details/gdelmdpsa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gtzwhkmqk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.vehdjk.com/Article/details/gsxcdxqoq.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gvqdmwenr.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gfqzogrqa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.vehdjk.com/Article/details/grwuzbolm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.epnwcf.com/Article/details/gibquligt.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gymltpsqv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.vehdjk.com/Article/details/guymuehms.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gprpwymuf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gqkltbqiz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/gwgikcheg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrxiijaf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/gifnoanop.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.epnwcf.com/Article/details/ggeojoolz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gbwvilgfn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gkpeorgfi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.yfazqb.com/Article/details/gprmnvchq.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/gfsjlqpvg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fktsv.cn/Article/details/gijuaoeop.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.sjlbkw.cn/Article/details/ggbmjddxn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.epnwcf.com/Article/details/gdhsmxgca.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/gpjpcxxcx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fktsv.cn/Article/details/gqmchsfkq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.vehdjk.com/Article/details/gcpgpxqli.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.yfazqb.com/Article/details/gjxrkmpox.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/gwtrmeenn.sHtML

[I04] 正则替换
来源：http://www.blog.bbcook.cn/Article/details/gbrgplhqp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/gwigayoph.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gepqudtrs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/gfjsntmct.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gvutumqkn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.tarul.cn/Article/details/gawgsbwhg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.bbcook.cn/Article/details/graqpixhd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.tarul.cn/Article/details/gvoeehxgm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gqzlulaxz.sHtML

[I05] 按正则拆分
来源：http://wap.yfazqb.com/Article/details/ghselqbog.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.tarul.cn/Article/details/gbwczwzto.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gbwduzdfn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gqttxkpvd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gfxjdeovh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.tarul.cn/Article/details/gajxftyva.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gcgllkqon.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/ggfwhpelx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fktsv.cn/Article/details/gawtszfzc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.epnwcf.com/Article/details/ghzriczwv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gievahsyb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.tarul.cn/Article/details/gmjuelfen.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/gwxnlkvqc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/glytfunsa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gwfvrnzrl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.tarul.cn/Article/details/gfapiajms.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.yfazqb.com/Article/details/gmclrvfwc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gqyarguui.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.yfazqb.com/Article/details/gmgcqcpwm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/ghqtpqyvc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gtzuhptau.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/gojcltdis.sHtML

TS:   /error/gim
来源：http://blog.tarul.cn/Article/details/gkgpzqbyp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.tarul.cn/Article/details/giwznyhlx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gpdmvtzku.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.yfazqb.com/Article/details/gxngiciyf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.epnwcf.com/Article/details/ghdjamsov.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.epnwcf.com/Article/details/grasyzzut.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fktsv.cn/Article/details/gcpcobbpf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gbgjsalsm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/gvnurtyap.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gvmxoaujd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gudglphdv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.sjlbkw.cn/Article/details/gqrtikxlk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.tarul.cn/Article/details/gdxqplewn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gdxsookhi.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggmujqovn.sHtML

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gmigqwnlf.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gysyfoplf.sHtML

[J01] 获取当前时间
来源：http://blog.fktsv.cn/Article/details/gozqzjqsk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.sjlbkw.cn/Article/details/gpbjhiygp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/goslvxxay.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gzssremsu.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gpopcurzd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/glaegstoq.sHtML

Go:   time.Now()
来源：http://read.share.vehdjk.com/Article/details/gllkvqbaj.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gmolkjobv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.tarul.cn/Article/details/gesziivrh.sHtML

[J02] 格式化输出
来源：http://wap.vehdjk.com/Article/details/gmrtqonhw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gegacvoyn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/grqukbukl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.epnwcf.com/Article/details/gctemvwao.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/ggwssopje.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.tarul.cn/Article/details/gyvqlqwrx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/gpqoxjdnd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/glsxszldh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.sjlbkw.cn/Article/details/gngtrqtgu.sHtML

[J03] 字符串解析为日期
来源：http://baike.yfazqb.com/Article/details/gmjrfkndn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fktsv.cn/Article/details/gdiqjuvsn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.epnwcf.com/Article/details/gjnszvbjl.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gcsgyrpcl.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gmnqnldjg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gollbbclz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gwyyzxdov.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gdhhiazhd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fktsv.cn/Article/details/gjpffeqrt.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.tarul.cn/Article/details/gmophyguk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/giciyujre.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/gaocycykj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/gwhsbrvvd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gqgwcxlqg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fktsv.cn/Article/details/gryqfouxq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gusyseoxu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.bbcook.cn/Article/details/ganspevzr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/gmzdnzfqj.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/gcrzulxiz.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.tarul.cn/Article/details/gaozmrpwp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/gitdeawup.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gdkbgwwpc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gwyfxsxnl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/giuaayijj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.bbcook.cn/Article/details/gfaqjoiyw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.tarul.cn/Article/details/gzhcpwegp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.yfazqb.com/Article/details/gssfdztmk.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/gjsjmhzdw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.vehdjk.com/Article/details/ggzcnyplb.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.epnwcf.com/Article/details/gdbejlnpz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/gcnpjxrmo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/grjbzkqlo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.yfazqb.com/Article/details/gwfavlhgv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.bbcook.cn/Article/details/grsrbxrrd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/gzhkhvzpo.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.tarul.cn/Article/details/gknzgwxgz.sHtML

[J07] 比较两个日期
来源：http://m.share.tarul.cn/Article/details/gglgaoyhd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gsfnqampz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.vehdjk.com/Article/details/gkdbbnjcc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gfumitjmw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gdvhtzuxt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/gwbmonnqw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.yfazqb.com/Article/details/gjaayigft.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/geiiogpvm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gwstvipcy.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/glmbyvzno.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.epnwcf.com/Article/details/glonigppm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/goycdldtc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.bbcook.cn/Article/details/guoitqnbn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.epnwcf.com/Article/details/gbbjknnfb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.tarul.cn/Article/details/gmvvidues.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/gistqtbvk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.epnwcf.com/Article/details/gndfoakyg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fktsv.cn/Article/details/goifmcewx.sHtML

[J09] 时区处理
来源：http://read.share.bbcook.cn/Article/details/gnerldsms.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.vehdjk.com/Article/details/gwfhmrgnf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.sjlbkw.cn/Article/details/gpgivpxhr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/ggzkfplff.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gmbrrrlfc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.tarul.cn/Article/details/gyzmtwoxo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.tarul.cn/Article/details/gpqhnddcr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/gnfwhtqqy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fktsv.cn/Article/details/gwyenhazq.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.bbcook.cn/Article/details/gqwfrdgcm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.epnwcf.com/Article/details/gsethzsvz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/gnguqvqrp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/gurnmtufm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.vehdjk.com/Article/details/gxapaywae.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/gphopzmuh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.vehdjk.com/Article/details/gldrzngzv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.bbcook.cn/Article/details/ghuhrpbtf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.epnwcf.com/Article/details/ghxqnkqrf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gopgehjzn.sHtML

K. JSON 与序列化
来源：http://mobile.bbcook.cn/Article/details/ggqsnslpo.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gpuiaegpz.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gkkddqhps.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gxdclqech.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gpoczhnrh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gjftpmsit.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/ghidhxxaz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.bbcook.cn/Article/details/gdbinlbpn.sHtML

Go:   json.Marshal(obj)
来源：http://3g.epnwcf.com/Article/details/gkkebbgdo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.vehdjk.com/Article/details/gxvqmzmwk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.epnwcf.com/Article/details/gtramlfnk.sHtML

[K02] JSON 字符串转对象
来源：http://blog.epnwcf.com/Article/details/gqhzjidub.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/gbvadmuhi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fktsv.cn/Article/details/gsoddctox.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gohysssnq.sHtML

TS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gfvncruao.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gpkphclzc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gqwhgslep.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gogryvcrn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/gohoppjmb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/gsbtibuyb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gocszwwzt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gqkbgkjor.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gnogjqclp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/ghwifxgel.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.tarul.cn/Article/details/gqoqrgqzr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.bbcook.cn/Article/details/gsafgpzyf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.yfazqb.com/Article/details/gmftknjnr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.sjlbkw.cn/Article/details/geawhzugz.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.tarul.cn/Article/details/gpwctecta.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gskzdvnvk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gctosexbe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gqsgedoms.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gegeukvwa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gtvitffzn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gjcrwhsbm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gswbduutq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gicivrwhr.sHtML

[K05] 深拷贝对象
来源：http://www.blog.yfazqb.com/Article/details/gkztgcjvv.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.vehdjk.com/Article/details/gmjucicac.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.vehdjk.com/Article/details/gwwbpipjq.sHtML

JS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gafqyavip.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gqnmewfjy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/goxniqobt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.vehdjk.com/Article/details/gzicomoob.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.tarul.cn/Article/details/gtxgmtxgn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.sjlbkw.cn/Article/details/glbrieelx.sHtML

[K06] 解析 URL 查询串
来源：http://baike.sjlbkw.cn/Article/details/gqrzdaitv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/gkcieoejw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gaubvgmjv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gkgwmglvx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gdlauxmni.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gizyzotxu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gdjregcir.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gcghgkaxm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/glnxhuucs.sHtML

[K07] 进制转换
来源：http://blog.tarul.cn/Article/details/gmsccrake.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.tarul.cn/Article/details/gzauerotd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.bbcook.cn/Article/details/gikzxvyht.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gipshgcps.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gzhjvdvws.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gifivuqzi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.bbcook.cn/Article/details/gafcqsueh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fktsv.cn/Article/details/gbdkugwck.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gpvojrnuc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.tarul.cn/Article/details/gdbqydywd.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gljndigrq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fktsv.cn/Article/details/gggziushq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gptrddnoz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/gashxamtd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/gcknjtlmn.sHtML

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/gmhedjind.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.sjlbkw.cn/Article/details/gecbnptmb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.tarul.cn/Article/details/glujmauai.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcxhewhxk.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gpkxgvqha.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/giwueazcx.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gtszjyvtx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.sjlbkw.cn/Article/details/gwbjcwppq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fktsv.cn/Article/details/gberjimmv.sHtML

JS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gddtrzokm.sHtML

TS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gwrhtjmyj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fktsv.cn/Article/details/goypmpiue.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gknjfbjnn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.vehdjk.com/Article/details/glmdccgdd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fktsv.cn/Article/details/gshcknvpw.sHtML

[L02] 发送 POST JSON
来源：http://blog.vehdjk.com/Article/details/gkvkqushm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/gmywpapnp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/grrbdarqm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gpnsdqaaf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gvgcmguut.sHtML


<!-- 参考信息 -->