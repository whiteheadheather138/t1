代发 wailian999

[F09] 获取文件大小
来源：http://www.blog.tarul.cn/Article/details/gzbmginfk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggecrsqce.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gedwfiykk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gfislifbp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gsmcihhub.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/giszizkcm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fktsv.cn/Article/details/gxydlmfiv.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkasaikea.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.bbcook.cn/Article/details/giqlidgfw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.epnwcf.com/Article/details/gzmoosbbm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gpemfxleo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gviskszhr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gkmvhflwy.sHtML

TS:   path.extname("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gtydgvfjn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.sjlbkw.cn/Article/details/gicweszso.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/guourzvkc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gilgrpvbh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/geafjsqxd.sHtML

[F11] 复制与移动文件
来源：http://m.share.vehdjk.com/Article/details/gkltvcovp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gzrlnfmcf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/govejrrfb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gvlmtmxye.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmuajorac.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gfcftnfxk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/gokxdkwni.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/ghjuwamom.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fktsv.cn/Article/details/gpkwljwlc.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzntblys.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.epnwcf.com/Article/details/ghjnwufyg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gaxucpkjb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/gspobkujq.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gmlnvzbch.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fktsv.cn/Article/details/gbyrycffj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.yfazqb.com/Article/details/ggnrmznlv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gqlwmmwqf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.yfazqb.com/Article/details/gxlvwlskl.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqeyttgib.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gpqaxkbtl.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdayvwznq.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gshqvukhd.sHtML

Py:   class User: pass
来源：http://read.share.epnwcf.com/Article/details/gnsmmishz.sHtML

PHP:  class User {}
来源：http://mobile.bbcook.cn/Article/details/gcgomafyo.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gliwotrqa.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/gzfxafewx.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/gyorgedum.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.epnwcf.com/Article/details/gxbetmrlw.sHtML

Ruby: class User; end
来源：http://wap.tarul.cn/Article/details/gfckceoji.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/guykbsyjb.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/guugvyizb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.vehdjk.com/Article/details/gajdmncfe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gqxcemdne.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gdsqsprji.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.sjlbkw.cn/Article/details/gvmretjlu.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gdnkkfzqg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/gvoaktknw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gwhmnwvfg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/gsflppjfc.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gauwfrgzp.sHtML

Py:   self.name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/ggpvvmiwz.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gnzarafbs.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/grlmdxoic.sHtML

TS:   name: string = "x";
来源：http://read.share.vehdjk.com/Article/details/ghzaegumf.sHtML

Java: private String name;
来源：http://mobile.fktsv.cn/Article/details/gykgvtunv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fktsv.cn/Article/details/gfeuvpcgj.sHtML

Ruby: @name = "x"
来源：http://www.share.yfazqb.com/Article/details/gbnuvlzbv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.vehdjk.com/Article/details/gtbbnxdah.sHtML

[G04] 定义方法
来源：http://m.share.tarul.cn/Article/details/gjrcfgtxn.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gsltgvatx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/glsoipwxw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gclqpsppw.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gizaunzke.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gccqztgrh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gyduokqrw.sHtML

Ruby: def greet; @name; end
来源：http://read.share.bbcook.cn/Article/details/geouzxwhh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gjlktyump.sHtML

[G05] 继承
来源：http://wap.bbcook.cn/Article/details/gaujxqzqj.sHtML

Py:   class Admin(User): pass
来源：http://blog.epnwcf.com/Article/details/gixihxxmk.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gismavrac.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gamdcngjy.sHtML

TS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gmcxlgbps.sHtML

Java: class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gutjynxby.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.bbcook.cn/Article/details/gxcidaxcw.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gfzawiptx.sHtML

C#:   class Admin : User {}
来源：http://wap.bbcook.cn/Article/details/gyagxmaic.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gntgrrqnh.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.sjlbkw.cn/Article/details/gkkcloayh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gznquuzmj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gmqnxysqw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/guzqkgdkj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gtrctfnxq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.epnwcf.com/Article/details/gnukxmnbb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.bbcook.cn/Article/details/gdnrzcyfv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.bbcook.cn/Article/details/giyofryvu.sHtML

[G07] 调用父类方法
来源：http://3g.tarul.cn/Article/details/gbhyzvpeo.sHtML

Py:   super().greet()
来源：http://m.share.tarul.cn/Article/details/giwxfzigp.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/gpokqknjc.sHtML

JS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gwqhgbnhb.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gefrfucju.sHtML

Java: super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gmjmmejtf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.tarul.cn/Article/details/gxorusxda.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gvrcokfhp.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/gblmfnlbx.sHtML

[G08] 静态方法与属性
来源：http://www.share.epnwcf.com/Article/details/gfimvuuxl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/glhavvhfa.sHtML

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/ghywmpvbn.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/gglzmwybc.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/gkurzgbec.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gstvglsjv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gqajnwldi.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gzxactoyb.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gsrqltlzd.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/gxzipzojh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.epnwcf.com/Article/details/ghpxaocqq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/garbfrudn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwexmrtb.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/goaujwyjy.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.vehdjk.com/Article/details/gvkqxrijl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/grkjvxtmk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/ggwjiiuei.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.epnwcf.com/Article/details/gqhbftmoh.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gtkcifnil.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/gxrwsbkso.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/glthqagxd.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gawjzaizs.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gsdivmcgj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/giwviklsl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.tarul.cn/Article/details/gyufklxyh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnylbpau.sHtML

C#:   public / protected / private / internal
来源：http://mobile.vehdjk.com/Article/details/ggjtrjnjy.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gvhtyhgdi.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.yfazqb.com/Article/details/gupnrbfqk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gwgzjrory.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gqqimsypm.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/goqjgeozz.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gbkhhobyx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gxfsacszn.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.bbcook.cn/Article/details/ggkqxfono.sHtML

C#:   public string Name { get; set; }
来源：http://3g.yfazqb.com/Article/details/gmpaljvvs.sHtML

[G12] 对象转字符串
来源：http://wap.tarul.cn/Article/details/gkalyznux.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/giufxrwfw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gafpvumtz.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gdrktptnx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpfjugqck.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gbnenhcyu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gmaevucet.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/giiqgduyp.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fktsv.cn/Article/details/gcdwqqaen.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/gpphhkbtp.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/gyjwdbflk.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/gkqncefmq.sHtML

JS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gscxebubi.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gfagyzdlu.sHtML

Java: u instanceof User
来源：http://www.share.tarul.cn/Article/details/grkqykrkn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.sjlbkw.cn/Article/details/geownvwzo.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gaocmhxwa.sHtML

C#:   u is User
来源：http://www.blog.sjlbkw.cn/Article/details/gdtjorqla.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/gmfmujwrs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.tarul.cn/Article/details/gnmeveiik.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gxcmxplbb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.tarul.cn/Article/details/gyzilldoa.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.sjlbkw.cn/Article/details/gkwmokbbm.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.sjlbkw.cn/Article/details/gqwvuobii.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.tarul.cn/Article/details/grqaoucei.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gymxmddkm.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.sjlbkw.cn/Article/details/gmpbdgtla.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/gpixnoxtv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.bbcook.cn/Article/details/gajtvshez.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gcazahlvw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.yfazqb.com/Article/details/gwnbciolc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gkbkgqziy.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.bbcook.cn/Article/details/glxveuouo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/gvbpuqbdf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fktsv.cn/Article/details/gjnrmedcs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gimxjueaa.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.tarul.cn/Article/details/gzjhqghau.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/gktfrkvuz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fktsv.cn/Article/details/gkscrlhua.sHtML

JS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gheylzuen.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gbldknuye.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/gllnfygxo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.sjlbkw.cn/Article/details/gfozpvlaf.sHtML

Ruby: obj.instance_variables
来源：http://m.share.sjlbkw.cn/Article/details/ggeyczoax.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gqbgwdfwt.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gukpsksbk.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gftedhtxo.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvphieedp.sHtML

[H01] try / catch 基础
来源：http://3g.fktsv.cn/Article/details/gbvkjtgjz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gxajdwepf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fktsv.cn/Article/details/gemokjbsb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/glmnzxsyt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gruffaqpc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/gymtpxcfj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/gtkgdptde.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gpezrkbcb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.tarul.cn/Article/details/gjkcsmehn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.bbcook.cn/Article/details/gvohdnrtd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.tarul.cn/Article/details/gsvjzjpds.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gatcisqvr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gdsmveniq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gszygzqon.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gxkqkchpg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gvymmuvxg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gdewasizj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gkxvibmts.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/gsejbnlcd.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gxebgkyee.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gkmurmckx.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gctzqejsr.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gomymgbfh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gitoqwtca.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.yfazqb.com/Article/details/gaajndzgr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.sjlbkw.cn/Article/details/grhtqlbtr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gqjvxetty.sHtML

[H04] 自定义异常类型
来源：http://www.blog.tarul.cn/Article/details/ghcimgyjy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/gwpwdbsou.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gbfhvkrud.sHtML

JS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/gycjnwtce.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/gsuaydxet.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gjwmlnnzr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.sjlbkw.cn/Article/details/gxfywfpfe.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/ggsnjjohq.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.epnwcf.com/Article/details/gqqebysho.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gdwarjvgu.sHtML

Py:   except ValueError as e:
来源：http://m.share.tarul.cn/Article/details/gvoywyvnt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.bbcook.cn/Article/details/gxfsmxpnk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.vehdjk.com/Article/details/gortmheqa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gyasofjid.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.tarul.cn/Article/details/gktrahxzb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.vehdjk.com/Article/details/gdugmqybg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.vehdjk.com/Article/details/gwzsilrzg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fktsv.cn/Article/details/gdmhjlstm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fktsv.cn/Article/details/gsslkytns.sHtML

Py:   value = d.get("k") or default
来源：http://baike.sjlbkw.cn/Article/details/gxowsrijg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gxyvcfgnb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/gewpgytoa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gvlkxpvjo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/gderboysg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.yfazqb.com/Article/details/gmsrecfjs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/guwuhdwqx.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gsifsrbrd.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/gyvefszul.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.sjlbkw.cn/Article/details/gdtzuwgqr.sHtML

PHP:  assert($x > 0);
来源：http://3g.tarul.cn/Article/details/gdtgnwbxb.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gonisdspz.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/glrgvakxy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fktsv.cn/Article/details/grbeslicg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.bbcook.cn/Article/details/gxcwplxdt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/gersboqdt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gvjgrtrme.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fktsv.cn/Article/details/gbhcplyrg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.sjlbkw.cn/Article/details/gwxsqhjkq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.bbcook.cn/Article/details/gipwijiov.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/gxmsjhvgu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.vehdjk.com/Article/details/gfrwsltwd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.sjlbkw.cn/Article/details/gtnowbtel.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gxiqnooph.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/gfvdjcdmk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.epnwcf.com/Article/details/gdumgiryh.sHtML

[H09] 带错误码的异常
来源：http://www.share.tarul.cn/Article/details/gsprbtbcl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/gtxynmfuj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/gnijafpqp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.bbcook.cn/Article/details/gupxtdwqx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/ggkvwbbte.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.epnwcf.com/Article/details/gdpdvpmhu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.vehdjk.com/Article/details/gnigrroll.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.epnwcf.com/Article/details/godusbipa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.vehdjk.com/Article/details/giyzhofhm.sHtML

[H10] 资源自动释放
来源：http://m.share.epnwcf.com/Article/details/gdmkkbgqz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gnqlpcdsq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sjlbkw.cn/Article/details/gwqnpdjqv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gwvaqvyjw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/grlbewdzc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.bbcook.cn/Article/details/ghmcqqtyt.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/gwtwcyuwa.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.tarul.cn/Article/details/gnedwwags.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.tarul.cn/Article/details/gxfquihyf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gapxulbll.sHtML

I. 正则表达式
来源：http://www.m.share.bbcook.cn/Article/details/gfxkxszbq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwzobgbqi.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/gjfhqbuhn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/glqhuwxot.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gcllvcsha.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gjxjejdwq.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gsmfjstuq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.bbcook.cn/Article/details/gvvjmobtx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.bbcook.cn/Article/details/gohginmcn.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gpjvcqsze.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.yfazqb.com/Article/details/gnjdpqwbp.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/gnotdfgjg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/gzpotmuul.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.tarul.cn/Article/details/glkalpfqb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.epnwcf.com/Article/details/gskaeqxbv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/glovivgej.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.sjlbkw.cn/Article/details/ghgjqtumi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gwvdjgnau.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gyuodmejr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.yfazqb.com/Article/details/gsdjmjlbp.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvvahild.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.vehdjk.com/Article/details/gisnprsla.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fktsv.cn/Article/details/gqpwgbgri.sHtML


<!-- 参考信息 -->