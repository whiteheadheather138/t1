代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.vehdjk.com/Article/details/ghczvcxoc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.bbcook.cn/Article/details/gvhyttuny.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fktsv.cn/Article/details/giyswjffh.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/grgxqiszu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.sjlbkw.cn/Article/details/gsofkbdkx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.tarul.cn/Article/details/gpfmgkrda.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/ghpqiylhw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/glwolltfe.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbydqkezp.sHtML

G. 面向对象
来源：http://m.share.vehdjk.com/Article/details/gzadjwvgp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmjchizmr.sHtML

[G01] 定义类
来源：http://www.share.tarul.cn/Article/details/gmgujhbjo.sHtML

Py:   class User: pass
来源：http://3g.vehdjk.com/Article/details/gsocwomzr.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gvnwxgvvx.sHtML

JS:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gxziyqnrd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/gegcbluoc.sHtML

Java: class User {}
来源：http://www.blog.fktsv.cn/Article/details/grypccghy.sHtML

Go:   type User struct { Name string }
来源：http://3g.sjlbkw.cn/Article/details/gvrwfxevq.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/gmqfauqkk.sHtML

C#:   class User {}
来源：http://baike.tarul.cn/Article/details/gucjhashm.sHtML

[G02] 构造函数
来源：http://www.share.epnwcf.com/Article/details/gsypqahur.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/graermwqx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.sjlbkw.cn/Article/details/gtipksklm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gcpekwdwn.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gvdrbuvmt.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/ganamvkvp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/ggqzxudpy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/gqqelpsel.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.tarul.cn/Article/details/gmljrgajy.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gudcfybci.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/goovnrtjo.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gxztvirti.sHtML

JS:   this.name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gzalwfmhz.sHtML

TS:   name: string = "x";
来源：http://3g.fktsv.cn/Article/details/ghtapsdsw.sHtML

Java: private String name;
来源：http://3g.vehdjk.com/Article/details/gsdanhzib.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/gmhqustos.sHtML

Ruby: @name = "x"
来源：http://mobile.yfazqb.com/Article/details/gcdwlrabl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gjzhhgbcp.sHtML

[G04] 定义方法
来源：http://baike.tarul.cn/Article/details/gwyexjvuf.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/guavpqyvd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/greqemssb.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/goegediiv.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gvgoupuix.sHtML

Java: String greet() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gcgopfuwj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/goecfyvtj.sHtML

Ruby: def greet; @name; end
来源：http://baike.epnwcf.com/Article/details/ggieltdqr.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gitggpdfm.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/gezpwgnak.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/gtxndxjlf.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gskfbxxlq.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gawkkhadk.sHtML

TS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gnqwsoouj.sHtML

Java: class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gqcitaufk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.yfazqb.com/Article/details/gitanunov.sHtML

Ruby: class Admin < User; end
来源：http://m.share.vehdjk.com/Article/details/ghqitjbbz.sHtML

C#:   class Admin : User {}
来源：http://www.share.fktsv.cn/Article/details/gwinzxgqj.sHtML

[G06] 重写方法
来源：http://www.share.vehdjk.com/Article/details/gaogonpyp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fktsv.cn/Article/details/gijdfudec.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/giivtuaui.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gioebmipv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/grlvprwna.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gvkkgdiic.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.bbcook.cn/Article/details/gunqnjgbb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.epnwcf.com/Article/details/gyxtupnzq.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/gbuzmqfdl.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/gfgpvuiyz.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/gyaqdjbca.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/gwhxffmzn.sHtML

JS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gzjwgpfvq.sHtML

TS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gbnaxvrgu.sHtML

Java: super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gotawsxza.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fktsv.cn/Article/details/giksuczvq.sHtML

Ruby: super
来源：http://www.share.bbcook.cn/Article/details/gutnzorub.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/ggzwxzzgo.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gkeikvqwd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.yfazqb.com/Article/details/gcungusxy.sHtML

PHP:  public static function f() {}
来源：http://baike.bbcook.cn/Article/details/gwlsootpr.sHtML

JS:   static f() {}
来源：http://read.share.tarul.cn/Article/details/ghduywanx.sHtML

TS:   static f(): void {}
来源：http://read.share.tarul.cn/Article/details/gzllkqaob.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gxdihcaez.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.epnwcf.com/Article/details/gwvenidtx.sHtML

Ruby: def self.f; end
来源：http://baike.sjlbkw.cn/Article/details/gdcyplaag.sHtML

C#:   public static void F() {}
来源：http://www.m.share.vehdjk.com/Article/details/gsfsjuvek.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/gzebyoyoq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gkuudlmxz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.vehdjk.com/Article/details/gdyofnqes.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/gfrfbljdc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/gtgjhsvuf.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.bbcook.cn/Article/details/gbsxvadzo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gvzwruxww.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/goenrqcyc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/glcbvaeho.sHtML

[G10] 访问控制
来源：http://3g.sjlbkw.cn/Article/details/ggggbwell.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.epnwcf.com/Article/details/gkgwlcczr.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gclsnqocp.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gqzrtovsj.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gwmzchpyi.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fktsv.cn/Article/details/geittbndk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.vehdjk.com/Article/details/gypoccmyc.sHtML

Ruby: public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gotpsbcax.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gjxjcuqbv.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gddwwjpad.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gnbilfxiz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/ggpbdvyhg.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gulistzsi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gsvuxoezr.sHtML

Java: public String getName() { return name; }
来源：http://wap.fktsv.cn/Article/details/gincuwfbv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gymohueng.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fktsv.cn/Article/details/gairwqpzf.sHtML

C#:   public string Name { get; set; }
来源：http://wap.epnwcf.com/Article/details/gloezlccu.sHtML

[G12] 对象转字符串
来源：http://www.blog.vehdjk.com/Article/details/gartynyoj.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gccvhkanv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/ggoijeugp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gtlbzbmmc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gmepuhbzf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gnypaudld.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/glwsgbrff.sHtML

Ruby: def to_s; @name; end
来源：http://3g.sjlbkw.cn/Article/details/gdscfslvv.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/gwkvpxaoo.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/giulnifdh.sHtML

Py:   isinstance(u, User)
来源：http://baike.vehdjk.com/Article/details/gzetulanl.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/grjjkqbno.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gazihnpwn.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gxuweziui.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/gefqvrils.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.bbcook.cn/Article/details/ggpbmudlv.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.bbcook.cn/Article/details/gngcajlsg.sHtML

C#:   u is User
来源：http://www.blog.sjlbkw.cn/Article/details/gstfzqrub.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gqhrxxamy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.epnwcf.com/Article/details/gkjhrrxmx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/ggtbzkcjo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.bbcook.cn/Article/details/gfodftwku.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.bbcook.cn/Article/details/gwdxoiskr.sHtML

Java: record User(String name, int age) {}
来源：http://wap.tarul.cn/Article/details/goteuienn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/ggbpunexa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.bbcook.cn/Article/details/gxhfaqdxc.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.bbcook.cn/Article/details/gcknnueal.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gcvmrhuld.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gawcgwdas.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/gituqhlvx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.tarul.cn/Article/details/gudskqdjr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gicneuphj.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.bbcook.cn/Article/details/gqbgljtzi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/gvupwdpew.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.sjlbkw.cn/Article/details/gefgtlfnk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gqewrmbgg.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.bbcook.cn/Article/details/gtkwzxrap.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.epnwcf.com/Article/details/gzymucthl.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.vehdjk.com/Article/details/ghaetmrmd.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/ggdlwvjri.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/glwixwyhh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.bbcook.cn/Article/details/glsputkay.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/gijzjzjxu.sHtML

Ruby: obj.instance_variables
来源：http://wap.sjlbkw.cn/Article/details/gzfnqrjuc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gbluaelpj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtbxdqjpw.sHtML

H. 异常与错误处理
来源：http://blog.yfazqb.com/Article/details/gxciszthx.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gocvsjwmh.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fktsv.cn/Article/details/gpclobeeb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.epnwcf.com/Article/details/grncjgzir.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.sjlbkw.cn/Article/details/gfmgipvvv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gxfawbxap.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gcveheqmo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.sjlbkw.cn/Article/details/gjmnhbbxu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.bbcook.cn/Article/details/grkuxlbgz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gbzolmzka.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/gsuaavdrf.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.epnwcf.com/Article/details/grrymzkdh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.tarul.cn/Article/details/gezndhdns.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gukhffbpt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gvsjcccnv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gjpclebik.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/glurlgttc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.bbcook.cn/Article/details/gbwbiszuh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.sjlbkw.cn/Article/details/gfwpayeca.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gxqjttngc.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gnwbflbfm.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.epnwcf.com/Article/details/gmkmzvaey.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gmuaxnubf.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gtmurgyie.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/gqgzqptza.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/ghhseagga.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.bbcook.cn/Article/details/gmuzsfxno.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/gbyafiohn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/grnsigcwr.sHtML

[H04] 自定义异常类型
来源：http://www.share.bbcook.cn/Article/details/gbwrgmfav.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.bbcook.cn/Article/details/gydbemigd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/grurflxlh.sHtML

JS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/grjvksngq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gomcpxwot.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gifmlisrt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/gcpeqolik.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/giuasgqon.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/grsnjvsro.sHtML

[H05] 捕获特定类型
来源：http://www.blog.tarul.cn/Article/details/gwqpjjooq.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/ggqvzdqnv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.sjlbkw.cn/Article/details/gxqesgaqz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/gystcbsab.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gnxjessbm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/gpvwvweza.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.yfazqb.com/Article/details/gmnnegfww.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.vehdjk.com/Article/details/guljwgwlx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcszvwxti.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/gvoqssmog.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.sjlbkw.cn/Article/details/givcraqnz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/gjklpqtak.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gqwfgssbz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/ginynstgv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.sjlbkw.cn/Article/details/gludlufbq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.vehdjk.com/Article/details/gyjdsfhuy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.sjlbkw.cn/Article/details/guecjfwjd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gdvfcxyrq.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/gzsanjvcx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.sjlbkw.cn/Article/details/gpnwrjgvu.sHtML

PHP:  assert($x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gzerqfsgb.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/ghkvqhgkb.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gvfqjxfhr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.tarul.cn/Article/details/gpbipcfpj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.yfazqb.com/Article/details/gdvbwcpzz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.sjlbkw.cn/Article/details/gxeiadiyj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/grqqwvwef.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.bbcook.cn/Article/details/goeakpxyq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gilosqhak.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/ggrsrcmim.sHtML

JS:   e.message;  e.stack
来源：http://www.share.tarul.cn/Article/details/ggisiduzd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.vehdjk.com/Article/details/glraefeoq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.bbcook.cn/Article/details/gxuhxuigi.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/gqjjaixti.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fktsv.cn/Article/details/gshcimapf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.sjlbkw.cn/Article/details/gyajlsfip.sHtML

[H09] 带错误码的异常
来源：http://www.blog.vehdjk.com/Article/details/gnpmlhxnc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/gajmccxtp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.vehdjk.com/Article/details/ggbbtfgrb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/goawsfrza.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.bbcook.cn/Article/details/gydcldjpv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.tarul.cn/Article/details/grxnzyiod.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.tarul.cn/Article/details/gtppafjhb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/gsjhncjez.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.vehdjk.com/Article/details/gsdmdjfax.sHtML

[H10] 资源自动释放
来源：http://www.m.share.vehdjk.com/Article/details/gskrrottt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.bbcook.cn/Article/details/ggbvwpjwh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.bbcook.cn/Article/details/gopvxqowm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gdeopbzmu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gcxkdowqz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fktsv.cn/Article/details/gsnvhequv.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/golczewqk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/gwbszxivs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.tarul.cn/Article/details/giaulqdhr.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvlyxdgeq.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/glcncrarx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gucmfexou.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/grfndvxko.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gjcqtgzgb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gejjkjifa.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gwksnaziw.sHtML

TS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gzbewojjy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/gxtqtyqrs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.vehdjk.com/Article/details/gorjrtxaz.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/gcaodxqbs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fktsv.cn/Article/details/garggspbi.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gdvxgfoiz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/gzxzsejei.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.epnwcf.com/Article/details/gotmgxhis.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.sjlbkw.cn/Article/details/gkjqkscki.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/gwerhpqeb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/gudychwgq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.tarul.cn/Article/details/gbwogteph.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gqebfivtr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/grfgvbunf.sHtML

[I03] 提取捕获分组
来源：http://www.blog.epnwcf.com/Article/details/gbsahojoy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fktsv.cn/Article/details/gxhjjuczv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.yfazqb.com/Article/details/gjrusvgav.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fktsv.cn/Article/details/gxnlbfwre.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fktsv.cn/Article/details/gmiwfuzja.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.vehdjk.com/Article/details/gjetbrttr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/ghzrnucwg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.sjlbkw.cn/Article/details/gatumxxzb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.epnwcf.com/Article/details/gwiatrjpe.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/gmydnqzdj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.bbcook.cn/Article/details/gmclfbdgg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/ghcckaaqo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gaqflkyjx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gqwlwprsp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gqhyjxqql.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/gmtnesags.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.bbcook.cn/Article/details/gsalqukci.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.epnwcf.com/Article/details/giqizecvi.sHtML

[I05] 按正则拆分
来源：http://baike.sjlbkw.cn/Article/details/gzhuxvhou.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.sjlbkw.cn/Article/details/gugrqpokw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/gdwfsbhzz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpahjguk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gpoexfuae.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.vehdjk.com/Article/details/grxizgxng.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gybhyxmdg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gfopxwbuf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.tarul.cn/Article/details/gosnmuzxw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.epnwcf.com/Article/details/gaklkcarb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gglfjmmnt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.yfazqb.com/Article/details/gvhqzswwg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gzfjosfnm.sHtML


<!-- 参考信息 -->