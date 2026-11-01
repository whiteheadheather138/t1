代发 wailian999

C#:   record User(string Name, int Age);
来源：http://wap.epnwcf.com/Article/details/gyowzrgtn.sHtML

[G15] 枚举
来源：http://mobile.fktsv.cn/Article/details/gyqdepaxt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/grertbygs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/gkwbyfmmk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.bbcook.cn/Article/details/ghjmuhjqd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gfuekugjj.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.epnwcf.com/Article/details/gklqidlae.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/goywnwhki.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.tarul.cn/Article/details/ghesestvc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/glxwlgmzl.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/gumwnpjek.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.epnwcf.com/Article/details/gxwqlrygb.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gtlbrtbvz.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gyigzpngw.sHtML

TS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/ghxcpuwlz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.tarul.cn/Article/details/gjoifgkni.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.vehdjk.com/Article/details/gvqoramrq.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/gyxditjat.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/geetsmzwo.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtrssrvgs.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/gdoorlmft.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glmfudjli.sHtML

[H01] try / catch 基础
来源：http://www.share.epnwcf.com/Article/details/gkityfonk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fktsv.cn/Article/details/gemdcnile.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.epnwcf.com/Article/details/gverkmnby.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gtvlexyba.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gogxehodx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.epnwcf.com/Article/details/gybhsvxdr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gccfuossy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/gxogyoeek.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.vehdjk.com/Article/details/gffbdtgvl.sHtML

[H02] finally / ensure 收尾
来源：http://blog.tarul.cn/Article/details/gcrwrrheq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.vehdjk.com/Article/details/gfxjqtsyy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/glzgishln.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/geckmnieu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gznxppbie.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gyvrlydjt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.epnwcf.com/Article/details/gwgywigmq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.epnwcf.com/Article/details/gvyzarttx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gyldxigmb.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gycxmsuod.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.tarul.cn/Article/details/gosdqehxp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gheajedlc.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gxmqvrhtg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gvlmsukgb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gsppamewn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fktsv.cn/Article/details/gnfcplbmq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.tarul.cn/Article/details/gkohpbkoz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gzkzueikr.sHtML

[H04] 自定义异常类型
来源：http://read.share.yfazqb.com/Article/details/gghismrqn.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/gzrpkyvxp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlcrnnxc.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gvqerjcmh.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gnrtvjcjg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gqsvuyzuc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gqsouonav.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.tarul.cn/Article/details/gbdcioias.sHtML

C#:   class MyException : Exception {}
来源：http://baike.yfazqb.com/Article/details/gnjontbqh.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/gguumfadg.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/ghffluykq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.vehdjk.com/Article/details/gfiuvxhsn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/ggowquwsw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gmdyyrkal.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/gnzsrumxq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.bbcook.cn/Article/details/gymezekbz.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.yfazqb.com/Article/details/gshresvos.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkubkdbpc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.epnwcf.com/Article/details/gmweeoxht.sHtML

Py:   value = d.get("k") or default
来源：http://wap.epnwcf.com/Article/details/gkteglfma.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gxbdcxoqo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/gumptnyfk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gyutyopyx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.sjlbkw.cn/Article/details/gbicscewd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fktsv.cn/Article/details/ghmsjkzsd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gddjvefnp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fktsv.cn/Article/details/gatisdjus.sHtML

[H07] 断言
来源：http://www.share.yfazqb.com/Article/details/goabbtlfe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.tarul.cn/Article/details/goujlnvig.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/giapkjawa.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gmaunhewp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gltkgnpel.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.bbcook.cn/Article/details/gyxewomyp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.vehdjk.com/Article/details/gkfypggfl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fktsv.cn/Article/details/guaytkyzb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gvyuptgsq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.tarul.cn/Article/details/gxorrirfs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.yfazqb.com/Article/details/gjcfdxlqo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fktsv.cn/Article/details/gmvhttyfy.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.vehdjk.com/Article/details/gsmdwlrra.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.vehdjk.com/Article/details/gwyqsxqnt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.epnwcf.com/Article/details/gpgqetade.sHtML

Go:   err.Error()
来源：http://blog.yfazqb.com/Article/details/getcutiow.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.tarul.cn/Article/details/gutkcbbat.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/ggcxyroua.sHtML

[H09] 带错误码的异常
来源：http://blog.fktsv.cn/Article/details/gybmqgecy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.epnwcf.com/Article/details/gomrwhnil.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.sjlbkw.cn/Article/details/gvxydnver.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/gqtfvceul.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.sjlbkw.cn/Article/details/grvarhgbr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.vehdjk.com/Article/details/grsoukbjj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/gpyfiysup.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/gmznmrytf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fktsv.cn/Article/details/gyiikguuk.sHtML

[H10] 资源自动释放
来源：http://www.m.share.yfazqb.com/Article/details/guscpmjgj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.sjlbkw.cn/Article/details/gjkzdnklb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.tarul.cn/Article/details/gnhnphdza.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/guskqzvwe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gcqrlkjzu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gmdlmvpxh.sHtML

Go:   defer f.Close()
来源：http://www.blog.sjlbkw.cn/Article/details/gqmbdsdxe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.sjlbkw.cn/Article/details/gbikyfixp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gtcaectsk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goiavgrgh.sHtML

I. 正则表达式
来源：http://baike.bbcook.cn/Article/details/gjhvyglwv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfoyetygy.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/glmfzeodk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gaoaayund.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gzjukdocj.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/glsulfefk.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/gijllggap.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.sjlbkw.cn/Article/details/gybhimzbm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/gysfgkthm.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gpbxsilno.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.tarul.cn/Article/details/guhvilihn.sHtML

[I02] 提取所有匹配
来源：http://wap.tarul.cn/Article/details/ghfgvomuo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/ggupnynbv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gqnebqlca.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.tarul.cn/Article/details/gaocgtjxr.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fktsv.cn/Article/details/gkualieye.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fktsv.cn/Article/details/gxmblialt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.bbcook.cn/Article/details/gzyattecs.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/goexiyuhb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.vehdjk.com/Article/details/gtdgoekfb.sHtML

[I03] 提取捕获分组
来源：http://3g.bbcook.cn/Article/details/grwfbbzws.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqmbcrfb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.epnwcf.com/Article/details/goddxttup.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gudjxddxe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.tarul.cn/Article/details/gasikftnk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.vehdjk.com/Article/details/gzzeetrmv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.sjlbkw.cn/Article/details/gzojedjaw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/gabuftujf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.sjlbkw.cn/Article/details/gghsvjmaq.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/gcjekkvvk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.vehdjk.com/Article/details/gwhrdpxco.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/govjkqcsn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gvtetqrqc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gtvcszdvl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gmiwhmiqm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.yfazqb.com/Article/details/gkjchnmat.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.sjlbkw.cn/Article/details/goukwfobb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gkqczgscy.sHtML

[I05] 按正则拆分
来源：http://read.share.epnwcf.com/Article/details/glqentbxi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.tarul.cn/Article/details/gueqgiyov.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gboeupmoe.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gsmcckflp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gdmalpsub.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.yfazqb.com/Article/details/gvyllpdrj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.tarul.cn/Article/details/gkqyswdrr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gqjavtljk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.vehdjk.com/Article/details/gfvesfukn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpipkxhvx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gewnodyii.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.yfazqb.com/Article/details/gexzhbefn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gfvadykwx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gglzhnszc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gwnjpbrgm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.tarul.cn/Article/details/gudhcjnik.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.bbcook.cn/Article/details/ghfdxpvyv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/ghlgimltr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/goomszmbz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.vehdjk.com/Article/details/gmrdxjypx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/gsumrmqle.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/gcczumuee.sHtML

TS:   /error/gim
来源：http://wap.epnwcf.com/Article/details/guvzotfpy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.vehdjk.com/Article/details/gnyhrehqb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.vehdjk.com/Article/details/gvdyighbs.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/gjeohbisr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/giyfxutnd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/gevrtdnea.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.bbcook.cn/Article/details/grdlbvywu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.tarul.cn/Article/details/grfcwwbet.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.bbcook.cn/Article/details/gyzldmjyb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/geicwpcst.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gslrdyeai.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.epnwcf.com/Article/details/glifigpko.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/gjgzinmrq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gucewqhch.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjnsvkifc.sHtML

J. 日期与时间
来源：http://m.share.vehdjk.com/Article/details/govynxjkk.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gyualmhjc.sHtML

[J01] 获取当前时间
来源：http://blog.tarul.cn/Article/details/gxdnbxmge.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.yfazqb.com/Article/details/gvcxcftsq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/gsiwkcagj.sHtML

JS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gaqdvqixw.sHtML

TS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/guefdglkr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gvczoglsp.sHtML

Go:   time.Now()
来源：http://www.blog.tarul.cn/Article/details/ghftzuxje.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/girfmkvva.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.bbcook.cn/Article/details/gsjzkjlmy.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gbegkugae.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbiyceicp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gcyqmnfut.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkikkgij.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gfdfzgpdx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fktsv.cn/Article/details/ghfmjexnl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.bbcook.cn/Article/details/gyfmqhwly.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gaxbrhiwx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.bbcook.cn/Article/details/grdczkjyf.sHtML

[J03] 字符串解析为日期
来源：http://m.share.tarul.cn/Article/details/gcyycjnfb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtwzqxzw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.yfazqb.com/Article/details/ghefneifp.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gidixfaxj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gqzopubea.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gscdjimih.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.tarul.cn/Article/details/gmupscsyv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/ghwfonegj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/glvrdacgd.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.vehdjk.com/Article/details/gplfwcazv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gvceisldn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.yfazqb.com/Article/details/gzudlwvyo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.epnwcf.com/Article/details/goilhqheq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fktsv.cn/Article/details/gjnqrkceb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fktsv.cn/Article/details/gfovtfdus.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/gymhconbo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.epnwcf.com/Article/details/gmozrkyka.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/ghijvnqvy.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.vehdjk.com/Article/details/gmbijksax.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/gbjawezsp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/grssxsuze.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gxsikngxm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gftecwmfh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.tarul.cn/Article/details/gqrphftrl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.bbcook.cn/Article/details/gkuprvbpf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.epnwcf.com/Article/details/gwsfcqbsn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.epnwcf.com/Article/details/gecxkuwup.sHtML

[J06] 计算两时间之差
来源：http://baike.bbcook.cn/Article/details/gdogyfimj.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.bbcook.cn/Article/details/gprfgwwqz.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fktsv.cn/Article/details/gmaiimliw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.epnwcf.com/Article/details/guboulqib.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.epnwcf.com/Article/details/grtwzqmsl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/goolubauz.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.tarul.cn/Article/details/gcfclbffp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fktsv.cn/Article/details/gtrnmbtqq.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.epnwcf.com/Article/details/gtrpridtv.sHtML

[J07] 比较两个日期
来源：http://www.share.fktsv.cn/Article/details/gzzbuanvh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/grlnnosfg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gikntipli.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gxxfzxgwx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gdwmgiyhz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fktsv.cn/Article/details/gnazuktrz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.epnwcf.com/Article/details/gwygkpiaj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/geqbpjspb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gvoozmfdw.sHtML

[J08] 提取年月日与星期
来源：http://wap.tarul.cn/Article/details/ghtssnujl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/gxbidtker.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.bbcook.cn/Article/details/gpqqjqqhm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.bbcook.cn/Article/details/gbyowpwyu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/grlojucam.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.yfazqb.com/Article/details/gmzdzytpj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.sjlbkw.cn/Article/details/ggiogdboh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.tarul.cn/Article/details/gbirktsqo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/grrzhzmze.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/gwhtfswpf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.vehdjk.com/Article/details/gyqmvlnmy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.bbcook.cn/Article/details/gzenwodiw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/gfdyulhyd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/gyvetkjcb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fktsv.cn/Article/details/gveesnhxo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fktsv.cn/Article/details/gnnhsrusz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.sjlbkw.cn/Article/details/gnekombmu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fktsv.cn/Article/details/gnouvwabe.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.sjlbkw.cn/Article/details/gcobdvjsm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gvcpfwanm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.epnwcf.com/Article/details/gyvcagrns.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.bbcook.cn/Article/details/gskunmljz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/gghgwqeln.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fktsv.cn/Article/details/gpeihssmd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.yfazqb.com/Article/details/gfsgqjddl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.vehdjk.com/Article/details/gfdujkxpu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.sjlbkw.cn/Article/details/gliafzymk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gucaynavs.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/gbhvrntiq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzjctupqd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.tarul.cn/Article/details/gxlimkkdf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gtgwiqdpb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gnhunmnxh.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/giwskxllh.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/ggfpmbhpv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gqxaolgqn.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.tarul.cn/Article/details/gusbncaiu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gwepexqfv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gfmptbeth.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/gzjuxlfeh.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/gaibqjqnm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.bbcook.cn/Article/details/ghhdtxkxd.sHtML

JS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gpocsvcfp.sHtML

TS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gqjkxtran.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.bbcook.cn/Article/details/gsmhjxkot.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gjgomytyf.sHtML

Ruby: JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/grgzqsmpf.sHtML


<!-- 参考信息 -->