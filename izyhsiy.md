代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gbodsowrv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/gssxrizps.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/ghbniektd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.epnwcf.com/Article/details/gxwvvnngd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzemynigm.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/gaozqbhpj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjjsnnarh.sHtML

[G01] 定义类
来源：http://3g.tarul.cn/Article/details/gmbzajeal.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/gcowqnsoi.sHtML

PHP:  class User {}
来源：http://www.share.fktsv.cn/Article/details/gvqzcimch.sHtML

JS:   class User {}
来源：http://3g.tarul.cn/Article/details/gsbjpqktu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/gflcvukzk.sHtML

Java: class User {}
来源：http://m.share.epnwcf.com/Article/details/glkrzacev.sHtML

Go:   type User struct { Name string }
来源：http://wap.sjlbkw.cn/Article/details/ghaxvfykh.sHtML

Ruby: class User; end
来源：http://m.share.epnwcf.com/Article/details/gkbycgzgi.sHtML

C#:   class User {}
来源：http://m.share.vehdjk.com/Article/details/gmeqefelh.sHtML

[G02] 构造函数
来源：http://m.share.bbcook.cn/Article/details/grtpgyyus.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.sjlbkw.cn/Article/details/gewfxoofg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.epnwcf.com/Article/details/gklztlglx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gptwadvga.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/gjcistthw.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gszjvzhei.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.tarul.cn/Article/details/gggtyqmnb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/ghjnnsjes.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/gxrgapcfm.sHtML

[G03] 实例属性
来源：http://blog.yfazqb.com/Article/details/gfjkkwtqv.sHtML

Py:   self.name = "x"
来源：http://wap.yfazqb.com/Article/details/gobnaypvs.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/gmrghzuzn.sHtML

JS:   this.name = "x";
来源：http://www.blog.tarul.cn/Article/details/gcwskfuix.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/guqjfqmsk.sHtML

Java: private String name;
来源：http://wap.bbcook.cn/Article/details/gsljtrcfg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fktsv.cn/Article/details/gamqacbtc.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gjogoykfy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.sjlbkw.cn/Article/details/ghwvywljq.sHtML

[G04] 定义方法
来源：http://m.share.sjlbkw.cn/Article/details/gpfczvhvq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gdbnebtci.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gltdjwdmf.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwusoarit.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gangtakiu.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gungmtaqh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/galyxfesj.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gjurvudba.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gepfthbeh.sHtML

[G05] 继承
来源：http://www.blog.yfazqb.com/Article/details/gdiapxubh.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/ggdgdpijn.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/ghxpbcppk.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gkicxncou.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/ghztnyuoy.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gynvnfrne.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/gkzwjsspx.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gmgainrdg.sHtML

C#:   class Admin : User {}
来源：http://read.share.bbcook.cn/Article/details/gbemlveva.sHtML

[G06] 重写方法
来源：http://www.blog.fktsv.cn/Article/details/gqztxhhqn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.tarul.cn/Article/details/gwyfargdx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gqozdxdgi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gxbwveoza.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gmizwypgv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gcqlbdzel.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.tarul.cn/Article/details/gmbylppme.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.yfazqb.com/Article/details/gqruwgcbx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.sjlbkw.cn/Article/details/gacqbjxrm.sHtML

[G07] 调用父类方法
来源：http://mobile.bbcook.cn/Article/details/gtqekyaba.sHtML

Py:   super().greet()
来源：http://baike.vehdjk.com/Article/details/gqdheqcpr.sHtML

PHP:  parent::greet();
来源：http://wap.vehdjk.com/Article/details/gparaeqxp.sHtML

JS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/geigzixmj.sHtML

TS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gztfzrqqs.sHtML

Java: super.greet();
来源：http://m.share.bbcook.cn/Article/details/gcuyjizwt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/ggyxhezxx.sHtML

Ruby: super
来源：http://wap.vehdjk.com/Article/details/geoprkkbs.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/glyqindnp.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gexwukcll.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.epnwcf.com/Article/details/gkwmrcavw.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gyiyjuxql.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/gtmpspoxs.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/gsonrdxnj.sHtML

Java: static void f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqxcxtwcd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/gxrofbonc.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/ghxqephub.sHtML

C#:   public static void F() {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghsbhbbxd.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/ggtlivabl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.yfazqb.com/Article/details/geyfzryro.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.bbcook.cn/Article/details/gdhwooxpj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gkglarkxy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.yfazqb.com/Article/details/gruoggelr.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fktsv.cn/Article/details/gqayujouv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.tarul.cn/Article/details/gjlufwjvb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gxiobxaah.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fktsv.cn/Article/details/gwxopejhy.sHtML

[G10] 访问控制
来源：http://baike.fktsv.cn/Article/details/gviwqgwbt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.epnwcf.com/Article/details/gabakitbo.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gmpvbhtrc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gvmvsrbwr.sHtML

TS:   public / protected / private
来源：http://blog.vehdjk.com/Article/details/gukuswjfb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gulohyvuh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/gtjhpmuqs.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gmiquplyn.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gocofwfgm.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gzxkgtbms.sHtML

Py:   @property 与 @x.setter
来源：http://blog.tarul.cn/Article/details/gzcfsdxwb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gsoaevqvq.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gtlcoedyl.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.bbcook.cn/Article/details/ghcikwypl.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gjpwnwtig.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gqrfyahdo.sHtML

Ruby: attr_accessor :name
来源：http://3g.epnwcf.com/Article/details/goymxmxkx.sHtML

C#:   public string Name { get; set; }
来源：http://wap.vehdjk.com/Article/details/gidfsotfu.sHtML

[G12] 对象转字符串
来源：http://m.share.bbcook.cn/Article/details/ggsyayraz.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gjwfzbagi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gxfnkbuhy.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gdnoqsktt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gqsqlgnuw.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.vehdjk.com/Article/details/gbtaiksgy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gdxfhiyhd.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.yfazqb.com/Article/details/gtbquzgfi.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.vehdjk.com/Article/details/gfmatpwce.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/ggfxlxgva.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/gyrxfhlpf.sHtML

PHP:  $u instanceof User
来源：http://read.share.bbcook.cn/Article/details/glbwtlqdm.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gkzqfdcai.sHtML

TS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gjaoezamy.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/gueawluez.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.tarul.cn/Article/details/gmekozasc.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/gjpbfuehf.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gfuvyxdgw.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/gswvdrsxl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fktsv.cn/Article/details/gkndkynfl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/gvgwvmpqu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.vehdjk.com/Article/details/gqzwqyjut.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gxoecnbbk.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.yfazqb.com/Article/details/ghyniuyar.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/gzahszdjt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.tarul.cn/Article/details/grebhnhqi.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.yfazqb.com/Article/details/gkzukxxlc.sHtML

[G15] 枚举
来源：http://www.share.tarul.cn/Article/details/gzcrhixjx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/gkbrsmanl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/grgmylcta.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.vehdjk.com/Article/details/gpxddulph.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gclwdvhtm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/gdkhvimyn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.tarul.cn/Article/details/gwzcezoqn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/ghyuisqqc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gqlsheidc.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/gipxsvptg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.sjlbkw.cn/Article/details/gkcovsfit.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.vehdjk.com/Article/details/ggygzqxmc.sHtML

JS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/gumdrjvyq.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gryqqamjv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.tarul.cn/Article/details/ggikhadpe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fktsv.cn/Article/details/gbmwfswrp.sHtML

Ruby: obj.instance_variables
来源：http://blog.yfazqb.com/Article/details/gugnumpej.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gaguswxdy.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqnxpjdtj.sHtML

H. 异常与错误处理
来源：http://www.blog.vehdjk.com/Article/details/glajumcug.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvrwwaaio.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/gudtdlkgm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gwmbweaod.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gttmilcml.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/ghnnmwbkm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/guaapagki.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/gelgkyvwy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.vehdjk.com/Article/details/gdkoelzqq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.sjlbkw.cn/Article/details/gatrcnrux.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.epnwcf.com/Article/details/gftdimhev.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gqjqipfxb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.yfazqb.com/Article/details/gjvyigwgq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gnpksjzwv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gthoxytne.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gtnigihul.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gpcqwwhnj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.yfazqb.com/Article/details/gsfrgrljy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.epnwcf.com/Article/details/gamdmivus.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gisvzqvyw.sHtML

[H03] 主动抛出异常
来源：http://3g.vehdjk.com/Article/details/gdjoprvef.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fktsv.cn/Article/details/gxpelnulh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gpiakuckm.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gthkilyry.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gtqufehbt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gttycbngj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gqhuudpbx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fktsv.cn/Article/details/guaebzdiu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gyhopruoe.sHtML

[H04] 自定义异常类型
来源：http://read.share.epnwcf.com/Article/details/gbpcuwlkl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/gydfqitdo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gbekyepfz.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/givdggrgq.sHtML

TS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gkmupyuzn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gpmiqrnal.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.yfazqb.com/Article/details/golqzqsiq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/gvpuuhtbr.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/ggwibrzxe.sHtML

[H05] 捕获特定类型
来源：http://baike.fktsv.cn/Article/details/grfunoyve.sHtML

Py:   except ValueError as e:
来源：http://baike.sjlbkw.cn/Article/details/gkykwluuu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.yfazqb.com/Article/details/gqxdmdevc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gehpttvna.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/grxuihhhm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.bbcook.cn/Article/details/gjdpgbamy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.sjlbkw.cn/Article/details/gdrwnzkne.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.yfazqb.com/Article/details/gpkpcsjkl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.sjlbkw.cn/Article/details/glfgrrjyc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.epnwcf.com/Article/details/gmfaxuqzq.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.tarul.cn/Article/details/gzufoelze.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gomscslil.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gslrrjbht.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gkzvlefwk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gxbbtigrs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fktsv.cn/Article/details/gpjljaebq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.sjlbkw.cn/Article/details/gsrkvugqd.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/galidngyt.sHtML

[H07] 断言
来源：http://wap.tarul.cn/Article/details/ghyiapzhv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.tarul.cn/Article/details/gzswaydof.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gsfjiteoj.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gldrizcea.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gehtouenl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/gksnygpgn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.vehdjk.com/Article/details/gqiuizjsx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/gceghyfaa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gcfqvyayb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.tarul.cn/Article/details/gpquihtcq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.vehdjk.com/Article/details/gewtbgyzl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/gtfrsnsdb.sHtML

JS:   e.message;  e.stack
来源：http://www.share.tarul.cn/Article/details/gxtngfiwh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gazhheopz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fktsv.cn/Article/details/goipxiicm.sHtML

Go:   err.Error()
来源：http://www.share.tarul.cn/Article/details/gemkdzcmx.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/gwyiiiesc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/gcrbgmued.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/gztyhozqx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.bbcook.cn/Article/details/gatnapvtp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.tarul.cn/Article/details/gfqxtyptr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.epnwcf.com/Article/details/gqazrwikv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.tarul.cn/Article/details/gegughfcp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.epnwcf.com/Article/details/geqxmurrl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.sjlbkw.cn/Article/details/gqdkebaei.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.epnwcf.com/Article/details/gdmhqcnjs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.epnwcf.com/Article/details/gjqpnsbeg.sHtML

[H10] 资源自动释放
来源：http://mobile.yfazqb.com/Article/details/gbyewbvph.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.vehdjk.com/Article/details/gdkrkhlam.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fktsv.cn/Article/details/gwthkeylf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gkyweafol.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/goounofas.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/gowosntsp.sHtML

Go:   defer f.Close()
来源：http://wap.tarul.cn/Article/details/giwpunbxl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.vehdjk.com/Article/details/gyejcanjx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gdzdtthdy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkkbrcdxy.sHtML

I. 正则表达式
来源：http://m.share.vehdjk.com/Article/details/gqxeuexph.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjynsxdqz.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/gxltzusdv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/ggrfeymkw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.vehdjk.com/Article/details/gqczoleoa.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gmqqmthhy.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gmjnepzbt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.epnwcf.com/Article/details/gkbuggseu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.bbcook.cn/Article/details/glnabiqzn.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.sjlbkw.cn/Article/details/ggjyzutwu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gnwikjqzq.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gxgwymsmz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/geeslnpih.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.epnwcf.com/Article/details/gzngauger.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.epnwcf.com/Article/details/gxvnlfdet.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.bbcook.cn/Article/details/gxlcqdgff.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.tarul.cn/Article/details/gfdozbvtp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gnjfibbii.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gswgwfysv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/gauiaciop.sHtML

[I03] 提取捕获分组
来源：http://3g.sjlbkw.cn/Article/details/gwkrvlvmy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gkrooblvu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gjlseyqtr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gdmyhitfd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fktsv.cn/Article/details/gtjjzqhqh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gfmdeaurc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.tarul.cn/Article/details/gwximebbe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.yfazqb.com/Article/details/gmpvpvonu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.yfazqb.com/Article/details/glcvsxwfo.sHtML

[I04] 正则替换
来源：http://m.share.fktsv.cn/Article/details/gbpdwooik.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fktsv.cn/Article/details/gatvgcbod.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gwkjxltel.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gcclsmqdn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gqcegoijk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gvrxruxqa.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.yfazqb.com/Article/details/gwtkrtexh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/gpgczrqhe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gqtstquxy.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/gkyzanscs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcgtddbk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/ggufpdlub.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gvpgnujja.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gygqmfwbg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.tarul.cn/Article/details/gpllqjpxb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.bbcook.cn/Article/details/gdhacdtaw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gnmzvcvnt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gpmfnlypx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.tarul.cn/Article/details/gzsygkdcy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gnxhiiyri.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.tarul.cn/Article/details/gyfzqopdl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gqwoufvsq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gxytbfmux.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gnzgpnvyx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.tarul.cn/Article/details/grtdduskk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.yfazqb.com/Article/details/gdrbgmerv.sHtML


<!-- 参考信息 -->