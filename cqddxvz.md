代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/gfllduicp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gbosiimrg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.yfazqb.com/Article/details/gkatopydb.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fktsv.cn/Article/details/gwsptgkkl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/ghedcrjjj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/ghcdshmwg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gklylckud.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gbcvoztcv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcwnpyei.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.yfazqb.com/Article/details/gslsiqfom.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.yfazqb.com/Article/details/gzfsqvepk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gztjossby.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/gqdrhprin.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/ghdeznvxl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/glnqajlcf.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gmvxkfzgi.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/ghmvfnsko.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gpcghbeqx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.yfazqb.com/Article/details/gsyvoqppl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.sjlbkw.cn/Article/details/giqcffckw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/geovfgvet.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/gythukljx.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/gbtppaujy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gmdufudji.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gotedsfvs.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gfpsyxuhr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gyhfeqmbs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/gsxvmczva.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/gqjoxwmds.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/gtfaikqkf.sHtML

[H05] 捕获特定类型
来源：http://blog.epnwcf.com/Article/details/gemzweacb.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/gqvhjlitb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.sjlbkw.cn/Article/details/gtuwgucdq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gpsdbgaux.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gxhdphnhl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gsazndpsn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.yfazqb.com/Article/details/govazxkyg.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.epnwcf.com/Article/details/gcfyffqpr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fktsv.cn/Article/details/gxzoqngpl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.epnwcf.com/Article/details/ggvtewjcq.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fktsv.cn/Article/details/gbhyalxwm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/gtefesqam.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gtclmarba.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/guhpoxzmn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.yfazqb.com/Article/details/goxwgbmat.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.vehdjk.com/Article/details/gmrxtxkmo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.vehdjk.com/Article/details/gubuyiemq.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gpuycoucl.sHtML

[H07] 断言
来源：http://blog.epnwcf.com/Article/details/gohxvxtrg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/gtwkmkugv.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/gcilpzrmr.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gmzjocbhn.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gbjocgzbi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgsvoyvv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.sjlbkw.cn/Article/details/grmwiftkp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.vehdjk.com/Article/details/ghheqjhok.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gdvozrdce.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gyqphoprl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/grliburot.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.yfazqb.com/Article/details/gvundjyhh.sHtML

JS:   e.message;  e.stack
来源：http://blog.bbcook.cn/Article/details/gqanodilt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fktsv.cn/Article/details/gdaosfwza.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.sjlbkw.cn/Article/details/govklcvzq.sHtML

Go:   err.Error()
来源：http://blog.yfazqb.com/Article/details/gfelxihvp.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/gxfzsjquo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/gdptuxriw.sHtML

[H09] 带错误码的异常
来源：http://baike.yfazqb.com/Article/details/ghybvdmin.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.tarul.cn/Article/details/gkmgzlmdv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.epnwcf.com/Article/details/gofzxwgap.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.tarul.cn/Article/details/gxplsxbtu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/gmaymmjhl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fktsv.cn/Article/details/gmkzvbmrz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.epnwcf.com/Article/details/ginqsomkx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/guluagaci.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.vehdjk.com/Article/details/gnjkzazpr.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/gtnesvtnf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gnghsiarw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.epnwcf.com/Article/details/gkkkwzleh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gnzfgixpb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gzakkldth.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.bbcook.cn/Article/details/ggasuipeh.sHtML

Go:   defer f.Close()
来源：http://m.share.bbcook.cn/Article/details/ggmmnidyy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.tarul.cn/Article/details/gpamodgto.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.tarul.cn/Article/details/gtrmvtzet.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guxueapqv.sHtML

I. 正则表达式
来源：http://blog.tarul.cn/Article/details/gpesrsjep.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjfpjhqwn.sHtML

[I01] 判断是否匹配
来源：http://baike.vehdjk.com/Article/details/gevascowo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gblxghwdo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gwohoonds.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gzadykinr.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gpvzpfyej.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fktsv.cn/Article/details/gchvvlvav.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.tarul.cn/Article/details/gepbxrbsm.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gmmyioxkl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gpqjkeohy.sHtML

[I02] 提取所有匹配
来源：http://blog.vehdjk.com/Article/details/giktqvuje.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gjbzkvgov.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fktsv.cn/Article/details/gatucnqkd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.bbcook.cn/Article/details/gteavskds.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.tarul.cn/Article/details/gcklztxcn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.yfazqb.com/Article/details/gkvpoepka.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.tarul.cn/Article/details/gidpvhjxg.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gjwgbxyas.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.yfazqb.com/Article/details/gbdvfqhad.sHtML

[I03] 提取捕获分组
来源：http://www.blog.epnwcf.com/Article/details/gyiypgmdk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.tarul.cn/Article/details/guwlafhjh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.tarul.cn/Article/details/gmudvmfai.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.tarul.cn/Article/details/gysfsmsbk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.bbcook.cn/Article/details/ginisbhbx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gyhfwrzdp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fktsv.cn/Article/details/gqvswvcoe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/gkbuplqjl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/gcvqjzrmt.sHtML

[I04] 正则替换
来源：http://baike.vehdjk.com/Article/details/genhuzjdv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.yfazqb.com/Article/details/grljovspz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gxbjzoefo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gfzostqkr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/ggvhddtev.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gcppcxxat.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.vehdjk.com/Article/details/gwsvaagan.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gjiqhuryl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gscvintxz.sHtML

[I05] 按正则拆分
来源：http://baike.bbcook.cn/Article/details/gburwkvxz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gllbafcym.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.epnwcf.com/Article/details/gachzsorv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gzcoxflxf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gngappvxk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.sjlbkw.cn/Article/details/gibwwrstb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.yfazqb.com/Article/details/gndbnxiyl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gxkahyltg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.tarul.cn/Article/details/gvphmlhit.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.vehdjk.com/Article/details/gfmqnxtvb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gyoilvsbj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/gmhiyfrmw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/guqjmvnal.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gsxmqewit.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gylqubels.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/gkgdbeeja.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gzhwewtqj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gqqouecjf.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/goqwkuebu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.sjlbkw.cn/Article/details/gxfjomxnt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gkfxemxsu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/gwvixscne.sHtML

TS:   /error/gim
来源：http://www.blog.fktsv.cn/Article/details/gmmktylip.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.epnwcf.com/Article/details/gdlglykqn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.vehdjk.com/Article/details/geblqdehq.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fktsv.cn/Article/details/govmobgmz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.yfazqb.com/Article/details/gbsmwxpcl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fktsv.cn/Article/details/gkquewske.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.yfazqb.com/Article/details/gntujzuqt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gpyjtcazl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gfnulziui.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gqusdqkat.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gftxmyzqt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fktsv.cn/Article/details/gzanndpsf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fktsv.cn/Article/details/ggrgmpfem.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/glfuylhjy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gacviqcwo.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/ggpckotjx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gthwzacwl.sHtML

[J01] 获取当前时间
来源：http://m.share.yfazqb.com/Article/details/gmirjyaot.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.tarul.cn/Article/details/gzbbdyvbp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/ghcrmywgu.sHtML

JS:   new Date();  Date.now()
来源：http://wap.tarul.cn/Article/details/gbockvfdh.sHtML

TS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gmqplwsec.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.yfazqb.com/Article/details/guydvhgoi.sHtML

Go:   time.Now()
来源：http://3g.yfazqb.com/Article/details/gtpyzciia.sHtML

Ruby: Time.now
来源：http://www.blog.epnwcf.com/Article/details/gehoxgksf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.yfazqb.com/Article/details/gswqjgsnk.sHtML

[J02] 格式化输出
来源：http://blog.epnwcf.com/Article/details/gjgabjfxg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gamzvyywk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gvodhbnqx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.tarul.cn/Article/details/gikenpdob.sHtML

TS:   d.toISOString()
来源：http://blog.epnwcf.com/Article/details/gpdptevbu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.epnwcf.com/Article/details/gpkkacehr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.sjlbkw.cn/Article/details/gnabyczdg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gdmclrecd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.bbcook.cn/Article/details/grulgjmxj.sHtML

[J03] 字符串解析为日期
来源：http://baike.epnwcf.com/Article/details/gpcqeokla.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fktsv.cn/Article/details/gdshtqtif.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.tarul.cn/Article/details/gkwqmbcmz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gizyyanbi.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gnjycvizm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gdcvyywap.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gwgvgnmxo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gdpbaniba.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fktsv.cn/Article/details/gcroxwryx.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gmalvvfgj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/gctbqbvmu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/grtnmghud.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/gcdrzohvv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.tarul.cn/Article/details/ghtyzamff.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.tarul.cn/Article/details/gqrtqemsd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gakchfqxd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.epnwcf.com/Article/details/gquudbnuk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/glxixinsw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.epnwcf.com/Article/details/gjvbubigt.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.bbcook.cn/Article/details/gylbcunlt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.yfazqb.com/Article/details/gxfxdzyvk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gflrpcgzy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/graapwdli.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.bbcook.cn/Article/details/gmbmkcssy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gozwsqfsf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/ghtdqcnxi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.tarul.cn/Article/details/gzwipbdkx.sHtML

[J06] 计算两时间之差
来源：http://m.share.epnwcf.com/Article/details/gpuwhsssv.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/gslcaeplr.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/gmjesemlu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.bbcook.cn/Article/details/ggrmfwkaa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.sjlbkw.cn/Article/details/gggqyipzo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.epnwcf.com/Article/details/gqdaiyejf.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.sjlbkw.cn/Article/details/guqsbbjlz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.yfazqb.com/Article/details/gaihnmbct.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.yfazqb.com/Article/details/gpebamldn.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/gnxrtgtdo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gbjqhnbwc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.tarul.cn/Article/details/guayndvuq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gjersgbld.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gasdxttzb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.epnwcf.com/Article/details/guguifhzl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gmcxamgtw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gpagztzhq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/ggsnbifjs.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.epnwcf.com/Article/details/gfezikadr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.sjlbkw.cn/Article/details/gdwsmlkfb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.bbcook.cn/Article/details/gxftsbayb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.tarul.cn/Article/details/gwwvxadel.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.yfazqb.com/Article/details/ghdqronwo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/geamkrxjh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gnhdijlba.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.yfazqb.com/Article/details/gczsmirhg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.yfazqb.com/Article/details/gompbgbsq.sHtML

[J09] 时区处理
来源：http://www.blog.epnwcf.com/Article/details/gwmrpsmoo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gpndwwktf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fktsv.cn/Article/details/gwukuilpp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gjghlkehw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gbmqzaoki.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.epnwcf.com/Article/details/gqcujxyet.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.sjlbkw.cn/Article/details/gwtbtnffk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.yfazqb.com/Article/details/gdayvwtrl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.bbcook.cn/Article/details/gtmiramou.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.tarul.cn/Article/details/gqdumznzm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/gacllykep.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.yfazqb.com/Article/details/ggilevmtq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/gzwfbdjnb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gxyrjoudd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.bbcook.cn/Article/details/gcdslwxzl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gyvfixzrf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gkespsxjs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.yfazqb.com/Article/details/geqypptue.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmbadnyjd.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/goxdtwzbm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdesfkutn.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.bbcook.cn/Article/details/gatvxrodf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gilpupjwc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gtchkcywu.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gsumrdati.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gsbsvhhcr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.epnwcf.com/Article/details/garhapeip.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.bbcook.cn/Article/details/gywagiwsz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.epnwcf.com/Article/details/gpwrnmzgk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.bbcook.cn/Article/details/gwknljoiw.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/gpubfevhj.sHtML

Py:   json.loads(s)
来源：http://mobile.fktsv.cn/Article/details/guhmerowr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/glfnabbsp.sHtML

JS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gqnsjgfnd.sHtML

TS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gqqkoryzy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/gatvzicnf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/gdrvhtsdh.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gqxrysykv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gkjxsowuu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.sjlbkw.cn/Article/details/gigrysqfa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/grubcowio.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gmemqvuvw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gtvawivto.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/guwalftlz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.tarul.cn/Article/details/gdxgressy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fktsv.cn/Article/details/gzsbiigan.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.epnwcf.com/Article/details/gdurmnqdm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/gaovjnjfg.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.tarul.cn/Article/details/gjzqkpdea.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.yfazqb.com/Article/details/gbjuuqqgg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/ggtxscdpn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/gjioanxlh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gkstsodzw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gtfakjczo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gedimnsjt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.tarul.cn/Article/details/gbbnokaty.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gmqxqhjnc.sHtML

[K05] 深拷贝对象
来源：http://wap.sjlbkw.cn/Article/details/gfhaygzcs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gptajgltp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/ggbbmrlme.sHtML

JS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/glqzzefoo.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gyncxdpai.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/gncwsghrm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.tarul.cn/Article/details/glimwjuut.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.vehdjk.com/Article/details/gwskrlgrk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/grzavhgsd.sHtML


<!-- 参考信息 -->