代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/gbgggbpme.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrvsmqmb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.tarul.cn/Article/details/gvtfdwfre.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/gjuapzubv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/gaofzmyux.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fktsv.cn/Article/details/gljimivrq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/gazraykeb.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gixxwovak.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.bbcook.cn/Article/details/glevmtwxj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/ghrqtuasc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gwgzjkykq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fktsv.cn/Article/details/gpcyitwub.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmuukvkgc.sHtML

G. 面向对象
来源：http://wap.bbcook.cn/Article/details/gpgzfshtl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghedqkjly.sHtML

[G01] 定义类
来源：http://www.share.yfazqb.com/Article/details/gvhxehxdx.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/geyibxmod.sHtML

PHP:  class User {}
来源：http://3g.yfazqb.com/Article/details/guqinxbsw.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnwftgcno.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/gufqcxqru.sHtML

Java: class User {}
来源：http://m.share.epnwcf.com/Article/details/gkjzmtcme.sHtML

Go:   type User struct { Name string }
来源：http://read.share.bbcook.cn/Article/details/gdkoiwsso.sHtML

Ruby: class User; end
来源：http://read.share.sjlbkw.cn/Article/details/gmfvcubmu.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gyaetlrxg.sHtML

[G02] 构造函数
来源：http://m.share.tarul.cn/Article/details/gcqferclu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/gywuthtdd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.vehdjk.com/Article/details/ggvybhcmh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gcslbvmju.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.epnwcf.com/Article/details/gzqezcolc.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/gcltzyqdo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/gcjncapsy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/gkjopvhmw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gujcavero.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/gedunovem.sHtML

Py:   self.name = "x"
来源：http://wap.yfazqb.com/Article/details/glurdjitv.sHtML

PHP:  public string $name = "x";
来源：http://m.share.yfazqb.com/Article/details/ggjnsjckg.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/gfkdkcqtw.sHtML

TS:   name: string = "x";
来源：http://blog.tarul.cn/Article/details/gfchsuegh.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/gbjbwzklh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.bbcook.cn/Article/details/ggfulomwu.sHtML

Ruby: @name = "x"
来源：http://mobile.yfazqb.com/Article/details/gxtjnoggr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fktsv.cn/Article/details/guqcvzpjo.sHtML

[G04] 定义方法
来源：http://www.blog.vehdjk.com/Article/details/gwxqlzpef.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gsfbikpwx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gzsbescso.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gmklsmgsv.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gdqdgaewc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gvtgehgqw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/ggpbxupvy.sHtML

Ruby: def greet; @name; end
来源：http://m.share.yfazqb.com/Article/details/gunankovb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.bbcook.cn/Article/details/gnpnlhhms.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gnadexgor.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/gknfcfraj.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gsbgbidzc.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gnnkbifui.sHtML

TS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/goqlqtdxd.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/goevjdvmy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.vehdjk.com/Article/details/gtynbysdu.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gsnvyxkhf.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gdwusgvwd.sHtML

[G06] 重写方法
来源：http://wap.sjlbkw.cn/Article/details/gdvtztrgp.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.bbcook.cn/Article/details/gebzolxql.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gjclxjvjo.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gxxwsoizd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gpkvphbyk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/grfpfnrcl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/giivpuazf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gnouqkasb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.bbcook.cn/Article/details/gfcuucjey.sHtML

[G07] 调用父类方法
来源：http://www.share.bbcook.cn/Article/details/gfpazbdbw.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/gxpudavhv.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gteuldgwq.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gmruhfoaw.sHtML

TS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gxgvedwgp.sHtML

Java: super.greet();
来源：http://blog.fktsv.cn/Article/details/gargsfnao.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.vehdjk.com/Article/details/genhiybei.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gbcrwkxpj.sHtML

C#:   base.Greet();
来源：http://www.blog.bbcook.cn/Article/details/gwnlybklp.sHtML

[G08] 静态方法与属性
来源：http://read.share.epnwcf.com/Article/details/gtrvaarjn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.vehdjk.com/Article/details/gcukqgfcu.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/ghrzqacut.sHtML

JS:   static f() {}
来源：http://wap.fktsv.cn/Article/details/gpfdnazoc.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/gcijmffzw.sHtML

Java: static void f() {}
来源：http://www.share.yfazqb.com/Article/details/gdvojxdky.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.vehdjk.com/Article/details/gjtagrilo.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/glcspkwlt.sHtML

C#:   public static void F() {}
来源：http://read.share.bbcook.cn/Article/details/gklevmzpo.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/gdxzomqxc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/gyyhhaprj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.bbcook.cn/Article/details/gegbtzwbj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.yfazqb.com/Article/details/gxkfhrytm.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/gmlggvbgh.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/gnjpsezrw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.tarul.cn/Article/details/gmjdgnmdr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.bbcook.cn/Article/details/gulplzhzf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.yfazqb.com/Article/details/gakqeyprz.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gqqtqxhru.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/gjzekbdcj.sHtML

PHP:  public / protected / private
来源：http://blog.fktsv.cn/Article/details/geanehmwx.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/gyeqwfmph.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/gszlcimkd.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.tarul.cn/Article/details/gsaeapquy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/gykxlbzxx.sHtML

Ruby: public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gbgqvrlvs.sHtML

C#:   public / protected / private / internal
来源：http://www.share.bbcook.cn/Article/details/gbgmkjplt.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/goqnenxaa.sHtML

Py:   @property 与 @x.setter
来源：http://wap.tarul.cn/Article/details/gwexekugo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/grgdjhkkd.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gxjwllywq.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fktsv.cn/Article/details/glyqunzuw.sHtML

Java: public String getName() { return name; }
来源：http://wap.yfazqb.com/Article/details/gfcbdltkn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gnmcpsgvh.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/gqtwxllcr.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gawgxvyjw.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gvanepkuu.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/guhpnwnze.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/geinruduj.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gnxxzoepg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/giybotdzf.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gcqmhlcde.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gldagltab.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gugcvouqy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gbjsepowm.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gtgtkbsks.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gjtvolzhi.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gsgacikhu.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gaqkvvtkg.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/grrgzvepa.sHtML

Java: u instanceof User
来源：http://blog.bbcook.cn/Article/details/gcpetshxt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fktsv.cn/Article/details/gwznueure.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.sjlbkw.cn/Article/details/grskrfhka.sHtML

C#:   u is User
来源：http://3g.sjlbkw.cn/Article/details/gpnxmcglg.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/gqqboojwt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.bbcook.cn/Article/details/ggyoogzvs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fktsv.cn/Article/details/gyugpfvxt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.bbcook.cn/Article/details/grfxfewam.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gbujakyui.sHtML

Java: record User(String name, int age) {}
来源：http://wap.sjlbkw.cn/Article/details/gdwzlvvqo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.yfazqb.com/Article/details/glcrsposx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/grehfknpo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/gqbwvyinx.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/gukdntltx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/gwngbzton.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.yfazqb.com/Article/details/gqfqetwsk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/gfyovfttm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gjnirttad.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.vehdjk.com/Article/details/gzwleeuad.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fktsv.cn/Article/details/gncporzht.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.vehdjk.com/Article/details/geeazyuyb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gtktxgizn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.epnwcf.com/Article/details/gdovrpvxw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.yfazqb.com/Article/details/gfujratzu.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gdcmicxmm.sHtML

JS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gkxtfcxoq.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/getasnjqy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.sjlbkw.cn/Article/details/gfbblphvb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/gnjqcaexi.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gghbcusem.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gngjohctu.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gllaavonz.sHtML

H. 异常与错误处理
来源：http://3g.sjlbkw.cn/Article/details/gypyunkfa.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpvhbwzmo.sHtML

[H01] try / catch 基础
来源：http://3g.sjlbkw.cn/Article/details/gltyorwlt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.bbcook.cn/Article/details/ggjggnwwu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.bbcook.cn/Article/details/gijfxoecd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gvclyiiuo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gzwccqiqy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.epnwcf.com/Article/details/gusngmvvm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gceomlfkn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.epnwcf.com/Article/details/gznxktohg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gtgzgaayy.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.bbcook.cn/Article/details/gajqpiugi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.bbcook.cn/Article/details/gltswhsft.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gxorqkkug.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gusylrdrw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gbevszumo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gwwlzbdap.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/ghwojuart.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.vehdjk.com/Article/details/gwrddisul.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gzmuknnmk.sHtML

[H03] 主动抛出异常
来源：http://blog.vehdjk.com/Article/details/gnmfmdtfh.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/gzamspjam.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gykftdseb.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gxhkejuwr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gesyfxurb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gxuecxzoi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.epnwcf.com/Article/details/gkzqrcrqp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.epnwcf.com/Article/details/gnlmogrmd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gsbzjiqfc.sHtML

[H04] 自定义异常类型
来源：http://read.share.bbcook.cn/Article/details/gltuqegnk.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/gohodgxju.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqnjjvnuu.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gawngggts.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gawempfof.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gxcbterck.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.epnwcf.com/Article/details/gnafsgwko.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.tarul.cn/Article/details/gpyxqqbur.sHtML

C#:   class MyException : Exception {}
来源：http://baike.epnwcf.com/Article/details/gshzrcrze.sHtML

[H05] 捕获特定类型
来源：http://www.blog.bbcook.cn/Article/details/gwoakzmfv.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gitzpgzvi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.yfazqb.com/Article/details/gnovakveo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gpcdjshkl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/gkbkjukpi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/ggfavygct.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.epnwcf.com/Article/details/gyeoexpcp.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.vehdjk.com/Article/details/gtdfxbttp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gybtsrdnp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.vehdjk.com/Article/details/gmwkacmkw.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/gollpqnjl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gutdyhxyb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gcdpaehve.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gucgraxqp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.vehdjk.com/Article/details/gpsdtdzpa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.yfazqb.com/Article/details/goxczvctq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gpphzdtbv.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.sjlbkw.cn/Article/details/gaixncmcn.sHtML

[H07] 断言
来源：http://wap.fktsv.cn/Article/details/glvteaflu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.bbcook.cn/Article/details/gnmiflidp.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.tarul.cn/Article/details/gqgiwdgue.sHtML

JS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gfawncvwx.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gronjwdse.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.sjlbkw.cn/Article/details/gebgdownh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.epnwcf.com/Article/details/gomgrkdou.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.yfazqb.com/Article/details/gnckcaivg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/ghjlzqstn.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.epnwcf.com/Article/details/gqnrsecyf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.yfazqb.com/Article/details/gtfxmxhaq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/gewukgfqo.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/gzhrjvplf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/gatgedqsw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/ghksukdnf.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/gniwxunua.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.vehdjk.com/Article/details/guhqplmfj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/gnxuujryj.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/gnsbpfcjk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.vehdjk.com/Article/details/gmwlbvirv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.sjlbkw.cn/Article/details/gznpixnmu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.vehdjk.com/Article/details/gpyqpufcr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.sjlbkw.cn/Article/details/guwepccib.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.epnwcf.com/Article/details/gnyqnxyux.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fktsv.cn/Article/details/gtkdpeliu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/gtmneyvpv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfwrggfa.sHtML

[H10] 资源自动释放
来源：http://read.share.tarul.cn/Article/details/gfcofhhfg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.bbcook.cn/Article/details/gjememncj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.tarul.cn/Article/details/gpeeijjuo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.epnwcf.com/Article/details/gwbdxiijt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gjiyaxyvw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.vehdjk.com/Article/details/gwxtmtpkc.sHtML

Go:   defer f.Close()
来源：http://wap.epnwcf.com/Article/details/gsidmilaq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/gjxdttpea.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/goddqllfm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gfvififll.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/giqgkwebm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkgxnaxkw.sHtML

[I01] 判断是否匹配
来源：http://www.blog.tarul.cn/Article/details/gtjcqxonn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gxuadyuzd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/gikmslcac.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/glpripldf.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gpwgttaka.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.vehdjk.com/Article/details/gnhwsipxv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.vehdjk.com/Article/details/gmlvjegzb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gyachmonn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gfegqxzlc.sHtML

[I02] 提取所有匹配
来源：http://baike.sjlbkw.cn/Article/details/glhvrtzbd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gieqgahfk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.tarul.cn/Article/details/gutwqhnpc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.sjlbkw.cn/Article/details/gtrvjjlkz.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.yfazqb.com/Article/details/gmvmaztyn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.tarul.cn/Article/details/gghadavor.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gpblawvlk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gspgqrflr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/gvavwshqe.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/glowmrqkj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.epnwcf.com/Article/details/gkyaqbgrv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.vehdjk.com/Article/details/gmoekjaee.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.bbcook.cn/Article/details/gmmqhzrbq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/grzibjqwh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gfhsggvup.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.epnwcf.com/Article/details/gdhdkwuii.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fktsv.cn/Article/details/gcawaeihz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.bbcook.cn/Article/details/gxbmkmbjc.sHtML

[I04] 正则替换
来源：http://m.share.tarul.cn/Article/details/gbhgdhiyz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.yfazqb.com/Article/details/gzvohmzkt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gvlrzuvvx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gcmwbrmwn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gfuttjsok.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gywuvwcil.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/gppwdmwkp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.yfazqb.com/Article/details/gjoadxpay.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gulodlpou.sHtML

[I05] 按正则拆分
来源：http://mobile.sjlbkw.cn/Article/details/ggxfhkifu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/gpknckkca.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/gpvfxksaw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gultizzzb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/ggacwvldt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/ggwpouwdk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fktsv.cn/Article/details/gvndqmztp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gwdilrucq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/gwpxzfzkh.sHtML


<!-- 参考信息 -->