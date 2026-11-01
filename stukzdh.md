代发 wailian999

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/ggovogkrh.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gpldokagr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/ghfuspmzq.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gwrwzcagj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gvkqhipah.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gmeibshdc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/giauevpvo.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.vehdjk.com/Article/details/gsauylwyb.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.vehdjk.com/Article/details/gcjicacay.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/gfqnycyxt.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/gwgnljuqj.sHtML

PHP:  parent::greet();
来源：http://www.share.sjlbkw.cn/Article/details/gdffflctu.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/ggtopmdqg.sHtML

TS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/grkqpzcxc.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/govgvklkc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.bbcook.cn/Article/details/gostdiasx.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/grmgboaam.sHtML

C#:   base.Greet();
来源：http://blog.vehdjk.com/Article/details/grfodntsr.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/gnmuowlnz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gdfliacbk.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/gzmouvmcw.sHtML

JS:   static f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gmvqfibzq.sHtML

TS:   static f(): void {}
来源：http://read.share.fktsv.cn/Article/details/gaxyyusij.sHtML

Java: static void f() {}
来源：http://baike.tarul.cn/Article/details/gzqxyyzwa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/glqjrhsiy.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/gfuoslakk.sHtML

C#:   public static void F() {}
来源：http://read.share.tarul.cn/Article/details/gqwurblkv.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fktsv.cn/Article/details/gudfyvphm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.tarul.cn/Article/details/gjbcjmlij.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.yfazqb.com/Article/details/ghgfiwlkm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.vehdjk.com/Article/details/goerfxntd.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.tarul.cn/Article/details/gtfsharwv.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/gblnbgnku.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gcsspsfag.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.vehdjk.com/Article/details/gsjekgyek.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gwxtpvxpq.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/gphwlxfli.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/gxwwrexzq.sHtML

PHP:  public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gnmivsymw.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.yfazqb.com/Article/details/gzpbvrzgl.sHtML

TS:   public / protected / private
来源：http://blog.yfazqb.com/Article/details/ginfqdpre.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.tarul.cn/Article/details/ggatgjdjg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gshrdwkbl.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/goghsbvee.sHtML

C#:   public / protected / private / internal
来源：http://3g.vehdjk.com/Article/details/gtxlueeii.sHtML

[G11] getter / setter
来源：http://www.share.fktsv.cn/Article/details/gwatdpqsg.sHtML

Py:   @property 与 @x.setter
来源：http://wap.epnwcf.com/Article/details/gdgxilzkt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gsqwusfer.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gqotmngyq.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gfrlkwmul.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/ghcbdhsmb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gbihnqyan.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gklgfxvui.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.epnwcf.com/Article/details/glxxwllxb.sHtML

[G12] 对象转字符串
来源：http://blog.vehdjk.com/Article/details/gdpzwuiqb.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gpgwctibh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gzzrziokb.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gvijdsqbh.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gkhtvyphe.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.tarul.cn/Article/details/gwuxqkfdj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/glezbkwth.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gjrkpeipy.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gvmxffvjv.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/ggdsbnqiv.sHtML

Py:   isinstance(u, User)
来源：http://wap.tarul.cn/Article/details/gyeroacsz.sHtML

PHP:  $u instanceof User
来源：http://wap.vehdjk.com/Article/details/ggmmwlxaj.sHtML

JS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gwxozdfmd.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gtquytrmv.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gzenrolgg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.vehdjk.com/Article/details/gjybbhrkl.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.bbcook.cn/Article/details/gzbvostxo.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/gqrugpnqz.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gtxazehry.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/gtmselzrt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.bbcook.cn/Article/details/gezevaksf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.bbcook.cn/Article/details/gujzynohh.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.vehdjk.com/Article/details/geasrwfgb.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.sjlbkw.cn/Article/details/goqzltcxx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/gcwvrcmfg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.epnwcf.com/Article/details/gowezumhl.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/giweicadp.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/gobcambjp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/grwkoodda.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/gzmhploaz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gbprsbcca.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gyuwplugr.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.epnwcf.com/Article/details/gtwaubkqh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/gnjtzkrer.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.epnwcf.com/Article/details/gwagwrhcg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gpudraure.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.tarul.cn/Article/details/geknyifje.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.vehdjk.com/Article/details/gloymebcw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.epnwcf.com/Article/details/gzrkhpdof.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gxmlgappw.sHtML

TS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/ggaliytqi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fktsv.cn/Article/details/ggxyjpsut.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.sjlbkw.cn/Article/details/gixpicxdy.sHtML

Ruby: obj.instance_variables
来源：http://www.share.yfazqb.com/Article/details/gbuokdhro.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gzjqfuumf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdixvaxub.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gwjwkusmb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gblkntcaj.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gxuclbxpn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/gqrtbynfr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.sjlbkw.cn/Article/details/gjiqjoypf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gzspszifx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gnzxkcnnj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/gjfwjtncm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/guqrxstox.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gjtiiomev.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gbgnbqsrc.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/gpnoikzaj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.sjlbkw.cn/Article/details/gbiyxkxrv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gvqqfqkcm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/ghrkiphrk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gatzircco.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gjweyavdb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gezhupxbs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.yfazqb.com/Article/details/gamsigacy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gwhhyoazb.sHtML

[H03] 主动抛出异常
来源：http://blog.yfazqb.com/Article/details/gfjgyjrko.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.sjlbkw.cn/Article/details/gztscmgaq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/glsxxqmlm.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/ggryfwnut.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/ghgxyaegt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/giodevnqq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.yfazqb.com/Article/details/glqgcimao.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.yfazqb.com/Article/details/gimuqellz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gbtdzpvby.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gssixgcto.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.yfazqb.com/Article/details/gndppxpfp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/glavmihcr.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gzneylrfv.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/ggwmhlmls.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gioyevmgm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/ghihrlubl.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.epnwcf.com/Article/details/gbywuixev.sHtML

C#:   class MyException : Exception {}
来源：http://baike.tarul.cn/Article/details/geujqtsso.sHtML

[H05] 捕获特定类型
来源：http://read.share.fktsv.cn/Article/details/govlneluq.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.yfazqb.com/Article/details/gumjvpkdm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/ghqghbxwz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/genfeekki.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gprtsxjcj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gqfkjvfuu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.bbcook.cn/Article/details/gqpfkpdaw.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gkycudcbz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.epnwcf.com/Article/details/gvkcuejps.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/gqkdzpcck.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.vehdjk.com/Article/details/guqqvxeqv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/godkanhed.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gpvcmiltu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/ggdxwgseb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.sjlbkw.cn/Article/details/gnxvqujbb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.sjlbkw.cn/Article/details/gzoqjzjpt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.tarul.cn/Article/details/gprbstkre.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.yfazqb.com/Article/details/gcrscejlo.sHtML

[H07] 断言
来源：http://3g.sjlbkw.cn/Article/details/gbjkclaqk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.tarul.cn/Article/details/gimvvkmit.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/gulsvyfmi.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gixglpmoh.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/goykponmf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.epnwcf.com/Article/details/gwyghdhxv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.epnwcf.com/Article/details/gdvvhvlod.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.vehdjk.com/Article/details/gcybpkzwp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/ghfaesubm.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.sjlbkw.cn/Article/details/gxelylwbe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.vehdjk.com/Article/details/gouyvtthy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.tarul.cn/Article/details/gtqaqcwda.sHtML

JS:   e.message;  e.stack
来源：http://www.share.yfazqb.com/Article/details/gbdahwjzi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.bbcook.cn/Article/details/gzsvxecst.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.bbcook.cn/Article/details/gfwvgobbz.sHtML

Go:   err.Error()
来源：http://mobile.fktsv.cn/Article/details/gtvpnaois.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/gwvxxshrn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.vehdjk.com/Article/details/gleeyjrwb.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.epnwcf.com/Article/details/glptnbnac.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/gczwilqfk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.tarul.cn/Article/details/gqfmahdqs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.yfazqb.com/Article/details/gyesypqzu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/gegqqomkk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fktsv.cn/Article/details/gngoynjwp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gcweqbxoz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/gmaxqkzrz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.epnwcf.com/Article/details/gvxcllvyi.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/ghhebkmyq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.vehdjk.com/Article/details/gyrzvcuib.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.bbcook.cn/Article/details/gajuoipzl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fktsv.cn/Article/details/gerxnkagq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gkinjsqyn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.epnwcf.com/Article/details/gryeugpsu.sHtML

Go:   defer f.Close()
来源：http://www.m.share.epnwcf.com/Article/details/gwkyousun.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/grqatjszr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gbczsdtgt.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtxyqswsb.sHtML

I. 正则表达式
来源：http://www.blog.yfazqb.com/Article/details/gjxkzloxx.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsbcwfsho.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/gsvejupcl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gfotqurkp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.yfazqb.com/Article/details/gswkgdgxs.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gabyqxdad.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gmnovassx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gjkceckkh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.vehdjk.com/Article/details/gwzpmkjlp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gunnprasw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.vehdjk.com/Article/details/gwhcofqhi.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/gotgmiycc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gqopzccfa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.vehdjk.com/Article/details/gvfthnxnn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/gyozhokda.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fktsv.cn/Article/details/gsfwxiuse.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.epnwcf.com/Article/details/gbaimlimj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gnjcpnssv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gkbeijzlk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.bbcook.cn/Article/details/giphykpxz.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/gqqsqogyy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.sjlbkw.cn/Article/details/gcpdwhdjy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.yfazqb.com/Article/details/guhzcdegu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.epnwcf.com/Article/details/gevmswiug.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.sjlbkw.cn/Article/details/gjkrtkzcj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.yfazqb.com/Article/details/ggspcqjnq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.vehdjk.com/Article/details/gssbtcvze.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.vehdjk.com/Article/details/gdiixgxtn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.bbcook.cn/Article/details/gefaiuwcv.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/gcpgrfyxq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fktsv.cn/Article/details/gjnipdcve.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/ghmmugkba.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gtxwiwvub.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/glpbcfess.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gbixnkgvb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fktsv.cn/Article/details/gzudfbidu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/gqpwpkjgg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gmkpgkrsa.sHtML

[I05] 按正则拆分
来源：http://wap.bbcook.cn/Article/details/gjtrngrnt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.tarul.cn/Article/details/geheuokpt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gsdwemnhu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gjbqlacwm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gxszzneon.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/gdhceswhe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gtcutbcjn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gonvlcwmk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gbucmgmrk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.sjlbkw.cn/Article/details/gylmiskzo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gkegolmnx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/gdpmzpmvr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gjpcllksi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gmdwkujfz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/ghuspyjej.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/gfngirrhl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fktsv.cn/Article/details/gblyendvs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwnejtpr.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.yfazqb.com/Article/details/gbbhzhrha.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.epnwcf.com/Article/details/guoqrrpcb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gjxtiahip.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/goybrewnd.sHtML

TS:   /error/gim
来源：http://3g.fktsv.cn/Article/details/ghaawbqtw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.sjlbkw.cn/Article/details/glqqxybjs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/gqwdspklu.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.tarul.cn/Article/details/gdceeggcq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/gecvnbnxx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.sjlbkw.cn/Article/details/gcmzvzydk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.sjlbkw.cn/Article/details/guhisiumj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.vehdjk.com/Article/details/geeopgbnq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gxuxnofyy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gzbodhkok.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gruiqnrwo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/gunezpcuo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/gncnmsfyo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/gipsesqok.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gklrmqhxx.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/ggfrovibg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhdqugir.sHtML

[J01] 获取当前时间
来源：http://wap.bbcook.cn/Article/details/guwrxrtfb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.vehdjk.com/Article/details/goxndyqgw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/glyeiydmf.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gekymwgtf.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/glxlpxslg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gevjjonfk.sHtML

Go:   time.Now()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghongawbk.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/gjxjspffd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/glccohjzm.sHtML

[J02] 格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gjtnopkge.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.yfazqb.com/Article/details/gdknnehni.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gjfgpdugy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.vehdjk.com/Article/details/gfphkwhpb.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/gyabhpjsz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gnaavfafe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.yfazqb.com/Article/details/gotruxdly.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gxkzvqtnk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.yfazqb.com/Article/details/gaomjljzi.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fktsv.cn/Article/details/gxhvqhdbg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/gkcxdxkfw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/gtsrcdeeo.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gwurdqfnj.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gnduzshro.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gnennfzxg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gweffthyy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gnfifeiwu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.vehdjk.com/Article/details/gcbwzdgwa.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gqpoespat.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.vehdjk.com/Article/details/glqtldprp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.sjlbkw.cn/Article/details/gpslazskg.sHtML


<!-- 参考信息 -->