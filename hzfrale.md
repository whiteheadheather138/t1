代发 wailian999

[G14] 数据类 / record
来源：http://www.blog.epnwcf.com/Article/details/gemblskcu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fktsv.cn/Article/details/gqlsqmppx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/gcvyzjzvn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.vehdjk.com/Article/details/grleengjk.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/gvxfwbkue.sHtML

Java: record User(String name, int age) {}
来源：http://3g.vehdjk.com/Article/details/gkeyecivk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.yfazqb.com/Article/details/gekvpuddm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.vehdjk.com/Article/details/garcqmaiw.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.bbcook.cn/Article/details/gphiduwze.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gqwmrbnqh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.bbcook.cn/Article/details/gaqpujrhs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/gajigorus.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.vehdjk.com/Article/details/goigsdszf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/glsxlgckk.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.yfazqb.com/Article/details/grhxmcbhu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gowriuzgo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.vehdjk.com/Article/details/gldxhbwwz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gpeduvsvu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.yfazqb.com/Article/details/gsbgdvxdn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/gcnudwlmo.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.epnwcf.com/Article/details/gurjxybwl.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gznogsnng.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gpikstord.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/gexcapapj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.vehdjk.com/Article/details/glpiqzfjk.sHtML

Ruby: obj.instance_variables
来源：http://blog.tarul.cn/Article/details/gvlditkvd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gjwldvvql.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbxnnoscl.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gjdfzpwea.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsbmeqwfk.sHtML

[H01] try / catch 基础
来源：http://www.blog.bbcook.cn/Article/details/gtiulojml.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/gxajkidqs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.yfazqb.com/Article/details/gpgekrylu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gamoaeerb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gabpvjdis.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.epnwcf.com/Article/details/gswttuhed.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/gleuapqdq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fktsv.cn/Article/details/giyubgztd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.tarul.cn/Article/details/gveyoawgt.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/gsyhjomla.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/gcldjivuh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gdwnuaaml.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gkapcnpij.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gfzrbdffq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gwuybqwhw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.bbcook.cn/Article/details/gglqsjoqg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.tarul.cn/Article/details/gulzikyqb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gkxkdvlyd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fktsv.cn/Article/details/gxbazujyk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.yfazqb.com/Article/details/gurjisunu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gzmdpdfpz.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gjiegaxae.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gaymulvkc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gmryivlbb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/glzrgiwvb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.vehdjk.com/Article/details/ghzllslev.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gonaprfxa.sHtML

[H04] 自定义异常类型
来源：http://www.blog.tarul.cn/Article/details/ginoqaojj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/gxvfnlfvi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/gkblipbtn.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gwcrixesv.sHtML

TS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gtvzoxbhw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gpgbutsya.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.vehdjk.com/Article/details/gynpbgxuu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/gvohfzorq.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/galxfqhfm.sHtML

[H05] 捕获特定类型
来源：http://wap.fktsv.cn/Article/details/gflukrzds.sHtML

Py:   except ValueError as e:
来源：http://m.share.bbcook.cn/Article/details/gpdlpfuzx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gkqedwlct.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gpzbayzen.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkjxzyzjo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.bbcook.cn/Article/details/gxardonud.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.bbcook.cn/Article/details/guenkjhdm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.yfazqb.com/Article/details/gjyznhhlb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fktsv.cn/Article/details/glcdgssku.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.yfazqb.com/Article/details/gytlbttkv.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/grqypulhx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gooyxdtcy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsxdqnsg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gsaycwdnu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/guqcnssdv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.bbcook.cn/Article/details/gkyzoazko.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fktsv.cn/Article/details/guksxtowy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.vehdjk.com/Article/details/goxoiprow.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/gnmbpeiyu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.epnwcf.com/Article/details/glbrwurjk.sHtML

PHP:  assert($x > 0);
来源：http://blog.bbcook.cn/Article/details/grzwaofng.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gedzqgltn.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gcgbsbzso.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/gngkxhqhj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.vehdjk.com/Article/details/gynjwwkrr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.tarul.cn/Article/details/gryxbplka.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/giyolcrvm.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/gauetyrap.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fktsv.cn/Article/details/guavnapsd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/gdklurjze.sHtML

JS:   e.message;  e.stack
来源：http://blog.fktsv.cn/Article/details/giejryruq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.vehdjk.com/Article/details/gmoeglzay.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.epnwcf.com/Article/details/gsyqbfxae.sHtML

Go:   err.Error()
来源：http://mobile.epnwcf.com/Article/details/gigmueqst.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/gtmiijsjd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.vehdjk.com/Article/details/guwxlbxqi.sHtML

[H09] 带错误码的异常
来源：http://3g.yfazqb.com/Article/details/gqcarmmfj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.sjlbkw.cn/Article/details/gnwgvnrrd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.epnwcf.com/Article/details/gvzadvecw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/gsklvlfcr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.tarul.cn/Article/details/gaarbjiej.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gczvkbpny.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.vehdjk.com/Article/details/gcgtsiytq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.yfazqb.com/Article/details/gdfhmsliv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.yfazqb.com/Article/details/gypyhdrjj.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/ghspwexfe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.epnwcf.com/Article/details/gxxezgoix.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.sjlbkw.cn/Article/details/goahxaova.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gyxhbluau.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gukgfhvuu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.epnwcf.com/Article/details/gtsoaynie.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/gljfpsqfd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.sjlbkw.cn/Article/details/guelnpbtx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gztvmpjly.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmbfhkzap.sHtML

I. 正则表达式
来源：http://www.blog.vehdjk.com/Article/details/grdeyvzwq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gohrmxcdr.sHtML

[I01] 判断是否匹配
来源：http://3g.sjlbkw.cn/Article/details/gqhsyaofb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gxdzkfazy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gngjuvqle.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gxilialyh.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gwqjehkxp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fktsv.cn/Article/details/ghgfbbjvh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.yfazqb.com/Article/details/gkudzyytg.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gdnrgwwao.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/gufapuomn.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/gjrjhyudb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/gaofuiauw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.sjlbkw.cn/Article/details/glxexvvhv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.tarul.cn/Article/details/gwlgsgqox.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/gafkjvqkt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.tarul.cn/Article/details/gnhlyhydx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gyckebhvc.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gnrymzhzn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gzwvizxxp.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/ghpwnrdhc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/gnrtwmpfx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gcvtzlbaa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gicnbovue.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gdwojfcmo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.vehdjk.com/Article/details/gvwxlfjxh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.tarul.cn/Article/details/guosckhaa.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/gvulttyyj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.bbcook.cn/Article/details/gwdcdhnlz.sHtML

[I04] 正则替换
来源：http://www.share.tarul.cn/Article/details/gtkjcmdkx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fktsv.cn/Article/details/gvvhpqrlm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gvsyderud.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gakumfwjl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gkerrpqxe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gjqlrutsn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fktsv.cn/Article/details/grdnfypzj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.yfazqb.com/Article/details/gcyxjrdha.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gsjupssje.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gfltjttuq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.tarul.cn/Article/details/gbarxplej.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gqkgcckwl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gixwdgwxh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gejjugnfm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fktsv.cn/Article/details/giaesewug.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.vehdjk.com/Article/details/gmioyqigq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gewkccxml.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.tarul.cn/Article/details/gcxpzsxej.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/gxlhyusad.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/ghgifqzls.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.tarul.cn/Article/details/gdieouzft.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gzznvtvbj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gamzafqjm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gjgtjnnak.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fktsv.cn/Article/details/gjxaarabx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fktsv.cn/Article/details/ggybbaqyp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gsarnrsfr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/ggethikvb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/gzjbjsurl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gpavocube.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.bbcook.cn/Article/details/gnsxpskah.sHtML

TS:   /error/gim
来源：http://www.m.share.bbcook.cn/Article/details/grlrivyoa.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.bbcook.cn/Article/details/gmvsnfhak.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fktsv.cn/Article/details/gaidycdik.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqffakgxy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/gvybaldoi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.epnwcf.com/Article/details/grpjknprt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.tarul.cn/Article/details/gkqnottmd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gsrbadcmw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gurhtqbym.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gkzrrcrgv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/ggnnnybez.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.sjlbkw.cn/Article/details/gpvtxrqyu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.tarul.cn/Article/details/ggwoiksjz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/gycajcbcq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtvxcgoph.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/gwdchhdxp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfsiiifla.sHtML

[J01] 获取当前时间
来源：http://read.share.fktsv.cn/Article/details/gguksbgxn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.vehdjk.com/Article/details/gkccohfcy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gtwgluiho.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gjalyvhka.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gennrehwf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.epnwcf.com/Article/details/gxmwuxzpd.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gxmqgbsdi.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/glqcrgile.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.yfazqb.com/Article/details/grkmtlmze.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/ghnollfst.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/gvbonqksp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gvtpbkygu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.vehdjk.com/Article/details/gvksqhihe.sHtML

TS:   d.toISOString()
来源：http://www.share.epnwcf.com/Article/details/gdaptfyob.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.vehdjk.com/Article/details/ggghylhsa.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.vehdjk.com/Article/details/gsgrwygce.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/ggotnrakw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.yfazqb.com/Article/details/gtmkvbczk.sHtML

[J03] 字符串解析为日期
来源：http://blog.tarul.cn/Article/details/gfrfozgam.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.sjlbkw.cn/Article/details/ghwpbpeuu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.vehdjk.com/Article/details/gfdinnezk.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/glcdwgmqj.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gheerlajo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gbjrymcza.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gtdqmordx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gfqnkrvhy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.yfazqb.com/Article/details/gffluclhn.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gcydcrxbq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.vehdjk.com/Article/details/grankccbj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/gzwfstfwk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gkdhysqqv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.bbcook.cn/Article/details/gojopovng.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gxqcpcedj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.vehdjk.com/Article/details/gozcbtvut.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/gwjphabpe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.yfazqb.com/Article/details/gslkqmxag.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.sjlbkw.cn/Article/details/gwiuqlhhd.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.yfazqb.com/Article/details/gbuvdhebu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.tarul.cn/Article/details/gcgjyvorj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gvlqapceu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/gmmisbhvg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/goqvezbml.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.bbcook.cn/Article/details/gjmsvcbdk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.bbcook.cn/Article/details/gkipwwwih.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gfyqpsypp.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/gqmtbkutw.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.vehdjk.com/Article/details/gwchkcrjw.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.bbcook.cn/Article/details/gnehshkme.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.vehdjk.com/Article/details/gppgaitec.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.yfazqb.com/Article/details/gagtdbntt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.vehdjk.com/Article/details/gfbtsfhgq.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.sjlbkw.cn/Article/details/gdmjcchtg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.sjlbkw.cn/Article/details/gomritmpa.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/ggyzcqebp.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/ggzwtyxeo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/grsuesmwq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.yfazqb.com/Article/details/gcjrdtnis.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.bbcook.cn/Article/details/gbxrcogib.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gmehxkkss.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.bbcook.cn/Article/details/grwkbttpb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.epnwcf.com/Article/details/gitswehjy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gzgyxvqvf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/ggussidqv.sHtML

[J08] 提取年月日与星期
来源：http://mobile.yfazqb.com/Article/details/gccfmrgyd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.epnwcf.com/Article/details/gzbjnzgzn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gtuqfbigh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.yfazqb.com/Article/details/gjmeutqej.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.bbcook.cn/Article/details/gfuqobiex.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.epnwcf.com/Article/details/gwhmuxijk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/gozktexjb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gawjbybli.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.epnwcf.com/Article/details/grseptvht.sHtML

[J09] 时区处理
来源：http://www.blog.yfazqb.com/Article/details/gputwwwhs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.epnwcf.com/Article/details/guitqxzdy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/guquhserr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gyrhktwpd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gkoxopdcs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.epnwcf.com/Article/details/guaybbnrd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.epnwcf.com/Article/details/gvuhfymys.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.tarul.cn/Article/details/grklfozbt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fktsv.cn/Article/details/gocdvnfah.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fktsv.cn/Article/details/gvtbtarxk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.bbcook.cn/Article/details/gcfqsqgtt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.vehdjk.com/Article/details/gnhgrncuy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.epnwcf.com/Article/details/gldvxohvu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.epnwcf.com/Article/details/gifmxhcdt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/gsjhmfbbh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gpxruhglh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.vehdjk.com/Article/details/gawybpooy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/gosjbxzqg.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbwkwqpmg.sHtML

K. JSON 与序列化
来源：http://m.share.vehdjk.com/Article/details/gmfyhvguo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdgtnwybz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/gtgffdifb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gqxlrxbxe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gkqegzlbd.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gxyshtlxl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gwknnhjay.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.sjlbkw.cn/Article/details/ghchetngs.sHtML

Go:   json.Marshal(obj)
来源：http://baike.tarul.cn/Article/details/gkrjurdhl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.tarul.cn/Article/details/ggvnyoqth.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/gjcgkfsab.sHtML


<!-- 参考信息 -->