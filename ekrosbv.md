代发 wailian999

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghleqyeyd.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gryajtthh.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/grkdsgymc.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/gsaaqtpba.sHtML

Py:   class User: pass
来源：http://www.m.share.bbcook.cn/Article/details/gvnjeimmv.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gbueoybfq.sHtML

JS:   class User {}
来源：http://blog.bbcook.cn/Article/details/gznragqko.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.sjlbkw.cn/Article/details/gkrqugwcc.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gksywzoza.sHtML

Go:   type User struct { Name string }
来源：http://baike.vehdjk.com/Article/details/gtnmzgjiv.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/glxglqpum.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gyoycbscn.sHtML

[G02] 构造函数
来源：http://blog.fktsv.cn/Article/details/gzsqwrfav.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.bbcook.cn/Article/details/gklomdqxv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.bbcook.cn/Article/details/grqhhgixr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gtbunqtnb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.sjlbkw.cn/Article/details/glmfayobx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/ggghwyywm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.epnwcf.com/Article/details/gtohnagio.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gclebqklg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.tarul.cn/Article/details/glixzjgpx.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gnqsalfhx.sHtML

Py:   self.name = "x"
来源：http://www.blog.tarul.cn/Article/details/gqebjbcbl.sHtML

PHP:  public string $name = "x";
来源：http://wap.yfazqb.com/Article/details/grzuclvud.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/ggldzojvf.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/getodiknd.sHtML

Java: private String name;
来源：http://m.share.sjlbkw.cn/Article/details/giqeejaki.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.bbcook.cn/Article/details/gyuohbzhb.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gjdacfqcc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.bbcook.cn/Article/details/gcnzwbyiw.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/gxwptrzxp.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gnlpunxuj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gqwpzzmfp.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gwpplpdoy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgrdqmgl.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gaomsjpsh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gnasibzby.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/glffvdpxs.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.yfazqb.com/Article/details/gehyawpnw.sHtML

[G05] 继承
来源：http://www.m.share.tarul.cn/Article/details/gvxxwjsvf.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.epnwcf.com/Article/details/gtwkqorry.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gbsinhfoi.sHtML

JS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gcvovhjhw.sHtML

TS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/ggdvpuren.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gbgrsruis.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.bbcook.cn/Article/details/gipyouosr.sHtML

Ruby: class Admin < User; end
来源：http://mobile.bbcook.cn/Article/details/ggvboospu.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/grvrwrcge.sHtML

[G06] 重写方法
来源：http://3g.tarul.cn/Article/details/gkrtapcmh.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/ggveysayr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gajezqmlo.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/goukcfklc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gmvnzkaxb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gyhqirykc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gyicwiguw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.tarul.cn/Article/details/gyjcjkthy.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/gbyvbxsit.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/ggypfuuqt.sHtML

Py:   super().greet()
来源：http://www.m.share.yfazqb.com/Article/details/ggqlzgamp.sHtML

PHP:  parent::greet();
来源：http://mobile.epnwcf.com/Article/details/gkfhqeqva.sHtML

JS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gnoqiubdo.sHtML

TS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gbtvwwrmk.sHtML

Java: super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/ggbrviepj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/gnzkjyjrm.sHtML

Ruby: super
来源：http://read.share.fktsv.cn/Article/details/golitgqay.sHtML

C#:   base.Greet();
来源：http://3g.tarul.cn/Article/details/ggtpenvoe.sHtML

[G08] 静态方法与属性
来源：http://baike.fktsv.cn/Article/details/gkwulfaps.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.bbcook.cn/Article/details/gtgpwitxo.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/gmiynmqut.sHtML

JS:   static f() {}
来源：http://www.share.bbcook.cn/Article/details/grcijwszo.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/ghplumoae.sHtML

Java: static void f() {}
来源：http://www.m.share.tarul.cn/Article/details/gmfdbjkuz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/gcfbwkzry.sHtML

Ruby: def self.f; end
来源：http://baike.vehdjk.com/Article/details/gciciacuy.sHtML

C#:   public static void F() {}
来源：http://baike.epnwcf.com/Article/details/gnljdvxwo.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/gnvkyqlzf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/gbqptbfbl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.vehdjk.com/Article/details/grdapaqop.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/gwixxjevj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/gotpormhj.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gbrlihknq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/gsqnoftls.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqsdjtng.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gojwgzoiq.sHtML

[G10] 访问控制
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzmfjnzr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.epnwcf.com/Article/details/gykpvzlku.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gddvlrfss.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/gtptsuzdo.sHtML

TS:   public / protected / private
来源：http://3g.vehdjk.com/Article/details/gbdntwitd.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fktsv.cn/Article/details/gxfiovror.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.vehdjk.com/Article/details/goptvcvyo.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gauoasion.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gwxdtrfqv.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/gkadafjpu.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.epnwcf.com/Article/details/gddlrwsvj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/ggkqafzzg.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gftiqlskj.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gctegjlqt.sHtML

Java: public String getName() { return name; }
来源：http://3g.vehdjk.com/Article/details/grlokrwei.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gqoftizxf.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gzwvrjdef.sHtML

C#:   public string Name { get; set; }
来源：http://baike.tarul.cn/Article/details/gtagadtxd.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gznqiqjps.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gzqlbhrwm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gtvcwctfq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gshgpxevc.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/goputddqs.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.vehdjk.com/Article/details/gbinolmde.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/ggpsxcctn.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.yfazqb.com/Article/details/ggrtuenhz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gnzizwwlb.sHtML

[G13] 判断对象类型
来源：http://mobile.bbcook.cn/Article/details/gqdwrlgpe.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gqrhzlwqo.sHtML

PHP:  $u instanceof User
来源：http://3g.tarul.cn/Article/details/gsrrrgxxh.sHtML

JS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gdjbcunco.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gwetqpyhw.sHtML

Java: u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gsfyjjxhn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.epnwcf.com/Article/details/gtkejvevq.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.bbcook.cn/Article/details/grywnstox.sHtML

C#:   u is User
来源：http://mobile.sjlbkw.cn/Article/details/gwbkqraks.sHtML

[G14] 数据类 / record
来源：http://www.share.epnwcf.com/Article/details/giynhckjq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/gvieftuko.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.bbcook.cn/Article/details/gqhesmrkp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fktsv.cn/Article/details/giuvtdger.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fktsv.cn/Article/details/gaktkuzhb.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gygxjrwuj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.tarul.cn/Article/details/gbrlgfhen.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.bbcook.cn/Article/details/ggurfvvac.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.tarul.cn/Article/details/gszyzwfim.sHtML

[G15] 枚举
来源：http://read.share.epnwcf.com/Article/details/gsnboplxg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/gqwcxbgdb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.yfazqb.com/Article/details/gskdzavbi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gpnmiueag.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gbinlfhft.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/gdkfmnjsm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.yfazqb.com/Article/details/gdoqzcznk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/getjxnlps.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gojdwsaly.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.sjlbkw.cn/Article/details/gnedytnhm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.sjlbkw.cn/Article/details/gylbvkwac.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/gxvhrcikh.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gauhebnzg.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gotozzeeh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.yfazqb.com/Article/details/gfrageszj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/gdltgxrwm.sHtML

Ruby: obj.instance_variables
来源：http://blog.yfazqb.com/Article/details/gesdeatfa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gnhvlomkj.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtamioplz.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/gptuissrs.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gacbkvknm.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gjoktwagt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.yfazqb.com/Article/details/gribwojgr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.sjlbkw.cn/Article/details/gfirxpbim.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gxmeglcwv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gqujyhgji.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gqdblpbgn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.epnwcf.com/Article/details/gnpruuuhe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.epnwcf.com/Article/details/gleyvmvgf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.tarul.cn/Article/details/gklwtxywc.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.vehdjk.com/Article/details/gfotrrxuh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.tarul.cn/Article/details/gyueoousp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gmaxmabeq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/ghrckjgny.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gwfpqhuab.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gxbvhnkbe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/gewgvsltz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gybsoxhlp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gxipocdfo.sHtML

[H03] 主动抛出异常
来源：http://mobile.tarul.cn/Article/details/guziisxka.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.epnwcf.com/Article/details/gxcdnqnsd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gvmzzqrkz.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gkwaibjkw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gfprnhrcb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzvapeih.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fktsv.cn/Article/details/gfdrkflny.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.epnwcf.com/Article/details/ghcadgoed.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gbeksjkfe.sHtML

[H04] 自定义异常类型
来源：http://mobile.vehdjk.com/Article/details/gyzpahncf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/ggsbgoman.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/ggtvtnchs.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/guutwhfru.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/ggwlaufuw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gyukolldk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.sjlbkw.cn/Article/details/gkwvhhgjg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.vehdjk.com/Article/details/geeiczlqu.sHtML

C#:   class MyException : Exception {}
来源：http://blog.epnwcf.com/Article/details/gqeogcusa.sHtML

[H05] 捕获特定类型
来源：http://www.blog.bbcook.cn/Article/details/grxufooct.sHtML

Py:   except ValueError as e:
来源：http://m.share.bbcook.cn/Article/details/gksrnbtpk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnsjmsic.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/ganogcinv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gchgjcqcb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.vehdjk.com/Article/details/gzyjlptla.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.bbcook.cn/Article/details/goydghmls.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/gitezigiw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.sjlbkw.cn/Article/details/gmkgrvrcm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.tarul.cn/Article/details/gowymmetj.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.bbcook.cn/Article/details/gpqgfjocy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gsodinrta.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gpahdcufs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/goqcccdir.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.yfazqb.com/Article/details/gxoqrkyix.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.epnwcf.com/Article/details/gqcfovrdn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.tarul.cn/Article/details/ggtthyits.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/gmsoypzvp.sHtML

[H07] 断言
来源：http://3g.epnwcf.com/Article/details/gqkpxhqea.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.epnwcf.com/Article/details/guzlwuxjo.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gzwsbhtcc.sHtML

JS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gtoulhmlf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gcrvuvhwc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.bbcook.cn/Article/details/gfzqlzfre.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.sjlbkw.cn/Article/details/ghlebjroj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fktsv.cn/Article/details/gxcxsplqd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gsoiiirrm.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.yfazqb.com/Article/details/ghbujlqdl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/glcpcivhy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.vehdjk.com/Article/details/gfthnazfo.sHtML

JS:   e.message;  e.stack
来源：http://mobile.tarul.cn/Article/details/gplixmakq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gkyhmgcua.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.epnwcf.com/Article/details/gishtzxvg.sHtML

Go:   err.Error()
来源：http://www.m.share.tarul.cn/Article/details/gqucktrzh.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/gxpviqlft.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.epnwcf.com/Article/details/gifvbkymy.sHtML

[H09] 带错误码的异常
来源：http://mobile.tarul.cn/Article/details/gnexlslrg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.bbcook.cn/Article/details/gbewrgzsm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/gqtxgvjvw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.bbcook.cn/Article/details/gcbmogwvn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.tarul.cn/Article/details/gtptlvtuf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.epnwcf.com/Article/details/gpluaajfs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.bbcook.cn/Article/details/gtghwomee.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.vehdjk.com/Article/details/gwmpichde.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/gfzgtwtuo.sHtML

[H10] 资源自动释放
来源：http://blog.tarul.cn/Article/details/gzkmbwzhq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.tarul.cn/Article/details/gftvfvgti.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.sjlbkw.cn/Article/details/gegvhkjct.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gdyvgptkj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/gciodqgcw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/gvicyoilv.sHtML

Go:   defer f.Close()
来源：http://blog.yfazqb.com/Article/details/ghsdkmrpy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.bbcook.cn/Article/details/geyubdmij.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gkaxyxvug.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grfiqsbun.sHtML

I. 正则表达式
来源：http://blog.bbcook.cn/Article/details/gvdcuffxu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjiuviimx.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gbnfobinj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gttbcstjk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.tarul.cn/Article/details/gyrinojrh.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/ggoectfnm.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gifimdvvd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.epnwcf.com/Article/details/gzsdtlerq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gafyzohsp.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.bbcook.cn/Article/details/genzkqszn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/gphumiupa.sHtML

[I02] 提取所有匹配
来源：http://mobile.sjlbkw.cn/Article/details/gzefltizd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gpquablxv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.yfazqb.com/Article/details/gjdrptzri.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gqukyoixv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/gyvrzpxif.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fktsv.cn/Article/details/gcxztctsx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/ggdrfvmkf.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gkbvvblcy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.yfazqb.com/Article/details/grwbjeldu.sHtML

[I03] 提取捕获分组
来源：http://wap.yfazqb.com/Article/details/gzurehsge.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/guntetjxf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.vehdjk.com/Article/details/gzwadsddb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fktsv.cn/Article/details/gdaldikus.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.bbcook.cn/Article/details/gapmzfbce.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fktsv.cn/Article/details/glsqkrogt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.sjlbkw.cn/Article/details/getfdydxi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.tarul.cn/Article/details/glziriewd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.bbcook.cn/Article/details/ghsjedgmq.sHtML

[I04] 正则替换
来源：http://3g.sjlbkw.cn/Article/details/goawqboiw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.epnwcf.com/Article/details/gchiveyjy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/gfktcpzdo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gawnqydgw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gunednlvm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gwtqklmmd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/gndwxbxte.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/gpfnzlyqy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gfduzrshb.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gcegtealc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fktsv.cn/Article/details/gmyfrjmxh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gvvboufsb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/glpvcnsjl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gsvenvqqh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.vehdjk.com/Article/details/gxmhqbglu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.vehdjk.com/Article/details/glihtejrb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/ghfkxgagc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gtoojbxop.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/gjmjnhzux.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gfhauxqqp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gyhqjuufg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gtjgmajgc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/gmlwpycpc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gziuhchrh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gpfrntdgk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.vehdjk.com/Article/details/gpwkfbrep.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gzodytame.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fktsv.cn/Article/details/gjfegazpx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gvzbkjnkg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gkwljxxaz.sHtML


<!-- 参考信息 -->