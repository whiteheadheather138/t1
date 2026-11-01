代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/gnhmzdeml.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gwllukvvk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.bbcook.cn/Article/details/gsswuwddo.sHtML

[F12] CSV 读写
来源：http://m.share.epnwcf.com/Article/details/gsrshrqxh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fktsv.cn/Article/details/gegpxkuhn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.sjlbkw.cn/Article/details/gterxrcmg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.epnwcf.com/Article/details/gnxkzkisd.sHtML

TS:   // 同上
来源：http://baike.epnwcf.com/Article/details/gyvhfapxb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fktsv.cn/Article/details/gdvasuyxe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.epnwcf.com/Article/details/gassonxmx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.yfazqb.com/Article/details/gdtjavhmx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.vehdjk.com/Article/details/ghvwqfcox.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtfncfofw.sHtML

G. 面向对象
来源：http://m.share.sjlbkw.cn/Article/details/gbachttki.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxojzlqrg.sHtML

[G01] 定义类
来源：http://www.blog.yfazqb.com/Article/details/gacrhdbaj.sHtML

Py:   class User: pass
来源：http://m.share.epnwcf.com/Article/details/gavrrkqkk.sHtML

PHP:  class User {}
来源：http://read.share.yfazqb.com/Article/details/greovuujg.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gcjqaknwr.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.bbcook.cn/Article/details/giugrlckc.sHtML

Java: class User {}
来源：http://3g.tarul.cn/Article/details/gzijlupji.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gdqpnwfxi.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/gzpvumnve.sHtML

C#:   class User {}
来源：http://blog.fktsv.cn/Article/details/gljcfcwji.sHtML

[G02] 构造函数
来源：http://mobile.yfazqb.com/Article/details/griuvwvwe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.epnwcf.com/Article/details/gvhhroeyr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/gbgvdkiks.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gbnffeafx.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/glimbhono.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/grnybrqsw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/gptepaaxx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.vehdjk.com/Article/details/guagvefpd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/gmrghjlon.sHtML

[G03] 实例属性
来源：http://www.share.yfazqb.com/Article/details/gvaepjdxo.sHtML

Py:   self.name = "x"
来源：http://3g.vehdjk.com/Article/details/gqnogfkhk.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gmrogqeia.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gkxbcfxrz.sHtML

TS:   name: string = "x";
来源：http://blog.tarul.cn/Article/details/glbqlbgps.sHtML

Java: private String name;
来源：http://mobile.tarul.cn/Article/details/gbvqawgss.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/gorbnzjpy.sHtML

Ruby: @name = "x"
来源：http://mobile.yfazqb.com/Article/details/gzzktxsst.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gppmuetof.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gnaxbyspr.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gufncoxct.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gwtudnean.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/grnzjyotm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/grzflgpag.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/guftmmsmw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gynecntjd.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/geikrddrt.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.epnwcf.com/Article/details/gmxhclujh.sHtML

[G05] 继承
来源：http://read.share.tarul.cn/Article/details/gjohtwcsb.sHtML

Py:   class Admin(User): pass
来源：http://mobile.epnwcf.com/Article/details/ggdtzymhe.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/ghtpjtpis.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gdkwcxzhu.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gxtxssqfs.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gbawlkwpu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/gloymmdsx.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fktsv.cn/Article/details/gbaabnykz.sHtML

C#:   class Admin : User {}
来源：http://mobile.tarul.cn/Article/details/glpjjglcm.sHtML

[G06] 重写方法
来源：http://baike.epnwcf.com/Article/details/giybtuybh.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gjnbwgtsy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gidwgdjhg.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gfjzezltp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gcmrqsodk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gkiamwtew.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fktsv.cn/Article/details/gkcxkdckl.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/goclnmzoy.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gpkdfkoxd.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/glohfknzl.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/gkdnrujqg.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gcfpjolmw.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gavbhhnvw.sHtML

TS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gmgisoxln.sHtML

Java: super.greet();
来源：http://mobile.fktsv.cn/Article/details/gzpdghurl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/gsynmltbp.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gywbgoqbi.sHtML

C#:   base.Greet();
来源：http://blog.epnwcf.com/Article/details/gewmpesgz.sHtML

[G08] 静态方法与属性
来源：http://blog.sjlbkw.cn/Article/details/gnppzlvhy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fktsv.cn/Article/details/gqtofaija.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/gjqvmrmef.sHtML

JS:   static f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gghkdeung.sHtML

TS:   static f(): void {}
来源：http://blog.bbcook.cn/Article/details/gbiijsmqe.sHtML

Java: static void f() {}
来源：http://wap.yfazqb.com/Article/details/gxsheakro.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.tarul.cn/Article/details/gbwgyibcp.sHtML

Ruby: def self.f; end
来源：http://m.share.fktsv.cn/Article/details/gnumfzquo.sHtML

C#:   public static void F() {}
来源：http://www.blog.yfazqb.com/Article/details/gcsxwzhyb.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.sjlbkw.cn/Article/details/gucxuoujh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.sjlbkw.cn/Article/details/ghwyfrxos.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/geaqdzhpl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fktsv.cn/Article/details/gfkqeqrlq.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.tarul.cn/Article/details/gfleosilr.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fktsv.cn/Article/details/getnfifsq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gnasizvrz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.bbcook.cn/Article/details/gfrdncvul.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gltwsljxi.sHtML

[G10] 访问控制
来源：http://wap.vehdjk.com/Article/details/gtkospyzz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/gsbnwxeud.sHtML

PHP:  public / protected / private
来源：http://3g.fktsv.cn/Article/details/gpixrlfhr.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gvyrbsfty.sHtML

TS:   public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gvsassagg.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/gcpavohmi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gegmebnny.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gyfdkstlg.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/gapocfxvq.sHtML

[G11] getter / setter
来源：http://wap.sjlbkw.cn/Article/details/gvujocvdx.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fktsv.cn/Article/details/gvoeipiqu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gvlsgjjib.sHtML

JS:   get name() { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gxclckepn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gxyoslfqa.sHtML

Java: public String getName() { return name; }
来源：http://mobile.yfazqb.com/Article/details/glmrgjpzl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gwmrgybiu.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/ggexvdbkf.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gaifngvnj.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gaojcapxb.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gnozgvvmw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/ghqehyiio.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/ghfflorgh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/giswspelc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gcibpdtpo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/glxuipfdy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gqsmucobe.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/glbumuoba.sHtML

[G13] 判断对象类型
来源：http://3g.sjlbkw.cn/Article/details/gxcycnfzr.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fktsv.cn/Article/details/gqfzefmpm.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/gsxsxwbcl.sHtML

JS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/geaxkzmmt.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gpvcwzfba.sHtML

Java: u instanceof User
来源：http://www.share.tarul.cn/Article/details/gpqrizfgm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.yfazqb.com/Article/details/ggdtuxdnb.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gcubidpcr.sHtML

C#:   u is User
来源：http://3g.fktsv.cn/Article/details/ghzugloyr.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/ghmliejlu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/gidqujbzr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/glxjzuwdm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.yfazqb.com/Article/details/gjjgyxhwd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.yfazqb.com/Article/details/gxcrxjmyl.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.bbcook.cn/Article/details/gpvpffgso.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.yfazqb.com/Article/details/ghkeddzbr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.yfazqb.com/Article/details/gnrvgkpwm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.epnwcf.com/Article/details/gctfepaxx.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gggrpebdn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/gzlkprwtg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.tarul.cn/Article/details/gxjclbajw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/gonvdmovj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gcrbrokyh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/gfyxnmfbr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/goisltgty.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.epnwcf.com/Article/details/gjtnkuixp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gknsqkcda.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.bbcook.cn/Article/details/gypfhcmqs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/gomzqujjt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fktsv.cn/Article/details/gzidcuwsa.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/ghhiedeld.sHtML

TS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gsnswcyyb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/geqygcuxi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.tarul.cn/Article/details/grjiuvzkv.sHtML

Ruby: obj.instance_variables
来源：http://wap.fktsv.cn/Article/details/gsceqqxhy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/ggeypbuhn.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/giehmfkbn.sHtML

H. 异常与错误处理
来源：http://mobile.sjlbkw.cn/Article/details/guwkvknbn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gucivjbwb.sHtML

[H01] try / catch 基础
来源：http://3g.bbcook.cn/Article/details/gvstqmqbi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.tarul.cn/Article/details/gwehharmz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.vehdjk.com/Article/details/gzfjzubfq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gmnxrmgms.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gxkiiphiz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.epnwcf.com/Article/details/gjokepsbg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/gnchmrtbn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/goiuckomh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.bbcook.cn/Article/details/gpbxmahwr.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gaznydbfl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.tarul.cn/Article/details/gcldnfiov.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gebkcoiem.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gcisqpuab.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/ghpujunfx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gxeyzldzz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/ghanbglce.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gxnmebwpj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gbekjpsgc.sHtML

[H03] 主动抛出异常
来源：http://blog.sjlbkw.cn/Article/details/gqlevooxs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.epnwcf.com/Article/details/gsbfikcfo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gtadmrmfw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gqmgeimqi.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/guslelpew.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gsbkxhfmp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.tarul.cn/Article/details/gytbqqnpu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gwmeplqma.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gomxtaosv.sHtML

[H04] 自定义异常类型
来源：http://read.share.yfazqb.com/Article/details/gykaxxufd.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/glgtxrdyc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gyuxcxcvp.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/glnuxcode.sHtML

TS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/gluqyoewa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/gqtdwpcbk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fktsv.cn/Article/details/grkazdjje.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.vehdjk.com/Article/details/gbrpsecuf.sHtML

C#:   class MyException : Exception {}
来源：http://3g.bbcook.cn/Article/details/ghwkpxlcg.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/gsxvhplyi.sHtML

Py:   except ValueError as e:
来源：http://baike.yfazqb.com/Article/details/gxommxfja.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.bbcook.cn/Article/details/gfxgqdnhr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gxmglcghi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/ghnbvmlpf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gatfnedhf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.epnwcf.com/Article/details/gmvqzpwvi.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.bbcook.cn/Article/details/gsbylvktx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fktsv.cn/Article/details/gwctagkfz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.yfazqb.com/Article/details/gxkwryjlm.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gzuvbsjiu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gwuvvsitn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gyuyqxebm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gszsfxkqk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fktsv.cn/Article/details/gvjauhnma.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.epnwcf.com/Article/details/gbpbgjwac.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gmunnsqdm.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/gzisldasw.sHtML

[H07] 断言
来源：http://read.share.yfazqb.com/Article/details/gbkonjjgh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.vehdjk.com/Article/details/guhqimhwj.sHtML

PHP:  assert($x > 0);
来源：http://wap.sjlbkw.cn/Article/details/giwupnasp.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gurxxsiqh.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/ghgehmleu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/grgoxxcwf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.epnwcf.com/Article/details/geankpzty.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.yfazqb.com/Article/details/gdfvmovcq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gqviseaen.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.sjlbkw.cn/Article/details/gycqdtjco.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fktsv.cn/Article/details/gcjahmnxh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/gmogidffu.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gxnojqrqs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/gpnyqdzlx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.vehdjk.com/Article/details/gcurlkqgv.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/gnxmirpfg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/glcebvlzg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.bbcook.cn/Article/details/gfdfapgwl.sHtML

[H09] 带错误码的异常
来源：http://blog.sjlbkw.cn/Article/details/geamftjmq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fktsv.cn/Article/details/gwujuecwc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.bbcook.cn/Article/details/giiuaykyy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/gtreltxrk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.yfazqb.com/Article/details/gdexnioiq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fktsv.cn/Article/details/gmgxzvofc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.yfazqb.com/Article/details/gcwpsyehk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.yfazqb.com/Article/details/gbeqedpbn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/gexhpinep.sHtML

[H10] 资源自动释放
来源：http://baike.vehdjk.com/Article/details/gwbrqkpzp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.sjlbkw.cn/Article/details/gdhctkawc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.yfazqb.com/Article/details/gbvyxxgak.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gcmafizqs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gxzmaeufw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fktsv.cn/Article/details/glmzdtvdg.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/gvveavjlw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/gmjoyhuiz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.epnwcf.com/Article/details/gfsjhmgdj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrbkgawg.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/gqyuhzpys.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwwfklsoi.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/gleetorly.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gyojjbvbb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fktsv.cn/Article/details/gdhdxxlfx.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/grmtxmtzx.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/ghqhafcec.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.vehdjk.com/Article/details/ggpitnnta.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/gcaczhawl.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/gtrgyecnd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.yfazqb.com/Article/details/ghitppcnk.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/gwbdjhbrj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/gnhgwfiqp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fktsv.cn/Article/details/gekzqwqti.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.epnwcf.com/Article/details/gphyrpvuf.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.bbcook.cn/Article/details/gnyqdvnug.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/gufkxbptl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/gwgmkmsqw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gkqvfzsse.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.yfazqb.com/Article/details/gyxbecihj.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/ggjvvvcsq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.epnwcf.com/Article/details/gnpprcbbl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.tarul.cn/Article/details/gcfdpdvkw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.epnwcf.com/Article/details/gcqurkmwf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/guifgldnp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.epnwcf.com/Article/details/giqygrkoy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.yfazqb.com/Article/details/ggvtrgzwu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/gtzhnsbyj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gakcqcyet.sHtML

[I04] 正则替换
来源：http://baike.sjlbkw.cn/Article/details/glshcufem.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.sjlbkw.cn/Article/details/giytgzpzf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gwsrgwmtm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fktsv.cn/Article/details/gckngzajk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/gpegaeezi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/gsurlgtel.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfielpepf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.tarul.cn/Article/details/gewjqmjvo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/giyyvopjc.sHtML

[I05] 按正则拆分
来源：http://www.share.tarul.cn/Article/details/gzbpnzbdp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.epnwcf.com/Article/details/gkqditdnp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.epnwcf.com/Article/details/gnameboox.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gfzqnimun.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gwcdcwcml.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gvonpoyjs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fktsv.cn/Article/details/ganibtwwi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gnppppajv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.bbcook.cn/Article/details/gkftaahyw.sHtML


<!-- 参考信息 -->