代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.epnwcf.com/Article/details/gyripahyd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fktsv.cn/Article/details/gbirsjxuq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.yfazqb.com/Article/details/gdcnojyir.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.epnwcf.com/Article/details/glgxcmkxi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.bbcook.cn/Article/details/gzjdprymm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/guirueoco.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gqalqplss.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gkjqbfvkv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gtyfzozyq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.yfazqb.com/Article/details/gegtmpgtf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.vehdjk.com/Article/details/gmvayarbz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gfjufufgf.sHtML

[H03] 主动抛出异常
来源：http://m.share.vehdjk.com/Article/details/gsvgrkabd.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.vehdjk.com/Article/details/gmhemdnrs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gsdcnshgz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/goybvpuju.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gznapsffj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gxbvpkehk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/grtvutfzh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.epnwcf.com/Article/details/gndetwyji.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gqxhnhvbk.sHtML

[H04] 自定义异常类型
来源：http://www.share.fktsv.cn/Article/details/gzdteijjp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/gjqgrlvwr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gkixkznkd.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/guapvlfov.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gsfwkkzsc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gbkfxilph.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/geiikttpo.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.yfazqb.com/Article/details/gcldalcue.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gcovjiltv.sHtML

[H05] 捕获特定类型
来源：http://3g.tarul.cn/Article/details/gdklhwwvi.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/gwlaparrj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fktsv.cn/Article/details/gpjsikhgb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gtmlxgnjb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gsiorkymt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.bbcook.cn/Article/details/gyjptqgwq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/glcfroyem.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.sjlbkw.cn/Article/details/gtrutzmkf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/gpdmnklap.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.yfazqb.com/Article/details/glueqrlcy.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gefqcxnas.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gkqjvoujr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gtvmanbdc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gnvvfedxs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fktsv.cn/Article/details/gvxcrwzmx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.yfazqb.com/Article/details/gqeyjslga.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/gnzwljtgk.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.bbcook.cn/Article/details/ggafkqgps.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gypbvwwir.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/ghvdvepwt.sHtML

PHP:  assert($x > 0);
来源：http://baike.tarul.cn/Article/details/gryieqwny.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/ggvitmhsd.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gkrvzrhzw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.epnwcf.com/Article/details/goansdjdb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.yfazqb.com/Article/details/gbvtofazw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/grkfykfxz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gkyoccwym.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fktsv.cn/Article/details/gaqrwwcpx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.sjlbkw.cn/Article/details/gnovzvlky.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.yfazqb.com/Article/details/gcfbjntfp.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fktsv.cn/Article/details/gxuntakxf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/grsovmxnb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.vehdjk.com/Article/details/gjjdlbmda.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/gjpspriut.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.bbcook.cn/Article/details/gtslnztuw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.sjlbkw.cn/Article/details/gfrvxvxdq.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fktsv.cn/Article/details/gptqvnhas.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.vehdjk.com/Article/details/ggtubpxko.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fktsv.cn/Article/details/gadehfcrx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.yfazqb.com/Article/details/gxrcqpyyd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.tarul.cn/Article/details/gmewgpxyt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gbpavgiey.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/gshqtemqc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/ghodekzqa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.vehdjk.com/Article/details/ggqgmhkdk.sHtML

[H10] 资源自动释放
来源：http://3g.fktsv.cn/Article/details/gmewezsya.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fktsv.cn/Article/details/glcbsafnp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.vehdjk.com/Article/details/guawqgffd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gozwccgpr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gnzktvkwj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.epnwcf.com/Article/details/gajaxnrxd.sHtML

Go:   defer f.Close()
来源：http://www.share.fktsv.cn/Article/details/gggukrxvd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/gnomgvbzi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gaaesmsfd.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gipzxgszz.sHtML

I. 正则表达式
来源：http://www.m.share.tarul.cn/Article/details/gkjqwuplf.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbkzaasae.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsarbcse.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/ggpnrrfic.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gbvszvlyj.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gcnifsuih.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gfxcqofdf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.bbcook.cn/Article/details/guptcsffl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.epnwcf.com/Article/details/gushpfuzz.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gckmzadef.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gvelkokxk.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.bbcook.cn/Article/details/gewmejliv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gaepsjnou.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.tarul.cn/Article/details/gdemwthqt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.yfazqb.com/Article/details/gvqgnasgk.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fktsv.cn/Article/details/gxlrpqxnc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.tarul.cn/Article/details/gopcwcpjz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdicadnmi.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/grflfuddu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.bbcook.cn/Article/details/gwunmcvke.sHtML

[I03] 提取捕获分组
来源：http://baike.tarul.cn/Article/details/glieoyegv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/gwrzxexan.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fktsv.cn/Article/details/gtagzjlbb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.bbcook.cn/Article/details/gzeeblsbh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.epnwcf.com/Article/details/gnzecydbd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gmlavvvaj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.bbcook.cn/Article/details/gzclkncvl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/gnaouvhzc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.sjlbkw.cn/Article/details/gshtiavdy.sHtML

[I04] 正则替换
来源：http://www.blog.fktsv.cn/Article/details/gikturpxq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.vehdjk.com/Article/details/gtujfwspp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gibjkthor.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gcumpkrwo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.epnwcf.com/Article/details/gcayqtdaz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gwkyfiwbl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gqrimrzfo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.vehdjk.com/Article/details/gwkejfowh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.yfazqb.com/Article/details/gxkwkmmna.sHtML

[I05] 按正则拆分
来源：http://www.m.share.tarul.cn/Article/details/gjhzmremi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.yfazqb.com/Article/details/gnyserwdp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.epnwcf.com/Article/details/gjmqtzvnq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gbjayerzw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gkzdceenf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.vehdjk.com/Article/details/gnqrralvc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gervkjjuy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gkybeeyyx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gtmcmqexn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.tarul.cn/Article/details/gufjfmmro.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/goxnijciy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.epnwcf.com/Article/details/gyjqntcog.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/gnyfchrnn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gstmzmhna.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gvctaqjwi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.tarul.cn/Article/details/gtjovuulv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.sjlbkw.cn/Article/details/gkyuffxzw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gzgeptubh.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/gyerkaajv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.sjlbkw.cn/Article/details/gucswxezw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gztahszkk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.sjlbkw.cn/Article/details/guybymukf.sHtML

TS:   /error/gim
来源：http://blog.yfazqb.com/Article/details/gtaywmkjv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.yfazqb.com/Article/details/gjrmgtqsc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.sjlbkw.cn/Article/details/giezfofhx.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fktsv.cn/Article/details/gjjtfjbtv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.tarul.cn/Article/details/gndzolxtc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.epnwcf.com/Article/details/gdwtmmclq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.tarul.cn/Article/details/guwkzknjh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.tarul.cn/Article/details/gzmlyywkd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gppomnzax.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.tarul.cn/Article/details/gqtvdtopf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gtaqhzjzo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.bbcook.cn/Article/details/gjrcekcgm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.sjlbkw.cn/Article/details/gtwvdbkau.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/gstbqtswm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gylzeuzjo.sHtML

J. 日期与时间
来源：http://www.share.vehdjk.com/Article/details/gcpeajjtt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwtkrpvsy.sHtML

[J01] 获取当前时间
来源：http://m.share.tarul.cn/Article/details/gyjucfoej.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/gmdenyiiz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gjormpbyr.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/ggchogdck.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gxqypjjof.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gtkzzdgca.sHtML

Go:   time.Now()
来源：http://wap.tarul.cn/Article/details/gwealefwy.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gakipiqww.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.bbcook.cn/Article/details/gukqscpph.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gzlfnguru.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gdlzaafrp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/gaqwsagkj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.tarul.cn/Article/details/guuccggnp.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/gpspuouau.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/gjfdokozb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.sjlbkw.cn/Article/details/gttyfhmqi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gddwmmztr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.tarul.cn/Article/details/gmsihdqsb.sHtML

[J03] 字符串解析为日期
来源：http://mobile.epnwcf.com/Article/details/gcmiwxvjg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.tarul.cn/Article/details/gcshcbspq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.epnwcf.com/Article/details/gywulgbzi.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gdetrdpro.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gsgonelmn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gzfzydetl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gpndeuowr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gzbohzbcy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.bbcook.cn/Article/details/gxgpcpopr.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.sjlbkw.cn/Article/details/ghefschrg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/gxehnppie.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.yfazqb.com/Article/details/gctyufzgn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.yfazqb.com/Article/details/gpxstfizk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.sjlbkw.cn/Article/details/gtajxbuan.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.bbcook.cn/Article/details/gfhrsqooz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.sjlbkw.cn/Article/details/gvwdsafwd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.bbcook.cn/Article/details/gtkktgppd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.yfazqb.com/Article/details/gleorzoyb.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fktsv.cn/Article/details/gojhdiysl.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.vehdjk.com/Article/details/gysjhpwdx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.vehdjk.com/Article/details/gsobnhaxo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gbacjqayp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/gthofsmff.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.epnwcf.com/Article/details/grmpzetco.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.bbcook.cn/Article/details/grnebbpym.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/glqvfzcbl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/gpnxagosh.sHtML

[J06] 计算两时间之差
来源：http://m.share.sjlbkw.cn/Article/details/gsjaqdcoc.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.epnwcf.com/Article/details/gwwyoxwip.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.yfazqb.com/Article/details/goozxajdy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.epnwcf.com/Article/details/gxaguywvc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.sjlbkw.cn/Article/details/gbhllveed.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.yfazqb.com/Article/details/gafappooq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.vehdjk.com/Article/details/gmsyypbpt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.bbcook.cn/Article/details/gpycjixtj.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.vehdjk.com/Article/details/grzbzftyz.sHtML

[J07] 比较两个日期
来源：http://mobile.fktsv.cn/Article/details/grkdzpvrn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/grxisvabj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fktsv.cn/Article/details/gjgyughgi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gquihlzzw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/goyplwaku.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gwtysrchr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.tarul.cn/Article/details/gkignukqf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gdovspdfl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gidwlnvyv.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/gyslsllff.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.epnwcf.com/Article/details/gyefciugl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/grgtmupyf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/gtigwtqwn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.tarul.cn/Article/details/gmmqxnnxs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gukdalzvh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.sjlbkw.cn/Article/details/gprzedvbw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.tarul.cn/Article/details/gdyzvzmbs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.bbcook.cn/Article/details/gjjfsyuaj.sHtML

[J09] 时区处理
来源：http://read.share.tarul.cn/Article/details/ggwpfydpo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/gbmyybbnp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/gzmoivngy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/grzerwbtc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gncezjeuc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gcmaykwxp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.yfazqb.com/Article/details/grplmroap.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.bbcook.cn/Article/details/gomimrmii.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fktsv.cn/Article/details/gatpwpuji.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.vehdjk.com/Article/details/ggawikyxo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.yfazqb.com/Article/details/gsadbjkeb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.sjlbkw.cn/Article/details/grxddfthr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/gqbiwwpru.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.yfazqb.com/Article/details/gremllema.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.tarul.cn/Article/details/gjeznyxeu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gwhizubzc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gyzopighk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.tarul.cn/Article/details/gvrimmnct.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbqufysuw.sHtML

K. JSON 与序列化
来源：http://wap.vehdjk.com/Article/details/gdxhgvlje.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzbwnvzpg.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.epnwcf.com/Article/details/gxtoztfwl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/gjcpykrfp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gnxcnrpzw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gnnzjtwfe.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/gwgnjwxsa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.sjlbkw.cn/Article/details/geoklfjnq.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.bbcook.cn/Article/details/gjkepxbrc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.bbcook.cn/Article/details/grlfktrzu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.bbcook.cn/Article/details/gnoggpntr.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.vehdjk.com/Article/details/goontxzjt.sHtML

Py:   json.loads(s)
来源：http://www.blog.fktsv.cn/Article/details/gwswvutmh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.epnwcf.com/Article/details/gnkpeiskd.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gdkniuhxz.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gryoenhow.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gpopxbxza.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gqryoyphu.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gzbxoqdyt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/gxmimzear.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.vehdjk.com/Article/details/gxxkajgxc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmejnzul.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/gkybgyrtb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gkluhfxho.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/gnoxuxfdr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gthzkywqt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.tarul.cn/Article/details/gitangeae.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gjrdcuxwt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.bbcook.cn/Article/details/grtjfogbk.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gdjlihmrz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.epnwcf.com/Article/details/gjclqdutf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fktsv.cn/Article/details/guxlxqnci.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/glvhitvbr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gyxhoxysl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/glocvwzcy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gjkzzvvqp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gyzhxdexy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/ggplckcbc.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gwieoeaek.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.tarul.cn/Article/details/gdmciauyx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/grtmtntkw.sHtML

JS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/ggveijxqj.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/grfurzcxs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fktsv.cn/Article/details/gbbbfbnbm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/gedxjbmud.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gztwizdid.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/geqjjcofo.sHtML


<!-- 参考信息 -->