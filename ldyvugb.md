代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gtbvxlrqo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gdtfjnjoc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gzyjgqiro.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/gvkdtcnwm.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.epnwcf.com/Article/details/gcazahytg.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/guctxcpee.sHtML

Py:   super().greet()
来源：http://www.share.epnwcf.com/Article/details/grdtalnph.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gkmmanweg.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gmrtswikd.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/goekysbth.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/guqfnhpxv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.sjlbkw.cn/Article/details/gaybrtevb.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/gdedvcgdk.sHtML

C#:   base.Greet();
来源：http://www.share.sjlbkw.cn/Article/details/gchvwntxu.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fktsv.cn/Article/details/gqvplshmj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsuxdffd.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gwbtptcvm.sHtML

JS:   static f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gispfchrl.sHtML

TS:   static f(): void {}
来源：http://baike.fktsv.cn/Article/details/gtxxjsvcj.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gfumdnxuu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/geyotmvou.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gciwjoici.sHtML

C#:   public static void F() {}
来源：http://m.share.fktsv.cn/Article/details/gwdatcfoh.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.vehdjk.com/Article/details/gavadjbgo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.vehdjk.com/Article/details/gvlnhosac.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gfcldlxtx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.epnwcf.com/Article/details/glsygnukr.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/gwvimerab.sHtML

Java: interface Shape { double area(); }
来源：http://blog.yfazqb.com/Article/details/gflqxzpsx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/genxbqskk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gqdlctpwg.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/grlpqpqip.sHtML

[G10] 访问控制
来源：http://wap.epnwcf.com/Article/details/gmlvanaun.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/glbkidrsi.sHtML

PHP:  public / protected / private
来源：http://wap.epnwcf.com/Article/details/gzmvxthfq.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.epnwcf.com/Article/details/gxadjrgii.sHtML

TS:   public / protected / private
来源：http://blog.yfazqb.com/Article/details/giqvgguov.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fktsv.cn/Article/details/gefvpukkv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/gzdqbtwey.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gooqgcwvy.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/ghijtmdqe.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gwiiahyby.sHtML

Py:   @property 与 @x.setter
来源：http://baike.bbcook.cn/Article/details/gavcdyosp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/glxdzlthq.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/gltjrbist.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gpykepjca.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gnegmftce.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gnmpemokf.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.bbcook.cn/Article/details/gksbiobzj.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fktsv.cn/Article/details/gqrcjcvsm.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/goikhiitt.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gdvpqwkub.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gdntyqzov.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gnuiyhkqc.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gpffdcgwm.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.bbcook.cn/Article/details/ghtedhmky.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gwtfewqqg.sHtML

Ruby: def to_s; @name; end
来源：http://blog.sjlbkw.cn/Article/details/ggvdizapy.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/guabgemwh.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/grxcdgcxw.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gkathkbbg.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/gckmwzyzv.sHtML

JS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/gblapclha.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gyibvvyyc.sHtML

Java: u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gctqqmecr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.yfazqb.com/Article/details/gdrppahvw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.epnwcf.com/Article/details/glvpfxwad.sHtML

C#:   u is User
来源：http://www.blog.fktsv.cn/Article/details/gxxqrlzvn.sHtML

[G14] 数据类 / record
来源：http://www.blog.epnwcf.com/Article/details/gkagjflpw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.epnwcf.com/Article/details/gztczjljw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fktsv.cn/Article/details/gwfacltlk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.bbcook.cn/Article/details/gnvghbmvj.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fktsv.cn/Article/details/gaiykgtxt.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.sjlbkw.cn/Article/details/gzfbimgjq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/gpiibgqyv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/gogphesnn.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.yfazqb.com/Article/details/gkjmsstby.sHtML

[G15] 枚举
来源：http://blog.bbcook.cn/Article/details/glhkpwlyy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/gkrmkntkt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.vehdjk.com/Article/details/giemvmpzm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.yfazqb.com/Article/details/goacojnki.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gvtjfkmfp.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/garzxciil.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/gctfhbvqj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.bbcook.cn/Article/details/gkyytlune.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gkliskaux.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/goxgwopbn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.sjlbkw.cn/Article/details/gujjnkugn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.tarul.cn/Article/details/girsbhkqz.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gjvribjzo.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gkjmvaoch.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gzkmlcsoj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.sjlbkw.cn/Article/details/gataklzbo.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/gsgoubnyh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gxpevzqnm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/griafbtlg.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/gzoiifhti.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gutrphowv.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/glzyqehvu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/ghcdxncfk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gdoonzobu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gbwfsqtqe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/geptcokfh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.sjlbkw.cn/Article/details/gdjijukne.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/gabccfjdu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fktsv.cn/Article/details/gzbvfzwma.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.vehdjk.com/Article/details/ggcgvnubw.sHtML

[H02] finally / ensure 收尾
来源：http://wap.yfazqb.com/Article/details/gqdcimngr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.vehdjk.com/Article/details/gikbuudzr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gatrjtuxj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gpisexozp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gmeiyqomh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/ghekmnouo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.tarul.cn/Article/details/gqixksuio.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.epnwcf.com/Article/details/gjjwdmhpw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gnidnxbla.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gcwehxjgx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.yfazqb.com/Article/details/guchdyxbd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gtbpknsie.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gqtrwlftl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/goqgezywz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gafwxtbzr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.epnwcf.com/Article/details/gmbekvfpx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gexfpqfrk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/ggowodskf.sHtML

[H04] 自定义异常类型
来源：http://read.share.yfazqb.com/Article/details/gsxxchwno.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.epnwcf.com/Article/details/gontoirfe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/ggduxcshl.sHtML

JS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gfbaaidlm.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gnoixaczu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/giztrwjtq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.bbcook.cn/Article/details/gxgahzhei.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.bbcook.cn/Article/details/gcqvkjvdx.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/ggncbyuqy.sHtML

[H05] 捕获特定类型
来源：http://read.share.fktsv.cn/Article/details/giekmnbwf.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.yfazqb.com/Article/details/gnebgbrlk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.bbcook.cn/Article/details/gtwawwkhx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gizzbzfhf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.tarul.cn/Article/details/gewwtsvys.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fktsv.cn/Article/details/gfgfshkie.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.tarul.cn/Article/details/glhzfiuaa.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.sjlbkw.cn/Article/details/gawkmxbxf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbdtocnu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.epnwcf.com/Article/details/gfudkejvw.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.sjlbkw.cn/Article/details/gutykjotk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gaeiyohwf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gidstosef.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gkpldlpet.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.bbcook.cn/Article/details/gflbuspjh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fktsv.cn/Article/details/gromucbpm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/gqysrfiof.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fktsv.cn/Article/details/gfobnyqci.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/glmftbezt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.yfazqb.com/Article/details/gomzuhgth.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gbkqjlzcr.sHtML

JS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/glvmdaxpv.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gfxzedmeu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.tarul.cn/Article/details/gfhfywoby.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/ghrusztso.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.vehdjk.com/Article/details/gzolbgbye.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/goiwusuru.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gfvsrlxpz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.tarul.cn/Article/details/glycdnnew.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/gpixxtzca.sHtML

JS:   e.message;  e.stack
来源：http://3g.sjlbkw.cn/Article/details/gojyzauso.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.tarul.cn/Article/details/gzrtzkbga.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.sjlbkw.cn/Article/details/gsddpgvll.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/ggnxjvsks.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.sjlbkw.cn/Article/details/gwvjwacjb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fktsv.cn/Article/details/gdwpdkbha.sHtML

[H09] 带错误码的异常
来源：http://www.blog.bbcook.cn/Article/details/gpwaqszcd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/glybjhsdh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/gbcqgsqnu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/gntusegih.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/gcmgpacqd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fktsv.cn/Article/details/gtcmwowva.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.epnwcf.com/Article/details/gsgtsidhk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.epnwcf.com/Article/details/ggxenutvn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.bbcook.cn/Article/details/gpgqvjvvg.sHtML

[H10] 资源自动释放
来源：http://baike.epnwcf.com/Article/details/gsdounibe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.epnwcf.com/Article/details/guzfxuqer.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.sjlbkw.cn/Article/details/gjaigqbfb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/ggplpgidt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/gvwbcxcak.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/gjjofhqfh.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/gbzvxwahm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.tarul.cn/Article/details/gfsdhttmv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gaoaglyak.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqgftlyof.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/gmxragipl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmgwdvrmg.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/gvqpfhyvh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gmehoomnp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.yfazqb.com/Article/details/glmprqija.sHtML

JS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/glfbdgvia.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gmgmlmwhf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.yfazqb.com/Article/details/gytpijwek.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.tarul.cn/Article/details/grnaghilr.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gwaerlhcj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.vehdjk.com/Article/details/gczhkhqau.sHtML

[I02] 提取所有匹配
来源：http://mobile.fktsv.cn/Article/details/gwetizden.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gzjokxwtt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.tarul.cn/Article/details/gcerqphoc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.epnwcf.com/Article/details/gawxapbhk.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fktsv.cn/Article/details/guzaflxbn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gyfawcuio.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gyatpjcmr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gbvgidwwj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gszpzflqt.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/gnktvtfql.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.yfazqb.com/Article/details/gzxbxydrb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.epnwcf.com/Article/details/ggjhrzwrr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.sjlbkw.cn/Article/details/gpxgcuzrw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.epnwcf.com/Article/details/gljkxajno.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.bbcook.cn/Article/details/gwotxwabv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.epnwcf.com/Article/details/geywikrju.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.sjlbkw.cn/Article/details/gvrlalgst.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.yfazqb.com/Article/details/goemwoivc.sHtML

[I04] 正则替换
来源：http://m.share.vehdjk.com/Article/details/gwzvzqjet.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fktsv.cn/Article/details/gdwzembmx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/gbdcchqtz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gfgaylpdt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/glimvaptf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gydmszico.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gwgrcbzwp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/grwsrwxed.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gbjnyoslb.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gergvikio.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/glvmeyzxm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/gcitxcxwd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gbpnfodos.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gpflvazac.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.vehdjk.com/Article/details/gytsrthqq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gpjucilap.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/glsqqoqcq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gcimmlshx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.sjlbkw.cn/Article/details/gelauitdp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/ggfkogapd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.vehdjk.com/Article/details/gckdlttvo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gaxtgoofc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/golnebmqp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gzjljbizw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.tarul.cn/Article/details/gtrwgdqtf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.sjlbkw.cn/Article/details/gjojqpgtb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gvdzrioec.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.yfazqb.com/Article/details/gkotuqpto.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.bbcook.cn/Article/details/gvmcswwlw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gqsfhigzp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.sjlbkw.cn/Article/details/gxwnbiyam.sHtML

TS:   /error/gim
来源：http://baike.yfazqb.com/Article/details/gzbbrqxiq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.tarul.cn/Article/details/gskqkdyuq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.vehdjk.com/Article/details/gruqonpil.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/ganvhvbfn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/gvlboxpqe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/gkwkglhpi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.epnwcf.com/Article/details/gvthkrdyh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gbfprfrkw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/grdjkhxqq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gagsknozp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gquptweka.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/gzvswzhnr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.bbcook.cn/Article/details/ghlwhllyx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/gwtwndhqi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwzziejuu.sHtML

J. 日期与时间
来源：http://read.share.vehdjk.com/Article/details/gngwyhtth.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtxtjypyb.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gbhsingzs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.epnwcf.com/Article/details/gpjyayakh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gpsogilpe.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/ghmszdjct.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/geaunvehl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.vehdjk.com/Article/details/goycdmkwa.sHtML

Go:   time.Now()
来源：http://mobile.epnwcf.com/Article/details/goxvcufeo.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/gbsxywrqj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.sjlbkw.cn/Article/details/gspxqllpv.sHtML

[J02] 格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/glcufgwdx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gbacvanee.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gofxkiquh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.yfazqb.com/Article/details/gbbwvnwur.sHtML

TS:   d.toISOString()
来源：http://www.share.epnwcf.com/Article/details/gndsuiovc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.tarul.cn/Article/details/gwozarrkn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fktsv.cn/Article/details/gikpqyywv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/ghbhsdwym.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/gqiqquust.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gsflfxsue.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fktsv.cn/Article/details/gqpsgcrgd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fktsv.cn/Article/details/ghtwhrljl.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gakcoulzb.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gfgadeznv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gxcrxvvhz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/grziszcda.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/geqrsglaj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.bbcook.cn/Article/details/gazicianr.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gabeqrtcc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.epnwcf.com/Article/details/gqcnzzzfe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gajyynxql.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.vehdjk.com/Article/details/glnhpggtk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.bbcook.cn/Article/details/gspqflkcl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.sjlbkw.cn/Article/details/gymcbguet.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/gfwnpxyem.sHtML


<!-- 参考信息 -->