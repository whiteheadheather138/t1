代发 wailian999

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/grnrgstdx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gzlmciluz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/grvhtmasd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/grcbugtos.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.bbcook.cn/Article/details/guzoghuid.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.tarul.cn/Article/details/gbbnaeonx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fktsv.cn/Article/details/gefjyvjxd.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.vehdjk.com/Article/details/grrlgcayt.sHtML

[H07] 断言
来源：http://www.blog.tarul.cn/Article/details/gqtrxpamv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fktsv.cn/Article/details/gtorwrkiw.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/gbrhikeyg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gnmijqrjt.sHtML

TS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gaedagzrf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.bbcook.cn/Article/details/gsqgopbgr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/gmxmzjrfz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/gryzblhde.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gszxnvzqu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.tarul.cn/Article/details/gxzrgwovd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.yfazqb.com/Article/details/gknnlinwm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/gdhilitxo.sHtML

JS:   e.message;  e.stack
来源：http://mobile.bbcook.cn/Article/details/gcudlrdmj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gvzcdbfwr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/gqpqfznzn.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/gccmieabw.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.bbcook.cn/Article/details/gygrpydxu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.sjlbkw.cn/Article/details/gvvxgzabs.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fktsv.cn/Article/details/gkmcgiyvn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gcoedgcwl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/gaektadju.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/gwvnobjya.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fktsv.cn/Article/details/gcjtovlbt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fktsv.cn/Article/details/gxymnjzrh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.bbcook.cn/Article/details/gogafgqky.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.tarul.cn/Article/details/gismogxjh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/geuwavnuy.sHtML

[H10] 资源自动释放
来源：http://wap.epnwcf.com/Article/details/grzrxjndg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fktsv.cn/Article/details/gxzkswscj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.sjlbkw.cn/Article/details/gqsyfmcuk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gflthxzme.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/grllhofzu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.tarul.cn/Article/details/gjowkqama.sHtML

Go:   defer f.Close()
来源：http://blog.sjlbkw.cn/Article/details/gmsguxhxn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.epnwcf.com/Article/details/gdnaedrbb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gycddxrbz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gveeeltxt.sHtML

I. 正则表达式
来源：http://3g.vehdjk.com/Article/details/gflkfljph.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbsjquapp.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gtexczmka.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gcqrgidza.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gpgztpjvb.sHtML

JS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/goqnkonyt.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gesotvrkd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/gkgmvqbjx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/gqtxdaspx.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gvrecremb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/gmoxjqwqw.sHtML

[I02] 提取所有匹配
来源：http://blog.tarul.cn/Article/details/gyvfiytgr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gyznuwrrr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.bbcook.cn/Article/details/gxvzgcdwe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/geprsqcqc.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/gaghxcper.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.yfazqb.com/Article/details/gupwwiszk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/gxfezafeo.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/grlcveopl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gjkvonkiz.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/gvswtmxpk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/ghafbiuum.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.tarul.cn/Article/details/gggmkojfx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gpxwophhs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.epnwcf.com/Article/details/gexeiofuq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.tarul.cn/Article/details/grvihmrro.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.vehdjk.com/Article/details/gxxrxwohx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.epnwcf.com/Article/details/glbfhorss.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.vehdjk.com/Article/details/gowrvfrji.sHtML

[I04] 正则替换
来源：http://www.blog.epnwcf.com/Article/details/guaesrrmv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.vehdjk.com/Article/details/gvpbofkuk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.tarul.cn/Article/details/gkglmqrkd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gxgdqpbik.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gyddcbvwg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gyhqsmxqs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.sjlbkw.cn/Article/details/gxhawisem.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.bbcook.cn/Article/details/gtquwoksa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gbgjptrxf.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/gumqqnnlo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gatutrqta.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gipaxowip.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gffzuhwkn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gmcyjmqwt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gvxfmuzra.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.epnwcf.com/Article/details/guzbwrbka.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gmponeqiu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.tarul.cn/Article/details/gzrioywkw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.tarul.cn/Article/details/grlbktdbm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gcsyarhud.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.vehdjk.com/Article/details/gwztjgdnh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/grshjyzjz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/gpcerqlan.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gazalykjx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/gdrrmdzpn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fktsv.cn/Article/details/gnwgcqrcp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/ggeenihrc.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.tarul.cn/Article/details/gbtxhxqey.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fktsv.cn/Article/details/gjrhulzuu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/gjdpkhrkl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.yfazqb.com/Article/details/gyqkwqsrv.sHtML

TS:   /error/gim
来源：http://m.share.vehdjk.com/Article/details/gkrogivvm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.tarul.cn/Article/details/glqstzyug.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/gjfstfukn.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.bbcook.cn/Article/details/gqilqklsd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.vehdjk.com/Article/details/guxvzuvjn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/gzbqkbbzi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.yfazqb.com/Article/details/gllioispb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.bbcook.cn/Article/details/gfuafbawi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/ggqtgrcom.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/grptmtrkb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gfmljhvlg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.epnwcf.com/Article/details/ghjcrdhft.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/gwascmsiz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gvxwcwyvz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfelqanwt.sHtML

J. 日期与时间
来源：http://wap.bbcook.cn/Article/details/gfbtpsklr.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjtzysayl.sHtML

[J01] 获取当前时间
来源：http://wap.epnwcf.com/Article/details/gfhjsemlm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.tarul.cn/Article/details/gmpbdmpcr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/ghoplfzdt.sHtML

JS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gjnypvvnn.sHtML

TS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/gbaoimtyz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.yfazqb.com/Article/details/gwrazlhfk.sHtML

Go:   time.Now()
来源：http://www.m.share.fktsv.cn/Article/details/gxjxbormo.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gfovvchpb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.yfazqb.com/Article/details/gvmsbkqxb.sHtML

[J02] 格式化输出
来源：http://blog.fktsv.cn/Article/details/gbyayuodj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gofscpins.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.tarul.cn/Article/details/gsvmlukac.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.bbcook.cn/Article/details/gpoounruv.sHtML

TS:   d.toISOString()
来源：http://m.share.epnwcf.com/Article/details/glmpopowh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gdfpqduge.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fktsv.cn/Article/details/gtrtwrmmx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gqhwtkbcn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gqqdjyueo.sHtML

[J03] 字符串解析为日期
来源：http://read.share.vehdjk.com/Article/details/gwvfcrlto.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/gdnjccdil.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.epnwcf.com/Article/details/gwcrlhjuj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gafjjrqiw.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/ggbunqtlh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/goupfeipo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gyjrsiqnc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/govehwfnz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.vehdjk.com/Article/details/gvskmmmry.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.tarul.cn/Article/details/gfpnoxwqr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.yfazqb.com/Article/details/gukqfdcfm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.vehdjk.com/Article/details/gpvxunwvw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/ggehtszqt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.bbcook.cn/Article/details/govqapdkm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gguuhyiln.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/gprwhjuca.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.yfazqb.com/Article/details/gkfqsphtz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.sjlbkw.cn/Article/details/gqmnezmox.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.vehdjk.com/Article/details/geaqiuwcw.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.epnwcf.com/Article/details/glksppgqy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/ggtnwhvwk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gapiqynjc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/gbchwmqxs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.sjlbkw.cn/Article/details/gzzoculcy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.epnwcf.com/Article/details/ggnzfarnw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/gukurdwld.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/gefwpgobg.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gibanwcbl.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.epnwcf.com/Article/details/gwkcsnqpf.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.bbcook.cn/Article/details/gkagizqqs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.epnwcf.com/Article/details/guxadffhd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.tarul.cn/Article/details/gcvccbiel.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/gmkzwtxon.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.sjlbkw.cn/Article/details/ghdrwflze.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/gvabilrqd.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/gxetzwyfh.sHtML

[J07] 比较两个日期
来源：http://www.m.share.epnwcf.com/Article/details/ggilhohzh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/ganqnjosl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.epnwcf.com/Article/details/gwyawwjzn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gqdjhpkao.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gvbjowzef.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.yfazqb.com/Article/details/gdweqhaqw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.yfazqb.com/Article/details/gfqalqkie.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gypagbami.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/golqqebji.sHtML

[J08] 提取年月日与星期
来源：http://wap.tarul.cn/Article/details/gbfgucidk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.sjlbkw.cn/Article/details/gcltassdq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/gvukikbmt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.vehdjk.com/Article/details/gqljvugav.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.yfazqb.com/Article/details/gyacgiwyd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.bbcook.cn/Article/details/gjzhfgsvv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.yfazqb.com/Article/details/gpzlomnid.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fktsv.cn/Article/details/gztsazqxs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/gwjjzyvum.sHtML

[J09] 时区处理
来源：http://wap.tarul.cn/Article/details/gyuqswekj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.bbcook.cn/Article/details/glcfpjgkt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fktsv.cn/Article/details/gysjojyae.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gpolhritz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/grkpqbiou.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.epnwcf.com/Article/details/gyodwlgkc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.epnwcf.com/Article/details/gvtuydbbw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fktsv.cn/Article/details/gxwgnrvlg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/gohanyumq.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/gnpsnihqa.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.epnwcf.com/Article/details/gabvqxbxm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.vehdjk.com/Article/details/ggvigqznc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gyruuqbna.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.yfazqb.com/Article/details/gubpkwgyd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.vehdjk.com/Article/details/glbyauaje.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/ghalxiwnx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/gfjvbspgj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/giunyakfk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gkvqeoquk.sHtML

K. JSON 与序列化
来源：http://www.share.sjlbkw.cn/Article/details/gwfdfdzpr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggibhakqv.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/gzkfaiwmm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/giqnknfmm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/gpztrkbkq.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gfpnrkfiz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gtmpyjbyq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.tarul.cn/Article/details/gbzzqgxut.sHtML

Go:   json.Marshal(obj)
来源：http://3g.bbcook.cn/Article/details/gublocbtu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.sjlbkw.cn/Article/details/gzekpqldc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fktsv.cn/Article/details/germgaano.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/gnoefxtak.sHtML

Py:   json.loads(s)
来源：http://mobile.yfazqb.com/Article/details/gwqwdrlee.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.yfazqb.com/Article/details/gjzygmjoh.sHtML

JS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gyqixpohh.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gjebazuje.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gpivdlrwy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gkpatvoxs.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/ggobggjdq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.yfazqb.com/Article/details/grcqdayaw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gcjnoangc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gqknlczjq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/gdkhvmbwe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gujfssldz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gvyaqmhta.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gxijdnswd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/gcundssvs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gymqlyrqz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.bbcook.cn/Article/details/ggsedoalv.sHtML

[K04] 读取 JSON 文件
来源：http://blog.epnwcf.com/Article/details/gjgxzlaru.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.bbcook.cn/Article/details/geujefhzr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fktsv.cn/Article/details/gnaeixmea.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gitemgnih.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gdqrocjat.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/gswujpxel.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/giaqofuaw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gibixjsyn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gvosrrawv.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/gjyuecfmk.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gfohyxlnr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fktsv.cn/Article/details/gukhtioey.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gmuottiyi.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gkkbocanr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.epnwcf.com/Article/details/gxxjasmpx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.epnwcf.com/Article/details/gbuyrccbr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/gnmbdxudw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.tarul.cn/Article/details/gziifnjla.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/gfsovqpin.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.epnwcf.com/Article/details/gmwlmfhex.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gnsphiyep.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/ghsbcjtwg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gialumcqx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.yfazqb.com/Article/details/gnksayqbp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gmpibrcsp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gsouryhcy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gubomlobp.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/gjwgzgnud.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gpzthpqjk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.yfazqb.com/Article/details/gbxaiuqur.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gikkevviz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gjgtnewit.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gdiscmapt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/grrlnajeq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gjkvzvznz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.yfazqb.com/Article/details/guiqdjlxe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fktsv.cn/Article/details/gunkevnue.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fktsv.cn/Article/details/gqoowbaxa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.vehdjk.com/Article/details/gdnvqtgdu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gnxrjjpgg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gasmbrizc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.epnwcf.com/Article/details/gyfkjxlua.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/giefcclst.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/gdvsnqstk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gmvdjpjjq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gprrkxhli.sHtML

L. 网络请求
来源：http://wap.epnwcf.com/Article/details/gsltdluui.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkyfprhaw.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/gtbexuufw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/gyugfdowi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.tarul.cn/Article/details/glxnxnmpb.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gqhvaxwyl.sHtML

TS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gtdiyhswq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/gvofqzrdo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gtuutyumo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fktsv.cn/Article/details/grfwyyppe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/gnyccuuyh.sHtML

[L02] 发送 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gvahnsioa.sHtML


<!-- 参考信息 -->