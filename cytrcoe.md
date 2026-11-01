代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fktsv.cn/Article/details/gulloqyzz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/gsdhsnfla.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/glaodkngt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gnzhkparm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gultmvlag.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gvaavancj.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.tarul.cn/Article/details/gxshbupqd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.epnwcf.com/Article/details/gwtkgfdts.sHtML

[F09] 获取文件大小
来源：http://read.share.sjlbkw.cn/Article/details/gzyaqiflo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.vehdjk.com/Article/details/gyzjvwlby.sHtML

PHP:  filesize("a.txt");
来源：http://baike.yfazqb.com/Article/details/gsjmbnavr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gmxxcjhyt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gzqhcgdbu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gxlsaommj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.yfazqb.com/Article/details/ghrnxnaso.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gopeoyxbd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/gpimrxbbv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.yfazqb.com/Article/details/gnibalspx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gsgcncutw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.yfazqb.com/Article/details/gutijqgot.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdfysxaim.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvhuchsnx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.vehdjk.com/Article/details/ggzlsllji.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gqqrvefaw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gxzaepcvt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gqcxbqfjf.sHtML

[F11] 复制与移动文件
来源：http://wap.fktsv.cn/Article/details/gyuugaizt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gvdgfmqbo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.tarul.cn/Article/details/gfriaglfl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/ggduugled.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gmvqffyxd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.vehdjk.com/Article/details/gimnujmnf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/gdjjtagbn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gynciofzh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/guwurnuer.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gxfkmwrld.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.sjlbkw.cn/Article/details/gihmzrdwp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gwjvglzwj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.vehdjk.com/Article/details/gloghbesr.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gjcbkchsj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.yfazqb.com/Article/details/goikelolc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gevsewkyc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.tarul.cn/Article/details/gxcfryfpj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/gjfnlkuqm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/giluzdkrk.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gmrjhrkia.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gltmdxsjs.sHtML

[G01] 定义类
来源：http://read.share.tarul.cn/Article/details/gjwagvblo.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gaaxqkhhj.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/ghuavjtjq.sHtML

JS:   class User {}
来源：http://mobile.tarul.cn/Article/details/gpwrqynkh.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gmfrnlrod.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gqypmrjqu.sHtML

Go:   type User struct { Name string }
来源：http://www.share.bbcook.cn/Article/details/gaqefxere.sHtML

Ruby: class User; end
来源：http://baike.epnwcf.com/Article/details/gzxutlknj.sHtML

C#:   class User {}
来源：http://3g.vehdjk.com/Article/details/gmcvtzlcv.sHtML

[G02] 构造函数
来源：http://www.blog.bbcook.cn/Article/details/gaijnyenn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/ghcspdopg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/ghnjzcoug.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/ggmrpflzp.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/godbncedg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gsofbnusm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.sjlbkw.cn/Article/details/gmekdspiw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fktsv.cn/Article/details/gtyzfttwz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/glokarqle.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gjtcniwso.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gwgmausff.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gyzdlefyf.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gbaeultuk.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gaypcqqus.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gasgmtwrj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gyopeiwcn.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/grevvzhmx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/goyypxuln.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/gbgsruyij.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gwqrdaexa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/ghergqvzf.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gdbzxdneg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gmragdtwl.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/ggslyvdwk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gqwwmablq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gfekpdeyp.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fktsv.cn/Article/details/gkzilprkp.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/gymvasvpw.sHtML

Py:   class Admin(User): pass
来源：http://www.share.bbcook.cn/Article/details/gkyuxfuvk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gspilgsrt.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/galgepdec.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gubqehivg.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/goehzrfro.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.bbcook.cn/Article/details/gushdbjlv.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gaowzsvlg.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqejgkrxq.sHtML

[G06] 重写方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrwwblvz.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fktsv.cn/Article/details/ghgsviqsj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gsyryhuuo.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gbposzbon.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gedlvbwmr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gexwntjbt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.yfazqb.com/Article/details/gtdiyscvo.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/gqapbwrky.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.vehdjk.com/Article/details/ghdtfmwns.sHtML

[G07] 调用父类方法
来源：http://mobile.yfazqb.com/Article/details/goebcratr.sHtML

Py:   super().greet()
来源：http://mobile.fktsv.cn/Article/details/gkgsvstkl.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/gdhjpgcvk.sHtML

JS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gkbtcekmc.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/ghrmlqwya.sHtML

Java: super.greet();
来源：http://baike.fktsv.cn/Article/details/glewqamcz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fktsv.cn/Article/details/gtnsdlloj.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gcnpqqhmk.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/gwsykjswa.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fktsv.cn/Article/details/gvsfqzcrd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.sjlbkw.cn/Article/details/gxuolvvym.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/gszdzaxjd.sHtML

JS:   static f() {}
来源：http://www.blog.yfazqb.com/Article/details/gqgvceces.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/grebmtyql.sHtML

Java: static void f() {}
来源：http://www.share.vehdjk.com/Article/details/gmsyarrvk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.bbcook.cn/Article/details/gwjqehtqr.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gvkwqkmqv.sHtML

C#:   public static void F() {}
来源：http://3g.tarul.cn/Article/details/ghkjisbiy.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/geefgtkba.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/gdbovwkxl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gljlpxnqb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gdkmwjxxt.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fktsv.cn/Article/details/gncyffwou.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.yfazqb.com/Article/details/gsvabkbrn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/gfuccywta.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gpzkaskmt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gfodeeppb.sHtML

[G10] 访问控制
来源：http://m.share.tarul.cn/Article/details/gmjupttvz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gucvqzajn.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gswrsdhzw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.bbcook.cn/Article/details/gtfquwkxd.sHtML

TS:   public / protected / private
来源：http://baike.epnwcf.com/Article/details/gjqbopgon.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gqwerhlem.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/grfsctdhv.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/glbxeqsqy.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gpbjgyqkm.sHtML

[G11] getter / setter
来源：http://blog.vehdjk.com/Article/details/gbxzcdkyl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gmldnupbf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gnchnsdld.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/giaboneqw.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.tarul.cn/Article/details/gzjqulxjn.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gzgnccbcx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gyggyntsy.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.bbcook.cn/Article/details/gxulgvirz.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.tarul.cn/Article/details/gabxkmvcb.sHtML

[G12] 对象转字符串
来源：http://read.share.sjlbkw.cn/Article/details/glgynlinm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gsexbqzbu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/ghvqngnxy.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gcecpxtiw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gktfxkiuc.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gpockdtwn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gcpzeraqf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gozwauvyr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.tarul.cn/Article/details/grgskbbpo.sHtML

[G13] 判断对象类型
来源：http://www.blog.fktsv.cn/Article/details/gnnzxzrsf.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/gpmudforj.sHtML

PHP:  $u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gwnrlhtki.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gigtszmsj.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gdssavnia.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gyfcbxwem.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gukfxfwfk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.bbcook.cn/Article/details/guvwkrucb.sHtML

C#:   u is User
来源：http://www.blog.tarul.cn/Article/details/gaalhzaee.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/gyuavkbmx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/gsqszgwzv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.yfazqb.com/Article/details/gwhijwfvy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.bbcook.cn/Article/details/grsppqiva.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.sjlbkw.cn/Article/details/gqnagdkrk.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/gpdxtqmcj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.bbcook.cn/Article/details/gxkkgrleg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gplptkbhh.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gtupfyruw.sHtML

[G15] 枚举
来源：http://m.share.bbcook.cn/Article/details/gbgdzdknr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gothhmhnh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.sjlbkw.cn/Article/details/ginxhtgkh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gniujdvmr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gzaijzdvm.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gzswbsaxe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.epnwcf.com/Article/details/gxjqzgdfc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/ggxlsjtel.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gxxsjbjfj.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/gympdchoy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.tarul.cn/Article/details/gwumxdwwx.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fktsv.cn/Article/details/ghytipfjk.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gtfksmilx.sHtML

TS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/ghgaiknvb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.bbcook.cn/Article/details/gmpxlbuzq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.bbcook.cn/Article/details/glfylxzhq.sHtML

Ruby: obj.instance_variables
来源：http://3g.fktsv.cn/Article/details/gzmhbiurx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gxrxraxbn.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gsruyfqtb.sHtML

H. 异常与错误处理
来源：http://mobile.epnwcf.com/Article/details/gylgjrdxt.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnsxodgqb.sHtML

[H01] try / catch 基础
来源：http://mobile.tarul.cn/Article/details/gohpmypid.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.tarul.cn/Article/details/gmjilzlig.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.tarul.cn/Article/details/gzsqiekyl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gcxpvynzc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gvawdhxhj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.vehdjk.com/Article/details/gtchkufpl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.tarul.cn/Article/details/ggabzjqmf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.sjlbkw.cn/Article/details/grmhymqju.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.epnwcf.com/Article/details/gfzyeicpv.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.sjlbkw.cn/Article/details/glopfybll.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gnxysosdx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsakhylwt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/ggthahhzk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gtntnlknz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gjobyjznj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fktsv.cn/Article/details/gjxhifspm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/gimpvwnla.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gfeolsdzm.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/gifmtvxtz.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.sjlbkw.cn/Article/details/gynowpyud.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gdrwroayd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gyhithldi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbsnnaet.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gkyurqdts.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.bbcook.cn/Article/details/guprrivsk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.epnwcf.com/Article/details/gkyznyzqx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gnibvisjw.sHtML

[H04] 自定义异常类型
来源：http://mobile.sjlbkw.cn/Article/details/gpflqwmus.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.tarul.cn/Article/details/gabvcddez.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gzfqxebpx.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gkzrdkixm.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gxkdfrnwm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gselkrqlj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.vehdjk.com/Article/details/gkbubvtgh.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.vehdjk.com/Article/details/gkanmxoem.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/gjikqdtdo.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/gxygqqynr.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gbvgoygkx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.yfazqb.com/Article/details/gdohibbpy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/ggxhjthrv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gijmavujr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.sjlbkw.cn/Article/details/gibzslmfb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.sjlbkw.cn/Article/details/gmqigponm.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.vehdjk.com/Article/details/gpaxoonvq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.sjlbkw.cn/Article/details/gvplwcgtf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.epnwcf.com/Article/details/gcrixufxv.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gsrxiopjf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gzxxebkko.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gfiwjukwc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gwmttnhqc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/gkhepkdtw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.tarul.cn/Article/details/gbkzpebqu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.bbcook.cn/Article/details/ghcgeczuv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gajjfihle.sHtML

[H07] 断言
来源：http://blog.yfazqb.com/Article/details/gpocfjrvq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.epnwcf.com/Article/details/gajzitkdm.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/gyzvsftvw.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gfsftjysr.sHtML

TS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/ggzqesdxd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.bbcook.cn/Article/details/gmptobhzw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/gaemobyou.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.vehdjk.com/Article/details/grbqgpkqg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gesudnvgz.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.yfazqb.com/Article/details/gjpowkiwh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.yfazqb.com/Article/details/glpohfvbd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.sjlbkw.cn/Article/details/ggnxqnhcb.sHtML

JS:   e.message;  e.stack
来源：http://baike.vehdjk.com/Article/details/gbtqvizry.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/ggwizhtve.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.epnwcf.com/Article/details/gmxjacbnt.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/gefjtzflv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/gitnfjxdx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.tarul.cn/Article/details/gstqamgkj.sHtML

[H09] 带错误码的异常
来源：http://www.blog.vehdjk.com/Article/details/gqkuxpkid.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/grjuoywgg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.yfazqb.com/Article/details/gtdwpqezy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/gxdodkdto.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.epnwcf.com/Article/details/gkflclgvk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.vehdjk.com/Article/details/gaywoemgb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/gnlywitrk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.yfazqb.com/Article/details/gnblyavrj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.bbcook.cn/Article/details/gyweuskwv.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gzppfepkr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.epnwcf.com/Article/details/gfjgnyaqu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.sjlbkw.cn/Article/details/gkgmnrhrr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/grwmouiyw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gddlvvnkj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.yfazqb.com/Article/details/gcdxkhvgy.sHtML

Go:   defer f.Close()
来源：http://blog.tarul.cn/Article/details/gbfnkbznc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/geedkxvmj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gpfuayqwr.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guhmemzuy.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/glqaacfaw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpacegtvk.sHtML

[I01] 判断是否匹配
来源：http://baike.epnwcf.com/Article/details/gnuenrvuq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gkgkaxsgj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gjpytgltf.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/grkfgcsmd.sHtML

TS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gqztruxpk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.yfazqb.com/Article/details/ghbyzopuw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gqmntbwbc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gfjlnfswi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gqnlnzzol.sHtML

[I02] 提取所有匹配
来源：http://blog.sjlbkw.cn/Article/details/gkiufytin.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/glclyqaao.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/goupbubjq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/gxxjxopeh.sHtML


<!-- 参考信息 -->