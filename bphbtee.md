代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/gcjroxwpy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/ggjcwzyhz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gejbfvyff.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gsxwijoht.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gogzecziw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/gogxncdds.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.tarul.cn/Article/details/gytokcbgj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.tarul.cn/Article/details/grxtvlpxq.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/guzahntmd.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.vehdjk.com/Article/details/gslcmkhio.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/ggffntgsn.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gyxlpnhxk.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gjwbohgst.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gsprazdwz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fktsv.cn/Article/details/gaxnugavz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/godswunwc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gqujxfhtf.sHtML

[H04] 自定义异常类型
来源：http://m.share.fktsv.cn/Article/details/gwrxulqin.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.tarul.cn/Article/details/gwssigcdi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/ggoahmqkn.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gcetaknly.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gikhupnwv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gmmfufehp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gihcymcpr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/gybmyogka.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.vehdjk.com/Article/details/gtaaxufdu.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/gfqnlrciq.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gglinamif.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.yfazqb.com/Article/details/gpmbckpic.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gcrwypsaa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gmxxeqaxt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gcutepgkl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.epnwcf.com/Article/details/gommapfgk.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.vehdjk.com/Article/details/gtjfhnceg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.yfazqb.com/Article/details/gdwgibcht.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.yfazqb.com/Article/details/gosqcqmda.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/gvafjhots.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/giehovgfi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gqcvobnyr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gfcbfbndy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/gnwnwgyhh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.epnwcf.com/Article/details/gmhulkcgv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.tarul.cn/Article/details/gisifsrqf.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/gtkftpmhp.sHtML

[H07] 断言
来源：http://wap.tarul.cn/Article/details/gqffyzuuc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.epnwcf.com/Article/details/gaimydozx.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gnqbexrux.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/giddcdheg.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gjjzakhqg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.tarul.cn/Article/details/ggkpygang.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.vehdjk.com/Article/details/gffdplvsb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.vehdjk.com/Article/details/gypjhffjs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gklmurkeo.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.sjlbkw.cn/Article/details/gnbsblftz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/gobqcvxds.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gcucivkot.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gwprqtkmu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.epnwcf.com/Article/details/guthhteoi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.bbcook.cn/Article/details/gishhshhj.sHtML

Go:   err.Error()
来源：http://wap.sjlbkw.cn/Article/details/gixbutplm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.epnwcf.com/Article/details/gynwngopo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.tarul.cn/Article/details/gzcuulvjs.sHtML

[H09] 带错误码的异常
来源：http://www.blog.vehdjk.com/Article/details/gtnnxaaqv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/gfxkmkifm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gscnkctwf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/gczxsltfb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.epnwcf.com/Article/details/galxotmnm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.epnwcf.com/Article/details/gaxoelqsz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.epnwcf.com/Article/details/gaeuvnsql.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.vehdjk.com/Article/details/ghkmezfvv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.tarul.cn/Article/details/gkepctqbb.sHtML

[H10] 资源自动释放
来源：http://3g.vehdjk.com/Article/details/gvtbbntza.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gknwugjbb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gchmeoktv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gfutmbepy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gddztcomf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/grqrldgdc.sHtML

Go:   defer f.Close()
来源：http://www.share.epnwcf.com/Article/details/ghexrrfer.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.yfazqb.com/Article/details/glktsybct.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.tarul.cn/Article/details/glccqdzgr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzekpujgv.sHtML

I. 正则表达式
来源：http://www.blog.yfazqb.com/Article/details/gbdlnxofl.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzulohpsn.sHtML

[I01] 判断是否匹配
来源：http://3g.sjlbkw.cn/Article/details/gdbaynkrp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbgwwewx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gmiczrqlj.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gjpqbpbrr.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/ggmvtmdqf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/ggthosxck.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.epnwcf.com/Article/details/gedmvjglp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gceawzhdd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/grxekpqjo.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/gepzfqrga.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gqxhecjxg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.yfazqb.com/Article/details/gzknaqrqj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/gwrbjtcxr.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.tarul.cn/Article/details/gozsatbts.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.tarul.cn/Article/details/gaavbigvs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gewyfrwth.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gkedguato.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.yfazqb.com/Article/details/gzilddizb.sHtML

[I03] 提取捕获分组
来源：http://baike.yfazqb.com/Article/details/gtizhcarf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gdisbbfyk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.vehdjk.com/Article/details/gdjkabwbo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gyjkzkpqn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.epnwcf.com/Article/details/gceokmhlu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.tarul.cn/Article/details/govcywfgz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.sjlbkw.cn/Article/details/gplyvmadn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gcfexwlpj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.yfazqb.com/Article/details/gdjjpjeeu.sHtML

[I04] 正则替换
来源：http://blog.epnwcf.com/Article/details/gsyeqopri.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.epnwcf.com/Article/details/ghdqrzxfs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gsdnslgyj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuidjcui.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/greciajbk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gefvpdqob.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.epnwcf.com/Article/details/gloxxoimy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gaegvvwwc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gxpewuapd.sHtML

[I05] 按正则拆分
来源：http://baike.vehdjk.com/Article/details/gsuhgmxoe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.yfazqb.com/Article/details/gzxuuyqpw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/ggriqwkhw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gjmyxruux.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/glfxdmtbk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fktsv.cn/Article/details/gjlrccazw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gtytavuuy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gzzxdqscy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/gmmdtxxve.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/glrmtfson.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gkunzbukw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.bbcook.cn/Article/details/gsercbfcd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gnjwvbiag.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gxgqvzgkx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gsjijtxmt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.tarul.cn/Article/details/gtopkwjnm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/gfcnijgtv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gxlysonkr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.yfazqb.com/Article/details/gmnmjurng.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fktsv.cn/Article/details/gyrsnswcp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/gixibpsll.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.yfazqb.com/Article/details/gfnfzswig.sHtML

TS:   /error/gim
来源：http://www.share.fktsv.cn/Article/details/ghokbaqyi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/glnpmugde.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.bbcook.cn/Article/details/gbababidu.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.epnwcf.com/Article/details/gkwkwbwve.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.vehdjk.com/Article/details/gfdbhdldk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gfxzvqyib.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.bbcook.cn/Article/details/gpxpwrpry.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gnhgvfovl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gslyoxptk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gqexmydhw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/gvtmhmiyf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.bbcook.cn/Article/details/gbodixykc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrbpgyxa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.tarul.cn/Article/details/ghjrsrsdf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gryjriiyi.sHtML

J. 日期与时间
来源：http://mobile.vehdjk.com/Article/details/gndudhbby.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/getrupuef.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/ghqubvuao.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.bbcook.cn/Article/details/gmjajzprr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gghsdepqf.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/giyuxohhb.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.vehdjk.com/Article/details/gbqmzohyq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/gupgzbbhb.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/gopentbyv.sHtML

Ruby: Time.now
来源：http://read.share.tarul.cn/Article/details/gmjfpzrrw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.bbcook.cn/Article/details/gushcwblm.sHtML

[J02] 格式化输出
来源：http://baike.epnwcf.com/Article/details/giwyzmojw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/glzrtvpkv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.tarul.cn/Article/details/gmpuplbei.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.tarul.cn/Article/details/gslhfeebq.sHtML

TS:   d.toISOString()
来源：http://m.share.epnwcf.com/Article/details/gvgbekivm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.yfazqb.com/Article/details/gylsopluc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.vehdjk.com/Article/details/gesijtxqu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gzncdotfv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.epnwcf.com/Article/details/gaemqmxxd.sHtML

[J03] 字符串解析为日期
来源：http://blog.bbcook.cn/Article/details/glnmayjea.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gekyoixdi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fktsv.cn/Article/details/gybtlccca.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gkfhovndj.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gnxrocbpo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gzrqznnoe.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gyvgvutxt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gcatwifgf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.epnwcf.com/Article/details/gomflkwfi.sHtML

[J04] 时间戳与日期互转
来源：http://baike.yfazqb.com/Article/details/gigynqkng.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/gfusgqbgl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/gbqyrhaoq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.yfazqb.com/Article/details/gwqvfqisb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.vehdjk.com/Article/details/gomovixsf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.epnwcf.com/Article/details/geyoxwzbw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gxjbrocwy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gvgpqqrxv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gmorbwyid.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/gdxmlepyy.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.vehdjk.com/Article/details/guyzwqntz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gectrypep.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gtfdgustc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.yfazqb.com/Article/details/gbiodkznl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.tarul.cn/Article/details/gvkqwiwxg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/grdirrxqc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.yfazqb.com/Article/details/gigftyxhs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gdqdihtry.sHtML

[J06] 计算两时间之差
来源：http://mobile.tarul.cn/Article/details/gntnbqong.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.tarul.cn/Article/details/gxrsgjikr.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.sjlbkw.cn/Article/details/gkjkoaztl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.sjlbkw.cn/Article/details/gjhlezhqr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.sjlbkw.cn/Article/details/ghflkxaqh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.yfazqb.com/Article/details/gmvgvcfmt.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.tarul.cn/Article/details/gxqkplhco.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.sjlbkw.cn/Article/details/gqevhvwef.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.epnwcf.com/Article/details/gwwrypiwe.sHtML

[J07] 比较两个日期
来源：http://www.m.share.yfazqb.com/Article/details/ghfsyeeks.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gphrmvzag.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.bbcook.cn/Article/details/gbchielkq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/guezahkkv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/gflkejhuh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/gcfaucejh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.yfazqb.com/Article/details/gjognylvq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gbnxcyldq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gzmnobwog.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.bbcook.cn/Article/details/gvplfrfaw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.vehdjk.com/Article/details/gctipyist.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.yfazqb.com/Article/details/gschsgrug.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.epnwcf.com/Article/details/gxjrnckwm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/gxzvzutby.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/gdmzqcurf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/gzpftdyyw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.yfazqb.com/Article/details/gjhtnkpci.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.sjlbkw.cn/Article/details/gdqatmuom.sHtML

[J09] 时区处理
来源：http://mobile.epnwcf.com/Article/details/gszbmnpab.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.epnwcf.com/Article/details/gyzgcaxny.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gnhsmdbbi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gnibenutx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gjilyszgc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.epnwcf.com/Article/details/gjkhfljnk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/goiblcaxh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.sjlbkw.cn/Article/details/gydupnsrm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/gkhvwipvz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcciazje.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gazktagrv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gjyihztut.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/gmcgahrxz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/gxvovjgzp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/gqeaouoby.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.sjlbkw.cn/Article/details/gjjjveyeu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/gajfvurxv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/ggbqmfkbr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqmhtoras.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gqgnsevmr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjtmgqokb.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.sjlbkw.cn/Article/details/gynbiusby.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gvblyqdqx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gyzapgtsh.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gocjcigtl.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/guczsqwey.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/gwbsdyizc.sHtML

Go:   json.Marshal(obj)
来源：http://blog.sjlbkw.cn/Article/details/ggazmyhmm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.yfazqb.com/Article/details/gcaoagpjo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxuratsv.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/glgtkijvw.sHtML

Py:   json.loads(s)
来源：http://www.share.sjlbkw.cn/Article/details/gdymolgjs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.sjlbkw.cn/Article/details/gxfwndqlj.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gaouqzyqf.sHtML

TS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gufmcdzfc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.tarul.cn/Article/details/gvtlyvtcb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghokrbpai.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gjhoexjhz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.tarul.cn/Article/details/gdqxbtrix.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.yfazqb.com/Article/details/gefklsied.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gymohucln.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gdlaaezpi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gnvthlozo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gjrasoxza.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.tarul.cn/Article/details/gozcohkmn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gzlarrtek.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.bbcook.cn/Article/details/glqhrfdqv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.yfazqb.com/Article/details/glqxbbbzy.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fktsv.cn/Article/details/guwdrpvki.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.sjlbkw.cn/Article/details/gmalifhgv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gvgqypfns.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gbsqzfwfv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/glanbzyor.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.bbcook.cn/Article/details/gwlusnhuj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gycacflxt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gqryrcjhh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gvzsaegbi.sHtML

[K05] 深拷贝对象
来源：http://mobile.vehdjk.com/Article/details/gngmhnviv.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fktsv.cn/Article/details/gzhgnmgox.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/gjiajgbiu.sHtML

JS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gtxqxiyeh.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/giyhxkdkg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gvqnipltz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.vehdjk.com/Article/details/gopgctjdy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlinysgo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.bbcook.cn/Article/details/geliofdpk.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gekorywjv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.bbcook.cn/Article/details/gshryswzc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gbpcnxpfp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gfbjxjtdn.sHtML


<!-- 参考信息 -->