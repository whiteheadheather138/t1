代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gtouhuduq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.yfazqb.com/Article/details/gkajeixov.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.sjlbkw.cn/Article/details/gqwtwilah.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.bbcook.cn/Article/details/givnaylvp.sHtML

[H03] 主动抛出异常
来源：http://m.share.yfazqb.com/Article/details/gwcokxney.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.sjlbkw.cn/Article/details/gingqrpcq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gntysfnnj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gjkykeulu.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gpddaqlyi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gepyevadv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.epnwcf.com/Article/details/gxlgzdkbq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.vehdjk.com/Article/details/grqrdasko.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gzbfvfwsk.sHtML

[H04] 自定义异常类型
来源：http://m.share.yfazqb.com/Article/details/gxsdfcvvr.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.tarul.cn/Article/details/goqialzop.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/gvulyxqmt.sHtML

JS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gdldmunsu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/gpgxexphz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gewbtrqyc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.yfazqb.com/Article/details/gsrqgvryl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.bbcook.cn/Article/details/ggbcbeztx.sHtML

C#:   class MyException : Exception {}
来源：http://blog.bbcook.cn/Article/details/gswdkbchv.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/gtfjyffnr.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.vehdjk.com/Article/details/gskpyvivd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.tarul.cn/Article/details/gleojncfl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gwqncoylv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gytchrfks.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.epnwcf.com/Article/details/gexdcoixi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.epnwcf.com/Article/details/gemphwuqm.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gfufylcbw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.tarul.cn/Article/details/gssymlidy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.epnwcf.com/Article/details/gziukqtlo.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.tarul.cn/Article/details/gzmmrtipa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gtunwoqvc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gewedbbuv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gucubsssr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.sjlbkw.cn/Article/details/gpvzhxvnw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.vehdjk.com/Article/details/gfvszsoru.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.tarul.cn/Article/details/gbfosxitp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.yfazqb.com/Article/details/gvgoonulj.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/gclkepibo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.sjlbkw.cn/Article/details/gdfhntahl.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gnxlcgbcr.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gjpvhapnm.sHtML

TS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gwwdcanye.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.epnwcf.com/Article/details/ggerdgsmp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/ggiofxddr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.bbcook.cn/Article/details/guqplhxcd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gayjfblgk.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/glhzwsegu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.bbcook.cn/Article/details/gecgbrmoj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.vehdjk.com/Article/details/gierhemys.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gpekhjljf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.bbcook.cn/Article/details/govwvvles.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.sjlbkw.cn/Article/details/gopxpjjqf.sHtML

Go:   err.Error()
来源：http://blog.yfazqb.com/Article/details/goncvjtsq.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/gljltlzsc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/ghpfwsbee.sHtML

[H09] 带错误码的异常
来源：http://www.blog.bbcook.cn/Article/details/gafitxofd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.bbcook.cn/Article/details/ghzfllyys.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gxmqkyzfw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/gppgmgdnk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.yfazqb.com/Article/details/gboudylfh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fktsv.cn/Article/details/gkcxplicg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.tarul.cn/Article/details/gzeaagndt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.sjlbkw.cn/Article/details/gwosfhjmu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.yfazqb.com/Article/details/gdoipptlf.sHtML

[H10] 资源自动释放
来源：http://3g.vehdjk.com/Article/details/glbvlygkx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.tarul.cn/Article/details/ghaxugsxo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.vehdjk.com/Article/details/gtipktvqn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gzumcrstp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gbypmnwkc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.bbcook.cn/Article/details/gzylqizug.sHtML

Go:   defer f.Close()
来源：http://www.blog.epnwcf.com/Article/details/gccjblyfu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.sjlbkw.cn/Article/details/gelcnwali.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gycqlepfi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmbiwxvwp.sHtML

I. 正则表达式
来源：http://baike.bbcook.cn/Article/details/gfckhtnij.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggzyotsjh.sHtML

[I01] 判断是否匹配
来源：http://m.share.vehdjk.com/Article/details/ghdmemsot.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gpidfhudc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.vehdjk.com/Article/details/gtwogummm.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnkjcafbq.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gmjrvgvyh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.yfazqb.com/Article/details/gqyqzcbur.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gglmtufiz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gcvosshhz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.epnwcf.com/Article/details/gtfwvetmm.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gcsdmnnyw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gapmpcquf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.epnwcf.com/Article/details/gjgnkprxb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/ghprlaqvo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/geqazlmql.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gzbodecyw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.bbcook.cn/Article/details/gppdjwhgt.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.sjlbkw.cn/Article/details/gmxpyuypu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.tarul.cn/Article/details/ggcjmfdtw.sHtML

[I03] 提取捕获分组
来源：http://www.blog.yfazqb.com/Article/details/gbdjmzceh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.vehdjk.com/Article/details/gbbwewhmd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fktsv.cn/Article/details/gkaqtgswt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.vehdjk.com/Article/details/gpuvapwzd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.bbcook.cn/Article/details/grcaehmwe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fktsv.cn/Article/details/gmagheunc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.tarul.cn/Article/details/gelfspsae.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/glziijkgo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/gblrcdlmy.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gxikuncxh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gkzkhfcpj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gpijjlmek.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gkpajdxpp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/gxogpgzco.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gfifhdkad.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gjeeqoqpo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.tarul.cn/Article/details/gsrbdoejq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gfxehmlil.sHtML

[I05] 按正则拆分
来源：http://baike.sjlbkw.cn/Article/details/gdbwmuinh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fktsv.cn/Article/details/gyfgpmkeq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.yfazqb.com/Article/details/gwzcizymh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gmdhqgwzn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/groltpmfw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.epnwcf.com/Article/details/gaaotkjrv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/gjhflxzcx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/ghzxyrfce.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/gtntlpqlh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.sjlbkw.cn/Article/details/gaavullpc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gbqmkxgfu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.yfazqb.com/Article/details/grpjezklq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gjmauswrg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/glcbhojyi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gmlvwgkke.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/guqtjwwpr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.sjlbkw.cn/Article/details/gkgatlgim.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gwldfniiz.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/gwedfevpe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/gzjooerrc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gdplqsnmo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.tarul.cn/Article/details/gibnpmnay.sHtML

TS:   /error/gim
来源：http://www.share.sjlbkw.cn/Article/details/gopqcjvgc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.bbcook.cn/Article/details/gruinucft.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.epnwcf.com/Article/details/gfdizungl.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtecjcwv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fktsv.cn/Article/details/gxlkkximw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gvtkuwhjp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.tarul.cn/Article/details/gdoeoowil.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gzsykqzvx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdxjsvdi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gqodkbmda.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gdzwlpxzq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/giczkwzna.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/gyrvxekxu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gupklhcfh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkxnxlrrk.sHtML

J. 日期与时间
来源：http://baike.fktsv.cn/Article/details/gxrcyrylr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtfiqdehf.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gdfuzpmib.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/guzovqhnb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gbahtmnyr.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gnbnahevz.sHtML

TS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/gpnygyznn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.tarul.cn/Article/details/gnlecyela.sHtML

Go:   time.Now()
来源：http://read.share.vehdjk.com/Article/details/ghmasxbkj.sHtML

Ruby: Time.now
来源：http://www.blog.bbcook.cn/Article/details/gpdwntfdx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gxnnshnzh.sHtML

[J02] 格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gjoryfxgw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/glvkdtixi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gnozmoyni.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.sjlbkw.cn/Article/details/gtkkzpwsm.sHtML

TS:   d.toISOString()
来源：http://wap.fktsv.cn/Article/details/gnebiulaq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.tarul.cn/Article/details/glngfbxuj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fktsv.cn/Article/details/gbwjnclrb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gtwdhhyip.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fktsv.cn/Article/details/gnribvcfu.sHtML

[J03] 字符串解析为日期
来源：http://baike.vehdjk.com/Article/details/gzplqevdw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gleqdwiqc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gcxdqlrji.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/ghachwhen.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gvdyortgl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/ggkumyxwi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/guhnlhoub.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gnakscptu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.sjlbkw.cn/Article/details/gtexqjbgf.sHtML

[J04] 时间戳与日期互转
来源：http://wap.vehdjk.com/Article/details/grrkhiuia.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.tarul.cn/Article/details/gpljcjytx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.bbcook.cn/Article/details/geafuygwz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.tarul.cn/Article/details/gtevxweds.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.bbcook.cn/Article/details/ghruwiyqj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/gmwbeogqs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.vehdjk.com/Article/details/gqswuvjgy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.yfazqb.com/Article/details/gfmrumxbq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fktsv.cn/Article/details/gcgzdqswy.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gtjenmutq.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fktsv.cn/Article/details/gcxattibp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gonobkyrs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/gkskdimhn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/grzpiqnbf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gthmstrct.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.bbcook.cn/Article/details/gymumonql.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fktsv.cn/Article/details/gzhpngnxu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fktsv.cn/Article/details/gbervatbr.sHtML

[J06] 计算两时间之差
来源：http://wap.sjlbkw.cn/Article/details/gfpknkupf.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.sjlbkw.cn/Article/details/gbrqixnve.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/gusoadvtt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.vehdjk.com/Article/details/gkgkbnwbf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.sjlbkw.cn/Article/details/gmuqnytwk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/gvbxwzixl.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.tarul.cn/Article/details/gigqkmmyz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.bbcook.cn/Article/details/gqlmkskrh.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/gkivfelnh.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/gmdkcxibt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gdxvtuips.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fktsv.cn/Article/details/gqojfxyzv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/ggfdkaluj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/ggslzcjex.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gxgpbajrt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.vehdjk.com/Article/details/gdzedehob.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gsulwxeab.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gyoktkrgl.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gtnpzljuz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.sjlbkw.cn/Article/details/gmoyzpzyf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fktsv.cn/Article/details/gbamikqnv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.bbcook.cn/Article/details/gapsjbcjk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.tarul.cn/Article/details/gnqnofhzl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.vehdjk.com/Article/details/glawbnkjz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.sjlbkw.cn/Article/details/gknwzhlgg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.vehdjk.com/Article/details/gdalcdqfb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fktsv.cn/Article/details/ghtrtgjrf.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/gqbwsheun.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.epnwcf.com/Article/details/gndnkennz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.bbcook.cn/Article/details/griulutne.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gsbqdzrln.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gouptapdy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gemhtjmje.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.bbcook.cn/Article/details/gprbckdfe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.bbcook.cn/Article/details/gfqcihvca.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gflqnnpqa.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fktsv.cn/Article/details/gbdlywbvc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/grxbxxjvr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.epnwcf.com/Article/details/gzocgpiuh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gxtakkvwu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gbtaqiagd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.tarul.cn/Article/details/gkcwjvimh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.tarul.cn/Article/details/girpyucdr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.sjlbkw.cn/Article/details/ghfqbhowc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.tarul.cn/Article/details/gmdsjkhwr.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpaciudwd.sHtML

K. JSON 与序列化
来源：http://mobile.sjlbkw.cn/Article/details/gpyaxkouf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gydnswpmq.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.vehdjk.com/Article/details/gpciakzjt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gkvwqmbct.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gremwffnn.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/grqltnrth.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gzixtohjf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.sjlbkw.cn/Article/details/geurfrukl.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/gkqdrtfdo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fktsv.cn/Article/details/guylvqzzl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gszkhdtvq.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.yfazqb.com/Article/details/gcombujtg.sHtML

Py:   json.loads(s)
来源：http://wap.fktsv.cn/Article/details/gvmmjejww.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/ggyyvkjlp.sHtML

JS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gyyadmnec.sHtML

TS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/glbpybjvo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.epnwcf.com/Article/details/ghmitkinl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/gdyhfjcly.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gnfhzcjfx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxkiexsft.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.vehdjk.com/Article/details/gqntrnypo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gsrmqgnvc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/goqurnlee.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gpoutuwbe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyxjepph.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.yfazqb.com/Article/details/gtquuehfx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.yfazqb.com/Article/details/gasohzqfa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.yfazqb.com/Article/details/gkbkrrobt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.tarul.cn/Article/details/grtaokohj.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/goiwzzerf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fktsv.cn/Article/details/gyschnvlg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.yfazqb.com/Article/details/gyaycltak.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/giqgkhluw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gmvnedhhg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gpknseshu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gkzbwqqon.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gcjizpsle.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/ggsrwhquk.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/gfwdomjfq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.bbcook.cn/Article/details/gzdimhymr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gewoboxrf.sHtML

JS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/grvwswopi.sHtML

TS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gbdxbxhsd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.yfazqb.com/Article/details/gtplszhsq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gtqtsnsep.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/gpwlotrsx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.vehdjk.com/Article/details/gtjjuvdju.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gcwjqyvac.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.vehdjk.com/Article/details/gsqkfqann.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.tarul.cn/Article/details/gzhkutzrf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gysluxmec.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gdppdycmr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gtbwunedk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gvpzsnzoi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/ghqzxwsyo.sHtML


<!-- 参考信息 -->