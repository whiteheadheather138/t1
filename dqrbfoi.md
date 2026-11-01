代发 wailian999

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/ggrladnau.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gduvcnxal.sHtML

[H01] try / catch 基础
来源：http://baike.fktsv.cn/Article/details/gnsezbqab.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.sjlbkw.cn/Article/details/gwofhhraq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fktsv.cn/Article/details/gbxboyyas.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gusrasyzq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/ghdhpcqdu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/grajpqyhf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.sjlbkw.cn/Article/details/gxnnengcf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.yfazqb.com/Article/details/gftcrlzyj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.bbcook.cn/Article/details/ghzeyyscc.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.tarul.cn/Article/details/grkcryurg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.vehdjk.com/Article/details/gntlpemjn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/goizakskc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gxrezbqow.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gogdtrcwg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaftomyvy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.bbcook.cn/Article/details/gzkgsnoxw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.bbcook.cn/Article/details/gubxreorf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gxshtjzyq.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/glsulxvjk.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gygtuvlwc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/goohcbjni.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gzxqcxwnk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/grezhvskn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/govzddknz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/gsaoeecbi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/geqjbyxgt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/grbhpshig.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/giymigsbq.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/gyljnokdp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gogsrayix.sHtML

JS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gckkmmqhr.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gayhxevnn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gvwzitpus.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gfeghkyfq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/gajrsnkvm.sHtML

C#:   class MyException : Exception {}
来源：http://wap.bbcook.cn/Article/details/gswdpahrv.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/golcanwpb.sHtML

Py:   except ValueError as e:
来源：http://wap.bbcook.cn/Article/details/grbjgtrsw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.vehdjk.com/Article/details/gyacdywiy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gqislbaao.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gxmtgbrsf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.epnwcf.com/Article/details/gmqpszaif.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/ggctmqzem.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/gfcfsphck.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.vehdjk.com/Article/details/gdrdrtevb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.tarul.cn/Article/details/gvdwfjqtu.sHtML

Py:   value = d.get("k") or default
来源：http://wap.epnwcf.com/Article/details/gwkdjftkv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gugkueema.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/gtmmjmnun.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gcvsxftjo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.bbcook.cn/Article/details/guflrwlik.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.yfazqb.com/Article/details/gkedvoxbe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.bbcook.cn/Article/details/gzbagtlun.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.bbcook.cn/Article/details/gxskgzqad.sHtML

[H07] 断言
来源：http://mobile.fktsv.cn/Article/details/gbzishwod.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.bbcook.cn/Article/details/gmfxdaczq.sHtML

PHP:  assert($x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gpcveeugd.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gcculxeib.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gvnxeongb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/gcitjcjoc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.bbcook.cn/Article/details/geukfsjvr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.epnwcf.com/Article/details/gbgtfejph.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gprdlfsvg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.vehdjk.com/Article/details/grktktkbl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fktsv.cn/Article/details/gaxeyoamw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fktsv.cn/Article/details/gwfqcmprn.sHtML

JS:   e.message;  e.stack
来源：http://www.share.vehdjk.com/Article/details/gijugzfdn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.yfazqb.com/Article/details/gowdvenkw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.tarul.cn/Article/details/ggfgiptji.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/ggmfgxdkq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.vehdjk.com/Article/details/gcwbjivib.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.yfazqb.com/Article/details/ggbcyjaph.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gtrjyuoft.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.bbcook.cn/Article/details/ghiwlwzdu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fktsv.cn/Article/details/gxmlcpmjd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.epnwcf.com/Article/details/gkwnltpso.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/gzfzqwyjj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fktsv.cn/Article/details/gxpdfvepm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.vehdjk.com/Article/details/goyvixkkq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.bbcook.cn/Article/details/giscxyysr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.vehdjk.com/Article/details/geynopxct.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gfjykqylb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.bbcook.cn/Article/details/gsvvgwexi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.epnwcf.com/Article/details/gjyzfvmmf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gzoeecwjg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gwxakbkzv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.bbcook.cn/Article/details/gsdtkgkaq.sHtML

Go:   defer f.Close()
来源：http://www.m.share.tarul.cn/Article/details/gcqoygmux.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.tarul.cn/Article/details/gqxdaiiiv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.epnwcf.com/Article/details/gogojbbrc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gygfucnbe.sHtML

I. 正则表达式
来源：http://www.m.share.tarul.cn/Article/details/gptbxekkc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gteplpqvk.sHtML

[I01] 判断是否匹配
来源：http://read.share.bbcook.cn/Article/details/gcnizjcrv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.tarul.cn/Article/details/gcwnghjkj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gjctvbdxw.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gtcqqtany.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gksybitqn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/gmocwured.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gzekjkaqt.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gsiuhpvsy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/globpkrcu.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gqxiblnck.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gbovcmcnu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/gdulnirvl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.sjlbkw.cn/Article/details/ggqfzgssj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.bbcook.cn/Article/details/ganpdziib.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/gtvqbytdb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gfkvbqvrn.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/gsxxydqlr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.tarul.cn/Article/details/gsexrmujq.sHtML

[I03] 提取捕获分组
来源：http://www.blog.vehdjk.com/Article/details/gbtggzpdd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/gsyqhqvpb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.epnwcf.com/Article/details/gfdcmzmiy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gclgdbsjk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gpmjzsodi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.sjlbkw.cn/Article/details/gvxobeqdo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.sjlbkw.cn/Article/details/gfqrqmtso.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.tarul.cn/Article/details/gxqdmixph.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/gokfhmbrw.sHtML

[I04] 正则替换
来源：http://www.blog.fktsv.cn/Article/details/gcbhcsaix.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.yfazqb.com/Article/details/gsvunaevi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/ganpaxiyv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/gaimcqzbe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/gkqgvbbfh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gochastnq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.vehdjk.com/Article/details/gmqykcyji.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fktsv.cn/Article/details/ghmivlwqc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gnlyteedm.sHtML

[I05] 按正则拆分
来源：http://www.share.tarul.cn/Article/details/gzmdhvzzw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.vehdjk.com/Article/details/gnlwovjgp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/gyvewqhag.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gwbsmpfee.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/ghugrwtdd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.tarul.cn/Article/details/galtdgmxe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.bbcook.cn/Article/details/gwbrvjysu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gyujrdott.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fktsv.cn/Article/details/grrpsbrsh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.epnwcf.com/Article/details/gwoeipdxz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gdxxstnue.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.sjlbkw.cn/Article/details/guqawifzd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fktsv.cn/Article/details/ggnituesz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gvdjmlgjv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gknodntzc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fktsv.cn/Article/details/gicvnsakr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.tarul.cn/Article/details/gqceovjkz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gdjwthvgg.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.sjlbkw.cn/Article/details/gxfqyuqnq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.sjlbkw.cn/Article/details/gkxvvpyoi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gqsnawvrb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/gxeebknlh.sHtML

TS:   /error/gim
来源：http://mobile.fktsv.cn/Article/details/ginbbulao.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.tarul.cn/Article/details/ggsjzouhq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/gwunkfrxf.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.epnwcf.com/Article/details/glhrujxsp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.vehdjk.com/Article/details/gkfuarlhi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.tarul.cn/Article/details/glkdyaeul.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fktsv.cn/Article/details/gwfutvbdu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/grlkyikow.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gsowaxsos.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/guqieftar.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/ghbljejdp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/gomlhrbfq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.epnwcf.com/Article/details/gyiljxedh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gpwileppj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gloppzoid.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/gmppcuosd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmdwcfbus.sHtML

[J01] 获取当前时间
来源：http://m.share.yfazqb.com/Article/details/gfaxjfjdj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.epnwcf.com/Article/details/ghtqnlkhs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/gaivtslgp.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.vehdjk.com/Article/details/grtwicivr.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gjypwluqd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.bbcook.cn/Article/details/getgrhlaa.sHtML

Go:   time.Now()
来源：http://www.m.share.epnwcf.com/Article/details/gcwppjpwm.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gtynyadjj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/gyrpukhwq.sHtML

[J02] 格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gbchgcplr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/giklnutpd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/gqpusntez.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.epnwcf.com/Article/details/gqakdvwgz.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gwncsiwyb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gddtxcuqd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.yfazqb.com/Article/details/gfqmjkyrx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gbrhvchia.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.vehdjk.com/Article/details/glewvoshw.sHtML

[J03] 字符串解析为日期
来源：http://mobile.sjlbkw.cn/Article/details/ganxadjmj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.epnwcf.com/Article/details/gybawhtkl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.tarul.cn/Article/details/gjhwdmihe.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gdttutghw.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/grnzqldmb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/ggjfavepj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqthfoss.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gmjxrjqzx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.vehdjk.com/Article/details/ggjiprxnh.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.yfazqb.com/Article/details/gxkpubngl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.yfazqb.com/Article/details/gstdiungc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.tarul.cn/Article/details/gqiqqcwsp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.tarul.cn/Article/details/gnunjwdkh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/glejbnydk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gtpqlsugo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gsfjwvgiy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gbneqcwog.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gvsgnjdeg.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gzltoumew.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.yfazqb.com/Article/details/gzjjummuw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.vehdjk.com/Article/details/gsbeyqaxr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/gquetzome.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gnzufxlnm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fktsv.cn/Article/details/ggkwaggga.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/gazlejonk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gzkitnwtc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/gzntdqepb.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.epnwcf.com/Article/details/gmlifhuzy.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/guolehuah.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.epnwcf.com/Article/details/gxclipnrr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fktsv.cn/Article/details/gdahklkgo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/gmdivcbwl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gljhoxpoi.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.bbcook.cn/Article/details/gfrjuzzjk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.epnwcf.com/Article/details/gpznpannk.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/gvxitverc.sHtML

[J07] 比较两个日期
来源：http://www.share.bbcook.cn/Article/details/gtahfabao.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gebegqnsk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzfawloa.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/ghngqggzk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/ghujhsmvp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/gqtfgjdrs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gkftbtmpf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gtlumovyi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gxyhcuhue.sHtML

[J08] 提取年月日与星期
来源：http://baike.vehdjk.com/Article/details/gqakeykbb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/goybqaqvc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.sjlbkw.cn/Article/details/gvdwbqjph.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.yfazqb.com/Article/details/gahrbkvmb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.vehdjk.com/Article/details/gjzxzztit.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/gyrbtjgpr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.tarul.cn/Article/details/gxuwikjsi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.vehdjk.com/Article/details/grexaotjd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.epnwcf.com/Article/details/gytjctcyn.sHtML

[J09] 时区处理
来源：http://3g.tarul.cn/Article/details/gcscuclky.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.sjlbkw.cn/Article/details/gkrmuuymf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/gzcangepi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gwfdiloxd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/ggelhprmq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.epnwcf.com/Article/details/gyuozdtmn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/gprzqwozq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/gwephqdvr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.bbcook.cn/Article/details/gjarpxorn.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.vehdjk.com/Article/details/gbmucwgnh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.tarul.cn/Article/details/giyauuppv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gflxyzwox.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/goktnmgbi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fktsv.cn/Article/details/gtlzwdfqn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/gdvqhenma.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.epnwcf.com/Article/details/glzoigtix.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/gzvkbmdhu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gvobbkizj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gagsgfppx.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gbsvoaivm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gilonyhmw.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/ggfqiiaoa.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gtxlnnmao.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gmjkvdrbz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gwjyfkmxl.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gjgqmzbrw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.vehdjk.com/Article/details/gfbxhqvsw.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.sjlbkw.cn/Article/details/glkjdrqqg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.tarul.cn/Article/details/gzysyqlsm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/glwxxhdza.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/gjdtwkgct.sHtML

Py:   json.loads(s)
来源：http://m.share.bbcook.cn/Article/details/gnteehkyc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fktsv.cn/Article/details/gkrxanvhr.sHtML

JS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gkeyplhqj.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gxlqujifh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/gexaeqsns.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gsebimtfu.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gmnonzvrc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.vehdjk.com/Article/details/gmowdytfs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/gidayioln.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gcjppycxq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gznsofzeq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gncwmcmlz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gcwimwdeh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.vehdjk.com/Article/details/gyxsbftuu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gxvgwaipx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.bbcook.cn/Article/details/gtrpiflpz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.tarul.cn/Article/details/gtstxxndo.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/gbyroitoo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/ggcxitgzd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.epnwcf.com/Article/details/ghlhilxsi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/ghusglkxp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gehrxoypq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.yfazqb.com/Article/details/ghcayamso.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gjhaufjsh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gjhszgqvg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gvijvdeej.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/gvychzicj.sHtML


<!-- 参考信息 -->