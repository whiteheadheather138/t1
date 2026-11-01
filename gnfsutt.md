代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://read.share.epnwcf.com/Article/details/giimgfjhf.sHtML

Java: record User(String name, int age) {}
来源：http://baike.epnwcf.com/Article/details/gqbouvwhv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/gfbfnofan.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gdabhyvfv.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.tarul.cn/Article/details/gwpzwyvho.sHtML

[G15] 枚举
来源：http://3g.yfazqb.com/Article/details/gmpkbvkmj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.epnwcf.com/Article/details/gwqbvcqlh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.yfazqb.com/Article/details/gvmlbhstl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.sjlbkw.cn/Article/details/gdjulxdpx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/guzqpnjta.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.sjlbkw.cn/Article/details/gpybyoanr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.epnwcf.com/Article/details/gionsdfyg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/gzisyataq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/gkkgacers.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.bbcook.cn/Article/details/gktasqyyn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.sjlbkw.cn/Article/details/gewdhlisk.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fktsv.cn/Article/details/gvkwmsxni.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gojosxtsf.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/ggbitgjhk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.yfazqb.com/Article/details/gsluhvgmn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/gcmnzeqfa.sHtML

Ruby: obj.instance_variables
来源：http://read.share.sjlbkw.cn/Article/details/gnbxpihvr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gxqmhfjfb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzvtfxozp.sHtML

H. 异常与错误处理
来源：http://mobile.epnwcf.com/Article/details/gdzfbpgtq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/guugkxdvg.sHtML

[H01] try / catch 基础
来源：http://www.blog.bbcook.cn/Article/details/giemrdcat.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.bbcook.cn/Article/details/gmvpmabsk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.tarul.cn/Article/details/gjbmwamqg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gfnzybmov.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gqaufstgz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.sjlbkw.cn/Article/details/gbtjfhvav.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/gfiizdibh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.bbcook.cn/Article/details/gzpprnkzh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/ggkvlvljd.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/gosrowflm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.bbcook.cn/Article/details/gsmgqyxlo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/ggozpzrqy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gcnagxrwd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gjsdycnnu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gfrrlrhlw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.bbcook.cn/Article/details/gpuiwboky.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.epnwcf.com/Article/details/grsulqzpc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gdzualczy.sHtML

[H03] 主动抛出异常
来源：http://3g.yfazqb.com/Article/details/gxdvblkxd.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gccsfqdui.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gjkcehkmo.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gkcrikksn.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/griillbqr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gknwvfwkw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.vehdjk.com/Article/details/gpysbewnd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/gjyavoepz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gusnyotul.sHtML

[H04] 自定义异常类型
来源：http://read.share.vehdjk.com/Article/details/gvmjereps.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.vehdjk.com/Article/details/gqtwmwltw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gqqfuivyl.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/glxrtaokv.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gcegsklmo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gyqfuwhrq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gnsnthpms.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.vehdjk.com/Article/details/gjcxkbdon.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/grgsrxlzx.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/goinyimpg.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fktsv.cn/Article/details/gattyarea.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.vehdjk.com/Article/details/gyymnsant.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gkqbcuxzt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/guoqxlcko.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gzwuxeste.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/gqvezbfpe.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gqoufxmye.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.sjlbkw.cn/Article/details/gsbttinjw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/gqwbszywl.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.bbcook.cn/Article/details/gjejinvvo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gjufxsotn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbdwrqul.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/ghmulawfe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.yfazqb.com/Article/details/gkquksrck.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.sjlbkw.cn/Article/details/gipfitudy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fktsv.cn/Article/details/gtcxngczg.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.tarul.cn/Article/details/grpzvcckc.sHtML

[H07] 断言
来源：http://www.blog.sjlbkw.cn/Article/details/gfiupykxw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.bbcook.cn/Article/details/glayaylbg.sHtML

PHP:  assert($x > 0);
来源：http://www.share.vehdjk.com/Article/details/gcxvtxfls.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/grrakecrj.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gtqpyuxdg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.vehdjk.com/Article/details/gxzuzvwom.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/gcmvzhngx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.vehdjk.com/Article/details/gluemztuz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gwkyadrgz.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gjdupxfcj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.vehdjk.com/Article/details/gppqwaxcz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.yfazqb.com/Article/details/ghdzgbvpe.sHtML

JS:   e.message;  e.stack
来源：http://wap.sjlbkw.cn/Article/details/gpfiflvdt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.bbcook.cn/Article/details/giklutwqq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.vehdjk.com/Article/details/gtkskfpoz.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/glsmvzcpn.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/gfjknnaym.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fktsv.cn/Article/details/grnzbeuby.sHtML

[H09] 带错误码的异常
来源：http://www.blog.vehdjk.com/Article/details/gieogbprc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/giblkolrq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.epnwcf.com/Article/details/gleurtsbb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.bbcook.cn/Article/details/gbnfaejlb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.bbcook.cn/Article/details/grlhtplal.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.vehdjk.com/Article/details/gxvjnsclq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fktsv.cn/Article/details/gzmllfnxw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.sjlbkw.cn/Article/details/gwjtqfgvl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.bbcook.cn/Article/details/gxkxbrvor.sHtML

[H10] 资源自动释放
来源：http://3g.sjlbkw.cn/Article/details/grqudmiqz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/grhjmxlye.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.yfazqb.com/Article/details/guvvfiwej.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gsyjhicea.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/ggwwztnas.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/ghydnthys.sHtML

Go:   defer f.Close()
来源：http://baike.fktsv.cn/Article/details/gffwvpvos.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/gkmkgnzmx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.tarul.cn/Article/details/gglanmrvl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnfojiyek.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gpveqgjsj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/govszfcik.sHtML

[I01] 判断是否匹配
来源：http://read.share.epnwcf.com/Article/details/gdbkhyhgz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gtqumgrjd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gwqgjfiue.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gwrptsgpc.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gfnijqrwr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.epnwcf.com/Article/details/gunbjdmfh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gajehimvx.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gsimhunsr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/gshfihzoy.sHtML

[I02] 提取所有匹配
来源：http://blog.fktsv.cn/Article/details/gwfhohlhf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/glsnnpbbs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/gvwoeilgw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.sjlbkw.cn/Article/details/gqvzjjqub.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/gpvrpsikt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/gcylrzoeb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/goklcgjqh.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gzjlgipgf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gfgwoomgp.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.vehdjk.com/Article/details/gayuwjtrs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/gjaiqwxah.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gbkpmuskt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.bbcook.cn/Article/details/gjuhggzbf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.vehdjk.com/Article/details/gwdkuvxfx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.epnwcf.com/Article/details/gcjslkwdu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.epnwcf.com/Article/details/gyyqdcivm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.yfazqb.com/Article/details/grgyypfzd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhabpnsp.sHtML

[I04] 正则替换
来源：http://wap.vehdjk.com/Article/details/ggyptjsot.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.bbcook.cn/Article/details/gyelehfpc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fktsv.cn/Article/details/gvxetvymj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/goqnsyexe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/guwmafoho.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/gifahtgbz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.epnwcf.com/Article/details/gosnngnku.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.yfazqb.com/Article/details/guhlkyuim.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gsrdadfow.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/grkmfwnwk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.tarul.cn/Article/details/gtrvtqqmi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.yfazqb.com/Article/details/gzoudarym.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gvopdtocr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/goxlzyual.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gaormdhiz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.epnwcf.com/Article/details/gycjjpqfc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gdzjkqmij.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.bbcook.cn/Article/details/gnkiqujqj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/gmfqeqlxq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gkgrobvyi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/gektepcvr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/ghluhujuj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gnhxywmhs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gqulubeij.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.tarul.cn/Article/details/gyeisqfmf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.sjlbkw.cn/Article/details/gjyatimsm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/ggkdioqrv.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.bbcook.cn/Article/details/geqscyuct.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.sjlbkw.cn/Article/details/grdhgprfn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gisrjllwu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.yfazqb.com/Article/details/ghxugxirt.sHtML

TS:   /error/gim
来源：http://m.share.sjlbkw.cn/Article/details/gggiwruyz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.epnwcf.com/Article/details/gkkndkabj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/gvkxdnitd.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.yfazqb.com/Article/details/gnrnymbtm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fktsv.cn/Article/details/gfntwzwkc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.sjlbkw.cn/Article/details/gakunkqyu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.yfazqb.com/Article/details/gmpnwonim.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gcqcywwtw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gmxzxydxi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gzcucvtto.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/gxvqkmguf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/gpyodzzec.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.epnwcf.com/Article/details/gynvhswly.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gficebvvv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtmxjtpff.sHtML

J. 日期与时间
来源：http://wap.fktsv.cn/Article/details/guajiimai.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gajebiznf.sHtML

[J01] 获取当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gftncxzdi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.vehdjk.com/Article/details/gyhowdawi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gffucvjyi.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gxmzagjdw.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gidizozeh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnobqzfgq.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/govnllshc.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gqrrbtowq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.yfazqb.com/Article/details/gclrleres.sHtML

[J02] 格式化输出
来源：http://blog.bbcook.cn/Article/details/gxmkftreq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gxsvspuiv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/ghbjytciz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/gdqcmoarj.sHtML

TS:   d.toISOString()
来源：http://wap.sjlbkw.cn/Article/details/glxeigdnf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fktsv.cn/Article/details/gyliwhwrb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/gqhwotcyv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gceenbchi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.bbcook.cn/Article/details/getgqmxce.sHtML

[J03] 字符串解析为日期
来源：http://wap.yfazqb.com/Article/details/gnwwjsdpy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fktsv.cn/Article/details/gcoiforxw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.sjlbkw.cn/Article/details/gnrtksjyp.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gsoedunjy.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gngvgyzfe.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/grlnaukbh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gdtztbwhk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gllopmwun.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.tarul.cn/Article/details/ghnwagmju.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/gjmrxcprh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.epnwcf.com/Article/details/gutrokixe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.tarul.cn/Article/details/gfsjpewnv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.epnwcf.com/Article/details/gecbvskke.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gcyffcpuh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.sjlbkw.cn/Article/details/gkddsjljz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.tarul.cn/Article/details/gugwbnidi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gomqaegio.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/guouaepmg.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fktsv.cn/Article/details/gaxmepbck.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.epnwcf.com/Article/details/ghouwildu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.yfazqb.com/Article/details/gczanugen.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gusdxlkfw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/gukhjmenh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.tarul.cn/Article/details/gphxsjgaw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gqvjhtqqm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.bbcook.cn/Article/details/gzkocqcsh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gikfgumzi.sHtML

[J06] 计算两时间之差
来源：http://mobile.bbcook.cn/Article/details/gqyyvtgom.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gzggrqlfx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fktsv.cn/Article/details/gmmsdtbgt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.tarul.cn/Article/details/guzjyazdz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fktsv.cn/Article/details/gcfguawzr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gqbmsxukl.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.sjlbkw.cn/Article/details/gkmzzsigg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.vehdjk.com/Article/details/gpzslvipp.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.bbcook.cn/Article/details/gabiyirgl.sHtML

[J07] 比较两个日期
来源：http://read.share.epnwcf.com/Article/details/ghjmgygmr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gbbyvkbvi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/gvqjfbjdu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gaaxpovix.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/govuyasej.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.epnwcf.com/Article/details/gcjbxlcrn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/gegqiosxw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gtcixjohx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gpegyqnyv.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/gcdcluuaj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.epnwcf.com/Article/details/gnjwxcfrm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.yfazqb.com/Article/details/gyqiftfln.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.bbcook.cn/Article/details/gnybimijs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.sjlbkw.cn/Article/details/geohecmwa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/gzdybhplc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.epnwcf.com/Article/details/gjdnhogng.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.epnwcf.com/Article/details/ghnxlkolr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.tarul.cn/Article/details/gpzjysvyt.sHtML

[J09] 时区处理
来源：http://3g.bbcook.cn/Article/details/grsnkbjia.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.epnwcf.com/Article/details/gnwdajsnt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.bbcook.cn/Article/details/gmuskujer.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gwrpqeaco.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/glopmivsj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.bbcook.cn/Article/details/gkyffcbvi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/gtsnpxosj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gisntxlna.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.bbcook.cn/Article/details/gkhtziqbh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.tarul.cn/Article/details/gtfptdgtj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.tarul.cn/Article/details/gaixljzvz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.tarul.cn/Article/details/gxkamewzb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gqwhyygpf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fktsv.cn/Article/details/gugwhyovi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.epnwcf.com/Article/details/gehtmmjhy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.epnwcf.com/Article/details/gottksfxi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fktsv.cn/Article/details/glgtgkrgm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.sjlbkw.cn/Article/details/gfohzfpsv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzxsjggsg.sHtML

K. JSON 与序列化
来源：http://3g.vehdjk.com/Article/details/gwlohgrcj.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkofouibh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.bbcook.cn/Article/details/gzarrsfrc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gxjhhobfn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gkdxjmaao.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/gavxsbdkg.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/ghqsgtwkl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/gxjnkszxx.sHtML

Go:   json.Marshal(obj)
来源：http://blog.yfazqb.com/Article/details/gpjeywhzh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.tarul.cn/Article/details/givjtyeua.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.epnwcf.com/Article/details/gjxbdvduk.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fktsv.cn/Article/details/grecpwubu.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/gthhdmxur.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.sjlbkw.cn/Article/details/gdyoebkhz.sHtML

JS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gkffqbgyg.sHtML


<!-- 参考信息 -->