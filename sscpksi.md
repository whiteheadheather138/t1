代发 wailian999

[F09] 获取文件大小
来源：http://mobile.tarul.cn/Article/details/gwjofymtm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gtlyxwvuv.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gkgkgmgdg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gmtvtwted.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gbpbhjogs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/giuhmbsga.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.bbcook.cn/Article/details/gtyjnjcka.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gafzgpfnw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.epnwcf.com/Article/details/gvqumnyty.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.epnwcf.com/Article/details/gardmacdk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gaghqwqyn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gkuptgzhb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gfeumgjoz.sHtML

TS:   path.extname("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gefkiycaj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.sjlbkw.cn/Article/details/gwyuvarow.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gmvhsimmy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gjigyxrty.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gvycugcwi.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/ghbhzvqod.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gzmfefjyt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gpknfhnjx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gzlfickpo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gldmoisgn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/gjjidjnzg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.vehdjk.com/Article/details/ggvmwfzxh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gozkcuhxv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/ggimdqwls.sHtML

[F12] CSV 读写
来源：http://blog.tarul.cn/Article/details/gkjrtfgoo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.yfazqb.com/Article/details/geceggfop.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/glvtknibe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.vehdjk.com/Article/details/gdtzbeyid.sHtML

TS:   // 同上
来源：http://www.blog.yfazqb.com/Article/details/gggchcfpd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/govnhlmws.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/gruqutecn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.sjlbkw.cn/Article/details/gexhujcgg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gvndbvwvx.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvxwlvpqw.sHtML

G. 面向对象
来源：http://m.share.fktsv.cn/Article/details/gditeaqyw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/genppkuyf.sHtML

[G01] 定义类
来源：http://www.blog.tarul.cn/Article/details/gpqjhsrxb.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/glrhcnxem.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/gjxsyvqxn.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gavnslftj.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.sjlbkw.cn/Article/details/gsxxzbthu.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/ghybixsfd.sHtML

Go:   type User struct { Name string }
来源：http://wap.bbcook.cn/Article/details/gbsekhwni.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gffiebgid.sHtML

C#:   class User {}
来源：http://baike.epnwcf.com/Article/details/gzwxlcdmn.sHtML

[G02] 构造函数
来源：http://wap.tarul.cn/Article/details/gjtxvyogw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.epnwcf.com/Article/details/gmjbadgru.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gzwaklldf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gwslkczql.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fktsv.cn/Article/details/gnzfsgxwt.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gqcadcdxc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.sjlbkw.cn/Article/details/glsluklqv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/ghoocopzz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gganvjzpg.sHtML

[G03] 实例属性
来源：http://www.blog.epnwcf.com/Article/details/gprddwyta.sHtML

Py:   self.name = "x"
来源：http://wap.fktsv.cn/Article/details/gkwgbpgcl.sHtML

PHP:  public string $name = "x";
来源：http://blog.epnwcf.com/Article/details/gyountiam.sHtML

JS:   this.name = "x";
来源：http://3g.epnwcf.com/Article/details/gwxfaqted.sHtML

TS:   name: string = "x";
来源：http://blog.epnwcf.com/Article/details/gpgogodin.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/gjbufrkkn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fktsv.cn/Article/details/gzsvvbcdr.sHtML

Ruby: @name = "x"
来源：http://m.share.yfazqb.com/Article/details/gvjjvmqcj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/gudntdvvk.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gwroujzop.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gduonjkdo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gnzvxdvoj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gvgjfeidu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gfrbpvzwc.sHtML

Java: String greet() { return name; }
来源：http://blog.fktsv.cn/Article/details/gibaceoag.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gylnvhxkm.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gyhrechja.sHtML

C#:   public string Greet() => Name;
来源：http://baike.vehdjk.com/Article/details/gcthxnryw.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gerxpvsaf.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fktsv.cn/Article/details/gcwgqxagm.sHtML

PHP:  class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/ghywruvdr.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gempmyaow.sHtML

TS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gbxiqdntu.sHtML

Java: class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gcxosyhej.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.vehdjk.com/Article/details/grhmrunvj.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fktsv.cn/Article/details/gtaluucox.sHtML

C#:   class Admin : User {}
来源：http://m.share.epnwcf.com/Article/details/gsjwvohdp.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gniifwmdz.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fktsv.cn/Article/details/gcfebpqsy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvwkrzft.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcxfziwk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gfnnoeagi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gfjrqxdet.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.yfazqb.com/Article/details/gycidmisg.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.bbcook.cn/Article/details/gyekcrxnf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.sjlbkw.cn/Article/details/gzsmjkyxu.sHtML

[G07] 调用父类方法
来源：http://baike.yfazqb.com/Article/details/ganbjpowr.sHtML

Py:   super().greet()
来源：http://www.m.share.epnwcf.com/Article/details/gbmsfreqt.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gitxgtuuh.sHtML

JS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gjejhkjxo.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/grqhxoqfk.sHtML

Java: super.greet();
来源：http://read.share.vehdjk.com/Article/details/goezpyrpz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gvctottke.sHtML

Ruby: super
来源：http://mobile.fktsv.cn/Article/details/gkbvxdhuh.sHtML

C#:   base.Greet();
来源：http://read.share.bbcook.cn/Article/details/gtcsbghog.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/gjhegofzz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/gcqdasupn.sHtML

PHP:  public static function f() {}
来源：http://3g.sjlbkw.cn/Article/details/gazrgyvrp.sHtML

JS:   static f() {}
来源：http://www.share.fktsv.cn/Article/details/glfbltfsu.sHtML

TS:   static f(): void {}
来源：http://blog.epnwcf.com/Article/details/gjngwtdfb.sHtML

Java: static void f() {}
来源：http://3g.tarul.cn/Article/details/gskynjxzd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/glwpdwjwn.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/gjcqxnwol.sHtML

C#:   public static void F() {}
来源：http://m.share.tarul.cn/Article/details/gxghotfbf.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.yfazqb.com/Article/details/gzedvnjso.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/gfnjhgyvr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.bbcook.cn/Article/details/gvjvfqvyn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.bbcook.cn/Article/details/gpzjywwti.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gacqjamws.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/gdfbcmfwf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fktsv.cn/Article/details/gzxykxkum.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.vehdjk.com/Article/details/gupltgrzr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gclqempxp.sHtML

[G10] 访问控制
来源：http://baike.fktsv.cn/Article/details/gefdhafam.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/gwbjoirpo.sHtML

PHP:  public / protected / private
来源：http://3g.fktsv.cn/Article/details/gihnyszbh.sHtML

JS:   #private 字段；其余公开
来源：http://blog.vehdjk.com/Article/details/ghrgmvvyc.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gtdhixfrv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.sjlbkw.cn/Article/details/gclougvtx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/gpgvlcumo.sHtML

Ruby: public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gpfeeryov.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gyxeqilwq.sHtML

[G11] getter / setter
来源：http://www.m.share.tarul.cn/Article/details/gdciekwly.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gfyjnlbep.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gwnrlrgvm.sHtML

JS:   get name() { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gwfaopuxj.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gjcyxbqmb.sHtML

Java: public String getName() { return name; }
来源：http://baike.epnwcf.com/Article/details/gnsdfxhwd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gvvjktrbm.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gyxkixyjq.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/gismheunq.sHtML

[G12] 对象转字符串
来源：http://mobile.yfazqb.com/Article/details/gyqjlrdge.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gaurontbk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gxiphnwxg.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gcmduvrti.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdpwzxfhh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gfhsasrds.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gnetqjqrq.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gbzlhjgqz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.vehdjk.com/Article/details/gizixovsg.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gfdgkfsvi.sHtML

Py:   isinstance(u, User)
来源：http://blog.fktsv.cn/Article/details/gvpiimqbe.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gwwxlzhfv.sHtML

JS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/grezgivkv.sHtML

TS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gefcnflca.sHtML

Java: u instanceof User
来源：http://wap.tarul.cn/Article/details/ghbbbvigt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gmcwonoyh.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.vehdjk.com/Article/details/gbkfgexhv.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/gawbieoxw.sHtML

[G14] 数据类 / record
来源：http://blog.fktsv.cn/Article/details/gdfjsdenc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.vehdjk.com/Article/details/gmkhikqrb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/gosmndhil.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.bbcook.cn/Article/details/ghuslzzyr.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.sjlbkw.cn/Article/details/gkllglztg.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.epnwcf.com/Article/details/gulombbau.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/gdpjgobfg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/ggvfszqmr.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gnfavbeig.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gtqraucxa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.bbcook.cn/Article/details/ghjeaycsm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/ghumltwfr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gcjawmosb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gyerchfue.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/gofobncyx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/gmktovbde.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/gpjtmjqma.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/geqxbmasl.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.sjlbkw.cn/Article/details/gtwaahurf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/gvcrluhwv.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.yfazqb.com/Article/details/gbxcnsjrk.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gxfoewsxm.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gpbleueah.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/gedartmlj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gbypqrtlp.sHtML

Ruby: obj.instance_variables
来源：http://blog.epnwcf.com/Article/details/gcjdsiecb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.tarul.cn/Article/details/gdkxneddt.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gbnbqrpal.sHtML

H. 异常与错误处理
来源：http://baike.fktsv.cn/Article/details/gacnpzuya.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxuaqttqt.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gwfiynqod.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gjshxdrty.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.yfazqb.com/Article/details/gzidmhciw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gechwsokx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/gvutwiahf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/gethidihp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.tarul.cn/Article/details/ggmwvfhmd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fktsv.cn/Article/details/gbznmphbe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gbghobjzr.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fktsv.cn/Article/details/gpylcdsui.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/gtaehqddm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/ggiepbllp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gwkxichbd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlzmugqi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/grvqxxmit.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gemgmqozf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.bbcook.cn/Article/details/grpdbmytb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gsavxjtlc.sHtML

[H03] 主动抛出异常
来源：http://mobile.tarul.cn/Article/details/ghcqvbmpg.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/ghxctyaxh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gbmwylpty.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gtxnoaros.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gdjnrrcta.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gwlagpbvc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fktsv.cn/Article/details/gptsrpvgp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.tarul.cn/Article/details/gbmeclljh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gvhktzjly.sHtML

[H04] 自定义异常类型
来源：http://mobile.tarul.cn/Article/details/gxoiimbgr.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gboffkbzr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/guojibzyv.sHtML

JS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/gwusxkbqr.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gevnywjut.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/guhssljcy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/goipvxzon.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.vehdjk.com/Article/details/grwkvzisl.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/gbdkvtgis.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/gylmfnsia.sHtML

Py:   except ValueError as e:
来源：http://read.share.bbcook.cn/Article/details/gxxzqgjut.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.sjlbkw.cn/Article/details/gtdcviqgj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gnggusbev.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmsslcfsm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.bbcook.cn/Article/details/gumnmpsjh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gwytutufe.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fktsv.cn/Article/details/gymfegkyw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.tarul.cn/Article/details/guryxzzeq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/gqkavsyyx.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.bbcook.cn/Article/details/gounzfwwh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/guggbfswo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gdciyrnug.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gahcbxqpo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.epnwcf.com/Article/details/gwlhoszfq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.yfazqb.com/Article/details/gzabhqmvx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.yfazqb.com/Article/details/glezkckqn.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/gykokgvyd.sHtML

[H07] 断言
来源：http://www.m.share.vehdjk.com/Article/details/grebtjzyk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.epnwcf.com/Article/details/gzcsywitx.sHtML

PHP:  assert($x > 0);
来源：http://wap.fktsv.cn/Article/details/glzhbklct.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/goaubotoo.sHtML

TS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gppjpscxe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fktsv.cn/Article/details/gwuppzznh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fktsv.cn/Article/details/grnhlyogq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.epnwcf.com/Article/details/gisuueapw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gpvlmyqbm.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.sjlbkw.cn/Article/details/gxcykhrju.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.bbcook.cn/Article/details/gvyotnzuo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gyxpaalnb.sHtML

JS:   e.message;  e.stack
来源：http://baike.sjlbkw.cn/Article/details/gjvjapasu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fktsv.cn/Article/details/gokfyeibc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fktsv.cn/Article/details/gxftzinjh.sHtML

Go:   err.Error()
来源：http://wap.fktsv.cn/Article/details/gurkoncjf.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.bbcook.cn/Article/details/gcnrvueyv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/gtuxamwei.sHtML

[H09] 带错误码的异常
来源：http://read.share.epnwcf.com/Article/details/gzuhnjodw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.sjlbkw.cn/Article/details/ggpxumxaf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/gmiaechxr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/gmcimokaz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.epnwcf.com/Article/details/gtgtrraac.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.bbcook.cn/Article/details/gyeelfljx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.epnwcf.com/Article/details/gyvauivxj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fktsv.cn/Article/details/gelqmtfmz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fktsv.cn/Article/details/gynypubyv.sHtML

[H10] 资源自动释放
来源：http://wap.epnwcf.com/Article/details/gsbypsnvv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fktsv.cn/Article/details/gxxzodgdy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fktsv.cn/Article/details/gfnmurgzy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gjhevapws.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gyhiblamn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.tarul.cn/Article/details/gbffudrxm.sHtML

Go:   defer f.Close()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfwiszsn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.yfazqb.com/Article/details/gnrxyijrb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gztqtniti.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gdxlalodz.sHtML

I. 正则表达式
来源：http://read.share.bbcook.cn/Article/details/ghtimzlub.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/glytnjsvw.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gpyvivmpm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gftpedhng.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gdioypobz.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gsoqllxyr.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gyequevpb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.bbcook.cn/Article/details/gaprsbjyh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/gmnuvtxml.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gutaeidej.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.epnwcf.com/Article/details/gobzobgzv.sHtML

[I02] 提取所有匹配
来源：http://read.share.epnwcf.com/Article/details/gyywherpc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.tarul.cn/Article/details/gbqycgtpm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.bbcook.cn/Article/details/givsrsmxf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.bbcook.cn/Article/details/gehkhefyj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.bbcook.cn/Article/details/gsxtcpyny.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gryismxti.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gbvuvboqt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/grvvepwkh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.yfazqb.com/Article/details/gfyoqzubf.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/gmluopfbe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gayjdleeg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.yfazqb.com/Article/details/gkihexbey.sHtML


<!-- 参考信息 -->