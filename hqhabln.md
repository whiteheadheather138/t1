代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.epnwcf.com/Article/details/gktexaydp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gechwqomb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gtdobpobn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.sjlbkw.cn/Article/details/gsfllkacv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grjasollj.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gpugbaygx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpyqmpqkd.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/grbjkhckv.sHtML

Py:   class User: pass
来源：http://www.blog.vehdjk.com/Article/details/gwlneawqh.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/grrlmnwek.sHtML

JS:   class User {}
来源：http://m.share.tarul.cn/Article/details/gsaztgutc.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/gronexksy.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gkzancoqe.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/ggyyrwuoe.sHtML

Ruby: class User; end
来源：http://read.share.vehdjk.com/Article/details/gpcboynop.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gechhphjk.sHtML

[G02] 构造函数
来源：http://wap.tarul.cn/Article/details/gwdsadohc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fktsv.cn/Article/details/greaaoluo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gybnblbue.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gbioadpbg.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.vehdjk.com/Article/details/glyrffnhb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/ghwaeijlr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.sjlbkw.cn/Article/details/guyxhecsz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/glocdxqfp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/guftrkgba.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gbmdzyirf.sHtML

Py:   self.name = "x"
来源：http://mobile.yfazqb.com/Article/details/glwucgenl.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gwnsbotir.sHtML

JS:   this.name = "x";
来源：http://www.share.tarul.cn/Article/details/gdpfbafqx.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/gjfgflmuu.sHtML

Java: private String name;
来源：http://www.blog.bbcook.cn/Article/details/gbafwbzoc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.tarul.cn/Article/details/gzaqzubnf.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gmozfstfz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gzcipgpzv.sHtML

[G04] 定义方法
来源：http://3g.sjlbkw.cn/Article/details/gblukfgwc.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gjbqefsao.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gmzpqkxvd.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gchcljvic.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gvzglryxc.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gdhhugmmq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gyoqxudww.sHtML

Ruby: def greet; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gptwfvwma.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gwlqxujsv.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/gonstbqui.sHtML

Py:   class Admin(User): pass
来源：http://wap.epnwcf.com/Article/details/ggzrochgo.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gtslgiqpi.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gejkfmkhs.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gcliljlnd.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/genwhflbs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/gtymiruod.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gtvoqctrg.sHtML

C#:   class Admin : User {}
来源：http://wap.sjlbkw.cn/Article/details/gkwzsfznv.sHtML

[G06] 重写方法
来源：http://mobile.vehdjk.com/Article/details/gznsvtnqu.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/ggdhajtae.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gzltufpbb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gpfcheccs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gqtvbsuhz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gnegxfele.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gdmomosle.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/gezealysb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/glmppbleh.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gypryzgnd.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gxwzryltp.sHtML

PHP:  parent::greet();
来源：http://www.m.share.yfazqb.com/Article/details/gbhecmmzo.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/ghxoqqmxm.sHtML

TS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gvteroxms.sHtML

Java: super.greet();
来源：http://read.share.vehdjk.com/Article/details/gwmojlqyv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.epnwcf.com/Article/details/gfcdkgizf.sHtML

Ruby: super
来源：http://read.share.fktsv.cn/Article/details/gbnxqtxge.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gqdgagdqu.sHtML

[G08] 静态方法与属性
来源：http://wap.vehdjk.com/Article/details/gsanegxjo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gpolonetv.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gquahcvgs.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/gsuxkbqcb.sHtML

TS:   static f(): void {}
来源：http://mobile.epnwcf.com/Article/details/gquaagtcb.sHtML

Java: static void f() {}
来源：http://mobile.bbcook.cn/Article/details/ggoihzbds.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.tarul.cn/Article/details/gamweuvcx.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/gaexvobmk.sHtML

C#:   public static void F() {}
来源：http://baike.bbcook.cn/Article/details/gbimdoqri.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/glqpmuitf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.yfazqb.com/Article/details/gajqesugs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghpuzqlqp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.epnwcf.com/Article/details/gwjwjsmyj.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gbnvoxyay.sHtML

Java: interface Shape { double area(); }
来源：http://blog.tarul.cn/Article/details/gtaipygdp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/gencexras.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/gxnagdslv.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.epnwcf.com/Article/details/gobbjxdcu.sHtML

[G10] 访问控制
来源：http://www.m.share.sjlbkw.cn/Article/details/ghaxmbvtv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/gkmiczbew.sHtML

PHP:  public / protected / private
来源：http://blog.fktsv.cn/Article/details/gskudxlnu.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/gfuwgopqe.sHtML

TS:   public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gsakhegvo.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gmmpfhatf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.vehdjk.com/Article/details/gkwdwipsy.sHtML

Ruby: public / protected / private
来源：http://baike.tarul.cn/Article/details/gfvzvjrki.sHtML

C#:   public / protected / private / internal
来源：http://wap.bbcook.cn/Article/details/gqktmonti.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/glocxswwe.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/gghuihjlz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/grbpsdeii.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gepmylzvu.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/gzoparddc.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gawdedfsz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gikstnpxo.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/gijejzlio.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/gnexmvnsg.sHtML

[G12] 对象转字符串
来源：http://www.share.bbcook.cn/Article/details/gidboovmu.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gjbtrubma.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxhuczbq.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gzluoifsl.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/ghengfmrb.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.vehdjk.com/Article/details/gmkyyhueg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gwenjvsmq.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gntmgepfe.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.tarul.cn/Article/details/gbgyztexi.sHtML

[G13] 判断对象类型
来源：http://mobile.epnwcf.com/Article/details/gffqigave.sHtML

Py:   isinstance(u, User)
来源：http://mobile.vehdjk.com/Article/details/glnbwrgug.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/ghivnmegv.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gemmvnnvu.sHtML

TS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gogvfjrka.sHtML

Java: u instanceof User
来源：http://baike.tarul.cn/Article/details/gfbwdmfok.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gnmwohdmd.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.vehdjk.com/Article/details/gzxnqftsz.sHtML

C#:   u is User
来源：http://3g.fktsv.cn/Article/details/gqdbaukpv.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/gvuylluec.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.vehdjk.com/Article/details/gehlqohfm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.bbcook.cn/Article/details/goxyepbhr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.sjlbkw.cn/Article/details/ggieejckd.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/geusdwfzj.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqjxzojwa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gvwwldigz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/gpcyaeakw.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.sjlbkw.cn/Article/details/gowaikxsd.sHtML

[G15] 枚举
来源：http://www.m.share.vehdjk.com/Article/details/gnalecftx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gjheveczo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.tarul.cn/Article/details/giyvnqcdz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.sjlbkw.cn/Article/details/gcopjumxs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gdigsdpcn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.yfazqb.com/Article/details/geafepwwg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/glzsqtiwz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.tarul.cn/Article/details/gzarrfrhm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gifnyahkm.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/gwqvprzfx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gaodfmehd.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/geszooomh.sHtML

JS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/glffmjzec.sHtML

TS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/gsewivcsw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/gvuslkllg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.epnwcf.com/Article/details/gcjfgkdra.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/gsygpcbnh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gsoltlgzn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gelbjwvrw.sHtML

H. 异常与错误处理
来源：http://blog.vehdjk.com/Article/details/gbwsoegic.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvwnrewji.sHtML

[H01] try / catch 基础
来源：http://baike.bbcook.cn/Article/details/gunakcdml.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.bbcook.cn/Article/details/grqbswpdx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.vehdjk.com/Article/details/gpxzuinnd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gldcukbff.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gydwlhrsn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.yfazqb.com/Article/details/gfonbofqs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.epnwcf.com/Article/details/gvkhnjqjx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.bbcook.cn/Article/details/gbhnelkho.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/gfacbvqgj.sHtML

[H02] finally / ensure 收尾
来源：http://baike.yfazqb.com/Article/details/ggsnlailu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.epnwcf.com/Article/details/guzdjliuo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gvbmidwwt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gfyuikrle.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/giocjhhqf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gbzdwrrdx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/gckteruxt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gpzzkswwe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gxrhffxzb.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/gbfpwuyvx.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.sjlbkw.cn/Article/details/gjmlewuis.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gctpxofsk.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/ghnmdhrwq.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gmgfihuhx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/ghdqqlqda.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.epnwcf.com/Article/details/gvslwekss.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.sjlbkw.cn/Article/details/gtarnpdlv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/ggcryrfri.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/grypogmhu.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.vehdjk.com/Article/details/gelohmeeo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gvtypepjf.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/glkzambhh.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gnwkhgqfh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gkvogxzzr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.sjlbkw.cn/Article/details/gpwapatpr.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/gwndflhqc.sHtML

C#:   class MyException : Exception {}
来源：http://blog.epnwcf.com/Article/details/gugsaijty.sHtML

[H05] 捕获特定类型
来源：http://mobile.tarul.cn/Article/details/guxwipwjm.sHtML

Py:   except ValueError as e:
来源：http://mobile.bbcook.cn/Article/details/gmhylupyx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.vehdjk.com/Article/details/gnfevgylt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gwzkwwjet.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.vehdjk.com/Article/details/gpdneetra.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.tarul.cn/Article/details/gilvxfxul.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fktsv.cn/Article/details/giyxkqqlx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.yfazqb.com/Article/details/gghndtfcc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.epnwcf.com/Article/details/gpwguaafx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.bbcook.cn/Article/details/gombvavsw.sHtML

Py:   value = d.get("k") or default
来源：http://baike.tarul.cn/Article/details/gxoadakkh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gmkyzbgab.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/ghodsiqdq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/gxrhtfsby.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.vehdjk.com/Article/details/gasqwpgzg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.yfazqb.com/Article/details/gwymtaevg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.epnwcf.com/Article/details/gfhkjfxym.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.sjlbkw.cn/Article/details/gpxjjgjtl.sHtML

[H07] 断言
来源：http://read.share.fktsv.cn/Article/details/gomjaeeby.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/gtnrqnfua.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gsbkrlpgx.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/goeotvszu.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gsimlnlom.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gsuxwyhvx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/gwweynxxf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.epnwcf.com/Article/details/gmmbkcibp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gpjgisbrk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fktsv.cn/Article/details/grjazwmxe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fktsv.cn/Article/details/gtquvckzu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fktsv.cn/Article/details/galvatqgj.sHtML

JS:   e.message;  e.stack
来源：http://read.share.tarul.cn/Article/details/gtouiykkg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/ggepuuuaf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gnuhdayfv.sHtML

Go:   err.Error()
来源：http://www.share.yfazqb.com/Article/details/guwxuoasp.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fktsv.cn/Article/details/gngmqjpkj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/gxudbortn.sHtML

[H09] 带错误码的异常
来源：http://wap.fktsv.cn/Article/details/grqdmxrcw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.vehdjk.com/Article/details/gacclrqhx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fktsv.cn/Article/details/gjejgjqwt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fktsv.cn/Article/details/gixoajmkd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.bbcook.cn/Article/details/gxlfrgwwt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.epnwcf.com/Article/details/gwsrtolxt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gquayiaou.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.yfazqb.com/Article/details/gbxpnrets.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.vehdjk.com/Article/details/goyrqxbyq.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gwxbetski.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.yfazqb.com/Article/details/gpetypboc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/gmtokvhin.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/gkfgdsczr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gtjmflwkq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gvgkdcdla.sHtML

Go:   defer f.Close()
来源：http://wap.vehdjk.com/Article/details/gzfziddvy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.epnwcf.com/Article/details/gqhzwtixd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gqzbyeboe.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsnxeiqmp.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gnzzuhsrw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gyypadaur.sHtML

[I01] 判断是否匹配
来源：http://www.share.epnwcf.com/Article/details/gbqybajbl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gycrvfrxr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gdaxksgci.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/ghsjfzuaw.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gqzdebozz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fktsv.cn/Article/details/gvgnawofl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjnqwvac.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/grnixbuce.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.epnwcf.com/Article/details/gaoqjhfmy.sHtML

[I02] 提取所有匹配
来源：http://3g.vehdjk.com/Article/details/goaiqjhmo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gisgeaabq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.sjlbkw.cn/Article/details/gslhhqtje.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.sjlbkw.cn/Article/details/gelimhcsg.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.vehdjk.com/Article/details/gdtnzdehe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.sjlbkw.cn/Article/details/gzhrfqqwv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gcrhkxzkf.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gfcprnmxe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.yfazqb.com/Article/details/glekqxodt.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gvijyqfha.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/gqeekvbpw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.tarul.cn/Article/details/gzxlfabbx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.vehdjk.com/Article/details/gxnuzxaex.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.tarul.cn/Article/details/gikzehjnq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fktsv.cn/Article/details/gwkqzhcak.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gugzusgoy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.bbcook.cn/Article/details/gzsxunoni.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.bbcook.cn/Article/details/gnzujhrdq.sHtML

[I04] 正则替换
来源：http://www.share.epnwcf.com/Article/details/gibkydmup.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.epnwcf.com/Article/details/gnzbavevi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/ggjduxrzg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gezcwrkds.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gfwqlqgvl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/grimxalfc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fktsv.cn/Article/details/gfyusjyog.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.vehdjk.com/Article/details/gnqwavmjq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gbymfklkt.sHtML

[I05] 按正则拆分
来源：http://baike.sjlbkw.cn/Article/details/ghiovvnod.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.vehdjk.com/Article/details/gteoiowmz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.tarul.cn/Article/details/gwtplsdux.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gvovpcoym.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gflawqits.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.yfazqb.com/Article/details/gjcbplndz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.epnwcf.com/Article/details/gmqzbwkyd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gkiisuysb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/gwptofgqf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.vehdjk.com/Article/details/gjifrvfmz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gzosasfji.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fktsv.cn/Article/details/gkiufrvsz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gimszlqjk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gwqqkpzve.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gtsyifosr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.yfazqb.com/Article/details/grdogxdvn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fktsv.cn/Article/details/ghrekiuju.sHtML


<!-- 参考信息 -->