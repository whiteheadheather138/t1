代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gareywdoy.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gloebznan.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/glufsdjep.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fktsv.cn/Article/details/gmfnlevrs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.yfazqb.com/Article/details/ghsqzhrrv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/gifpzpytl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.tarul.cn/Article/details/gqoofanrd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/gogtzonse.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fktsv.cn/Article/details/ggskykyee.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.epnwcf.com/Article/details/ggfgyevnu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.tarul.cn/Article/details/gwatywodx.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gcyzxadms.sHtML

[G10] 访问控制
来源：http://wap.sjlbkw.cn/Article/details/gegwfxjdb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gxzynjuab.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gqkebsbnp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.bbcook.cn/Article/details/gqsdrattj.sHtML

TS:   public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gzfupbyqj.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.vehdjk.com/Article/details/gijkieman.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.sjlbkw.cn/Article/details/ggfxhxbpb.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gkdzcscik.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.vehdjk.com/Article/details/gzqjdghig.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/grdfayqic.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gwtkizvjn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gbzzdyzik.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/glrpyfyrf.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.tarul.cn/Article/details/gnhhqjccm.sHtML

Java: public String getName() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gptsshcfd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/geatoacyr.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gbizwlhbc.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.yfazqb.com/Article/details/gosiyxmhk.sHtML

[G12] 对象转字符串
来源：http://blog.bbcook.cn/Article/details/ghstzemqx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gchkzwhro.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gegakzyzk.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gflqwrznt.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gdtidnruv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gruhebuws.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gncvzbhzl.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.vehdjk.com/Article/details/geskfswnm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gjpjlbjzs.sHtML

[G13] 判断对象类型
来源：http://wap.fktsv.cn/Article/details/ghqfnnmgx.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fktsv.cn/Article/details/grxnwntfg.sHtML

PHP:  $u instanceof User
来源：http://3g.epnwcf.com/Article/details/gphqsnvuw.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gevleanjb.sHtML

TS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gtktbjaub.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/glwdmziln.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.vehdjk.com/Article/details/gtltjlvuq.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.vehdjk.com/Article/details/gdorvnrgw.sHtML

C#:   u is User
来源：http://m.share.sjlbkw.cn/Article/details/ggmclxson.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/gupfttpjj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gyuvztyeb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/gzllmwvuu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.tarul.cn/Article/details/gmzjmlfkw.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/gwbmbhvny.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.sjlbkw.cn/Article/details/geowsralh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.vehdjk.com/Article/details/grrkrzkcd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.epnwcf.com/Article/details/glcleqqfd.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/geheuyfvy.sHtML

[G15] 枚举
来源：http://wap.vehdjk.com/Article/details/gfdedkkjo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.epnwcf.com/Article/details/gwlkommww.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/giiqxobtr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/gpyjebsla.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gmsvuqzgy.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/gfptnpduj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/gsmchuvex.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.sjlbkw.cn/Article/details/gurwuxdds.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/guarogehi.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/glthvagos.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.sjlbkw.cn/Article/details/gwbslvmdh.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/ghhkbggts.sHtML

JS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gthojzufv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gvjgchbuu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gnbkevukh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.epnwcf.com/Article/details/gncsqxfeo.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/gfnkttgcc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.bbcook.cn/Article/details/gejdtehnt.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcconfkln.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/gvvvslcai.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqtrxmryl.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/gmlsfqxwx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.bbcook.cn/Article/details/gdkqpfdqv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gkkymehhe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gntkvakwl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gbfwdljlf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.tarul.cn/Article/details/gzaimzins.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.yfazqb.com/Article/details/gnfrylxod.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.tarul.cn/Article/details/gfxaovrsv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/gtkactzht.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.epnwcf.com/Article/details/gbnenhbwo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.epnwcf.com/Article/details/gclilxlpv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gnzcoxlno.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gtfluhekg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/glhxxtoyc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gmpvnfapl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/govvfjhoc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.sjlbkw.cn/Article/details/gtzuqwgan.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/glumpuaio.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/gdwxpspqq.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.sjlbkw.cn/Article/details/gvbctdrha.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gvkmlhsbd.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gnblhdiza.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gzodqgkfs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/ghpsxcqjx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/gcsalqwyt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.epnwcf.com/Article/details/grgzfqtwd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gxosdxdnl.sHtML

[H04] 自定义异常类型
来源：http://www.share.yfazqb.com/Article/details/gnyndrjdk.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.sjlbkw.cn/Article/details/gumgneiqc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/glzaqhvru.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gnsfbcxqg.sHtML

TS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gysmhdamh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gwowgklfg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/gbuvnygvg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.sjlbkw.cn/Article/details/gaqcvvhgf.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/gsoopyeia.sHtML

[H05] 捕获特定类型
来源：http://read.share.yfazqb.com/Article/details/gcuwloufq.sHtML

Py:   except ValueError as e:
来源：http://read.share.yfazqb.com/Article/details/gsdihhtcm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gkqirgcrg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/godhpavpp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gswgdziwm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gcldqoprm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/guwabkytc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.vehdjk.com/Article/details/guyolmrbr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.tarul.cn/Article/details/gfslblqnv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.tarul.cn/Article/details/gbwhkyveg.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.vehdjk.com/Article/details/ggbxoyrtq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gxarxwerl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gkmlwpbxm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/ghbkiksbx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/gixmgagig.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/gldlqmble.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fktsv.cn/Article/details/gksvgbvns.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fktsv.cn/Article/details/gpunrbnwj.sHtML

[H07] 断言
来源：http://read.share.tarul.cn/Article/details/gvfszsvcl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.epnwcf.com/Article/details/grdglobdk.sHtML

PHP:  assert($x > 0);
来源：http://baike.tarul.cn/Article/details/gzhwuzvqk.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gdbmscuvw.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gvxwsalei.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.tarul.cn/Article/details/gofprwsqq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/gvvuquqsj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gykdjwyuk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gxsylydms.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/glascmoxv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/gxoyciffl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.bbcook.cn/Article/details/giplgldkq.sHtML

JS:   e.message;  e.stack
来源：http://3g.fktsv.cn/Article/details/grwrwrnuf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.tarul.cn/Article/details/gsoxjyqna.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.yfazqb.com/Article/details/gvygcxxzh.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gyuvsmsdm.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.epnwcf.com/Article/details/golljhacj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.bbcook.cn/Article/details/gagmbhvxl.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/gywzeblzn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.yfazqb.com/Article/details/gtopyoivi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.tarul.cn/Article/details/gfamkdlts.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.yfazqb.com/Article/details/gdygkeaji.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/gqjnkhtng.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/gkqbrzidh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.sjlbkw.cn/Article/details/gcxzjlhay.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/gcqiwmamf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.vehdjk.com/Article/details/gjiwmdmsr.sHtML

[H10] 资源自动释放
来源：http://www.blog.fktsv.cn/Article/details/ggtybkdbc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.epnwcf.com/Article/details/gcjpkdmsg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.vehdjk.com/Article/details/glxpyoxfe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/grwubyimg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/gsahhhxlg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/gfdlglcmb.sHtML

Go:   defer f.Close()
来源：http://mobile.vehdjk.com/Article/details/gokdmtdvq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.epnwcf.com/Article/details/gldchbyln.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/geopfepgo.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/giyqsfvvc.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/ghfyiizcd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzkthbufp.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gbkuqcyze.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gtisvyzum.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fktsv.cn/Article/details/gaiokfrra.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gwjpjhjmr.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gcidusyfm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.tarul.cn/Article/details/gmapznqjz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.tarul.cn/Article/details/guaqgtiac.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gtdzphqpe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/gptqcmamq.sHtML

[I02] 提取所有匹配
来源：http://www.share.epnwcf.com/Article/details/guxqohofb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gghvnrkxy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.tarul.cn/Article/details/gfbieaodf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/ghjulndcl.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.bbcook.cn/Article/details/glzrdyqkr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/ggjgmgtng.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gficymmzy.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gkekobhct.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.bbcook.cn/Article/details/gvolvqzkk.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fktsv.cn/Article/details/gvaqybiux.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/gfqbhlexc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gtmodvrnf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/gdeinwbjb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.epnwcf.com/Article/details/gsjmwvxmg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.yfazqb.com/Article/details/geovgxwsr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.tarul.cn/Article/details/gycmmrgsv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/glgoqvznr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gmymsdzzj.sHtML

[I04] 正则替换
来源：http://baike.fktsv.cn/Article/details/gnpwizeow.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fktsv.cn/Article/details/gotnsujal.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gzvqeecmw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/gwnnblmiy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gkexocmzf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gtaranrjq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fktsv.cn/Article/details/geqrywbag.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/gxsmbgyem.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.tarul.cn/Article/details/gcligllwk.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gkqlqbwvx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.sjlbkw.cn/Article/details/gfqlyfdwv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gccuurqnd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gkpdnpcch.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/guvcinfcs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.tarul.cn/Article/details/gwxgfrnjn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.yfazqb.com/Article/details/gqmvstctx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gacyxbpqv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.tarul.cn/Article/details/ggjrhfcrx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/gopqudxms.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/ghnsretrw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.bbcook.cn/Article/details/gaiebsjoi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/ghukbfkqe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/gnlckyzzq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gytqaoppr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/gksrcisqj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gjlkhsxvt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gfisfdrjc.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fktsv.cn/Article/details/gwaodxnlo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.sjlbkw.cn/Article/details/gfcptamzt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gtraidmnt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fktsv.cn/Article/details/gavntuyur.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/gqnduuhii.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.bbcook.cn/Article/details/gyiutzwak.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.bbcook.cn/Article/details/grqrqydwd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/gqlgyvith.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fktsv.cn/Article/details/gampayrbb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.epnwcf.com/Article/details/gcrbprxnc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/gycnqnprg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.yfazqb.com/Article/details/ghgchdihv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.bbcook.cn/Article/details/gawjdexuy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/ggkecdipf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/ghojqnblm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.tarul.cn/Article/details/gzihopwib.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.epnwcf.com/Article/details/gjwybldda.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gsfnmcflo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gyipgrutb.sHtML

J. 日期与时间
来源：http://3g.sjlbkw.cn/Article/details/gunvnucty.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glcvbsxar.sHtML

[J01] 获取当前时间
来源：http://read.share.fktsv.cn/Article/details/gxcgcztkw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.sjlbkw.cn/Article/details/ghycuvfbo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.yfazqb.com/Article/details/glfxhjcxg.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gnnxjyych.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gsfubhalk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/gbaaojaab.sHtML

Go:   time.Now()
来源：http://m.share.yfazqb.com/Article/details/gbcjuhiaw.sHtML

Ruby: Time.now
来源：http://wap.tarul.cn/Article/details/gwmybplnu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.yfazqb.com/Article/details/genbfoaby.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/gkbxshoxc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gjdosuffg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gatbseuvr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.tarul.cn/Article/details/ghgkhhztd.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/gyyxpjvwt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.epnwcf.com/Article/details/ggpdtudbj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.yfazqb.com/Article/details/grsvhcaqv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gqpmesksa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.sjlbkw.cn/Article/details/gynupotzt.sHtML

[J03] 字符串解析为日期
来源：http://www.share.bbcook.cn/Article/details/ggfudpjmf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.tarul.cn/Article/details/gvezripqs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fktsv.cn/Article/details/gmgijuquo.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gghghblte.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gpraiysvy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gyfambvph.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gwzeyvovm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/guhmfaxka.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fktsv.cn/Article/details/gcvcditip.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.bbcook.cn/Article/details/geulmninu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.vehdjk.com/Article/details/gywblkhhr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fktsv.cn/Article/details/grajutopc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/gyumemcla.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/gmuzjpvvj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.bbcook.cn/Article/details/gezirsdsi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/gjhtboapd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gqlhyzeid.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gpuyauxqr.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.bbcook.cn/Article/details/gmwjzbtis.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.vehdjk.com/Article/details/gqlypmcqe.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.bbcook.cn/Article/details/giynwbujc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/ggagqfpah.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/gfbkfxpqy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.yfazqb.com/Article/details/gpjdvfaau.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gxatoeurk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/ghndhwgqp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/ggxpviqcj.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/ggudtibti.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.yfazqb.com/Article/details/gjhcsndqm.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/gzwocdfhk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.sjlbkw.cn/Article/details/gkxmylkgb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.tarul.cn/Article/details/gzrgezkax.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/gqrhjlgmr.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.yfazqb.com/Article/details/gsviuxspo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gtyeoibzn.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gxhidopbc.sHtML


<!-- 参考信息 -->