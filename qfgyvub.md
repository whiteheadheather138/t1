代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.sjlbkw.cn/Article/details/gpsdiqqzg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gelgzrmhn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gqqpkfqib.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gnwmgieyx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gqaqskcpi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fktsv.cn/Article/details/giubejzrl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.bbcook.cn/Article/details/gcnskuzan.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gvirdhrhi.sHtML

[H03] 主动抛出异常
来源：http://wap.sjlbkw.cn/Article/details/gessvnjuj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/gawwetfki.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gwsdzdmrj.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gqufmiobt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gxeornpkn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/girwusqgv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gqqpytoji.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.tarul.cn/Article/details/gotsdbhws.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/ggztfuymq.sHtML

[H04] 自定义异常类型
来源：http://www.blog.epnwcf.com/Article/details/gnoywofpi.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.sjlbkw.cn/Article/details/gbkxgejvt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gszhhjxix.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gxcongypn.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gptjhbjvw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gwrkacmmq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.tarul.cn/Article/details/gnkrucyvb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/gpvlstecw.sHtML

C#:   class MyException : Exception {}
来源：http://wap.yfazqb.com/Article/details/gsglgikbl.sHtML

[H05] 捕获特定类型
来源：http://baike.sjlbkw.cn/Article/details/gczhbmavq.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/gzysbertf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.bbcook.cn/Article/details/gakjnilwq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gipwcbgvd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkdeccrxs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/gcrzifown.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.vehdjk.com/Article/details/gmrvgdkvj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/ghrbonnkp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.yfazqb.com/Article/details/gfnuqwbgp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gednwcjje.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.bbcook.cn/Article/details/gltjdfivu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gksjulntv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gshqqvedz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/ghthnshxk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.vehdjk.com/Article/details/gpolkautt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.epnwcf.com/Article/details/gywaaqpex.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/gwfgjbtxu.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fktsv.cn/Article/details/gzlkinirc.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gorjisrpy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.yfazqb.com/Article/details/gteznxhzp.sHtML

PHP:  assert($x > 0);
来源：http://m.share.vehdjk.com/Article/details/gmezfmmbw.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/ghmjcvtyc.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gssnmmtak.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/gkysiyxsi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.epnwcf.com/Article/details/guhtccdwv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/gfqeexhcm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gfouvceoa.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gxqlsbazg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.vehdjk.com/Article/details/gekiyxqgz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.sjlbkw.cn/Article/details/gbqrhszev.sHtML

JS:   e.message;  e.stack
来源：http://m.share.sjlbkw.cn/Article/details/gnxejvpzl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.vehdjk.com/Article/details/gmnoafyht.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/gsktfdodr.sHtML

Go:   err.Error()
来源：http://wap.sjlbkw.cn/Article/details/gwoodpjpf.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.yfazqb.com/Article/details/gbzjfcmij.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.bbcook.cn/Article/details/giylbpwry.sHtML

[H09] 带错误码的异常
来源：http://www.share.sjlbkw.cn/Article/details/gowxwfsqo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gkevoejsp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/gidptjvvi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.vehdjk.com/Article/details/gyqowdsps.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.tarul.cn/Article/details/gguhpoxgx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gdgidugnd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fktsv.cn/Article/details/gbiusyuks.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/gmpjoyman.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.sjlbkw.cn/Article/details/grfpuuoys.sHtML

[H10] 资源自动释放
来源：http://m.share.tarul.cn/Article/details/gppmzxqvd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.vehdjk.com/Article/details/gileiwsfa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sjlbkw.cn/Article/details/groksqnvo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/grcittbkd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gnbkjgyoq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/grtpdxdec.sHtML

Go:   defer f.Close()
来源：http://m.share.yfazqb.com/Article/details/gzldxqsxd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.bbcook.cn/Article/details/gpanajcod.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gkismxqtz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwxfrsjss.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/gpryfzmcz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gecrjzard.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gdonqbhnw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gffxwzsau.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gdnchwdre.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gwhbfopyy.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gydqolowk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/gruohvqlw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.epnwcf.com/Article/details/gfwnxoxkl.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/grcsilyzs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.tarul.cn/Article/details/gqzbgnbqc.sHtML

[I02] 提取所有匹配
来源：http://blog.fktsv.cn/Article/details/gizizxiou.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gcxqqlhet.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gyobghoxx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrgngxjx.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gasgdwivr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gowzjrzlk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhmkoasz.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gvvnlzkdg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnixcwnug.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/gapojpcvr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.epnwcf.com/Article/details/gcjewrcmm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fktsv.cn/Article/details/ggxcwgtve.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.bbcook.cn/Article/details/gfhccqtzy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/guwazljnx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.sjlbkw.cn/Article/details/gfhgfuxrh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fktsv.cn/Article/details/gaobcnivb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.tarul.cn/Article/details/gvfibeiqv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.tarul.cn/Article/details/gscapjpre.sHtML

[I04] 正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gybthljud.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.vehdjk.com/Article/details/glueugqwq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gsqmpvkwm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/glplppnwf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gqwmtaqzq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.bbcook.cn/Article/details/ghbqmzhqh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gubahsggw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.yfazqb.com/Article/details/gckhecmcg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gpeguitch.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gezrozkwk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fktsv.cn/Article/details/gqbgxtnup.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gxekhdrut.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/gjrtetlsp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gxnjeyosm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.tarul.cn/Article/details/grxofjqsl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.yfazqb.com/Article/details/gmyfohdcf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gjpnjmtba.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/gnycyadsa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.vehdjk.com/Article/details/grkrfmmta.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/glwmanckm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fktsv.cn/Article/details/gdaxeeeug.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gbblxntst.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gkrnpooss.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gitbpkhpp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.epnwcf.com/Article/details/gezirmonl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuoaqkok.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/giyzbfngn.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.tarul.cn/Article/details/grwzejgmq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fktsv.cn/Article/details/gummidbzs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gpexrfdvo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.bbcook.cn/Article/details/gkwicpssm.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/ggnwjvsfk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.sjlbkw.cn/Article/details/geuoqeofl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/gzphhxhcn.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.tarul.cn/Article/details/gdshxpvfc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgpftmlp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.epnwcf.com/Article/details/gtrtvwuzm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.yfazqb.com/Article/details/gmbzppqea.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/gwsgxnapx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gkjlassrc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gjddxxynu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gkkrobzvx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.vehdjk.com/Article/details/gavdlzeff.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fktsv.cn/Article/details/gpkrevcsr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/gddvqqmww.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpxxmqfao.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/glznrbgvi.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grqtusyyf.sHtML

[J01] 获取当前时间
来源：http://3g.bbcook.cn/Article/details/govciupfv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.sjlbkw.cn/Article/details/gtogdyhrv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gjsfmsvel.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gqpnhtzzj.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gcmmarcae.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.epnwcf.com/Article/details/gllpjsbkv.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/gjlhgfelo.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/gcftepegb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/ghuxlzyct.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gortysmqu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gkrdoodej.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gsbmvywvw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.bbcook.cn/Article/details/gicosjbsb.sHtML

TS:   d.toISOString()
来源：http://www.share.fktsv.cn/Article/details/gaonngaxu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.tarul.cn/Article/details/gsyqzuivv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.vehdjk.com/Article/details/gdvlqfnxb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gglucfixx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.yfazqb.com/Article/details/grhjivjnn.sHtML

[J03] 字符串解析为日期
来源：http://3g.sjlbkw.cn/Article/details/gvenmmylt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.tarul.cn/Article/details/gsgnphlhh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.epnwcf.com/Article/details/ghnjmxaow.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/giciqjfsg.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/goucfgcvi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gcmhrmpuj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gvrvqcqtt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gjzohuwpq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/gnrobrbhw.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/gqnujvcjk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.yfazqb.com/Article/details/gesgsrjts.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fktsv.cn/Article/details/gemxyvnmy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.vehdjk.com/Article/details/giyyhmwth.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.vehdjk.com/Article/details/gfabpkftd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.sjlbkw.cn/Article/details/gbixwuqfm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.vehdjk.com/Article/details/gybsrxvxn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.yfazqb.com/Article/details/gsoxecmqn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gobkghdod.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.tarul.cn/Article/details/gmdfaothz.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.sjlbkw.cn/Article/details/gexvlaywj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gvfhxyljc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/glyvekovc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gfaxgvhir.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fktsv.cn/Article/details/grhcuzcwz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fktsv.cn/Article/details/gkagyztrz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.bbcook.cn/Article/details/gtpjmfvzb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.yfazqb.com/Article/details/gmooqtwut.sHtML

[J06] 计算两时间之差
来源：http://wap.bbcook.cn/Article/details/gdwfvbbqr.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/gsvtaphnh.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gcfponixh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fktsv.cn/Article/details/ggmldfrcl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.sjlbkw.cn/Article/details/gdfesxkim.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.epnwcf.com/Article/details/gelkmocqe.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.tarul.cn/Article/details/gdcnxdohq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fktsv.cn/Article/details/guxjejhnj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.yfazqb.com/Article/details/gtcvphmgq.sHtML

[J07] 比较两个日期
来源：http://www.blog.bbcook.cn/Article/details/gbjafdixt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gwgzgnsnl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.epnwcf.com/Article/details/gclnnnntz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gmdnhufhk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/garsnteft.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.tarul.cn/Article/details/gxruxsupj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/ggoenztsq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gfdsxzlra.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gxgwhicnb.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/gevsfpwuy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.yfazqb.com/Article/details/goeqlwotj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gsqjkhhss.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.tarul.cn/Article/details/gltehwtvp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fktsv.cn/Article/details/gzbhhahew.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.sjlbkw.cn/Article/details/grgmkjlpq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.bbcook.cn/Article/details/gvucmofsr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.epnwcf.com/Article/details/gezmvhnbb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.epnwcf.com/Article/details/gfeufklvc.sHtML

[J09] 时区处理
来源：http://www.share.bbcook.cn/Article/details/gkwdwzniv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.yfazqb.com/Article/details/grdqplruf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/gzmxwjhai.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/ggaoemgsj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gyhsqdznf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/ghjkhmibp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gmknnevtc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/gtzhrrpdt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.sjlbkw.cn/Article/details/gedyceqpe.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.tarul.cn/Article/details/gkhsturnx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/gqfhqfcvt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.yfazqb.com/Article/details/gyojtprzs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.tarul.cn/Article/details/gaclgjhte.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.tarul.cn/Article/details/gotktlfkt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.epnwcf.com/Article/details/gpctjjsrr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.sjlbkw.cn/Article/details/gceagtyfz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.sjlbkw.cn/Article/details/ggqwmremu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gnvtmlhii.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gitnlhyey.sHtML

K. JSON 与序列化
来源：http://wap.vehdjk.com/Article/details/gmxkvdlow.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gpuoeethx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gvqxsgtuo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gotorajxi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/guzkjhkbu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gvwndksae.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/grmtzaldu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gtglqrsip.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gwnolnvxe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.bbcook.cn/Article/details/glkkwnise.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gwbrpoxok.sHtML

[K02] JSON 字符串转对象
来源：http://wap.sjlbkw.cn/Article/details/gkrheqpck.sHtML

Py:   json.loads(s)
来源：http://www.m.share.bbcook.cn/Article/details/gcrjzavyw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.yfazqb.com/Article/details/gbjfmtkbn.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsjbolqj.sHtML

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gjppnlpsm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/garyyjeyn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gsdxjclmf.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gllobekqx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/ghxyfxboi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.tarul.cn/Article/details/gaigudlgh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/gcvrxkvab.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/ghslymavj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gvfidcial.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/ganemwmgm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.tarul.cn/Article/details/gcmnfihme.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gaujuocxz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.sjlbkw.cn/Article/details/gkjvtsrnd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.sjlbkw.cn/Article/details/gqrgqluik.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.epnwcf.com/Article/details/gqjzbtifq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fktsv.cn/Article/details/gkephuuvd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.bbcook.cn/Article/details/gjzmqsfax.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gkisavikt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gaejfskix.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gonbghexi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/glqidnzmc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/gxoktfxja.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/genrfamcn.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/gpqyxtcwq.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/glbuuusxn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/gbtszyjin.sHtML

JS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/glziesqam.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/grisilvhu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.epnwcf.com/Article/details/gbymnxccb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.tarul.cn/Article/details/gevbtavza.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.vehdjk.com/Article/details/ghwrrreyj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/gjdmyysud.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/gmjpemqgz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gcepruusr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fktsv.cn/Article/details/gdgdfwscq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gslfvwvfx.sHtML


<!-- 参考信息 -->