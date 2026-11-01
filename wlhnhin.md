代发 wailian999

Ruby: super
来源：http://blog.vehdjk.com/Article/details/gkmwoxgif.sHtML

C#:   base.Greet();
来源：http://3g.sjlbkw.cn/Article/details/goankttnu.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/gekgzdxjj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.vehdjk.com/Article/details/gaghxcjda.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gpjsckjyo.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/grimmknru.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gkltboneb.sHtML

Java: static void f() {}
来源：http://mobile.tarul.cn/Article/details/gsfavnguh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.sjlbkw.cn/Article/details/gwpvtlseu.sHtML

Ruby: def self.f; end
来源：http://baike.fktsv.cn/Article/details/gngvkoouc.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gvgfebovy.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.sjlbkw.cn/Article/details/gytjfhqbr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.epnwcf.com/Article/details/gihxynkzh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gwrhtdpud.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/grhatoozj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fktsv.cn/Article/details/gkwgpplwi.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.tarul.cn/Article/details/gvapciijc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.bbcook.cn/Article/details/gbmmptmfx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gnrccrcfd.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.sjlbkw.cn/Article/details/gktcowhmc.sHtML

[G10] 访问控制
来源：http://m.share.tarul.cn/Article/details/gnreolnle.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gswkqtkkh.sHtML

PHP:  public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gcqdudbln.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gsgsctefg.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gxndwfhfq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/gbekfkpee.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fktsv.cn/Article/details/gxouehgmy.sHtML

Ruby: public / protected / private
来源：http://wap.epnwcf.com/Article/details/gbdxtkezp.sHtML

C#:   public / protected / private / internal
来源：http://blog.fktsv.cn/Article/details/gxhufjrte.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/groocmvuh.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gnkcgonci.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/guebnwoay.sHtML

JS:   get name() { return this._name; }
来源：http://baike.epnwcf.com/Article/details/guojbqgzy.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gbsijktyn.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gwabwscpo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gnwpiakqc.sHtML

Ruby: attr_accessor :name
来源：http://blog.vehdjk.com/Article/details/gdfreqgft.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fktsv.cn/Article/details/gxsdwkrjx.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/guinltlti.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/geutcdnrr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gcjmtgcrg.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gprlbnaey.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/grbnumgui.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gkjggzyby.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gkdbdlphy.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfozzcug.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.vehdjk.com/Article/details/gznwadgqh.sHtML

[G13] 判断对象类型
来源：http://blog.fktsv.cn/Article/details/gpghsuhih.sHtML

Py:   isinstance(u, User)
来源：http://mobile.bbcook.cn/Article/details/gbirgimiy.sHtML

PHP:  $u instanceof User
来源：http://baike.vehdjk.com/Article/details/ghlenupza.sHtML

JS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/ghyfzigsm.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gnctjwewl.sHtML

Java: u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/godwcccmb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/gjwcajxwm.sHtML

Ruby: u.is_a?(User)
来源：http://wap.yfazqb.com/Article/details/gzppwotmb.sHtML

C#:   u is User
来源：http://read.share.tarul.cn/Article/details/gnlfnbiig.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/gldmkkrho.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.sjlbkw.cn/Article/details/gcynxkqxm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/gupsmunrq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/gelrkhtsn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.tarul.cn/Article/details/gcubcctvy.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.vehdjk.com/Article/details/gsgnqhszo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fktsv.cn/Article/details/gjpsxtvwd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.bbcook.cn/Article/details/gktoubvcw.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.tarul.cn/Article/details/gajehxolh.sHtML

[G15] 枚举
来源：http://read.share.fktsv.cn/Article/details/gqzidznmy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fktsv.cn/Article/details/gysplucia.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fktsv.cn/Article/details/gwjulboqt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.tarul.cn/Article/details/gsekohsct.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gfhwbpuda.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gezepqxcs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.yfazqb.com/Article/details/grkegeiut.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.bbcook.cn/Article/details/gyqzlever.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gdkebalcr.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fktsv.cn/Article/details/gwmfoylft.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/ggbciyjdu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/gwjfzmgng.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gtsdtnbej.sHtML

TS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gnoljpenb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.epnwcf.com/Article/details/gdorhprru.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.vehdjk.com/Article/details/gigigetad.sHtML

Ruby: obj.instance_variables
来源：http://read.share.sjlbkw.cn/Article/details/gwrpivvmv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gcygkugtf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gugeoqsqn.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/ghkaepcfy.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfuxouksn.sHtML

[H01] try / catch 基础
来源：http://blog.vehdjk.com/Article/details/ggfhrlzdu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gkygyufpo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.bbcook.cn/Article/details/grstgxulk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/grliykcsr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gaaorwpmm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fktsv.cn/Article/details/gulhsljus.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.yfazqb.com/Article/details/genrbgxgm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.epnwcf.com/Article/details/gnmmxguai.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.vehdjk.com/Article/details/gwjfotkdu.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/gzhxadjca.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.yfazqb.com/Article/details/grvbsqjvx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gkhfkuyik.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gtlamxknz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gvewmyapm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gtjnxlyar.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fktsv.cn/Article/details/gvlficolw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/gkljkulmv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.tarul.cn/Article/details/gtzyokvfk.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/gnknmfjsu.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/gmuuyoqka.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gcunznwok.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gzljznzlt.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gfuijmzcq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/guduerqgv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/gqhftrypw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gwcpnecmc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gttuntkth.sHtML

[H04] 自定义异常类型
来源：http://wap.fktsv.cn/Article/details/gssasswge.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gkyhgwurw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gpkfnlyfu.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gbffdjzqc.sHtML

TS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/gfvsgjgvt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gdqrocjzy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.bbcook.cn/Article/details/ggvhmnprc.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.tarul.cn/Article/details/gaxjctksi.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/givezzbqw.sHtML

[H05] 捕获特定类型
来源：http://www.blog.bbcook.cn/Article/details/gptoropzf.sHtML

Py:   except ValueError as e:
来源：http://3g.yfazqb.com/Article/details/gpvyihkro.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.vehdjk.com/Article/details/ghqzrazib.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/grnkugicl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/glwmzrowe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.epnwcf.com/Article/details/gysutikau.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/gmoprkstv.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.epnwcf.com/Article/details/gcybjrzzh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.yfazqb.com/Article/details/gxuypogdf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/gmtmsuqhg.sHtML

Py:   value = d.get("k") or default
来源：http://baike.vehdjk.com/Article/details/gdmqgjtrf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.bbcook.cn/Article/details/ghxqjhvhw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/guhfggcdt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gzkxqcudb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fktsv.cn/Article/details/gealvqysw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.bbcook.cn/Article/details/gqlgqgcfb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/ggnttevkg.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gopaehven.sHtML

[H07] 断言
来源：http://m.share.tarul.cn/Article/details/gydihmxty.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/gthimnkdt.sHtML

PHP:  assert($x > 0);
来源：http://read.share.epnwcf.com/Article/details/gmvldedvy.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gnnolythz.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gqemlfdqf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.vehdjk.com/Article/details/giuixwnyy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.bbcook.cn/Article/details/gsxakemss.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/ggnzspzbq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gkhtrqums.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fktsv.cn/Article/details/gmutyzohl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gyxgjgnxi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/gnkeatmco.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.tarul.cn/Article/details/gznmmnbty.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fktsv.cn/Article/details/gmrtmvxuv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.sjlbkw.cn/Article/details/gjbfiqapt.sHtML

Go:   err.Error()
来源：http://baike.bbcook.cn/Article/details/gkyjodthq.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.yfazqb.com/Article/details/gqigpvoub.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.epnwcf.com/Article/details/gvbkqplpg.sHtML

[H09] 带错误码的异常
来源：http://www.blog.vehdjk.com/Article/details/gtimbnlqn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.sjlbkw.cn/Article/details/ghxgemggc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gmexhskne.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.sjlbkw.cn/Article/details/guhptgysz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.vehdjk.com/Article/details/gxozgwguq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.tarul.cn/Article/details/grqwhbvux.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.sjlbkw.cn/Article/details/gqgycjgox.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.epnwcf.com/Article/details/gskpugwcl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gmobppkgc.sHtML

[H10] 资源自动释放
来源：http://www.blog.vehdjk.com/Article/details/ghadzyaob.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.sjlbkw.cn/Article/details/gicoompit.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.yfazqb.com/Article/details/gsfakjsqj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gqakdljbd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/gqohyhzsw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.epnwcf.com/Article/details/gemdfarwq.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/geousgcel.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/gyspfgebd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gloeucihs.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gedlzqezq.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/gsyjzzgfe.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmchpmmwu.sHtML

[I01] 判断是否匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gzamhhtfb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fktsv.cn/Article/details/gcoyrzavt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.yfazqb.com/Article/details/gsjujiufy.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/ghbkdmfvc.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gekwiiheo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/gmsgutook.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fktsv.cn/Article/details/grnpvmvmv.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.bbcook.cn/Article/details/grijwmsyb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.vehdjk.com/Article/details/gtkyemcdx.sHtML

[I02] 提取所有匹配
来源：http://www.share.sjlbkw.cn/Article/details/gehrviega.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gtxhomqjt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/gtbbjjbdc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fktsv.cn/Article/details/gndxppter.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.sjlbkw.cn/Article/details/gvwtsharq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.vehdjk.com/Article/details/geukjjcnd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gjyfysvya.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gxycdttkh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gpelxpgzm.sHtML

[I03] 提取捕获分组
来源：http://read.share.yfazqb.com/Article/details/gonteefdq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.tarul.cn/Article/details/gpwrweqzs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fktsv.cn/Article/details/gtlylvrgf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.tarul.cn/Article/details/gbixrrjaw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.sjlbkw.cn/Article/details/ggzxaxnrh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.bbcook.cn/Article/details/gmysotkbw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/gvrgpkxdy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.bbcook.cn/Article/details/ganjzxwgo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fktsv.cn/Article/details/gufhhyqur.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/gobrdtgzy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.tarul.cn/Article/details/gugtwiked.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.epnwcf.com/Article/details/gahfvvsme.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/ghwcigzzv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gjtkkraio.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/guhesdkyh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.vehdjk.com/Article/details/gjcgoygnb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fktsv.cn/Article/details/gdplnqzfu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gopjaanuf.sHtML

[I05] 按正则拆分
来源：http://mobile.tarul.cn/Article/details/gyyywnpld.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/gqsrbfbth.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.epnwcf.com/Article/details/gkudiubqz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gwrdpcauo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gygowgivg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fktsv.cn/Article/details/gzldbopzm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.tarul.cn/Article/details/gbovumkmb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gzpuwqxin.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/gtzkgubjy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/ghvslaqry.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gsowmruhm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.bbcook.cn/Article/details/gnmsaadpv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gpsfudeys.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gsuhcidop.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyxivklj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.bbcook.cn/Article/details/gfnzbwjbn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.yfazqb.com/Article/details/gavqtyveu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gpbwgpcow.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.vehdjk.com/Article/details/gjtdlqlsc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.vehdjk.com/Article/details/gfsnegyzn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.bbcook.cn/Article/details/gkkaibupj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fktsv.cn/Article/details/gmpcxnaor.sHtML

TS:   /error/gim
来源：http://read.share.yfazqb.com/Article/details/gerumylla.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.bbcook.cn/Article/details/gdpslitnt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.sjlbkw.cn/Article/details/gdqhdajjr.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.sjlbkw.cn/Article/details/gbxlqzwvb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.tarul.cn/Article/details/gimslbilr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.vehdjk.com/Article/details/ghniaoqya.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fktsv.cn/Article/details/gvsngoxxz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gjjatdtzu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gboqkfuso.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/glzvrkfnr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/gvhhgqosk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gsxdqnptx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.vehdjk.com/Article/details/gyliqweyy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gelvrshqg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtpkcbghq.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gycvdppjg.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjvyhjlzv.sHtML

[J01] 获取当前时间
来源：http://baike.vehdjk.com/Article/details/gvkzfwjib.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.epnwcf.com/Article/details/ggkpvdvpn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/gyvtwsqcj.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gqqprwdgu.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gxepggpze.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.tarul.cn/Article/details/gswfbivun.sHtML

Go:   time.Now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfxzpzbt.sHtML

Ruby: Time.now
来源：http://m.share.sjlbkw.cn/Article/details/gzxuimnbh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.bbcook.cn/Article/details/gchexzamo.sHtML

[J02] 格式化输出
来源：http://blog.vehdjk.com/Article/details/geufhfzww.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gchuujgrc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.tarul.cn/Article/details/gqdolixdj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fktsv.cn/Article/details/gbudvrviy.sHtML

TS:   d.toISOString()
来源：http://www.share.sjlbkw.cn/Article/details/gfalhojhg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.yfazqb.com/Article/details/gzwviqrjf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.yfazqb.com/Article/details/ghaoljlxu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gjyrabyyw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.yfazqb.com/Article/details/gbdlfwtyo.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.yfazqb.com/Article/details/gsqhwmpyu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/gpkbtlarw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.epnwcf.com/Article/details/gbjlftcck.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gtqtumren.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gxigdptgj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gqfqilmgc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gfkcskdbf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gnysjswsj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.yfazqb.com/Article/details/gkpqjcloh.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.bbcook.cn/Article/details/glyqbdjdi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/gjhtszdrp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.bbcook.cn/Article/details/gjyvinthp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.epnwcf.com/Article/details/gplkytuph.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.yfazqb.com/Article/details/ghddchmfy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/ghkpibjlz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/gxtgqreyj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.tarul.cn/Article/details/garwjyquo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.vehdjk.com/Article/details/gujlgkjen.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gqbuydofd.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.sjlbkw.cn/Article/details/gfiiqzdtv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.yfazqb.com/Article/details/gzkmoqrbf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/ggxvwuewa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gtqnvxnrm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gwzkizlbf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.epnwcf.com/Article/details/gifncqamd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/gpedrkrpl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.bbcook.cn/Article/details/gwprqtapy.sHtML

[J06] 计算两时间之差
来源：http://baike.vehdjk.com/Article/details/gohvimlut.sHtML


<!-- 参考信息 -->