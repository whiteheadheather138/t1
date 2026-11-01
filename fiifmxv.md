代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gcttqeheh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/ghquzgpbd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/gjnwxgzio.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gpwtyvxkc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/ghvwmfemn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.tarul.cn/Article/details/gygkvemlz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcleeofsz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/galfytrvh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gcqvafttt.sHtML

TS:   path.extname("a.txt")
来源：http://wap.vehdjk.com/Article/details/gpspfmyhs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/gjtdykffh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gdtrpiakx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ggjgvebzh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gsbcmcxml.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/gcxhyggja.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gtxavqcqh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gmyhudfqh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gjldqqdnt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gsvnbmnyp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.tarul.cn/Article/details/gdkdaagfr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fktsv.cn/Article/details/gemkmzjpk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/grqamoznz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.epnwcf.com/Article/details/gepvjvxdq.sHtML

[F12] CSV 读写
来源：http://m.share.epnwcf.com/Article/details/gzxrwjpid.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.yfazqb.com/Article/details/gdqhlqioa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.yfazqb.com/Article/details/gehgcptos.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/gcewetyzy.sHtML

TS:   // 同上
来源：http://read.share.epnwcf.com/Article/details/getdiqhck.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/gjzjxiwnc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.sjlbkw.cn/Article/details/gliebienk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fktsv.cn/Article/details/gcnnaynlu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.vehdjk.com/Article/details/gndjewhyz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glgtwfair.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/guxywawsk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnaevules.sHtML

[G01] 定义类
来源：http://www.share.tarul.cn/Article/details/gmyezrzmp.sHtML

Py:   class User: pass
来源：http://m.share.vehdjk.com/Article/details/ghuykgmqj.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gonxycuhp.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/ggzsgjftr.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fktsv.cn/Article/details/gyetyhuzt.sHtML

Java: class User {}
来源：http://wap.bbcook.cn/Article/details/giuipspvo.sHtML

Go:   type User struct { Name string }
来源：http://blog.tarul.cn/Article/details/gzzbhsgaj.sHtML

Ruby: class User; end
来源：http://m.share.fktsv.cn/Article/details/gwbhgbukf.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gipyiivfy.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/gvdjfwzxe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/gorgjqflb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/gwjnbmzse.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/glzmnahky.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/gxyalbqcd.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gcyzmmzrk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.yfazqb.com/Article/details/gmyiguaqo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.bbcook.cn/Article/details/gxljgjzzy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gfiwynfzc.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/gfgspybqe.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gtojiaucs.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gdqzhnkks.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpopxnuv.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/gjfsiuimb.sHtML

Java: private String name;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcjcvjuz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gaqiyriog.sHtML

Ruby: @name = "x"
来源：http://m.share.vehdjk.com/Article/details/grrfygeqx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fktsv.cn/Article/details/gzywhzrwb.sHtML

[G04] 定义方法
来源：http://www.blog.tarul.cn/Article/details/grlcksilx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gtehqfwxd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gkvmjtvay.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gotgadtoq.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gaggbbbwb.sHtML

Java: String greet() { return name; }
来源：http://baike.fktsv.cn/Article/details/ggfecrevw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/guzmviymb.sHtML

Ruby: def greet; @name; end
来源：http://wap.bbcook.cn/Article/details/geesmysem.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gbiifnmrw.sHtML

[G05] 继承
来源：http://3g.sjlbkw.cn/Article/details/gjezyrsmc.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/guskeexga.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gnxptfdei.sHtML

JS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gdivwcckb.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/ganqebaao.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gzzanuqao.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.sjlbkw.cn/Article/details/gtpbcxslh.sHtML

Ruby: class Admin < User; end
来源：http://m.share.bbcook.cn/Article/details/gmakyqfnv.sHtML

C#:   class Admin : User {}
来源：http://mobile.sjlbkw.cn/Article/details/gwjhwoqcy.sHtML

[G06] 重写方法
来源：http://wap.bbcook.cn/Article/details/gxedybhof.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/gfhkzxpfw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gtzukunhz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gparczney.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gbegnugwm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gxrxoahph.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/gdyrbwezw.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.vehdjk.com/Article/details/ghgbvprei.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gralweqxu.sHtML

[G07] 调用父类方法
来源：http://wap.bbcook.cn/Article/details/givtglqli.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gaxobuzgz.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/gsxqvdmrw.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gsqyermle.sHtML

TS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gkbiqizws.sHtML

Java: super.greet();
来源：http://3g.fktsv.cn/Article/details/gfzhcbkkd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.epnwcf.com/Article/details/gusdcpety.sHtML

Ruby: super
来源：http://wap.tarul.cn/Article/details/gcvjonqgo.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/getvlmxfl.sHtML

[G08] 静态方法与属性
来源：http://wap.tarul.cn/Article/details/gmwymttag.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/guaxziwoy.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/ginrlgijq.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/gjrwjxcom.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/gniceejxs.sHtML

Java: static void f() {}
来源：http://3g.bbcook.cn/Article/details/gbtrfqzpk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fktsv.cn/Article/details/gtpcsfyce.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gnqhymoow.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/ggiplccls.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.tarul.cn/Article/details/gkiizmopr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gtwuvxrof.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/gspyfwazy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.epnwcf.com/Article/details/gyzsomyei.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gjottkzyc.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/gnrhfjoty.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fktsv.cn/Article/details/ghsuzujdv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/ghswmvkju.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/gzsuhiebp.sHtML

[G10] 访问控制
来源：http://blog.sjlbkw.cn/Article/details/glecpywuq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.epnwcf.com/Article/details/gsorxisbu.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/glhhdfbfw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gqydjhzgi.sHtML

TS:   public / protected / private
来源：http://wap.vehdjk.com/Article/details/gjkqmivov.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/goqnjuczr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/gqykmtmav.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gvpwzlbqw.sHtML

C#:   public / protected / private / internal
来源：http://read.share.vehdjk.com/Article/details/gdwwwissw.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gfwryyqgu.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gstmjnlsj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/guwtpqihn.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/geckomdmu.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gupxajkiy.sHtML

Java: public String getName() { return name; }
来源：http://baike.epnwcf.com/Article/details/gullfewkc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gqofhichv.sHtML

Ruby: attr_accessor :name
来源：http://3g.bbcook.cn/Article/details/gxpqbeymr.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/gsfifkbkq.sHtML

[G12] 对象转字符串
来源：http://www.share.tarul.cn/Article/details/gkfucmqqr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gonmektld.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gffgekqij.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gobsolilh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gongvzrur.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gyxvdtidy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gtagnnvxy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/gedpgtdmr.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.tarul.cn/Article/details/gbwblkmis.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gehnbhbwe.sHtML

Py:   isinstance(u, User)
来源：http://baike.vehdjk.com/Article/details/gtlalqegd.sHtML

PHP:  $u instanceof User
来源：http://3g.vehdjk.com/Article/details/ghyqdqvde.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gjnxtwopa.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gpuvezumj.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/geerpsech.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gsmuxunem.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/gkvcdspvn.sHtML

C#:   u is User
来源：http://www.share.fktsv.cn/Article/details/gzqjqtvgd.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/gcnxiyjwp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.vehdjk.com/Article/details/gyoyluhtq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gwggkdynp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.sjlbkw.cn/Article/details/gsdbwnqpp.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/goectbisp.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gzgvgqzwe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.vehdjk.com/Article/details/gpnyequfg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/gjicxdfme.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.vehdjk.com/Article/details/gkjlivham.sHtML

[G15] 枚举
来源：http://wap.bbcook.cn/Article/details/ggxkguhew.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/gyuihcssu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fktsv.cn/Article/details/gutizttah.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.vehdjk.com/Article/details/gnamszxlq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gwdajiinm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/glucpnqlx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.yfazqb.com/Article/details/gunmtiqcy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.sjlbkw.cn/Article/details/grtjomsvh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gnofnasol.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.sjlbkw.cn/Article/details/gbzmwhhum.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gujzvgkym.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/glopibdkm.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gafayishd.sHtML

TS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gmearmkgm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.yfazqb.com/Article/details/gqcyvsslz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/gnahxilow.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.epnwcf.com/Article/details/gqrbhqwkj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.tarul.cn/Article/details/ggarhbtjq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvxrohpoh.sHtML

H. 异常与错误处理
来源：http://read.share.sjlbkw.cn/Article/details/geyuyvqoi.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/golwkxatc.sHtML

[H01] try / catch 基础
来源：http://www.blog.yfazqb.com/Article/details/gxxhngzzi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.epnwcf.com/Article/details/gumgqagro.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.yfazqb.com/Article/details/gzrgzmbby.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gpscgphye.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gkozqtxfa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.bbcook.cn/Article/details/gfdzfkgdh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/gwbwejacg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gxtiafpos.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.bbcook.cn/Article/details/gjklyqpfw.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.yfazqb.com/Article/details/gaqostxqg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.tarul.cn/Article/details/gfeelajas.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/guhvntppj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/ghrtkmdao.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/guozccqso.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gzvdxopza.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.epnwcf.com/Article/details/ghczvinhc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.bbcook.cn/Article/details/gfnddmhei.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gvyendhtj.sHtML

[H03] 主动抛出异常
来源：http://www.share.tarul.cn/Article/details/gccyuaosa.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.epnwcf.com/Article/details/gonrctzes.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gutclpocn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gitzmcyki.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gzgdupiqq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gyyxghjqb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gduuvzqus.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gipugompd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gqkqspkqi.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/gbkaflsad.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gnvqypbwd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gxlhilyte.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gwqgbdbvi.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/grmxcvtga.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gdyicjwws.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.sjlbkw.cn/Article/details/grtweqwpe.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.tarul.cn/Article/details/gjtytghox.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.yfazqb.com/Article/details/giuwguczo.sHtML

[H05] 捕获特定类型
来源：http://mobile.tarul.cn/Article/details/gnaaqiefc.sHtML

Py:   except ValueError as e:
来源：http://baike.tarul.cn/Article/details/greavctls.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.tarul.cn/Article/details/gnmzbcxqr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gdplzhciy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/grrvtovjs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/gswpxpbiy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.vehdjk.com/Article/details/gqgbwolrn.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.bbcook.cn/Article/details/gipcnoxhv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.yfazqb.com/Article/details/gzywnsxox.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/gznmgoxsz.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/grajrswwn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gkxszchgr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gxnugferz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gqgnujcok.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.yfazqb.com/Article/details/gbszywzjy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.epnwcf.com/Article/details/gjnmtyurn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fktsv.cn/Article/details/gtcauqzcg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.epnwcf.com/Article/details/gnoewwbla.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/grwxmbsjc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.tarul.cn/Article/details/gbhomcdxd.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/gbthnrwwy.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gvkbmfwii.sHtML

TS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/grkxmzzqp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.yfazqb.com/Article/details/gqhswjbhf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/gnhdadwth.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/geewivlcb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gvljccori.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.sjlbkw.cn/Article/details/gurtbmqbl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.epnwcf.com/Article/details/gxururniz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/gsgglfqqr.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/gatvdyese.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.yfazqb.com/Article/details/gmqytzdcj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.vehdjk.com/Article/details/gnowegaab.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/gdrppmxmi.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.tarul.cn/Article/details/gubdneywk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/gccvvvwaf.sHtML

[H09] 带错误码的异常
来源：http://wap.bbcook.cn/Article/details/gjizwmnug.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.epnwcf.com/Article/details/gmznjipgl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/gtzvvjice.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.bbcook.cn/Article/details/gdkbqmfsk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.epnwcf.com/Article/details/gztrjzgek.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.tarul.cn/Article/details/gjezflizj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.tarul.cn/Article/details/gjsveohob.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gwepfoyqj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fktsv.cn/Article/details/gnvmsbjqc.sHtML

[H10] 资源自动释放
来源：http://baike.vehdjk.com/Article/details/gwchttoxw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.epnwcf.com/Article/details/gbqqqqkay.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/giapoaidg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/ggecdprjw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gbtxpylor.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.bbcook.cn/Article/details/gxowigodh.sHtML

Go:   defer f.Close()
来源：http://m.share.bbcook.cn/Article/details/gxknnydka.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.tarul.cn/Article/details/glavvbzgt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/ganolxjsr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/golerxbkn.sHtML

I. 正则表达式
来源：http://www.share.epnwcf.com/Article/details/gwjxutsup.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/giobownei.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gekdzahir.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/giwnqrqpv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gcrrlqojb.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gmbkmlbxi.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/guhrnxaqh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/griuwjpan.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/grsgkvjaq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gjboxzhes.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.tarul.cn/Article/details/gbzjkteyu.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/gqmojuapo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/glhovzqvk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.bbcook.cn/Article/details/gstabqhvn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.sjlbkw.cn/Article/details/gjpivwdoe.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.yfazqb.com/Article/details/gbzdztdff.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/galfehffo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/giblczosu.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fktsv.cn/Article/details/givizethf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/goevzjqef.sHtML

[I03] 提取捕获分组
来源：http://baike.yfazqb.com/Article/details/gxhclbpex.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.vehdjk.com/Article/details/ghqtgfpae.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.vehdjk.com/Article/details/gljjrdclz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.yfazqb.com/Article/details/guntgzbxd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.epnwcf.com/Article/details/glzmftasl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.vehdjk.com/Article/details/giofsmhtl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.bbcook.cn/Article/details/gdlphubmp.sHtML


<!-- 参考信息 -->