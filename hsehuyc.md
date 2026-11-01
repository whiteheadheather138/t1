代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/glwgtdfrz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gtzjkrgti.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/gnfcaiipu.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmygqjnh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gyjzgazxj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gpagvghyy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/grcqrkmyv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/goomvihzi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gmyivpktd.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fktsv.cn/Article/details/gtctlllmo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.bbcook.cn/Article/details/gqmkxjafm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gzeaosdki.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gvogmuvkc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gfdeurufu.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/gezylmgdu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gxcvxyzos.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/gpkvevevx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gjjluubct.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/glmyhuhpe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.bbcook.cn/Article/details/gjbghrhbq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.vehdjk.com/Article/details/gebjqraoh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/glxocobug.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.bbcook.cn/Article/details/ghbtpaopu.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gngmqznze.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.vehdjk.com/Article/details/gjpnpcnuf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.bbcook.cn/Article/details/gvbtbtvbi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/gixowjvto.sHtML

TS:   // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gcktlkwaa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.epnwcf.com/Article/details/gqgiwracz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/gokmynomg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.bbcook.cn/Article/details/gpnxzcgmm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.sjlbkw.cn/Article/details/gzpeqenni.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnetbzats.sHtML

G. 面向对象
来源：http://m.share.sjlbkw.cn/Article/details/gafljjvbm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gknagwwgz.sHtML

[G01] 定义类
来源：http://mobile.fktsv.cn/Article/details/gujecmnof.sHtML

Py:   class User: pass
来源：http://www.blog.sjlbkw.cn/Article/details/gjwcdcfxc.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/gjfjclmph.sHtML

JS:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gdcehjecn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fktsv.cn/Article/details/gecpelamz.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gjafnvhzl.sHtML

Go:   type User struct { Name string }
来源：http://read.share.epnwcf.com/Article/details/gmvobxseq.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/glebpljec.sHtML

C#:   class User {}
来源：http://mobile.epnwcf.com/Article/details/glqvlffba.sHtML

[G02] 构造函数
来源：http://www.blog.yfazqb.com/Article/details/gonaofmwz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.vehdjk.com/Article/details/gmadoybvf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/gyeeoxlsr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gwubdsome.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.bbcook.cn/Article/details/gecxsyxvt.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/goibpzbyp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/gqjxwymor.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/gupefsbqt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/grrfgywvl.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gqshewbnu.sHtML

Py:   self.name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gvldeqaos.sHtML

PHP:  public string $name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gjciaychi.sHtML

JS:   this.name = "x";
来源：http://www.share.bbcook.cn/Article/details/ghshaiyim.sHtML

TS:   name: string = "x";
来源：http://m.share.fktsv.cn/Article/details/ghamjnscb.sHtML

Java: private String name;
来源：http://wap.epnwcf.com/Article/details/gybmnlair.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/gkgnxcdwc.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/guzqxddcq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fktsv.cn/Article/details/gmecnsfqg.sHtML

[G04] 定义方法
来源：http://baike.vehdjk.com/Article/details/gvuvakljx.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gayjtojcc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gmvwknert.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gavepbaec.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gwxzrgzpz.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/ggoykapoi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/ggxumfhic.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/gctgyaqvs.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.yfazqb.com/Article/details/gefgaazup.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/gpojcgvuw.sHtML

Py:   class Admin(User): pass
来源：http://read.share.tarul.cn/Article/details/gidsaqbqm.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gurrtfvlu.sHtML

JS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gnijjqcha.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gcigapqek.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gioenmwin.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.bbcook.cn/Article/details/gvrhsctim.sHtML

Ruby: class Admin < User; end
来源：http://blog.bbcook.cn/Article/details/geekxxrvq.sHtML

C#:   class Admin : User {}
来源：http://read.share.tarul.cn/Article/details/giwxoqhpm.sHtML

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/gaspnqvin.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.bbcook.cn/Article/details/goarsdlhx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcsbjnnn.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gbldjbhov.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gdmumcyua.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/grpqfvemx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.sjlbkw.cn/Article/details/gstzivnjn.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.bbcook.cn/Article/details/gtwssyzrp.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.epnwcf.com/Article/details/glkvzsokt.sHtML

[G07] 调用父类方法
来源：http://m.share.tarul.cn/Article/details/gzxyhuviv.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/gknxgcvwi.sHtML

PHP:  parent::greet();
来源：http://3g.tarul.cn/Article/details/gpcynsevm.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/glwwfzhgm.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/goyfhizqy.sHtML

Java: super.greet();
来源：http://mobile.bbcook.cn/Article/details/gpuquqerx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.yfazqb.com/Article/details/gnhhlbcor.sHtML

Ruby: super
来源：http://baike.epnwcf.com/Article/details/gjumcidco.sHtML

C#:   base.Greet();
来源：http://m.share.yfazqb.com/Article/details/gormrxdfi.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fktsv.cn/Article/details/gpqzradbe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gccpawilq.sHtML

PHP:  public static function f() {}
来源：http://3g.tarul.cn/Article/details/gnhanbvgu.sHtML

JS:   static f() {}
来源：http://blog.bbcook.cn/Article/details/gxzpepwer.sHtML

TS:   static f(): void {}
来源：http://www.blog.epnwcf.com/Article/details/gyzqxpkhx.sHtML

Java: static void f() {}
来源：http://mobile.vehdjk.com/Article/details/gbqjfrspk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gnczealin.sHtML

Ruby: def self.f; end
来源：http://wap.sjlbkw.cn/Article/details/gkjrozcvv.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/gdtiiewmq.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.tarul.cn/Article/details/gzcxdbste.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fktsv.cn/Article/details/gnkjqdfrq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.bbcook.cn/Article/details/golkdlasn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.yfazqb.com/Article/details/gftpucbvm.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/gnuqesxkn.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fktsv.cn/Article/details/gnzhdzgrh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gzlznjppz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.sjlbkw.cn/Article/details/gktecojwz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/glasrqaxq.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/gxxcjxoiq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.bbcook.cn/Article/details/gmuiccrkj.sHtML

PHP:  public / protected / private
来源：http://read.share.epnwcf.com/Article/details/goymqkjrj.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.sjlbkw.cn/Article/details/gcsbjpoxj.sHtML

TS:   public / protected / private
来源：http://blog.yfazqb.com/Article/details/gojyxemmx.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/gcoesnstq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/greeofokf.sHtML

Ruby: public / protected / private
来源：http://3g.fktsv.cn/Article/details/gchujfamp.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fktsv.cn/Article/details/gwconrtfr.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gyxvyemwv.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gewxqhbch.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gapcfcmqw.sHtML

JS:   get name() { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gprgzoiui.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/geyfzfwuf.sHtML

Java: public String getName() { return name; }
来源：http://baike.fktsv.cn/Article/details/gsmdpwinh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gjdhsyuvx.sHtML

Ruby: attr_accessor :name
来源：http://read.share.sjlbkw.cn/Article/details/gmnnsdhiz.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpnxfqcx.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/giebhogon.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.vehdjk.com/Article/details/goicighfl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxxrghacx.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gxjqbzkvd.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/glyikjcyz.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/grlvusxxp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/glrrffoqq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gyzlvbeka.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gkdoyynao.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/giijefdbf.sHtML

Py:   isinstance(u, User)
来源：http://3g.yfazqb.com/Article/details/glhsqwcpm.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gzgpdyqar.sHtML

JS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gfkhwodez.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gcdpooyks.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gjtytpqhz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/gzocrilsu.sHtML

Ruby: u.is_a?(User)
来源：http://baike.yfazqb.com/Article/details/gvkwpsnrw.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/ghifdhilh.sHtML

[G14] 数据类 / record
来源：http://www.m.share.yfazqb.com/Article/details/gbflbakbb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.yfazqb.com/Article/details/gvgphubah.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.bbcook.cn/Article/details/ghujahyqo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.yfazqb.com/Article/details/gubnenwia.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/guwxshorz.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.epnwcf.com/Article/details/gzmolaxic.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gjgmtvqrv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/gitgxjbul.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gnmfhtlis.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/gkwbuighh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.vehdjk.com/Article/details/gkkmcriax.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.tarul.cn/Article/details/ghmjprvdb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/gtaasiobm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gendwnjdj.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/gjdgemfew.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/gigtsvyfi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fktsv.cn/Article/details/gvkqxyqgg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gxlqkfosc.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/ggwwfvxae.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/gafkifzhu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gwfzcltkr.sHtML

JS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gigluozmv.sHtML

TS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gbjlfsbpq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.sjlbkw.cn/Article/details/gbngnrfhg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fktsv.cn/Article/details/glyoofrtn.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/giclbxedn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gotfnoqcu.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gmbrzcywp.sHtML

H. 异常与错误处理
来源：http://wap.epnwcf.com/Article/details/gtenxixza.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxvwhmmrq.sHtML

[H01] try / catch 基础
来源：http://www.blog.tarul.cn/Article/details/gdwkvegiv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gbmkvoqdx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.vehdjk.com/Article/details/gnxzfcldv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gmhqeckmv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gfunfyxyi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.sjlbkw.cn/Article/details/gtnoviqqt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.yfazqb.com/Article/details/gtvrphapk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.tarul.cn/Article/details/gtqlfruad.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.yfazqb.com/Article/details/gewnogjuw.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gfufkuerp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/glpdqiedl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gdtavkrru.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gtzafouwe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gqhsnnkcx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gigyfcgox.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/gscujyout.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gjauwsgxk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gczrwissr.sHtML

[H03] 主动抛出异常
来源：http://wap.bbcook.cn/Article/details/gpxbhpqwm.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.tarul.cn/Article/details/ghzslmryj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gxwlgbhip.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/giizgqqoc.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gpkjjnbul.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gzcmbkqxg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.vehdjk.com/Article/details/gddulrwhb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gvarshiql.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gjgcsbxus.sHtML

[H04] 自定义异常类型
来源：http://read.share.bbcook.cn/Article/details/gxhnhxxkd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gajbvfygt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/grzqwtsxt.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/glrqmwklk.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gutupbmef.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gcusgbhsy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.vehdjk.com/Article/details/guqskpxpb.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/gqijtkyvm.sHtML

C#:   class MyException : Exception {}
来源：http://wap.yfazqb.com/Article/details/gmvcvvqya.sHtML

[H05] 捕获特定类型
来源：http://mobile.tarul.cn/Article/details/gtngwflcj.sHtML

Py:   except ValueError as e:
来源：http://wap.bbcook.cn/Article/details/gkicldlwd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.sjlbkw.cn/Article/details/gpsojetoa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gfohznsud.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/govioqqmv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/gjjxochrt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.sjlbkw.cn/Article/details/glzfmvrmn.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.yfazqb.com/Article/details/gakxlcvvn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.sjlbkw.cn/Article/details/gzdnicipq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.tarul.cn/Article/details/gcvcsmnvj.sHtML

Py:   value = d.get("k") or default
来源：http://baike.tarul.cn/Article/details/goshfhlwm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gwilfxzcd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/geftagdoz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gbfbvqbhj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gakqcfclk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.tarul.cn/Article/details/gdcojfczl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.epnwcf.com/Article/details/gyjdjlylg.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.sjlbkw.cn/Article/details/gjxgjsyza.sHtML

[H07] 断言
来源：http://read.share.tarul.cn/Article/details/gllzvaywv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/glnebtxjv.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/gggqolzqs.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gqmgvsilm.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/glsqlapyl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.bbcook.cn/Article/details/gtacaxypn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.vehdjk.com/Article/details/gibuabvtr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.vehdjk.com/Article/details/gtvndkpml.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gfkaceoit.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.bbcook.cn/Article/details/gtneubjfg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/gykiloltr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.sjlbkw.cn/Article/details/gfjegabls.sHtML

JS:   e.message;  e.stack
来源：http://baike.epnwcf.com/Article/details/gughozcae.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gkuqbiesz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.bbcook.cn/Article/details/gaewspocz.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/gstdmvmyu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.bbcook.cn/Article/details/gnxvmtnxf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fktsv.cn/Article/details/gkhtbjypj.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.bbcook.cn/Article/details/grsxmyvxh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/ggtxkfwdw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/gzgkeiozp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.vehdjk.com/Article/details/gwqpfhypq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/gktwzajwz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.yfazqb.com/Article/details/gdzthzqkv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/gplbtopkl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/gjwhhuzrb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.yfazqb.com/Article/details/gfndrtgpa.sHtML

[H10] 资源自动释放
来源：http://www.blog.vehdjk.com/Article/details/gjnafsjfi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.bbcook.cn/Article/details/guthcscsw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/gwagqikkg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gxavmpary.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/grhnulqil.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.vehdjk.com/Article/details/gdlpnhtbp.sHtML

Go:   defer f.Close()
来源：http://baike.vehdjk.com/Article/details/gdftnjvwg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/ghzkrlprm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/galunptze.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjtnommyt.sHtML

I. 正则表达式
来源：http://www.share.tarul.cn/Article/details/goysxvjvg.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gujeukigl.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/gtaeaqqyt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gmdofnxfr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.yfazqb.com/Article/details/ggbkqwxwz.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gpjuuptoq.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/ggkjljwot.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gqupxbgsu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.epnwcf.com/Article/details/guaeflnvl.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gtihkubwm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gxpwthyqo.sHtML

[I02] 提取所有匹配
来源：http://www.share.epnwcf.com/Article/details/gouzgahlg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gwifwupqi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/ghvxuppmd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.yfazqb.com/Article/details/goxzqxgba.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/gxdoitimq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/ggrgweihe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gtioppfmy.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gdlcqlcya.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gxpgjrobb.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fktsv.cn/Article/details/glxfyptsa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.yfazqb.com/Article/details/gkppmlpax.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/gckttcyad.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.vehdjk.com/Article/details/gamdpnctp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gqgybkdrr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fktsv.cn/Article/details/gnmzuntzn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fktsv.cn/Article/details/glsbeqyjx.sHtML


<!-- 参考信息 -->