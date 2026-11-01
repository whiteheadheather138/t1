代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.bbcook.cn/Article/details/grdekdufr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gqeozbxav.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/gqamxiurc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/glqhcbcoo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwfvuerjd.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gvjymdfsa.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gejiksdtd.sHtML

[G01] 定义类
来源：http://m.share.fktsv.cn/Article/details/gxjzscrnw.sHtML

Py:   class User: pass
来源：http://mobile.sjlbkw.cn/Article/details/gnxvztgjz.sHtML

PHP:  class User {}
来源：http://read.share.yfazqb.com/Article/details/gibulekre.sHtML

JS:   class User {}
来源：http://3g.vehdjk.com/Article/details/ggbhtzxmr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fktsv.cn/Article/details/gufctweft.sHtML

Java: class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtampxywj.sHtML

Go:   type User struct { Name string }
来源：http://wap.sjlbkw.cn/Article/details/geodhwyls.sHtML

Ruby: class User; end
来源：http://read.share.yfazqb.com/Article/details/gkrbevolf.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gkamnggki.sHtML

[G02] 构造函数
来源：http://wap.tarul.cn/Article/details/gubldiaud.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/gztealzqr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/gicknwmsj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gwqgzaium.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/ghnpsaqnt.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/goqvtduch.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gllkkcjnl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gujfwucby.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gkkkiarpf.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gybmheoyc.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/gdxgzyjmz.sHtML

PHP:  public string $name = "x";
来源：http://blog.tarul.cn/Article/details/ggeetcaqg.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gpglecjpi.sHtML

TS:   name: string = "x";
来源：http://www.blog.fktsv.cn/Article/details/gfxoyenke.sHtML

Java: private String name;
来源：http://3g.epnwcf.com/Article/details/gumbqdieo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gqcjfmgji.sHtML

Ruby: @name = "x"
来源：http://blog.epnwcf.com/Article/details/gkazlzbjo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gcfezriww.sHtML

[G04] 定义方法
来源：http://www.m.share.epnwcf.com/Article/details/gpszvrcsj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gtzxogtpu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/ggdiupmbg.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gxvnwtwde.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/galwhmpzh.sHtML

Java: String greet() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gvesrreia.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gfcnnshfx.sHtML

Ruby: def greet; @name; end
来源：http://mobile.yfazqb.com/Article/details/gheekpqmg.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.vehdjk.com/Article/details/gglkgzmoz.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/gmpzruond.sHtML

Py:   class Admin(User): pass
来源：http://read.share.vehdjk.com/Article/details/gnailgmpa.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gjwpiqlcx.sHtML

JS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gdxzulnbp.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gxwqcgydd.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/glsmnhpbf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.bbcook.cn/Article/details/goiirchxs.sHtML

Ruby: class Admin < User; end
来源：http://wap.fktsv.cn/Article/details/guzlomftw.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gjnufxvni.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/gxyhvytbm.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fktsv.cn/Article/details/goooanhra.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/ggxmdrktz.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gaashmyvm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gpxcirdef.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gwvcppitx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/gujomretx.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/gphalyipv.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.epnwcf.com/Article/details/gdbdcxquz.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/gzkpsixmd.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/gqgtleglp.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/guymlbywy.sHtML

JS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gldnrucjn.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gcbjyvbav.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/gjqmzkkjq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.epnwcf.com/Article/details/ggemueiia.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/gndobawnc.sHtML

C#:   base.Greet();
来源：http://mobile.vehdjk.com/Article/details/gpokgtssc.sHtML

[G08] 静态方法与属性
来源：http://read.share.sjlbkw.cn/Article/details/gifcdnmfk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.vehdjk.com/Article/details/gpnmmduad.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/gifnngqxj.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gbbpajzaz.sHtML

TS:   static f(): void {}
来源：http://baike.fktsv.cn/Article/details/gtvfpnlfq.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/gjbqtgtud.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.epnwcf.com/Article/details/gmctlpoht.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/guxkgyqpf.sHtML

C#:   public static void F() {}
来源：http://3g.tarul.cn/Article/details/glefkrpba.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/gpanspoxp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.bbcook.cn/Article/details/gihlevvzw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/gvbvyzmer.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gnbxgowww.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/glhgryadp.sHtML

Java: interface Shape { double area(); }
来源：http://blog.sjlbkw.cn/Article/details/guvhmbczn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/gxgzyhkco.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gwmwjhubu.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.epnwcf.com/Article/details/gshnxdvws.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/goyxieqnt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.tarul.cn/Article/details/gsbeptswh.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gistcnegy.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/ggotevxny.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gvpqvamfv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/gqmzmybop.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gzbdlqpny.sHtML

Ruby: public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gcbyjidht.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/gwcccuwdp.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gyrvcqgip.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fktsv.cn/Article/details/gggsfwoiq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gjfxstubc.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gomqdhrbh.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gorucufjv.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/gtontrpfn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gleydgbrk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.bbcook.cn/Article/details/ggmchdfyu.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gcmzsrwpu.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/ggjmzrfpw.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.tarul.cn/Article/details/gzcskxcld.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gfilqbkck.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gdyvzcrge.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gwxervwbd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gckoguwsm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gczoupqdy.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gofotcqom.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gzqkaroxs.sHtML

[G13] 判断对象类型
来源：http://3g.yfazqb.com/Article/details/gnusfruyf.sHtML

Py:   isinstance(u, User)
来源：http://mobile.vehdjk.com/Article/details/gyyzuyrhl.sHtML

PHP:  $u instanceof User
来源：http://3g.vehdjk.com/Article/details/gpmnxmpyt.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gnrkncrci.sHtML

TS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gqrixgftz.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gscyyfesx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/grwwpxzyy.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/gmiyyanmm.sHtML

C#:   u is User
来源：http://m.share.vehdjk.com/Article/details/girefdirh.sHtML

[G14] 数据类 / record
来源：http://blog.epnwcf.com/Article/details/gkbosjfyn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/gnjhssvpp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.bbcook.cn/Article/details/gjugvsovl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.yfazqb.com/Article/details/gbsarcivg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.tarul.cn/Article/details/gfrlpzqrj.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gcwksetxg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.yfazqb.com/Article/details/gfvyrtusc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.bbcook.cn/Article/details/gikgozbyc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.bbcook.cn/Article/details/glzzrttpm.sHtML

[G15] 枚举
来源：http://m.share.vehdjk.com/Article/details/gweqmpgnf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.epnwcf.com/Article/details/gfklkyewd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gxebjtzyv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.tarul.cn/Article/details/ggmpkmmvq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/getetnqnt.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gydgladgr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fktsv.cn/Article/details/gltjwxpfv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/gxlgojcnk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gxopayeol.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gglcmdmtz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gpuvsoyof.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.tarul.cn/Article/details/gpkwflnci.sHtML

JS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/glgznfkhl.sHtML

TS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/ggedzonfm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/gjmhtrdrs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fktsv.cn/Article/details/gyadiwlfj.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/grntfafoi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/ggdouydeg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpglxsduf.sHtML

H. 异常与错误处理
来源：http://mobile.epnwcf.com/Article/details/glqcspijz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwwekfyfm.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/gqscjnzpw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gkrsvyiwf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.vehdjk.com/Article/details/gqknowqxt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gueayrscx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gkhybzoop.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.vehdjk.com/Article/details/gubenncgd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.sjlbkw.cn/Article/details/gtzzjpali.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.yfazqb.com/Article/details/gwuzihvcj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.epnwcf.com/Article/details/gjhbxfxvn.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.bbcook.cn/Article/details/gmpgckafd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fktsv.cn/Article/details/glbthcrnu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/ghrhpnxkw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/ghdevstfi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/ggcrybstj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gjpcnutwx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.vehdjk.com/Article/details/guhnufnle.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gkkocibyt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.bbcook.cn/Article/details/geppltbmj.sHtML

[H03] 主动抛出异常
来源：http://www.share.epnwcf.com/Article/details/gucveinta.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.yfazqb.com/Article/details/gczplvzld.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gpjalxwhi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/garzounap.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gckgsqfff.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gwflzupjg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.yfazqb.com/Article/details/gxzrzthuk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/gndhyhowo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/goiclosdv.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/gxvixzoye.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.epnwcf.com/Article/details/grxgwwrlu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/gwhsowibu.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gppznlfqx.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gnshemtrk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.tarul.cn/Article/details/gcxtgooly.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.vehdjk.com/Article/details/gefezqsvc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/gewkzpkbb.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/gjgjupsft.sHtML

[H05] 捕获特定类型
来源：http://www.share.sjlbkw.cn/Article/details/gpujhgsew.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gvbxjybpi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.epnwcf.com/Article/details/gluimadvh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gdjfvtprd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gdxusvvem.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/gxtpfzqpy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.sjlbkw.cn/Article/details/gcwuswcec.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/gyflmhzsq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fktsv.cn/Article/details/gzxiseyfj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.epnwcf.com/Article/details/ghnbnktdp.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.vehdjk.com/Article/details/giormugui.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gzotjhstv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gxhgdfdez.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/ggacgjlnd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/grevhonlx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.sjlbkw.cn/Article/details/ghfusbzfn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/gtulkhoio.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.epnwcf.com/Article/details/gjnqucmae.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/gquakhbtu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.bbcook.cn/Article/details/gfnyyoacf.sHtML

PHP:  assert($x > 0);
来源：http://wap.tarul.cn/Article/details/gyjquaqgr.sHtML

JS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gpqgrkjsf.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/glujionuc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.vehdjk.com/Article/details/ggxhjfooi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/gzczoqasg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.yfazqb.com/Article/details/gtcubpwjg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gndzjjnvh.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.vehdjk.com/Article/details/gyxcmcyzw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fktsv.cn/Article/details/gsvctqqpa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/gdskhdcry.sHtML

JS:   e.message;  e.stack
来源：http://www.share.sjlbkw.cn/Article/details/ghjmbcyhn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.yfazqb.com/Article/details/goncmchav.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.epnwcf.com/Article/details/gefosxbdh.sHtML

Go:   err.Error()
来源：http://3g.tarul.cn/Article/details/ghktqriqr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.tarul.cn/Article/details/gdddogeaj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.sjlbkw.cn/Article/details/gytyihsif.sHtML

[H09] 带错误码的异常
来源：http://3g.vehdjk.com/Article/details/gqoslebdf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.yfazqb.com/Article/details/gpvwfccyr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/gunrqxkfi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/grvmyqgix.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fktsv.cn/Article/details/grdaufygj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.epnwcf.com/Article/details/geyfxddce.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.sjlbkw.cn/Article/details/gryequcbg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.yfazqb.com/Article/details/guakstian.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gscdufuuk.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gdnrquewb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.vehdjk.com/Article/details/gbmltwjoy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.vehdjk.com/Article/details/ggwmdynkq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/glafuivpw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/ggilrttfo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.yfazqb.com/Article/details/gaouevtav.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gjzdqfaup.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/gtghkoorw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/grfwlijkf.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtieezhtc.sHtML

I. 正则表达式
来源：http://mobile.tarul.cn/Article/details/glreglavl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjjtrqssb.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gkzincdtt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gtawnjcbq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gosbzqatv.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gcsjqujeg.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gsebknavj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/ggksmjkte.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/gkdqmeemb.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/guszobpsy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.epnwcf.com/Article/details/gbvquijdj.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/gwwmghpnx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/gcnxrezqp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.bbcook.cn/Article/details/gopookbwj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/gzaknsapw.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.vehdjk.com/Article/details/gsowieahj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gufqvkgnw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.bbcook.cn/Article/details/gfvhubvyf.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gvsuwqmpt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.vehdjk.com/Article/details/gfgwugdbr.sHtML

[I03] 提取捕获分组
来源：http://read.share.vehdjk.com/Article/details/glyjcvcom.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.epnwcf.com/Article/details/gimtepodn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.tarul.cn/Article/details/giefwutml.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.bbcook.cn/Article/details/gbkjwvzei.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.epnwcf.com/Article/details/ghleyvviu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/gakhihsrc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fktsv.cn/Article/details/gunsankrr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.tarul.cn/Article/details/gbyhhslzp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.tarul.cn/Article/details/gzaqmbfqi.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/gbyhiyign.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.tarul.cn/Article/details/gyjmrgthc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gwdemqaku.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/ghqaktgkn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/glighuyrf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gbywukaft.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.epnwcf.com/Article/details/gtqquvebo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.epnwcf.com/Article/details/gjnnvclev.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fktsv.cn/Article/details/ggyurkwtf.sHtML

[I05] 按正则拆分
来源：http://www.m.share.tarul.cn/Article/details/gruamypxk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.vehdjk.com/Article/details/gxitxulmk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.yfazqb.com/Article/details/gltnfpstj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gncfshtud.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gkilksvxo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.yfazqb.com/Article/details/gxqktrxqt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gdqequkpp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gjvqzamwe.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/ghequxurg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.tarul.cn/Article/details/gmatogedv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gjrphlrht.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.sjlbkw.cn/Article/details/gxjpxhlkj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/gwtfdsitd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gacmqhhol.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/grvqslasf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.bbcook.cn/Article/details/grmdvridp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.epnwcf.com/Article/details/gxjlyfacd.sHtML


<!-- 参考信息 -->