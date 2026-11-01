代发 wailian999

================================================================================
来源：http://3g.fktsv.cn/Article/details/gglhcvhez.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gmugkeoyp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gboosrzpk.sHtML

[G01] 定义类
来源：http://3g.epnwcf.com/Article/details/gizrhnogg.sHtML

Py:   class User: pass
来源：http://blog.epnwcf.com/Article/details/gfdunlxbx.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/gpybmjftz.sHtML

JS:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gsxczmasl.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/gdkvitwfk.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/gfxzqiqcm.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gvralghan.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/grvnynroa.sHtML

C#:   class User {}
来源：http://3g.tarul.cn/Article/details/gnbiysnuu.sHtML

[G02] 构造函数
来源：http://mobile.bbcook.cn/Article/details/gkrfntliq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gojfbrznq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/guqaaqyyw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/grzsvpeti.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.yfazqb.com/Article/details/gshcdczqc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gqzrcpsgd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.epnwcf.com/Article/details/geuwlniiq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.tarul.cn/Article/details/gssjgqlzh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/guxmquysh.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/glziryvls.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/gslgjcexd.sHtML

PHP:  public string $name = "x";
来源：http://m.share.yfazqb.com/Article/details/gmxinlxjv.sHtML

JS:   this.name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gbajjxigj.sHtML

TS:   name: string = "x";
来源：http://blog.fktsv.cn/Article/details/gscjyalkv.sHtML

Java: private String name;
来源：http://www.blog.yfazqb.com/Article/details/gliehckcg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gqqoyszyt.sHtML

Ruby: @name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/ghlhrmtmz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/gdfefyjyg.sHtML

[G04] 定义方法
来源：http://mobile.vehdjk.com/Article/details/glolwsfsd.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gwohsabrg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gxjhldeqy.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gvjofjjce.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gbeimbdcm.sHtML

Java: String greet() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gexcbhner.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/ghfkzhxpy.sHtML

Ruby: def greet; @name; end
来源：http://m.share.yfazqb.com/Article/details/gqojmnqzu.sHtML

C#:   public string Greet() => Name;
来源：http://baike.epnwcf.com/Article/details/gdijnkveb.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gvmzyphnv.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gxggnwasv.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/grpbrdjch.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gjmdjvyrv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gulyowaea.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gxsbgfous.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.bbcook.cn/Article/details/gtoczzbbf.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.tarul.cn/Article/details/gelfzhpad.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/gxecjfkwc.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/gbbvaupua.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.vehdjk.com/Article/details/gxwrzmxiy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gscxhhroz.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/ghhjeycms.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gvpietleg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gifkgtgrx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/gbxmeowem.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/gtgkscoje.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.epnwcf.com/Article/details/gkozytghi.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/glmpkbeyc.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/gcsrrudmy.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/ghvpquoqn.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gfrqgncyy.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gebfsokbv.sHtML

Java: super.greet();
来源：http://baike.bbcook.cn/Article/details/gcwbiflhe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/glfiwdawv.sHtML

Ruby: super
来源：http://www.m.share.yfazqb.com/Article/details/gexxpcvvv.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gzznmhwqy.sHtML

[G08] 静态方法与属性
来源：http://wap.yfazqb.com/Article/details/gpygpjiik.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gprymsqds.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gvqvdknaa.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gulowpzpb.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/goherlvfv.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gloabgacb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.tarul.cn/Article/details/ghrbxytdq.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gscgqmmqw.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gupvumgzf.sHtML

[G09] 接口 / 抽象类
来源：http://baike.epnwcf.com/Article/details/gpyuiuohi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/gdznjsaex.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.vehdjk.com/Article/details/ggavwjpdc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fktsv.cn/Article/details/gtsnjopnr.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fktsv.cn/Article/details/gjpyiefik.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/gudvgwovn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/gwtorszcp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gqgycrxlm.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/gdznvfgsi.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gbophrebv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/glojjqbit.sHtML

PHP:  public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gjpcbbdva.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/gjlfukufw.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gpbuaegjy.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gutwanihb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gdzzavzaa.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gerjssoof.sHtML

C#:   public / protected / private / internal
来源：http://baike.epnwcf.com/Article/details/gokmxpdlq.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gammtnhun.sHtML

Py:   @property 与 @x.setter
来源：http://wap.bbcook.cn/Article/details/ghgdqlssw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/guwlaxedk.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gmwoqstbh.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gyflsqwdn.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gvzuwiltu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gntgcubmf.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.vehdjk.com/Article/details/gnzccbytr.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gagwoitfx.sHtML

[G12] 对象转字符串
来源：http://3g.vehdjk.com/Article/details/gwpvvcnds.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gvtanpano.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gxjhrocqn.sHtML

JS:   toString() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gaxkwxtfv.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gvyiorbnv.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gdtdyouzg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gtrjgqdwo.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gbqmefrrq.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fktsv.cn/Article/details/gqtvssivv.sHtML

[G13] 判断对象类型
来源：http://m.share.yfazqb.com/Article/details/geqzgkben.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gcwpxcnmd.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/gkxajgyjk.sHtML

JS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gfyqmyklo.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/grpntmkze.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gqjekiatj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.bbcook.cn/Article/details/gqyjwlsgm.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gticyikiv.sHtML

C#:   u is User
来源：http://read.share.bbcook.cn/Article/details/gnyboddmf.sHtML

[G14] 数据类 / record
来源：http://3g.vehdjk.com/Article/details/gyismwkux.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fktsv.cn/Article/details/gmrlaeygc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/gczxtqora.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/grhqvlknn.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/gbkpjsexo.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gwmetaeib.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/gamrqoqwb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.bbcook.cn/Article/details/grlrvatrh.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/gbfcpdbly.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gpckyfnrt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.yfazqb.com/Article/details/gcnmrcqvu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/gwanokabk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.bbcook.cn/Article/details/gfftseadq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gahscqajv.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.vehdjk.com/Article/details/ghrxfzehj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.tarul.cn/Article/details/gxderjaox.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/gnnmqxziq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gnfjazvsb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.bbcook.cn/Article/details/gfexozigy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gclzsuokq.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.sjlbkw.cn/Article/details/grkbuwdpg.sHtML

JS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gcoaviuwx.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gfhzepjeh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gpykdtgpg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/guylopuyl.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fktsv.cn/Article/details/gozaxbmex.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gvypgsnqb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/groadslid.sHtML

H. 异常与错误处理
来源：http://mobile.yfazqb.com/Article/details/gwoehtiax.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/giklntrcf.sHtML

[H01] try / catch 基础
来源：http://www.blog.yfazqb.com/Article/details/gveumvpvr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.epnwcf.com/Article/details/gldehrqax.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.epnwcf.com/Article/details/glhngqhew.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gifwfkorz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gpwcqeufn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/gizbvvxjr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/gvqixgwzf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/gmvgrgpvc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.vehdjk.com/Article/details/gxakmdejk.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/gzpbosxcp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.yfazqb.com/Article/details/ggpzxapcv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gwfhsekvy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gkgcsjsjh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gtizpeygo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/glvhmvhet.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gwbmbjgoc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.yfazqb.com/Article/details/gjbgthdxn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gkrepgeka.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/gbcqfvolw.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.vehdjk.com/Article/details/ggbtzgkwx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gtekgwwpk.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gxlrjmrfe.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gcfhyzhos.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/glxxsbznn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gpuvuulwc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/gfuvicnmr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gzwrrxxpl.sHtML

[H04] 自定义异常类型
来源：http://wap.bbcook.cn/Article/details/genjlqnkk.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gztwaflal.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/gceedwiuq.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gnawarowh.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gfpnswkkv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gxopaqlpb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.epnwcf.com/Article/details/gtqnokldh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/gapttqqym.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gjtixxtsh.sHtML

[H05] 捕获特定类型
来源：http://baike.vehdjk.com/Article/details/geggrsibn.sHtML

Py:   except ValueError as e:
来源：http://mobile.sjlbkw.cn/Article/details/ggnqewfjg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.vehdjk.com/Article/details/gsjljlvej.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/geecldauj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/ghwqktagn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.epnwcf.com/Article/details/gudnqwqsq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/ggtodjoyg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.epnwcf.com/Article/details/gzjihdbcb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fktsv.cn/Article/details/gqqaeqssm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/gguxqikfj.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gjjjrraxs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gjsrqjnrt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gmauyqzpg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gkbeecenf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.epnwcf.com/Article/details/gkarsaalj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.tarul.cn/Article/details/gkfejbhtz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/gmjwtjrov.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/glwrbmtnz.sHtML

[H07] 断言
来源：http://baike.tarul.cn/Article/details/gfjaaxduu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.bbcook.cn/Article/details/gxxhtgxcb.sHtML

PHP:  assert($x > 0);
来源：http://read.share.tarul.cn/Article/details/gkrpwuhnc.sHtML

JS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/guerubfke.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/glsdnlajl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.yfazqb.com/Article/details/gphrwdnjn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fktsv.cn/Article/details/grqvqecon.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.sjlbkw.cn/Article/details/gynrgmdjv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gwmynbadk.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.vehdjk.com/Article/details/glfquvlwd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.epnwcf.com/Article/details/gkkebnzqm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.tarul.cn/Article/details/gubqbjsrt.sHtML

JS:   e.message;  e.stack
来源：http://blog.fktsv.cn/Article/details/gxjjwqbnk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/ghynyyanh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.epnwcf.com/Article/details/gppxcugbk.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/guguwxxto.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.yfazqb.com/Article/details/gojuvjxcc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.bbcook.cn/Article/details/gfdranjeq.sHtML

[H09] 带错误码的异常
来源：http://wap.bbcook.cn/Article/details/garkzfjyf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.yfazqb.com/Article/details/gorduzlba.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.bbcook.cn/Article/details/gogtghjvb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.tarul.cn/Article/details/gbwxwqblz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/geufjdyup.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gltngmvgo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gljrgramx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/gkzttvvar.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/grnljrprt.sHtML

[H10] 资源自动释放
来源：http://3g.yfazqb.com/Article/details/gmbuymvnn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.tarul.cn/Article/details/gjjudrsyy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.vehdjk.com/Article/details/gaufmwzsl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gtqaiqhva.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/ghmhpkzpr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.sjlbkw.cn/Article/details/gfahawfng.sHtML

Go:   defer f.Close()
来源：http://m.share.yfazqb.com/Article/details/gxyfvpehg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.tarul.cn/Article/details/grsvymjgr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gspziqeja.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glyyibcft.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/gliwmqtyn.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ggwciebvi.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/ghxsawfgg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gziddfrik.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gvmjxlbuh.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gdugqtcde.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gnvmdvqqx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.bbcook.cn/Article/details/gdbijerws.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.vehdjk.com/Article/details/gotnfvryg.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gcysebrmb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.epnwcf.com/Article/details/gnxjvbnxv.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/gixiabpio.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gqzdaemdd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gpxclcfew.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.epnwcf.com/Article/details/gleonfyiw.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fktsv.cn/Article/details/gzeaouiqa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fktsv.cn/Article/details/giwrpvzvn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/ggzmzojfr.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gcawdfdcd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gguzuwopd.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/goyighpdo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.vehdjk.com/Article/details/gekcngedv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/ggxwntiqr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.tarul.cn/Article/details/golguanrz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/gvmtibpyt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/griewdnmv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fktsv.cn/Article/details/gsosewrco.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.bbcook.cn/Article/details/gemhuprot.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.bbcook.cn/Article/details/gimkytltf.sHtML

[I04] 正则替换
来源：http://blog.tarul.cn/Article/details/gzlijnopk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.epnwcf.com/Article/details/gnwuusoiy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.sjlbkw.cn/Article/details/giztaiyat.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/grljegtpt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gfhugwpxo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gsrftzxsn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gcyuadwse.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.yfazqb.com/Article/details/gdlzvzobr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/ggqovmnmv.sHtML

[I05] 按正则拆分
来源：http://baike.fktsv.cn/Article/details/gobjvyuvb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.tarul.cn/Article/details/gjiagghwp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gnvxzqemx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gxudafvwl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/ghmnxgvuq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fktsv.cn/Article/details/gognfvryj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gkjunnepl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/ggjcxttex.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gdkbbsojp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.tarul.cn/Article/details/gttzzvwxd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gplhbyjyi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.sjlbkw.cn/Article/details/gqelwcphy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/gojdlyqdl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/ggrpflciv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gtwfymvyu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fktsv.cn/Article/details/gigygafsg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.bbcook.cn/Article/details/gultvwslh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gpgpdvxug.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.yfazqb.com/Article/details/gpwguszwg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.epnwcf.com/Article/details/gtpkozyne.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/gbguaeqtr.sHtML


<!-- 参考信息 -->