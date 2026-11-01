代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://baike.epnwcf.com/Article/details/gpibqnnla.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gdsvjikps.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gljoafbuk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gzhelqnhw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gduasvxoc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/gywyanoms.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.vehdjk.com/Article/details/gnnifnzoh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gzqxemvgu.sHtML

[H03] 主动抛出异常
来源：http://blog.fktsv.cn/Article/details/glgrlqubb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.bbcook.cn/Article/details/gcqtdheym.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/grpaspzrz.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gposwedyr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/grkbtpctn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gojzxlakz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.bbcook.cn/Article/details/gaxatnbyk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.tarul.cn/Article/details/gndlxithe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/goltheppc.sHtML

[H04] 自定义异常类型
来源：http://m.share.bbcook.cn/Article/details/gphtljkzi.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.vehdjk.com/Article/details/gjqqgectn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gxwnavadw.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/ganmwijvt.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gielrlznr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/ggoiietcx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.sjlbkw.cn/Article/details/gowvwgjgx.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gkqeaqimp.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gdoxbktjk.sHtML

[H05] 捕获特定类型
来源：http://m.share.bbcook.cn/Article/details/gxtusnwdq.sHtML

Py:   except ValueError as e:
来源：http://baike.yfazqb.com/Article/details/gtomgkukd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.sjlbkw.cn/Article/details/gcemxtshv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/ghflthngp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gqawplfrn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/ginshdvny.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.vehdjk.com/Article/details/gbcvsnuby.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.sjlbkw.cn/Article/details/gdybydnud.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.vehdjk.com/Article/details/gtnqvvojf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.tarul.cn/Article/details/gjbopyiof.sHtML

Py:   value = d.get("k") or default
来源：http://wap.sjlbkw.cn/Article/details/giewocigc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gsgznosie.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gtufrpjpa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/ggonadfxz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.bbcook.cn/Article/details/gemunxzih.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.bbcook.cn/Article/details/gucwcsbdr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.epnwcf.com/Article/details/gvqmjpibs.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.sjlbkw.cn/Article/details/gvxarmadh.sHtML

[H07] 断言
来源：http://www.share.tarul.cn/Article/details/gewhrbjyh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.vehdjk.com/Article/details/gdgjugwem.sHtML

PHP:  assert($x > 0);
来源：http://read.share.tarul.cn/Article/details/gxynwazki.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gugctociu.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gcusoocbj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.bbcook.cn/Article/details/glghnxvfn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.epnwcf.com/Article/details/ghhwdlxte.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.sjlbkw.cn/Article/details/gmgoursnp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gufjansrt.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.yfazqb.com/Article/details/gkflogemo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.epnwcf.com/Article/details/gsyenksnk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fktsv.cn/Article/details/gyyzrgwmx.sHtML

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/graqrfspr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.sjlbkw.cn/Article/details/gpookygpj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gkvtihtzv.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/gseoueosj.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.sjlbkw.cn/Article/details/gyidjliid.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fktsv.cn/Article/details/gozslfqcm.sHtML

[H09] 带错误码的异常
来源：http://baike.epnwcf.com/Article/details/ghuxmgspr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbetxddr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/gwdynzocf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnelrqlmv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.yfazqb.com/Article/details/gezhnsjau.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.sjlbkw.cn/Article/details/gekuvphkg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.epnwcf.com/Article/details/gndcclnup.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.vehdjk.com/Article/details/gjftjujbv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.vehdjk.com/Article/details/giljbiawn.sHtML

[H10] 资源自动释放
来源：http://www.m.share.bbcook.cn/Article/details/grormhtvi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/gefmhxmrg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/gpprmysnp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/ghvvqelpa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/giahdpbcs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.epnwcf.com/Article/details/golwlgpcu.sHtML

Go:   defer f.Close()
来源：http://3g.tarul.cn/Article/details/gmyajpvtm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.epnwcf.com/Article/details/gyjotzfln.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gkzrlpwge.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjaoaulfd.sHtML

I. 正则表达式
来源：http://3g.epnwcf.com/Article/details/ggmrvlqvn.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsompcjpr.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fktsv.cn/Article/details/gclvxielt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.yfazqb.com/Article/details/gjccfdjtz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/gctpqobeu.sHtML

JS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gbiyaohgq.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/gciocemxw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/guifpwxbz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.tarul.cn/Article/details/gzluchqfd.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gsibtmrlq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.tarul.cn/Article/details/gdaprgpeb.sHtML

[I02] 提取所有匹配
来源：http://read.share.tarul.cn/Article/details/gbdgvgxkt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gnqcjhpxl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.yfazqb.com/Article/details/gpjsygfzm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/gcgooprqd.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.tarul.cn/Article/details/ghxuotdfi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.sjlbkw.cn/Article/details/gxxrigkqi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gkkystixp.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gvgdrakya.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gvomuqwbw.sHtML

[I03] 提取捕获分组
来源：http://wap.fktsv.cn/Article/details/gopmsdshb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.sjlbkw.cn/Article/details/gmqizgzdm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.vehdjk.com/Article/details/gauhlilpk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.vehdjk.com/Article/details/gwdedrpyj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.epnwcf.com/Article/details/ggvbuelpe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/gxssmmugu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gwoboidbv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/gnzqpksfg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gjjsdlzrf.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gazyixsjc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.bbcook.cn/Article/details/gmomzeeyd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/godthpchj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.tarul.cn/Article/details/gyifqzaqr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gftzgdzkj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gwcqjsuru.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.bbcook.cn/Article/details/gjvvosnuv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fktsv.cn/Article/details/gdnafqoiw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/ghxowtodx.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fktsv.cn/Article/details/glqwcwggn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gopphjhdo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.vehdjk.com/Article/details/gwlkzlezq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/geukvwnfu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gzfrphtau.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.vehdjk.com/Article/details/gbnxuhtzl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fktsv.cn/Article/details/ghjelftlh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/golsybgas.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/gykfocbap.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.tarul.cn/Article/details/gninypgli.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/goybghnfy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/ganfhodnn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/gegrncgbh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/guwwbnlut.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gpbzjuedz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.sjlbkw.cn/Article/details/gikowjmmq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.sjlbkw.cn/Article/details/gbgsyeids.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gpvcpykhm.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.vehdjk.com/Article/details/gnrqizdly.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/gwnietuot.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/gmjocacng.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.sjlbkw.cn/Article/details/gurrzqtix.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/gwdozszam.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.bbcook.cn/Article/details/gzcxrotoz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.epnwcf.com/Article/details/ghedrnilm.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/ggkrmqpsi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.epnwcf.com/Article/details/gyzhdlijx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/geneczbho.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.tarul.cn/Article/details/gbjmakcce.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.tarul.cn/Article/details/gphnuiuaq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gtntymsje.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gjmkdujnu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gyzqtrcsx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.tarul.cn/Article/details/gpaalbind.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.tarul.cn/Article/details/gaidouwpa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gstirdvum.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtekvkvka.sHtML

J. 日期与时间
来源：http://3g.bbcook.cn/Article/details/gbveltoma.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzohfmjmb.sHtML

[J01] 获取当前时间
来源：http://3g.tarul.cn/Article/details/gqwdlvghi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.epnwcf.com/Article/details/grsmqxxac.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gsskdekds.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/gyunjfobj.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fktsv.cn/Article/details/gkfsphllt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnjxluva.sHtML

Go:   time.Now()
来源：http://blog.tarul.cn/Article/details/gezvuwwlu.sHtML

Ruby: Time.now
来源：http://baike.yfazqb.com/Article/details/ganykgqvz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.epnwcf.com/Article/details/gflmlozms.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gzrhdfjjp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/ggojzfgwz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gaepxbngr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.tarul.cn/Article/details/ggswierfi.sHtML

TS:   d.toISOString()
来源：http://baike.sjlbkw.cn/Article/details/gtubfuvio.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.tarul.cn/Article/details/gseqyeegr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.bbcook.cn/Article/details/gmazppztj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gfeidrdnk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.epnwcf.com/Article/details/gaptuoitp.sHtML

[J03] 字符串解析为日期
来源：http://3g.bbcook.cn/Article/details/gvdpztcap.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/gfnrgtomz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.vehdjk.com/Article/details/gcfklhbzy.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gpescgxgo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gelcsmtsf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gjmeufyzg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/ggajetrxd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gojbjytes.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.sjlbkw.cn/Article/details/gakmxhlsx.sHtML

[J04] 时间戳与日期互转
来源：http://3g.sjlbkw.cn/Article/details/gzkbixfcc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.vehdjk.com/Article/details/gdpxgbrcj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gernqoktf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.epnwcf.com/Article/details/gonffudwv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/gwpzqkisd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gzdrmfoho.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/gqozujtxb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/gbetmyrvs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.tarul.cn/Article/details/geqcbkyci.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.yfazqb.com/Article/details/gganowmnj.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.bbcook.cn/Article/details/gnykmjeqd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.bbcook.cn/Article/details/gsmjblldy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/greevcqim.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gmgmnmfiq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gpmtgmoxx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.epnwcf.com/Article/details/gjedhjeph.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.yfazqb.com/Article/details/gszouksxc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.vehdjk.com/Article/details/gxhainyqp.sHtML

[J06] 计算两时间之差
来源：http://mobile.yfazqb.com/Article/details/gwcwgqsft.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.tarul.cn/Article/details/gehlzwauq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gohoroqsf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/ghgzvhkyi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.yfazqb.com/Article/details/gnwmccytu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/gpwnsicus.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/ganrwdxxo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.yfazqb.com/Article/details/gvctjhruc.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/grzzxsspp.sHtML

[J07] 比较两个日期
来源：http://read.share.bbcook.cn/Article/details/gacvzlxof.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/glfyuzhrq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/grecjmuyd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gzvyubqzu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gsyxmwmmp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.yfazqb.com/Article/details/gpmodmwvj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.bbcook.cn/Article/details/gwhmeuuri.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gudpiglzs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gucporjts.sHtML

[J08] 提取年月日与星期
来源：http://3g.epnwcf.com/Article/details/gebxegukj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/gkdsqcdgd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/gqcjiyhjs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.tarul.cn/Article/details/gxfeoskug.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.tarul.cn/Article/details/gfyyqrhud.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gqsfribqb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.yfazqb.com/Article/details/gnjmduvil.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.epnwcf.com/Article/details/gbincqgdp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.bbcook.cn/Article/details/gutapixjk.sHtML

[J09] 时区处理
来源：http://read.share.vehdjk.com/Article/details/gdnqmhyut.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fktsv.cn/Article/details/guldsjmga.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.bbcook.cn/Article/details/gceuqcqcx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gzhqqemrl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gufhywesx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.yfazqb.com/Article/details/gydirhbrg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/gcsssrqem.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/ghqocjtcv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.tarul.cn/Article/details/gwapvclum.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/gxwcxvodm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.yfazqb.com/Article/details/ghoqbrbtf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbsqkjfp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.tarul.cn/Article/details/ggucadyfs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaiisfzd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gbfomojka.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.vehdjk.com/Article/details/gamazzkxz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.bbcook.cn/Article/details/goyrdrwob.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.bbcook.cn/Article/details/gapektzoq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/getkhzchi.sHtML

K. JSON 与序列化
来源：http://wap.tarul.cn/Article/details/godiuqwdq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gkigzjppa.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.tarul.cn/Article/details/gndasuxwi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/glwqobbnm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gkobzrdic.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gqjmmcvld.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gvkhiovpv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.tarul.cn/Article/details/gahthzmvq.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fktsv.cn/Article/details/gomvejjne.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.epnwcf.com/Article/details/gdourbdqt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/ghvurhgwo.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gntzelvyi.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/gsypjjuqf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/gqrxyowxx.sHtML

JS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/glnwqgkgn.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gyyvxemdr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.vehdjk.com/Article/details/gqiojscud.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/ghbraljxe.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gwzccjubb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.sjlbkw.cn/Article/details/gcyectwte.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/gdaobrxyf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/ggzlftffh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gqhyuyfdi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.epnwcf.com/Article/details/ghykeoprb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gcylncxcf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/gluynhisv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.epnwcf.com/Article/details/gofcztwgx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.yfazqb.com/Article/details/gwefbvqxi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.tarul.cn/Article/details/gphdycruo.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.sjlbkw.cn/Article/details/gcxrvoozu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/giektsqdt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fktsv.cn/Article/details/gelqltjcw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gknqicgsk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gwzvaagbl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gruldikqv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/geqtdlcgc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gfplgbgup.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gbpiidcor.sHtML

[K05] 深拷贝对象
来源：http://m.share.bbcook.cn/Article/details/grdznjdnq.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/gmazqimpa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fktsv.cn/Article/details/gzmlgmjtm.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/glklbhrho.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gqojqwhwg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/gcyvphwhc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.yfazqb.com/Article/details/gsidohfoh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/gzoijgzjm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/ggpfjghzv.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.bbcook.cn/Article/details/gsbjspxbn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gtbyugpiw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.yfazqb.com/Article/details/gcmxjesjw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gcenpqyas.sHtML


<!-- 参考信息 -->