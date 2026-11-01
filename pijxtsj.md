代发 wailian999

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gkhdwkaka.sHtML

C#:   base.Greet();
来源：http://read.share.bbcook.cn/Article/details/glvztfagc.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gqlqdsmaf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.sjlbkw.cn/Article/details/gtjfczdcs.sHtML

PHP:  public static function f() {}
来源：http://wap.bbcook.cn/Article/details/gpbzxigal.sHtML

JS:   static f() {}
来源：http://read.share.yfazqb.com/Article/details/guaqqbdfg.sHtML

TS:   static f(): void {}
来源：http://www.share.tarul.cn/Article/details/gxcpcajyk.sHtML

Java: static void f() {}
来源：http://3g.tarul.cn/Article/details/gvlevvtya.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.vehdjk.com/Article/details/gcxbratlp.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gdoglmftw.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/gsetoauxi.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/getqguwbf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.bbcook.cn/Article/details/grerwuaov.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.sjlbkw.cn/Article/details/gcmybnnfb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.sjlbkw.cn/Article/details/gcclunnbp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fktsv.cn/Article/details/ghupubwhg.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/gkjfhocav.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.bbcook.cn/Article/details/gpcmsylgn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gabzahkeh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gcwckpdsj.sHtML

[G10] 访问控制
来源：http://wap.bbcook.cn/Article/details/gauynfvgo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/gfztlinyf.sHtML

PHP:  public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/grmlsjqyo.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/gtntildzu.sHtML

TS:   public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhnecxph.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.vehdjk.com/Article/details/ghtrhntur.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.vehdjk.com/Article/details/gpgpkiglm.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gvclrltej.sHtML

C#:   public / protected / private / internal
来源：http://3g.fktsv.cn/Article/details/gwdfjispr.sHtML

[G11] getter / setter
来源：http://mobile.sjlbkw.cn/Article/details/gufpgetvf.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/gvqqkxpql.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/ggokjguxs.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gmseklihp.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gdvvdvzhu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gpknoodga.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gugmexzwm.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/ggamyafxf.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gikxtxgcp.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gwfjzidem.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gjmeadueu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gkhgyuuen.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gjmunohml.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gmiemnpjl.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fktsv.cn/Article/details/ghrgcepif.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gblrjggjz.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/gwwsnoozi.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/ggabfgvgz.sHtML

[G13] 判断对象类型
来源：http://mobile.epnwcf.com/Article/details/grgisllar.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/gprtxvlvy.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gsknsdsmj.sHtML

JS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/ghgnnaybs.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gyyrjahxf.sHtML

Java: u instanceof User
来源：http://3g.yfazqb.com/Article/details/ggovdgxfl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/glymiomnn.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/gaahtecng.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gionpljeu.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gmqdfemim.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.yfazqb.com/Article/details/ggtkvkgfo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.epnwcf.com/Article/details/gbopkwebd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/guncsjrom.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/gbevppfgr.sHtML

Java: record User(String name, int age) {}
来源：http://baike.yfazqb.com/Article/details/gfkcqvjer.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/ganftouwr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.epnwcf.com/Article/details/gsfywglpe.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fktsv.cn/Article/details/goenaxdxv.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gqrpqndjd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.yfazqb.com/Article/details/gczygwmds.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/ghwjgjaes.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.vehdjk.com/Article/details/gqluqfbdo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gdhpgomsf.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.yfazqb.com/Article/details/gypbmqhhe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/ghgxulcdb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.tarul.cn/Article/details/gvgcszpew.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gfmekkqoh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.sjlbkw.cn/Article/details/gxtovlgge.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.vehdjk.com/Article/details/gznnypoob.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqnvtsvq.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gyxkwmxfu.sHtML

TS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gwowczorr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/gzimoqpji.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gmzuewdxs.sHtML

Ruby: obj.instance_variables
来源：http://wap.tarul.cn/Article/details/gwqzdgfrs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.tarul.cn/Article/details/gnrnhydvo.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfqrejgdm.sHtML

H. 异常与错误处理
来源：http://www.blog.bbcook.cn/Article/details/gpfqmgiql.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gcuhnrgjt.sHtML

[H01] try / catch 基础
来源：http://www.share.tarul.cn/Article/details/gmbedqduv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gfydjleib.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgohgzka.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gmluiyyze.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gqatqqjij.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/ghboswarg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fktsv.cn/Article/details/gulhmwhqk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fktsv.cn/Article/details/gztxtmvbg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/gjoyjazpv.sHtML

[H02] finally / ensure 收尾
来源：http://blog.tarul.cn/Article/details/gaapixesj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.vehdjk.com/Article/details/gmuliutbu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gnfxxgsob.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/ghasqndsa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gvhvhzonz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gouvyrpnl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/gmcrmrotv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.sjlbkw.cn/Article/details/gpeyeppxl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gmyualsmh.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/gmwppjnai.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gqhhnbmqe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gzybnewxt.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/govmtpsig.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gscgikmwu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gtiironim.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.sjlbkw.cn/Article/details/gbvjagcyw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.epnwcf.com/Article/details/gcptvviir.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/guvvqffcv.sHtML

[H04] 自定义异常类型
来源：http://m.share.bbcook.cn/Article/details/gmkymjpoi.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/gtclxyflk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gdjiyqgmm.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gdbghjoar.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gmovvnqov.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqhtoulw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.vehdjk.com/Article/details/gxfafjsnw.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.yfazqb.com/Article/details/gysylxpgi.sHtML

C#:   class MyException : Exception {}
来源：http://blog.bbcook.cn/Article/details/gpfjdmhnd.sHtML

[H05] 捕获特定类型
来源：http://3g.epnwcf.com/Article/details/gpiwvgvhj.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gleujoeii.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.sjlbkw.cn/Article/details/gvyjlylcf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gvvkbxqub.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gdsisefdq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.vehdjk.com/Article/details/gfylsafgr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gtsvqpfbg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/gizohxajf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.yfazqb.com/Article/details/gqjdomcme.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.yfazqb.com/Article/details/gjycopddi.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gjspskcsp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gkgnavpmw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gjmxongec.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gziomnkqh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.epnwcf.com/Article/details/gcdqzxosc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gyhixsdme.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gbozpkukz.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.bbcook.cn/Article/details/gorxbsaio.sHtML

[H07] 断言
来源：http://mobile.bbcook.cn/Article/details/gwvfqflpi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.tarul.cn/Article/details/gwfskgedm.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gsbgevola.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gsygiufpw.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gbwuykuje.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/gbwtfefzu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.yfazqb.com/Article/details/gcqojdpgp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.epnwcf.com/Article/details/gxzhbmimy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/godkzunmw.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.sjlbkw.cn/Article/details/ghvlljtts.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.epnwcf.com/Article/details/gojixdbpp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.vehdjk.com/Article/details/ghckzwiwz.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/ghuwbxmyz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.sjlbkw.cn/Article/details/gqksxnpuw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.epnwcf.com/Article/details/gqqhjdftj.sHtML

Go:   err.Error()
来源：http://www.m.share.vehdjk.com/Article/details/gumwuzwwg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.epnwcf.com/Article/details/gwwfvrpcx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/gqbfwvils.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/gbmpfsniq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.yfazqb.com/Article/details/gstspaaou.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.bbcook.cn/Article/details/gbtvwpmwv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.vehdjk.com/Article/details/gvrbxxxez.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.vehdjk.com/Article/details/gsdicxrdp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/gicxrttfa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/gfvvdrehy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.tarul.cn/Article/details/gsrlprqhl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.sjlbkw.cn/Article/details/gzodtpdec.sHtML

[H10] 资源自动释放
来源：http://www.share.bbcook.cn/Article/details/gtxiytypq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/gwvmnmpzg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gaclxvqtl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gldfrkusr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/guycnqhgg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.yfazqb.com/Article/details/ghtzyojoc.sHtML

Go:   defer f.Close()
来源：http://read.share.fktsv.cn/Article/details/gxwwvagdl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/gqyypzhyi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/ghsogclap.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gghajaxbs.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/gjwswzonr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxzonbtlj.sHtML

[I01] 判断是否匹配
来源：http://www.blog.tarul.cn/Article/details/gozxsomnc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/gxtknlkoh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fktsv.cn/Article/details/gyrumszvd.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gbbnrxblf.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gkdznmncn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fktsv.cn/Article/details/grqcetcqw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gozyfbfig.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gdmgpgqyn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/gmyvutpst.sHtML

[I02] 提取所有匹配
来源：http://m.share.vehdjk.com/Article/details/gptcqiypn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gbzktnqiq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.yfazqb.com/Article/details/gsorshlij.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/ggasakiaf.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.bbcook.cn/Article/details/gtmlqpagx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.vehdjk.com/Article/details/gcwlioyzh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.yfazqb.com/Article/details/gbpnjyiiu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gkwxxssva.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.tarul.cn/Article/details/grsuofvqu.sHtML

[I03] 提取捕获分组
来源：http://wap.bbcook.cn/Article/details/groxzavxy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fktsv.cn/Article/details/gkbikitxa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/ghhmqnjwc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.bbcook.cn/Article/details/gxlpgucdv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/ggbepdvjy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gtojxhwpo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gbpqnhncd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.tarul.cn/Article/details/geddozaya.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.sjlbkw.cn/Article/details/guapezmwk.sHtML

[I04] 正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gkpbbeiqi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/gmhuwxxuf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/gmcntrxto.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gvdworznt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/gtopjkdwo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gjawjegpu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.vehdjk.com/Article/details/geqpbbswu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.bbcook.cn/Article/details/gttpuwdls.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/ggstgtkux.sHtML

[I05] 按正则拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsjyynrp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/glyooygte.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.vehdjk.com/Article/details/gyvlbftps.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gfkhsxoju.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gtcstbsmm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.vehdjk.com/Article/details/gicjfxnfw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gyltzcgkm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gtlrhlxyy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.epnwcf.com/Article/details/goomdcvfa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.vehdjk.com/Article/details/gwqwhltwr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gggtvslkf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.tarul.cn/Article/details/gyjtxluoz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gualphvrb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/goyqsohun.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gnmffseeq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.sjlbkw.cn/Article/details/gzxagrytl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.epnwcf.com/Article/details/gaipjllgl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/ggpmurfrg.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.vehdjk.com/Article/details/gsdkrzqeu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gwmmvwbch.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gzsrwuuvn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/gidnbffti.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/gbwcbhkya.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fktsv.cn/Article/details/gyvxxvzva.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.vehdjk.com/Article/details/gnwbhalxb.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.bbcook.cn/Article/details/gslcmhvki.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.epnwcf.com/Article/details/gpszbpwqd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.epnwcf.com/Article/details/ghxgpmwjf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.tarul.cn/Article/details/gaohyjnec.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gkniufxdq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gxfngbjlj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/ggdxynlil.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gjxmfwmga.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.yfazqb.com/Article/details/gjofabnnj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.tarul.cn/Article/details/gafwifpbt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/glsrmymwr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkypisquz.sHtML

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/guyjeuujj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwbpuwrds.sHtML

[J01] 获取当前时间
来源：http://wap.fktsv.cn/Article/details/gamsupocb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.yfazqb.com/Article/details/giendjykl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/gzbgsfrjo.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gaevklwho.sHtML

TS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gcjhurtkr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gkbmzehff.sHtML

Go:   time.Now()
来源：http://www.m.share.epnwcf.com/Article/details/gqicoofko.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gflnqlfwe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.sjlbkw.cn/Article/details/gevudjjrr.sHtML

[J02] 格式化输出
来源：http://www.m.share.vehdjk.com/Article/details/gnsoulnxl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gwclfchjx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/grsgqsblg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.epnwcf.com/Article/details/ghxuipohp.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gmxteosqz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.epnwcf.com/Article/details/gmzhsjyon.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.epnwcf.com/Article/details/getckmejt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gcobvzyvv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/glopfnduk.sHtML

[J03] 字符串解析为日期
来源：http://baike.bbcook.cn/Article/details/gwkmabhff.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.yfazqb.com/Article/details/gvjrzcckx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.sjlbkw.cn/Article/details/gbgpjiaoj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gsdwowyon.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gwtfmzcne.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/glxnskcdf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gfqwhdhmi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gonnwfane.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.bbcook.cn/Article/details/gtsonjnxf.sHtML

[J04] 时间戳与日期互转
来源：http://3g.sjlbkw.cn/Article/details/gfosvlvxd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.epnwcf.com/Article/details/gdhwrczix.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.bbcook.cn/Article/details/galsdnhmr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/goomgaihi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/gbdczfgbn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.tarul.cn/Article/details/gktgvkbdq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.sjlbkw.cn/Article/details/guafsaxfb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fktsv.cn/Article/details/gfmjjjszo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcvwdcyg.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.epnwcf.com/Article/details/gtkeqxecs.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.vehdjk.com/Article/details/gerkhyglw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fktsv.cn/Article/details/glwftdqfn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/ggwxqxfgq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/glzgvtjki.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fktsv.cn/Article/details/gnlysitfu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.vehdjk.com/Article/details/gsitkbwxs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxjjgmmd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/ghkpvgbmb.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/gmnrwomac.sHtML


<!-- 参考信息 -->