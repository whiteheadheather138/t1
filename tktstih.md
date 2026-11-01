代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/gshfstvtq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/ggupekpsx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.bbcook.cn/Article/details/gebieugpi.sHtML

[F12] CSV 读写
来源：http://read.share.tarul.cn/Article/details/gwxziugwq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.sjlbkw.cn/Article/details/gjyhkmikj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.yfazqb.com/Article/details/gikyavefu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.bbcook.cn/Article/details/gwsjsozcq.sHtML

TS:   // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gfdztxgxv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gebvpluty.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.sjlbkw.cn/Article/details/gvmjfcvtc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fktsv.cn/Article/details/gkpsfdarc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.epnwcf.com/Article/details/gcpvzsqoc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfyilfzok.sHtML

G. 面向对象
来源：http://www.share.vehdjk.com/Article/details/gaffdezvu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grbfxhioz.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/gxugknocu.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/gniqjbtjw.sHtML

PHP:  class User {}
来源：http://baike.fktsv.cn/Article/details/ghyfyjeru.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/ggfmevkwn.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/gyzskuqdf.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/glatkmkjp.sHtML

Go:   type User struct { Name string }
来源：http://www.share.sjlbkw.cn/Article/details/gmlsovynt.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gfdtchdya.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/guabwriic.sHtML

[G02] 构造函数
来源：http://www.blog.tarul.cn/Article/details/govvhzeyl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/goapnlsrb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/gljmnymfw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gntmpfxxc.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/ghtjpqblg.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gsfemxhch.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.yfazqb.com/Article/details/gxvyoqsnp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.bbcook.cn/Article/details/giqapkvmc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gqxkhudbh.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/guzxsqtxv.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gupdbutca.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/giypwqmsr.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/gihigxqmd.sHtML

TS:   name: string = "x";
来源：http://www.share.fktsv.cn/Article/details/ghawnkzwu.sHtML

Java: private String name;
来源：http://m.share.tarul.cn/Article/details/gskatrmsc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/ghxxwetct.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/gmjbplapq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gifysdcui.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/gbokyyvro.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gaqtuufju.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gbltcpvmk.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gwbqdtwpw.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/ggscabjgy.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gbyjltfjr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/geveanxjc.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gmpelmmhf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.tarul.cn/Article/details/gohletigb.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/geybvfqme.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.epnwcf.com/Article/details/gdxsnnybq.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gdhtjvher.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gsamowubm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gejeclufu.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gezzhrunf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gfhjbykjb.sHtML

Ruby: class Admin < User; end
来源：http://mobile.yfazqb.com/Article/details/guhnnhtmj.sHtML

C#:   class Admin : User {}
来源：http://3g.vehdjk.com/Article/details/gnyzbroti.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/gepglaiaj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/gvotisvfy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/ggeupbzrl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gibctecte.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/glovnvvtq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gasitibiu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/gmrxcwtnl.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.yfazqb.com/Article/details/gphtsyihu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fktsv.cn/Article/details/gpqwnerpt.sHtML

[G07] 调用父类方法
来源：http://baike.bbcook.cn/Article/details/gxwvgygai.sHtML

Py:   super().greet()
来源：http://www.m.share.fktsv.cn/Article/details/gxpvojyuh.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gvfdqhywq.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gjvvtvxec.sHtML

TS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gigjvedpq.sHtML

Java: super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gzkbtrtwo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoxbigde.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/giyoibbsh.sHtML

C#:   base.Greet();
来源：http://www.m.share.bbcook.cn/Article/details/gmmhddgik.sHtML

[G08] 静态方法与属性
来源：http://wap.vehdjk.com/Article/details/ggehzpllo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/gzqspexem.sHtML

PHP:  public static function f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gkjrzmqen.sHtML

JS:   static f() {}
来源：http://www.blog.yfazqb.com/Article/details/gflggtink.sHtML

TS:   static f(): void {}
来源：http://blog.tarul.cn/Article/details/grsrjdzef.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/gewqsftyu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/gpxzpxftf.sHtML

Ruby: def self.f; end
来源：http://wap.sjlbkw.cn/Article/details/gylozbwio.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/glvjgveek.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gqkkkqunk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/gvekzqeia.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gzvzasvdn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gwdqtxclq.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/glicjxpyc.sHtML

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/gyduznxad.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.vehdjk.com/Article/details/gpnuunnup.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.vehdjk.com/Article/details/gyopxmpdf.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fktsv.cn/Article/details/gobvubiwd.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gqihfhifh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gqsptctqg.sHtML

PHP:  public / protected / private
来源：http://wap.yfazqb.com/Article/details/gryuoexlc.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/guzvxjjcr.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gziaoyngi.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/ghggiftzq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/gsawjlngc.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gwdxkucpk.sHtML

C#:   public / protected / private / internal
来源：http://3g.bbcook.cn/Article/details/gtnkyfybl.sHtML

[G11] getter / setter
来源：http://www.blog.sjlbkw.cn/Article/details/gxokwnwvy.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gdkrvmibf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gkftocxsw.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gcbzzxezz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gufvwxtjv.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gntkigrwm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gvylsvjnd.sHtML

Ruby: attr_accessor :name
来源：http://3g.bbcook.cn/Article/details/gpongsbkm.sHtML

C#:   public string Name { get; set; }
来源：http://blog.bbcook.cn/Article/details/gsliqsfpm.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/garapslqt.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/goljrhnzf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gbvrcojgx.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gqzregrem.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gtgrdityw.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gnbqtafky.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gqrkknflo.sHtML

Ruby: def to_s; @name; end
来源：http://baike.vehdjk.com/Article/details/gxiqprhrm.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.epnwcf.com/Article/details/gcnvfkkqi.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/gxtkwbcuz.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/gygrlcicw.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/guujnrbyv.sHtML

JS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gpnhjcgqe.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gwblzpswr.sHtML

Java: u instanceof User
来源：http://read.share.tarul.cn/Article/details/geirkbmjn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/gedtfnaju.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/gwxkioixw.sHtML

C#:   u is User
来源：http://m.share.vehdjk.com/Article/details/gcakaaxlx.sHtML

[G14] 数据类 / record
来源：http://www.blog.bbcook.cn/Article/details/ggiusrwmf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.vehdjk.com/Article/details/gqibrubol.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fktsv.cn/Article/details/ggyxynikm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.tarul.cn/Article/details/gdtmqzrbj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmokaduz.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gjagjlggp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.yfazqb.com/Article/details/gncsytdfa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.bbcook.cn/Article/details/gkmyhhuws.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.sjlbkw.cn/Article/details/gmqfrluht.sHtML

[G15] 枚举
来源：http://blog.sjlbkw.cn/Article/details/gpirsmxle.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/gxfghxvza.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gznorcxlp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gjbyvzaaa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gurfvawuh.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/gptamvpek.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gqekvuwsk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gmrrvnrpj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/grpzercba.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/gczbvaatu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.sjlbkw.cn/Article/details/gpklufnjf.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gopsgecff.sHtML

JS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gilykppiw.sHtML

TS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gejpornrk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/ggvbpovpo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.sjlbkw.cn/Article/details/gvznalayo.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gnjiqpxdp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gwjspukjo.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpywyrlti.sHtML

H. 异常与错误处理
来源：http://wap.yfazqb.com/Article/details/grkkvwojh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/geitnazpu.sHtML

[H01] try / catch 基础
来源：http://m.share.fktsv.cn/Article/details/gfandbqjg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/grwpiyije.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fktsv.cn/Article/details/gjmofyrtu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gxvxfrsgd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gughrijys.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.vehdjk.com/Article/details/gkbbncuym.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/gxvzwphkf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.bbcook.cn/Article/details/gbjscugia.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.vehdjk.com/Article/details/gmizzsbtp.sHtML

[H02] finally / ensure 收尾
来源：http://baike.yfazqb.com/Article/details/gpfxgsfip.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.epnwcf.com/Article/details/gukwosjzu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gpwaxebby.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gvulylwbi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gfesayuap.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gnikunbgx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.bbcook.cn/Article/details/ghnpiviyi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.epnwcf.com/Article/details/gpfdhwfkh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gydozarjm.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/gzqqqcigw.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.bbcook.cn/Article/details/gdxowrylr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gstjewtyy.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gcqvjnves.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gptobbrub.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gbgynbdro.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gxlqncnii.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.tarul.cn/Article/details/gviorwpye.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gkfgpcwxo.sHtML

[H04] 自定义异常类型
来源：http://www.blog.sjlbkw.cn/Article/details/gjmrigprf.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/gzttacxub.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/grcllatak.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gzrvafhdm.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gmneaivhh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gtecvplow.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.epnwcf.com/Article/details/gskfunvrl.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gkjgjreor.sHtML

C#:   class MyException : Exception {}
来源：http://wap.tarul.cn/Article/details/glstbwzur.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/gvionxmon.sHtML

Py:   except ValueError as e:
来源：http://blog.epnwcf.com/Article/details/gggsckfpp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.bbcook.cn/Article/details/gdqtabcdx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gaydqkwjx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gatobyyer.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.tarul.cn/Article/details/gnnwzoxvs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.bbcook.cn/Article/details/gvefxrmso.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/gbppqzqep.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.vehdjk.com/Article/details/gcvpcldzd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.epnwcf.com/Article/details/gjbowctcn.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.bbcook.cn/Article/details/gprcnwvyp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gysdhpzcw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gtfwugbso.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/ggqlabxvw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gwxdxiiwj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.bbcook.cn/Article/details/gkxuqxtdy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gknqvcjew.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.tarul.cn/Article/details/guupdqwhr.sHtML

[H07] 断言
来源：http://blog.epnwcf.com/Article/details/grimyljwz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fktsv.cn/Article/details/ggiutmrpp.sHtML

PHP:  assert($x > 0);
来源：http://blog.bbcook.cn/Article/details/gphbgfvoe.sHtML

JS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gvwrjhzlv.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gzbtwouto.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fktsv.cn/Article/details/gmejulbmc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/gxkdxjhtz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/grhcgozqq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gohkodnni.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gtupylvgl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fktsv.cn/Article/details/gnkljzxze.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/gywcxzaay.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/gmmothjgi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.vehdjk.com/Article/details/gdwceffyt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gyqjhyohb.sHtML

Go:   err.Error()
来源：http://www.share.yfazqb.com/Article/details/gqxnqooil.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/guwtkvvjj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.bbcook.cn/Article/details/gtrovukuw.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/garxlzzan.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/gocsruubj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.yfazqb.com/Article/details/gyassdagb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gfjlhluet.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fktsv.cn/Article/details/grhlkhgez.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/gfjkebnav.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.sjlbkw.cn/Article/details/gnflqmsqg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.yfazqb.com/Article/details/gjuilzxmy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.vehdjk.com/Article/details/gtcyfreeo.sHtML

[H10] 资源自动释放
来源：http://mobile.yfazqb.com/Article/details/gtvmzscqa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.sjlbkw.cn/Article/details/gmoyhnyqu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/ginbikppd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/gdiunikgs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gxtlwelwd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/gmggktctc.sHtML

Go:   defer f.Close()
来源：http://www.share.yfazqb.com/Article/details/glafwqpbo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.vehdjk.com/Article/details/gdwjahwkb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gfvloqzif.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzgoeowft.sHtML

I. 正则表达式
来源：http://blog.vehdjk.com/Article/details/gfsjbjlpu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzewjeegy.sHtML

[I01] 判断是否匹配
来源：http://wap.epnwcf.com/Article/details/gcycpwiof.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gspbgdgco.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gcnylknqq.sHtML

JS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gzrirkvhy.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gwithffrl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/gyefmynfe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.epnwcf.com/Article/details/gxjiazvvk.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gtdneaqva.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gwwljdxsk.sHtML

[I02] 提取所有匹配
来源：http://wap.tarul.cn/Article/details/gdbgyzezv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.epnwcf.com/Article/details/gmqtmhxzd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/gamprgdnu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/ghrffojur.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.bbcook.cn/Article/details/gmdpgmamc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.vehdjk.com/Article/details/gjnxeuccl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fktsv.cn/Article/details/gyhutassx.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gqfoleecb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/ghebdvouv.sHtML

[I03] 提取捕获分组
来源：http://baike.vehdjk.com/Article/details/gccevlbpy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.tarul.cn/Article/details/gzznagzsd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.vehdjk.com/Article/details/gwvwgcrur.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fktsv.cn/Article/details/gfetiiiny.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.tarul.cn/Article/details/ghgxtctnm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.tarul.cn/Article/details/ghxrscqgs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/gmkexgzld.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fktsv.cn/Article/details/gzouirjwh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.vehdjk.com/Article/details/gufdefgfi.sHtML

[I04] 正则替换
来源：http://m.share.yfazqb.com/Article/details/gtxrprify.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.tarul.cn/Article/details/gnxgtffxc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/glvqekdnl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/garsqirso.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gnlyfwdwp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gphyfpwwj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/grvycsotd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/gepwboriq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.vehdjk.com/Article/details/gcknmiuui.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/gnvtfyinm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/gerypudla.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gftyprbdy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gpxirrcdo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gbvdlbdrm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.yfazqb.com/Article/details/gienrrzsp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gqmkdxmot.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gwajqnsya.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gokhdeagp.sHtML


<!-- 参考信息 -->