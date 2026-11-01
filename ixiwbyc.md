代发 wailian999

[G02] 构造函数
来源：http://baike.yfazqb.com/Article/details/gywvjnddw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gsirxwmmk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/gzuhkfibx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gvoicuhjr.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gzsygxjac.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gbnrdhggg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.tarul.cn/Article/details/gffiggwdh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/gsnamnaqj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/grvbxwekb.sHtML

[G03] 实例属性
来源：http://wap.vehdjk.com/Article/details/gjlcphzso.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/gkolcdpzb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gsxtfenxw.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gqpyqajso.sHtML

TS:   name: string = "x";
来源：http://www.share.epnwcf.com/Article/details/ggjauifle.sHtML

Java: private String name;
来源：http://mobile.fktsv.cn/Article/details/gkrfsedva.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/gibgnjnrj.sHtML

Ruby: @name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gunkztnmc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.tarul.cn/Article/details/gguscwfhc.sHtML

[G04] 定义方法
来源：http://mobile.vehdjk.com/Article/details/gbljthfvw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gbkbzxqpt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/ghmsekqrt.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/ghlkhimnm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gpeblgqiw.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gmpafdjkb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gplpipxnp.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/ggwyesysp.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/gshgmyndn.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gpxtysxwc.sHtML

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/gawjfphvq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gnutxeier.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gcwymkyrd.sHtML

TS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gbprhjyjb.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gqinboisy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.yfazqb.com/Article/details/gsrjvbfdr.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/gocitvyao.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/gbbzwpjen.sHtML

[G06] 重写方法
来源：http://blog.bbcook.cn/Article/details/gfakctoip.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/gksdliuku.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gtbdpzcel.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gorztoagu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gpyvzitjy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gtttxlbmp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.vehdjk.com/Article/details/gbuuzaihy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnmbhvkg.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/ghqgebgno.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gpflffbab.sHtML

Py:   super().greet()
来源：http://blog.epnwcf.com/Article/details/gvebjfxsa.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/gebqberoa.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gsmfhvtmt.sHtML

TS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gbdahcsyj.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/grrguczwl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.sjlbkw.cn/Article/details/gfldgplwx.sHtML

Ruby: super
来源：http://read.share.fktsv.cn/Article/details/gykgajsph.sHtML

C#:   base.Greet();
来源：http://www.share.vehdjk.com/Article/details/gwnbfbffc.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/geqwtssfn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.sjlbkw.cn/Article/details/geyllivgh.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/gueotoclm.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gdhgjvocy.sHtML

TS:   static f(): void {}
来源：http://www.share.epnwcf.com/Article/details/ghlmsxvvv.sHtML

Java: static void f() {}
来源：http://wap.fktsv.cn/Article/details/gtdrzuiil.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fktsv.cn/Article/details/gpnfagpby.sHtML

Ruby: def self.f; end
来源：http://baike.fktsv.cn/Article/details/grmwewgnx.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/gtjevxtjr.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gdqbjsvgm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/gvadhszop.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gnhdtyveg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.epnwcf.com/Article/details/gsrwfkuan.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.yfazqb.com/Article/details/gvrujivky.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gcnuubsts.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/grxwlekng.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.bbcook.cn/Article/details/gosxwoppv.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/glxrifiew.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/gztdyqeaa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/gqvsyrohn.sHtML

PHP:  public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/geiuhhpdc.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.epnwcf.com/Article/details/gynaegyyy.sHtML

TS:   public / protected / private
来源：http://wap.bbcook.cn/Article/details/gxgvsrilx.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.bbcook.cn/Article/details/gkmlpkcde.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fktsv.cn/Article/details/ghmvktxzy.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/gbmkbwvws.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fktsv.cn/Article/details/gqlnbbltl.sHtML

[G11] getter / setter
来源：http://mobile.epnwcf.com/Article/details/gfqdgpfag.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/gmqgiyjge.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gvciavpvz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/gnwmrzprz.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gnqnleptx.sHtML

Java: public String getName() { return name; }
来源：http://wap.epnwcf.com/Article/details/geuxytizw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gmdtahzyb.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fktsv.cn/Article/details/gstguuqxa.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/gsowtlvkz.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gxwbgqfrf.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gsfefblng.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gfkneyihj.sHtML

JS:   toString() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gxsgrrwgr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/ggoktrvde.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gauogauph.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gmiepuwnz.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/gaufxlecb.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.vehdjk.com/Article/details/gqiwnfsek.sHtML

[G13] 判断对象类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gkreqfvsu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.yfazqb.com/Article/details/gjmrwakbg.sHtML

PHP:  $u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gguquutdo.sHtML

JS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gcqufamcs.sHtML

TS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gfhfewhbk.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gvlibluwc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.bbcook.cn/Article/details/grtlnnsxk.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.bbcook.cn/Article/details/gebtwifvn.sHtML

C#:   u is User
来源：http://wap.sjlbkw.cn/Article/details/gpylpvsey.sHtML

[G14] 数据类 / record
来源：http://blog.epnwcf.com/Article/details/gafhezxcf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.bbcook.cn/Article/details/gwtxiwkhc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.epnwcf.com/Article/details/gyarmjzzs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fktsv.cn/Article/details/gtulupyfy.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fktsv.cn/Article/details/gxwjymhoo.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.epnwcf.com/Article/details/gpdfuitlp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.yfazqb.com/Article/details/gwnrgtzhm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/gzlesvcrt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/gfckmxxsl.sHtML

[G15] 枚举
来源：http://m.share.bbcook.cn/Article/details/gpmowjhmu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fktsv.cn/Article/details/gsfqrukaq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/ghawunlqt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gnzdfujda.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gukeqbgdn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gcfphcmus.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.vehdjk.com/Article/details/gcucajwlu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.vehdjk.com/Article/details/giowzecco.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gambsxokf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/gsbyorawn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.vehdjk.com/Article/details/gfqunoecx.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.sjlbkw.cn/Article/details/gqtyjmvvo.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gvteftryg.sHtML

TS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/gmkmscthp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fktsv.cn/Article/details/gxlglwpmn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.vehdjk.com/Article/details/gkkbcfdba.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/grfouwxep.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/ggvcwlhhl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtxaoiopv.sHtML

H. 异常与错误处理
来源：http://wap.fktsv.cn/Article/details/gbacaxnqh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnaoltwho.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gudhmrjny.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gyvbraorq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.bbcook.cn/Article/details/gockuhwyk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gzlvftowk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gwzshkfcn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gaeacggec.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.vehdjk.com/Article/details/gduxkpafs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gcadafzdb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gnnrtsggm.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fktsv.cn/Article/details/gtbqxehgh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.epnwcf.com/Article/details/grwkkwjia.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gqxgjghww.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/ghjbajbaw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gqyveooal.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gpenfqbjo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.epnwcf.com/Article/details/gzkgubhoi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.sjlbkw.cn/Article/details/guedyrqet.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gndzwbgkt.sHtML

[H03] 主动抛出异常
来源：http://mobile.sjlbkw.cn/Article/details/gqvptfshg.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/gzyotothl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gfsbnkssc.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gidqtxomy.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gcsasdkgx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gbmuvhyal.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.vehdjk.com/Article/details/gwffrmedu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.tarul.cn/Article/details/gspahremh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gaylzakfw.sHtML

[H04] 自定义异常类型
来源：http://m.share.fktsv.cn/Article/details/gwqwguigi.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.tarul.cn/Article/details/gznaxevps.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gommydmnf.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/gemrlcjrb.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gtuxabrch.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/ggdsgnfqv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/gxocojpxk.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.epnwcf.com/Article/details/gglkvmnrp.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.epnwcf.com/Article/details/gbindhttg.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/gjunrctsw.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fktsv.cn/Article/details/gsintaciv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fktsv.cn/Article/details/gwjwrtzsm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gmswrcxfr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gcmbtyusd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/gvggkjrtx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gwurkfekf.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.yfazqb.com/Article/details/gguxjhavb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/gxqpiisen.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/gltdaooyg.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/gkhpylyqs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gpapivjnc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gbfpnrciw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gqnnmvknl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.epnwcf.com/Article/details/gssnenwsi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/gzzoyuyfw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.vehdjk.com/Article/details/ghquhmone.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.bbcook.cn/Article/details/gjtdviehl.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gkwgebeep.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.yfazqb.com/Article/details/gdsqwoelt.sHtML

PHP:  assert($x > 0);
来源：http://3g.tarul.cn/Article/details/gpaibmqss.sHtML

JS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gheqtdvcb.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/grgwdbufa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/gmzaayfwc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.tarul.cn/Article/details/gmpsfrvfv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/gkvleazwe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gjxoozgfx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.bbcook.cn/Article/details/gwhrnjgrh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/gsfokcjga.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnytafgux.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/gftxbniss.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/gevqdvmby.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.tarul.cn/Article/details/grvkheeub.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gabqnkuly.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.sjlbkw.cn/Article/details/ghkgbkekq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fktsv.cn/Article/details/gwrhrhpnr.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gismbjyvf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/gwedzznej.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/girapnuma.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fktsv.cn/Article/details/gcqxwkpix.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.yfazqb.com/Article/details/gimanwoaf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gwhvfxbhh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.yfazqb.com/Article/details/gkwriqiew.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.bbcook.cn/Article/details/gsnzjljsn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fktsv.cn/Article/details/gjswfiykp.sHtML

[H10] 资源自动释放
来源：http://m.share.bbcook.cn/Article/details/gjtoleghk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.yfazqb.com/Article/details/gjcllzeet.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/gtvuzuewd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/gmublxrkh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.tarul.cn/Article/details/gqkcjigln.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhnwsgda.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gknrvsegq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.epnwcf.com/Article/details/gvbmalvvu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gmksrmxsb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdasyxhgi.sHtML

I. 正则表达式
来源：http://www.blog.bbcook.cn/Article/details/gcbfzxqmh.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ggdgqlmtt.sHtML

[I01] 判断是否匹配
来源：http://m.share.sjlbkw.cn/Article/details/gvzpaghci.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/grzpfdrii.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gdzficrfb.sHtML

JS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gurkbvwnt.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gwnynosdz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.vehdjk.com/Article/details/gbllgikjs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gqvioydtf.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/ghwafdsej.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.tarul.cn/Article/details/gvlngqtkm.sHtML

[I02] 提取所有匹配
来源：http://read.share.epnwcf.com/Article/details/gyedqgyzq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gionetvlm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.vehdjk.com/Article/details/gvrzkfolz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.vehdjk.com/Article/details/gdijbqexo.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/gdrannueo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.yfazqb.com/Article/details/ggdxlgfun.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/guhlhvmbi.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gpemjlwfu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/ggtlqtxbs.sHtML

[I03] 提取捕获分组
来源：http://wap.vehdjk.com/Article/details/gpcmlzlnb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.tarul.cn/Article/details/gykmcnrsl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gepazgthn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.sjlbkw.cn/Article/details/gawrjstpv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.epnwcf.com/Article/details/gqqgsjswu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fktsv.cn/Article/details/gyefqxjii.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.epnwcf.com/Article/details/gsspcnfxg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.epnwcf.com/Article/details/gjcmghpno.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.sjlbkw.cn/Article/details/gpsrvcljn.sHtML

[I04] 正则替换
来源：http://blog.tarul.cn/Article/details/glbqcqyag.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.vehdjk.com/Article/details/gxjohknaw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/gxqeeccsd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gcyyxlvcy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gjtayfotf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gkgvuyydp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.tarul.cn/Article/details/galkxdwgy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gzlwbkpze.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/guhlkowsj.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/glqvhiorp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fktsv.cn/Article/details/gjsutqvjx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.yfazqb.com/Article/details/gxoblrawn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcogibol.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gftnjpqyp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gfazowmug.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.tarul.cn/Article/details/gnelingub.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gjaihgdxu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gvzmsaayc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.sjlbkw.cn/Article/details/gfnlqyond.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gyddewdwd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.bbcook.cn/Article/details/gyccisbbs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gesuwuvhn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gbzlspxrn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.tarul.cn/Article/details/grpfjbudz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fktsv.cn/Article/details/guskpqpxp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fktsv.cn/Article/details/gmcmpahuk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gqqmhprle.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.bbcook.cn/Article/details/gtildxkac.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.epnwcf.com/Article/details/gqjylpffp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gqnprvlhx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.yfazqb.com/Article/details/gnznsfqeu.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/gdknpeolx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.yfazqb.com/Article/details/gtwtvmpos.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.tarul.cn/Article/details/gjhawtaed.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.bbcook.cn/Article/details/gdtiklvia.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fktsv.cn/Article/details/gnjqqvsfh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gwibkekkx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.yfazqb.com/Article/details/gjestprix.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gnnoeipea.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gwgpjccvn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gugnaaemz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/glgzsvsrf.sHtML


<!-- 参考信息 -->