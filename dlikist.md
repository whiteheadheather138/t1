代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/gqzpgcbzx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.sjlbkw.cn/Article/details/gxuhkodxq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/gqxkeette.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.bbcook.cn/Article/details/gktaabpdj.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/gbwszbhik.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/gdnetqywf.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gplocnvja.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/gbpbnfpqz.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gusmywahb.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.yfazqb.com/Article/details/gffuzwijp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.bbcook.cn/Article/details/gaibcwfjp.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/glvsuntmy.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/gliouxouv.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/gzewdmwpg.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gceocdevx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/ghjkinpzm.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/guxcytddm.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/ggekrmnrk.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/grpazztir.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gajxveykj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/gieoevqjg.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gotdmotha.sHtML

[G12] 对象转字符串
来源：http://baike.vehdjk.com/Article/details/grgosidrp.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.tarul.cn/Article/details/gjjazmglb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gbqnklyuf.sHtML

JS:   toString() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gpxdmulwy.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gtlgrgovr.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/giqtysexq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gdgciqsci.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/gyzdjjqlr.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gpgerfrup.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/grgjfuett.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fktsv.cn/Article/details/gqqwdhzoa.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gdzdxflrz.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gwffgzeik.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gvnludkzi.sHtML

Java: u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/ghorvbguz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fktsv.cn/Article/details/gpzqrdcap.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.yfazqb.com/Article/details/gysmxlcma.sHtML

C#:   u is User
来源：http://read.share.tarul.cn/Article/details/gawrhhmca.sHtML

[G14] 数据类 / record
来源：http://blog.yfazqb.com/Article/details/gwnpqwgue.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.vehdjk.com/Article/details/gzfjllasl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/gnictkxyy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/ghdgfwwrk.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.epnwcf.com/Article/details/ghltifgfb.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/gjcunvpnv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fktsv.cn/Article/details/gojqyikgi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/gajiuqbjp.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/grjcdjoij.sHtML

[G15] 枚举
来源：http://baike.bbcook.cn/Article/details/gklwpeqrj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/genlvkgoi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.tarul.cn/Article/details/glutinqzg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.vehdjk.com/Article/details/gcjbvqtxh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/grkyqhjfe.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fktsv.cn/Article/details/ggsbnolsh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.epnwcf.com/Article/details/gtihtwing.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgsvntjd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gbfcmntbe.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/gvlnvkmak.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gbdjnoixy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/gnmyhneam.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/giasgnacr.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/geyhbufxk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.tarul.cn/Article/details/ghbaxdanl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.tarul.cn/Article/details/gleczjbgm.sHtML

Ruby: obj.instance_variables
来源：http://www.share.epnwcf.com/Article/details/gnnzcfjsx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gprjcqjwe.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guozuslgd.sHtML

H. 异常与错误处理
来源：http://wap.bbcook.cn/Article/details/gtpekodvc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqxuikmah.sHtML

[H01] try / catch 基础
来源：http://www.share.sjlbkw.cn/Article/details/gppgqrlkf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fktsv.cn/Article/details/gylyogkfq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gxaaaaikx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gdbyhtpgm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gmiihpyla.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gmjqdirok.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/gqebpdrdz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.bbcook.cn/Article/details/gcvyehfzy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/grqgxnhed.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/ggcslasda.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fktsv.cn/Article/details/gfivlbcti.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gsitfwkem.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/guxphgajm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gmytvqwxt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/glmnylnww.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fktsv.cn/Article/details/giagurtck.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/ghhiqohus.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gmvufiofy.sHtML

[H03] 主动抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/gvpxiskbb.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.sjlbkw.cn/Article/details/gutbczamk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gdukgonwe.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gfnmctump.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/grqkdaeum.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gucezykso.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.vehdjk.com/Article/details/gjwqoxqnt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.yfazqb.com/Article/details/gcfxboudm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gzrmwaujo.sHtML

[H04] 自定义异常类型
来源：http://blog.yfazqb.com/Article/details/glkbvbllz.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/gxnjhndzo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gwxpdpfey.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gowglodao.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/grdrqybms.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gigumzkun.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.bbcook.cn/Article/details/gkppldpmq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.tarul.cn/Article/details/gmegjchbx.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgyilvmf.sHtML

[H05] 捕获特定类型
来源：http://3g.fktsv.cn/Article/details/gcjugaxux.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gltgibmhs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.sjlbkw.cn/Article/details/gvmjgddxd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gqpgcgpqt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gyexyjvmp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gcstrhpvd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/gvedkfzcs.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.yfazqb.com/Article/details/gzzdcxgyw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/gbkkekahx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fktsv.cn/Article/details/gjmkpwayv.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/gcflxkjtu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gvbwlbyea.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gxgeignoy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/galqxdcsr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fktsv.cn/Article/details/gudswehwu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fktsv.cn/Article/details/guufhuswu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.sjlbkw.cn/Article/details/gqrxysxso.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gdarrqsbe.sHtML

[H07] 断言
来源：http://www.m.share.epnwcf.com/Article/details/gcbntmupx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.yfazqb.com/Article/details/gmmpuxbgn.sHtML

PHP:  assert($x > 0);
来源：http://www.share.epnwcf.com/Article/details/gwxibgbib.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gctrwsaap.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gihpxxksq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.sjlbkw.cn/Article/details/ghdorlxgk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.vehdjk.com/Article/details/gqcdsuxey.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fktsv.cn/Article/details/gsfbqphfa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gnjazwypp.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/giqphveil.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.yfazqb.com/Article/details/giplcbgwd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fktsv.cn/Article/details/gfaoyyrbn.sHtML

JS:   e.message;  e.stack
来源：http://mobile.sjlbkw.cn/Article/details/grwuypbcs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.bbcook.cn/Article/details/gszcdlydg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.yfazqb.com/Article/details/gjjdypgxv.sHtML

Go:   err.Error()
来源：http://www.share.yfazqb.com/Article/details/gzzwotpuc.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gswmittif.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fktsv.cn/Article/details/goggkmkic.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fktsv.cn/Article/details/gpzhfslxp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.yfazqb.com/Article/details/gblxegvzu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gggkeqxwf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/gzgietxso.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/gtalksdjc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/guaulegqx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.tarul.cn/Article/details/gwzagcyhh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.epnwcf.com/Article/details/ghecajwys.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/gtcqulsud.sHtML

[H10] 资源自动释放
来源：http://3g.sjlbkw.cn/Article/details/ghbbawzmc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.sjlbkw.cn/Article/details/grekjfwjv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/gwwdlvzqk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gqktjyjwj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/ghvawbzax.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.tarul.cn/Article/details/gadkepkpu.sHtML

Go:   defer f.Close()
来源：http://mobile.vehdjk.com/Article/details/gukfudqdh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.vehdjk.com/Article/details/ghqdxzpda.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.vehdjk.com/Article/details/gmfdwkyge.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghuvaidip.sHtML

I. 正则表达式
来源：http://blog.sjlbkw.cn/Article/details/gpwkreqwi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvgddzmmd.sHtML

[I01] 判断是否匹配
来源：http://m.share.yfazqb.com/Article/details/guxfafepq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/glwwoizag.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/ghsbccxqi.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gcgddshkl.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/gtvomwjwv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.epnwcf.com/Article/details/glbbptlxj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.epnwcf.com/Article/details/gbmgmdfwk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.vehdjk.com/Article/details/gwytkfvem.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.sjlbkw.cn/Article/details/gefmtgkxz.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.bbcook.cn/Article/details/gvmgrnqxd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gwjvplivw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.bbcook.cn/Article/details/giycmmtzg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.vehdjk.com/Article/details/goefwcity.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.epnwcf.com/Article/details/ghhhucccg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gfzdeprco.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.vehdjk.com/Article/details/gqytmfgsp.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gibvpywrx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/gbvlddthd.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbjkwnzg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmhnhxcy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.bbcook.cn/Article/details/gzjupbxji.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gmfwmsvrn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gddeimnzz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gnlvtxamu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gbgksovye.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.epnwcf.com/Article/details/gykbsjskc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.sjlbkw.cn/Article/details/guobxeqsx.sHtML

[I04] 正则替换
来源：http://www.blog.fktsv.cn/Article/details/glperewfp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.bbcook.cn/Article/details/gjibxqovs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/gbffbtvcc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gxpvoanny.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.yfazqb.com/Article/details/geujkeqtu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gfihhkvue.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/ggbieuayx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fktsv.cn/Article/details/gwsjsplrd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gpodkdphc.sHtML

[I05] 按正则拆分
来源：http://read.share.bbcook.cn/Article/details/gkfgpjggm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.bbcook.cn/Article/details/gruqxgjtx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.bbcook.cn/Article/details/gzmjnzyqg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gzqamenwi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gcthruuuw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.sjlbkw.cn/Article/details/gmjkbhonh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gttjoujhc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/glzsucgll.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.sjlbkw.cn/Article/details/gcepiycol.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.vehdjk.com/Article/details/govfsobhc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/goultyxdv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.vehdjk.com/Article/details/gvuatxrpr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gfxestewo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gnjezngng.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gskheoyni.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.sjlbkw.cn/Article/details/gpuefwucz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.yfazqb.com/Article/details/ghxkfbryt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gvykbogzc.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.sjlbkw.cn/Article/details/gcpiqcsea.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.epnwcf.com/Article/details/gtjuujgjd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/ggycvearn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.yfazqb.com/Article/details/geglrjdtg.sHtML

TS:   /error/gim
来源：http://read.share.sjlbkw.cn/Article/details/gvcxiarzf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.sjlbkw.cn/Article/details/gqysbzgct.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fktsv.cn/Article/details/gwigjrptv.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gxypmquku.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.epnwcf.com/Article/details/gwgfwqouh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.epnwcf.com/Article/details/gtceiyiri.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.bbcook.cn/Article/details/gkzfqwbsb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/gpfzztbwp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gpyuhqrae.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gcbfjlrqz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/geqyyfnjd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.epnwcf.com/Article/details/gizgvhfei.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.tarul.cn/Article/details/grriecdni.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gbjvkfkim.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbvswkqjw.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/grrsmxfpo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwjpllrdm.sHtML

[J01] 获取当前时间
来源：http://baike.tarul.cn/Article/details/gzldfuftq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.sjlbkw.cn/Article/details/gbghushlx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gwcbcrczm.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gwtpwcnwv.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/guldmhegs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/gunimhsis.sHtML

Go:   time.Now()
来源：http://www.blog.vehdjk.com/Article/details/gkrskbqnb.sHtML

Ruby: Time.now
来源：http://baike.tarul.cn/Article/details/gxbhfjjmg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.epnwcf.com/Article/details/gfdtgqeti.sHtML

[J02] 格式化输出
来源：http://read.share.epnwcf.com/Article/details/gkcqrlgvq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gdauxlbxc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.bbcook.cn/Article/details/ghztziyis.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/gzsvflrmu.sHtML

TS:   d.toISOString()
来源：http://3g.yfazqb.com/Article/details/gqtgwgbxj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gmxxawtub.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.sjlbkw.cn/Article/details/gfuqprklg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/grhwdoswv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.yfazqb.com/Article/details/givzorjko.sHtML

[J03] 字符串解析为日期
来源：http://www.share.bbcook.cn/Article/details/gmfzibcru.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.bbcook.cn/Article/details/gitxhitbf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/gyjzrxjqs.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gykbeslea.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gboihqzbq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gkvomljjq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gtjvwbuxm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gvdfmkuoz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.bbcook.cn/Article/details/gomvrxcxa.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.bbcook.cn/Article/details/ghhgjbxjh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/ghwmtzkhf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fktsv.cn/Article/details/gniivfhxg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.yfazqb.com/Article/details/ghgphnhau.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.bbcook.cn/Article/details/ghgrucjys.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.bbcook.cn/Article/details/gfrymsqlg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.vehdjk.com/Article/details/gjrhekiac.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gfppmwftr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.epnwcf.com/Article/details/gopfgawyj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/gtvqmrgfp.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.epnwcf.com/Article/details/gbtypsbtb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.bbcook.cn/Article/details/gfjuxuehv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/gewuljfyq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gnaepuoul.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/girkdcbhg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.tarul.cn/Article/details/gbsxpyftp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.sjlbkw.cn/Article/details/gsrqcauag.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.bbcook.cn/Article/details/ghpeqqtus.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/gpmsglxxt.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/gghspdbvw.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.yfazqb.com/Article/details/gkpcqlmqp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.sjlbkw.cn/Article/details/gcyxpkbff.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.sjlbkw.cn/Article/details/glyfttrdq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.sjlbkw.cn/Article/details/gdjgpokol.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.epnwcf.com/Article/details/ggmskqrwq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.epnwcf.com/Article/details/gueutwgge.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.bbcook.cn/Article/details/gjwslotdr.sHtML

[J07] 比较两个日期
来源：http://www.m.share.yfazqb.com/Article/details/gaiycvrnu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gywneuvxv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fktsv.cn/Article/details/gkkfungtl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gxevcdksk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gnzovftnr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fktsv.cn/Article/details/gkphhmnbx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.tarul.cn/Article/details/gjxejioum.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gntxddblc.sHtML


<!-- 参考信息 -->