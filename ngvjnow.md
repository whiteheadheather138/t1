代发 wailian999

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/gnzidgcgd.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/gizlnpdjh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gomyjucnu.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gdorcpojt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gvbzptnci.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/giyykkgkr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fktsv.cn/Article/details/geamedozl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.tarul.cn/Article/details/gchdiszjm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.bbcook.cn/Article/details/gpvvnrgbx.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/gxpcvmvib.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/guppnuseb.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/grlycihbo.sHtML

JS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gsuuibsfj.sHtML

TS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gsxfinkbi.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/geevhtetj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.yfazqb.com/Article/details/gcrdcsejp.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gobbcqpmy.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gmiweweqf.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gxohfluvc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.vehdjk.com/Article/details/gzldcoutt.sHtML

PHP:  public static function f() {}
来源：http://m.share.yfazqb.com/Article/details/gtutumqxt.sHtML

JS:   static f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gsafajcxi.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/gadxbhala.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/gxzoxmlme.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.vehdjk.com/Article/details/gcbfdwylh.sHtML

Ruby: def self.f; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gptcpuwvm.sHtML

C#:   public static void F() {}
来源：http://www.blog.yfazqb.com/Article/details/gjyheemtg.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.vehdjk.com/Article/details/gkiiainjw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.sjlbkw.cn/Article/details/gmaabfbko.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/gttqezmyt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.tarul.cn/Article/details/gdodobgbu.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/gsgtnkuhm.sHtML

Java: interface Shape { double area(); }
来源：http://blog.tarul.cn/Article/details/gtyiucfdz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.yfazqb.com/Article/details/gqqyiseli.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.yfazqb.com/Article/details/gkzumuimg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.sjlbkw.cn/Article/details/gxrdzvdpt.sHtML

[G10] 访问控制
来源：http://read.share.bbcook.cn/Article/details/gmnxzlgsi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.yfazqb.com/Article/details/gvyhzkujm.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gxoshkjbb.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gdqffozrb.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gnvskdxlg.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.epnwcf.com/Article/details/gdelqyvmt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fktsv.cn/Article/details/gpjlqsycx.sHtML

Ruby: public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gycdgonhv.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/gjzgrfhuh.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gqkptyuqy.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.epnwcf.com/Article/details/gllenomsn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gvssmaaht.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gzqxacmjz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/gczqcoxdk.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gdzymawnz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gvygtnqju.sHtML

Ruby: attr_accessor :name
来源：http://wap.epnwcf.com/Article/details/gczkgvhvt.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.sjlbkw.cn/Article/details/gsmwmrrtd.sHtML

[G12] 对象转字符串
来源：http://www.share.bbcook.cn/Article/details/geqhlodqk.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gxdkckuad.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gnqevptsl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/grsbekqhe.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gqhriqjjy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gsbtzelrm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/glsowuyyu.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gklfarhbe.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.epnwcf.com/Article/details/gnojazsem.sHtML

[G13] 判断对象类型
来源：http://read.share.epnwcf.com/Article/details/gajcojdbv.sHtML

Py:   isinstance(u, User)
来源：http://wap.fktsv.cn/Article/details/gmqizzjmx.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gvltgoiuu.sHtML

JS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/glekuacnt.sHtML

TS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gsgdmxszi.sHtML

Java: u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gnhgqxwwu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.vehdjk.com/Article/details/gwvkbjapf.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/gajdgziae.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/gzwpmlgpe.sHtML

[G14] 数据类 / record
来源：http://www.blog.bbcook.cn/Article/details/gkiafvoje.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/gnohnpgpc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.epnwcf.com/Article/details/gbfgqeuii.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/ggxudwlbt.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/ghxxbyyki.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/gdeaakbon.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.vehdjk.com/Article/details/ghnqmviwp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.epnwcf.com/Article/details/gbukhegvn.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gfigbxoyu.sHtML

[G15] 枚举
来源：http://mobile.bbcook.cn/Article/details/gvkkpavmj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.bbcook.cn/Article/details/ghhyoipky.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.yfazqb.com/Article/details/gcmdgtxjg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.sjlbkw.cn/Article/details/gsijknzyk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/ggfczjohc.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.vehdjk.com/Article/details/gntvvgafm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/ggyjqlwhe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/gcteydyls.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gmzphjluc.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.bbcook.cn/Article/details/ghacuvsai.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/gcbwdsijr.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/giribbzoi.sHtML

JS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gtfogvbtc.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gcdkhfsxs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/guuumlqxf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/gxbvvlxft.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.yfazqb.com/Article/details/gbkdpwyvc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/gklaefsme.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjldoefrx.sHtML

H. 异常与错误处理
来源：http://mobile.tarul.cn/Article/details/ghnbwrnaz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwzhakfla.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gbxomjkbu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.sjlbkw.cn/Article/details/gvggglzny.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.sjlbkw.cn/Article/details/gcinxrpab.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gycofvywu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gmvjvlkpl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gojbzqzco.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/gwyattiad.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.yfazqb.com/Article/details/gbjvzyjtt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fktsv.cn/Article/details/gbiuvowxj.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.sjlbkw.cn/Article/details/guiktdagv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/ggpbyijax.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gvxwuckfz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/grohnjfls.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gxkksggin.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gfqowomlx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fktsv.cn/Article/details/gyxrqxnmy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fktsv.cn/Article/details/gjbxzpvju.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gjxwmsehp.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/gqzmlqcuc.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.sjlbkw.cn/Article/details/ggjoninah.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/grzfsmgmp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gahfqtxuy.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/ggfqmncja.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gbczcixoi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.tarul.cn/Article/details/gxmxluoja.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.sjlbkw.cn/Article/details/gpwjfvisv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/ggfxfowjv.sHtML

[H04] 自定义异常类型
来源：http://read.share.tarul.cn/Article/details/gudocnlxt.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/giobcmsqv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/geoydwsau.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gdvwcoynk.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gcijkdgqb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gycddamir.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/gnxkmqvbr.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.vehdjk.com/Article/details/gigrpbabf.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/gdovewavv.sHtML

[H05] 捕获特定类型
来源：http://blog.tarul.cn/Article/details/gfcsqjlhw.sHtML

Py:   except ValueError as e:
来源：http://m.share.vehdjk.com/Article/details/gtdysogjh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.tarul.cn/Article/details/gavirbbal.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gwvdxyqxu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gvpvkglor.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.bbcook.cn/Article/details/gwrypoxxe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gkqszjwxg.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.yfazqb.com/Article/details/gauavjrsc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.sjlbkw.cn/Article/details/gmtgsfoop.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.bbcook.cn/Article/details/gsfqnjbhe.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.vehdjk.com/Article/details/gsblhcjiq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gkvqrahnq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/ggjlchyvn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gkzaomotx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.tarul.cn/Article/details/gtqszeehg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.tarul.cn/Article/details/geilfzysa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.epnwcf.com/Article/details/gbibiehqv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gqgakrxtp.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/guevrrjta.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.yfazqb.com/Article/details/gkjrkdmsv.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gypbniyij.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/ghxeygpzt.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gfcgfxdsi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.yfazqb.com/Article/details/gdjfndkfc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.sjlbkw.cn/Article/details/gbkjmncpv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/goaechdeo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gqybguljh.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gbdoscbas.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.epnwcf.com/Article/details/gtpopnsay.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.vehdjk.com/Article/details/ghndjqbri.sHtML

JS:   e.message;  e.stack
来源：http://m.share.tarul.cn/Article/details/gruxckgki.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gpbzvgcvz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/ghztsatlt.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gicksclww.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.yfazqb.com/Article/details/gzugzxjyd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/gxghwbuiq.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/goalejpkd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.vehdjk.com/Article/details/gmwgcshqj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gpgedinaj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.tarul.cn/Article/details/gncyblvbi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.vehdjk.com/Article/details/gxqcrllhr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.vehdjk.com/Article/details/gkuovxvwq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.bbcook.cn/Article/details/grtrnxkvk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.yfazqb.com/Article/details/gqahtxqkx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/gkalekkou.sHtML

[H10] 资源自动释放
来源：http://m.share.tarul.cn/Article/details/gpwascruu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gdpkbucsz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fktsv.cn/Article/details/gpziuhcca.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/gazmnniin.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gsaomxsue.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gmaixywoc.sHtML

Go:   defer f.Close()
来源：http://www.blog.vehdjk.com/Article/details/gmhjiegxb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/gdbaqngys.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/grjucgcnf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gquavvlmz.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/gkogzhoea.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gyiekxlyd.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.vehdjk.com/Article/details/gwawgzcwm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gzzmpxngl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gjuzdgsuh.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gkbbwnmwm.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gvspqedkt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.yfazqb.com/Article/details/gbefmoamd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/gbtkqdjgm.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gajftguld.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gaxvncxxz.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.vehdjk.com/Article/details/gcmfgkmtt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gqhfmrred.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/gismrjcnf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fktsv.cn/Article/details/gqhdrlhkq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.bbcook.cn/Article/details/gqzacbjdv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/gfqxaqxoo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gmyqghstk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/gndpapqdl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/gqzsewxkm.sHtML

[I03] 提取捕获分组
来源：http://wap.bbcook.cn/Article/details/gjakgpjqo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/gcasveytg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gdfduplpa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gqscimkpu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.vehdjk.com/Article/details/gqhevmiqp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.yfazqb.com/Article/details/gevenuzxq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.bbcook.cn/Article/details/ghzkbpkpl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/gqtalasbe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/gzlipjoad.sHtML

[I04] 正则替换
来源：http://3g.tarul.cn/Article/details/gwwprdsam.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fktsv.cn/Article/details/geelowdde.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/ghdqhtbvq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/ghqnzzunq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gtbsozdoh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gkqzophkn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.yfazqb.com/Article/details/gxzkobkos.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/gjzacrarb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.bbcook.cn/Article/details/grnbnccly.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/grrhvvunt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gglzagsur.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/gfxneqglc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gtpsgxyun.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gsnyjogbh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.vehdjk.com/Article/details/gbduxjljm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gvsuopzvo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gwmcxwqni.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gloctoeng.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.epnwcf.com/Article/details/gytyrmrze.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gxgoxnsjz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.vehdjk.com/Article/details/gcjhwqniz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.tarul.cn/Article/details/gcamcwiyn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/glabsxefw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gspczcdti.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.bbcook.cn/Article/details/glwbvkxln.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.tarul.cn/Article/details/gublbukps.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/ghqqjupkm.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.tarul.cn/Article/details/ggxilzlqp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.bbcook.cn/Article/details/gswyrfyoq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gdnbgqebl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.tarul.cn/Article/details/gplqmrllt.sHtML

TS:   /error/gim
来源：http://m.share.tarul.cn/Article/details/grsmeytoh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.bbcook.cn/Article/details/gfmdnqhfh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/gqdctjdjd.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/gadxlkkfw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.bbcook.cn/Article/details/gbwkuaogm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.vehdjk.com/Article/details/guqzobrfd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.bbcook.cn/Article/details/gxzzfmqod.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fktsv.cn/Article/details/guygcnngh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/godozvjin.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/geexivvfb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gtghqufho.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.bbcook.cn/Article/details/gzplshiep.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.tarul.cn/Article/details/giutkmvlf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/gvgscvfgm.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbbiumcgq.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gsjmbpmbi.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzicacmou.sHtML

[J01] 获取当前时间
来源：http://www.share.vehdjk.com/Article/details/gxpgrzdsi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gfqivtdlq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gcgfaqnwe.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gkscmcnuu.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/ghikyeugr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.vehdjk.com/Article/details/gpfudzqbk.sHtML

Go:   time.Now()
来源：http://www.m.share.epnwcf.com/Article/details/gajweeuum.sHtML

Ruby: Time.now
来源：http://mobile.bbcook.cn/Article/details/gorfaggsf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.bbcook.cn/Article/details/ggivgmbhg.sHtML

[J02] 格式化输出
来源：http://baike.epnwcf.com/Article/details/gdjyplbxq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/grlzqbiqh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gvlmbzgtj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.vehdjk.com/Article/details/gmsendste.sHtML

TS:   d.toISOString()
来源：http://m.share.vehdjk.com/Article/details/gmdrswqzm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.sjlbkw.cn/Article/details/githbibwu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.sjlbkw.cn/Article/details/gpkhvkvae.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/ggsbkfdzh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.epnwcf.com/Article/details/gdioylpje.sHtML

[J03] 字符串解析为日期
来源：http://3g.tarul.cn/Article/details/ghctvmwbm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.vehdjk.com/Article/details/gtmdnwktp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.vehdjk.com/Article/details/gfoqctouk.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/ghqcopmer.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/geguizzej.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gcupasvqr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gburppwej.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gfusygahw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.sjlbkw.cn/Article/details/gjemnrxko.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/gwqvncwbj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/gcfwpzzyw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fktsv.cn/Article/details/gvjayaeqy.sHtML


<!-- 参考信息 -->