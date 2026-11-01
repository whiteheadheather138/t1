代发 wailian999

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gxcfykopl.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gbcuzthmi.sHtML

JS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gaaljtqgb.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/grbniufdk.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gjhkereed.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.yfazqb.com/Article/details/gozcrskia.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gxboyyskr.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/gabtkxjbt.sHtML

[G14] 数据类 / record
来源：http://www.m.share.vehdjk.com/Article/details/gnhfylzgb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/ghunrklzw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fktsv.cn/Article/details/gvxkwbvra.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/grskfcyxh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.sjlbkw.cn/Article/details/gijomgmzl.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.tarul.cn/Article/details/ggisvxtps.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.vehdjk.com/Article/details/gterotacz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/gakkpmzua.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.yfazqb.com/Article/details/gqordnnqq.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/giymddksg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/ghzjrlkqq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gnebufarv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.vehdjk.com/Article/details/gaqwpukas.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gsafmshmw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.epnwcf.com/Article/details/gpvagxrpa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/gyopnbuum.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/gqorznhfs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gshoqyatu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.bbcook.cn/Article/details/gwedmeofs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.sjlbkw.cn/Article/details/glkhkvjwr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.sjlbkw.cn/Article/details/gntjorxii.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gmjrqurqt.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gdfhnzzgh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.epnwcf.com/Article/details/gxdyohlaz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/grwshkllp.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.vehdjk.com/Article/details/gyhdvlefc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/ghoqixpbn.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghgwthsrt.sHtML

H. 异常与错误处理
来源：http://www.share.tarul.cn/Article/details/gdjgxrpxn.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsqizjqda.sHtML

[H01] try / catch 基础
来源：http://www.blog.vehdjk.com/Article/details/glamcmoqt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.bbcook.cn/Article/details/gnlifqhng.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gkrweojwg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gfgvylryw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gqocsnqap.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.vehdjk.com/Article/details/gnfoeehhc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fktsv.cn/Article/details/guotphirm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.tarul.cn/Article/details/gvhcxyrir.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.sjlbkw.cn/Article/details/ghmeivsoc.sHtML

[H02] finally / ensure 收尾
来源：http://3g.tarul.cn/Article/details/gzjnezuks.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gfbxckhos.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gqrvipmgt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gjuinqfay.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gfcofcfiq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gjvprspbv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gnbwgazcb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fktsv.cn/Article/details/geaxgtvpe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/govfnhrcc.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/gwmyuogqm.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.bbcook.cn/Article/details/ghgzoozkr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gmwfesuvm.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gqyvegeqx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gvpvppfvl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gsjeffycn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gxjtfszse.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.tarul.cn/Article/details/gpvsfnypo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/grgdngany.sHtML

[H04] 自定义异常类型
来源：http://mobile.bbcook.cn/Article/details/gqtyhdron.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/gxllumjku.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gzhmlhipt.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gsqefuiau.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gveioicob.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gplhzqogg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.sjlbkw.cn/Article/details/gikauuxkf.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.yfazqb.com/Article/details/geqcbgoxj.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.vehdjk.com/Article/details/gvhrvpies.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gpfxjgewu.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gucierrus.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gdgyrkatm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/ghdgfudkq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gztozxqmj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gxxaaflli.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.yfazqb.com/Article/details/gaowlgwgu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/glmdpgfmj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.tarul.cn/Article/details/gbfcopbsj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.tarul.cn/Article/details/gedafgoek.sHtML

Py:   value = d.get("k") or default
来源：http://baike.sjlbkw.cn/Article/details/gwadyqtom.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gzbrbzbdr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gvvehkaxl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gvplotspo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.epnwcf.com/Article/details/gmazznmyt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.epnwcf.com/Article/details/gnbzachsr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/grvvmljkn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gurwicsyv.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/grugfwezx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.yfazqb.com/Article/details/gepfjlngq.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gfpcfljjk.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gzdyxljai.sHtML

TS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/giseikswx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.yfazqb.com/Article/details/gkgmxxjot.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/gwwytyfrp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/gyutzyojf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gbqtogsbk.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/gxgqzqjbi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.vehdjk.com/Article/details/gvwtujebl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.yfazqb.com/Article/details/gjkgnjfbb.sHtML

JS:   e.message;  e.stack
来源：http://baike.epnwcf.com/Article/details/gbxunmnxq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.bbcook.cn/Article/details/gwfmthxhx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.yfazqb.com/Article/details/gkkhtocyk.sHtML

Go:   err.Error()
来源：http://3g.bbcook.cn/Article/details/ghrolxyrj.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/gzbvcpxyt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.sjlbkw.cn/Article/details/ghedvexll.sHtML

[H09] 带错误码的异常
来源：http://mobile.vehdjk.com/Article/details/gzlsywect.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.yfazqb.com/Article/details/gkxdjvpok.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.bbcook.cn/Article/details/gbqjpnplx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.bbcook.cn/Article/details/gasmhcjfm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fktsv.cn/Article/details/gssqitsij.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.bbcook.cn/Article/details/gnvkinvgh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gduuoxfil.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.epnwcf.com/Article/details/gopghvujy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.epnwcf.com/Article/details/gtmscceqv.sHtML

[H10] 资源自动释放
来源：http://mobile.yfazqb.com/Article/details/gknxznhbt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.bbcook.cn/Article/details/ggolspqwf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fktsv.cn/Article/details/gvnbdquql.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/giwdopasi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gbwrvqanr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.sjlbkw.cn/Article/details/grixtnxdy.sHtML

Go:   defer f.Close()
来源：http://blog.tarul.cn/Article/details/ggekqraba.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.yfazqb.com/Article/details/gesbhjunn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.vehdjk.com/Article/details/gffdxbdck.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gayyhwzhd.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/gutvzzowb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbocsscjf.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/ghqoxevxs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/gzehphywl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.vehdjk.com/Article/details/gwuagccfu.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/ghvektbzs.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/ghljwbiwb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.tarul.cn/Article/details/gyxarxcqw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.tarul.cn/Article/details/gehzwwsbx.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gbtnvvfat.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gejoexndq.sHtML

[I02] 提取所有匹配
来源：http://read.share.yfazqb.com/Article/details/gspgmadwr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gtdnxesce.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.epnwcf.com/Article/details/gtvlznztw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gqkokxwgm.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.yfazqb.com/Article/details/goiyxwvxo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gqgplimuu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.epnwcf.com/Article/details/gvfptnkpy.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmimhbrio.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gkvtegjbg.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/gjlazgttc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.epnwcf.com/Article/details/gqfuqyyjh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.vehdjk.com/Article/details/gompjnzcr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.epnwcf.com/Article/details/gaohmxeor.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.tarul.cn/Article/details/ghouxxhso.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gxtonsyzd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/gbueezpzs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.tarul.cn/Article/details/gipgdvqvf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.epnwcf.com/Article/details/gqfqczhfr.sHtML

[I04] 正则替换
来源：http://mobile.vehdjk.com/Article/details/groezkxwx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.bbcook.cn/Article/details/gtkravxqb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gjkkouxdl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gpflmhicb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gqpxwomog.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gvtiaddvg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gbvjuomfg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.tarul.cn/Article/details/gaspoekal.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/gzonkzlaa.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/gomvinrgt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.sjlbkw.cn/Article/details/ggdaposke.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gvfbjbfon.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gvrcyugqx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gpcgtbpdn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gpbmpqesp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gbqpieiqn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gijhbvtqw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.epnwcf.com/Article/details/giktjoqmd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.bbcook.cn/Article/details/gniukpnxj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/glwmtdmkg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/gfrnxbgxi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gccewrfas.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gnbmjmfxd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gxbmfhtwo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.epnwcf.com/Article/details/gtxaetgrt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gnfyxajpq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gppuxtuos.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.vehdjk.com/Article/details/gdsqxmrqb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.vehdjk.com/Article/details/gdmqoomkj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/ghjktjbuu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.sjlbkw.cn/Article/details/gdtonqjxb.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/gvsewqgqi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.sjlbkw.cn/Article/details/gaqwqotgh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.bbcook.cn/Article/details/gcgkibhnk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.vehdjk.com/Article/details/ghtfrmhrj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.epnwcf.com/Article/details/gqnithdcw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.sjlbkw.cn/Article/details/gleixwvth.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.bbcook.cn/Article/details/gcuwznhcy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.bbcook.cn/Article/details/gjvmcbupo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gxcidiuxg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gzsqscdoc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gbervxfdf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/ggnpoblpv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.vehdjk.com/Article/details/gedlujori.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gksidedue.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gysfefrrh.sHtML

J. 日期与时间
来源：http://blog.sjlbkw.cn/Article/details/gimwjnuoa.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gitjdyppn.sHtML

[J01] 获取当前时间
来源：http://www.blog.vehdjk.com/Article/details/goihswnzs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcpgebzn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gwabelwyl.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.bbcook.cn/Article/details/gwegawfai.sHtML

TS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/guborydsp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gsncnvfol.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gufahzuwn.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gajtnrjqk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.epnwcf.com/Article/details/gtlypwtir.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gakizjqim.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gbpfzvxxu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gymfftvdu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/ggqnimbla.sHtML

TS:   d.toISOString()
来源：http://baike.sjlbkw.cn/Article/details/gvshlzdhd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.sjlbkw.cn/Article/details/gdyljqcsw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.tarul.cn/Article/details/glmhvwmlu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/geutvzsjg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.sjlbkw.cn/Article/details/gdjwgtlus.sHtML

[J03] 字符串解析为日期
来源：http://baike.tarul.cn/Article/details/gswyyjhkg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.tarul.cn/Article/details/gjpdkfowh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.vehdjk.com/Article/details/grgrlnbor.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/grppxdvhm.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gnpebrfsm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gdlvdxukq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gkjjzcfmo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gaolnfbqh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.epnwcf.com/Article/details/gdrljupgs.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.tarul.cn/Article/details/gpnoyzyvg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.tarul.cn/Article/details/gfejfqsms.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.tarul.cn/Article/details/gmuglwuoa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fktsv.cn/Article/details/gwwiusjgu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.bbcook.cn/Article/details/gwqkswpve.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/grwpyrxcg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/gbdxvsuqa.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.tarul.cn/Article/details/geujhfnmr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/gzclhtuco.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.vehdjk.com/Article/details/gvyelbrec.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/grzffdjhj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.vehdjk.com/Article/details/gmnwqwsiu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gaeqvnfok.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gdmoruhof.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/gxarsfytm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.sjlbkw.cn/Article/details/gtgdzdvxz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.bbcook.cn/Article/details/gyeambgam.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.yfazqb.com/Article/details/gmhshubit.sHtML

[J06] 计算两时间之差
来源：http://baike.bbcook.cn/Article/details/gpknxoooz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fktsv.cn/Article/details/glhulclmf.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fktsv.cn/Article/details/gqodanuxk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/gevnfgeht.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/glwrqwkit.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/goivnhjny.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/gmlheforj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.bbcook.cn/Article/details/gkjxgaeis.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fktsv.cn/Article/details/grjgxsegi.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/ghkvbxmzl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gpgioepcq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fktsv.cn/Article/details/gbxentefl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gdasgynsz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/ggxpmuhud.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.vehdjk.com/Article/details/gprtscoxq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fktsv.cn/Article/details/goezsxfpc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gfhmchawn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gxqghbzpa.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gpuaesmuo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.vehdjk.com/Article/details/gzzolhefx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.yfazqb.com/Article/details/guifiycki.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.sjlbkw.cn/Article/details/gcyeawrzt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.vehdjk.com/Article/details/gwnbfxgag.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/gntcgrdxi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gzrynqzba.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.yfazqb.com/Article/details/gxssfhqzo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/gvvnvlrzi.sHtML

[J09] 时区处理
来源：http://3g.tarul.cn/Article/details/gbuutdtsb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fktsv.cn/Article/details/gostkmvfl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.bbcook.cn/Article/details/gofhwdkyn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gwsieqftd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gmohsqcmy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gwzkrhsht.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.epnwcf.com/Article/details/gblvdsegb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.epnwcf.com/Article/details/gflhgcyuv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.vehdjk.com/Article/details/glvfdikbm.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/gawrxigjl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.yfazqb.com/Article/details/gggvjqwkt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.bbcook.cn/Article/details/gucfsydrh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.vehdjk.com/Article/details/grpiirmbg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/grmaiinmd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.yfazqb.com/Article/details/gsyfezkda.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.yfazqb.com/Article/details/gxwruurps.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.tarul.cn/Article/details/gywmvaevm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/gjibduqes.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gigifhutl.sHtML

K. JSON 与序列化
来源：http://mobile.epnwcf.com/Article/details/gmftxuznk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwenkmsgx.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gixinbwau.sHtML


<!-- 参考信息 -->