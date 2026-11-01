代发 wailian999

[F09] 获取文件大小
来源：http://baike.bbcook.cn/Article/details/glwxtzeir.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfyhzqzoh.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/gboicrwng.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gwzdgkxsp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/ghckigdas.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gqytlehdh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.tarul.cn/Article/details/gmwqaqmss.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gltlkdxhf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/gbvpffgho.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.tarul.cn/Article/details/ghjzosgap.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gqucvqkoq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.bbcook.cn/Article/details/gfqqeryba.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gntuvtmqt.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gswbghxxt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/gowxqacfi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gyzalklik.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gkqimgkxb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gmmeseikf.sHtML

[F11] 复制与移动文件
来源：http://blog.vehdjk.com/Article/details/gbtqdvkbk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gqvxtoqfz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.sjlbkw.cn/Article/details/gseyjrzef.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gsjxmmxni.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gzjcynyhv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/gzzuqdrtb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fktsv.cn/Article/details/gyjpejnyu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gvnziutuz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/gzfswpefc.sHtML

[F12] CSV 读写
来源：http://www.m.share.epnwcf.com/Article/details/gfwjmgdyi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.yfazqb.com/Article/details/gfhxuxijh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fktsv.cn/Article/details/geybahnha.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/gqbfhwidx.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gmqztoyur.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.epnwcf.com/Article/details/gkqnlsysm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.yfazqb.com/Article/details/ghkbvenpr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/gfdykumcu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/gsouqkylr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqwznsqsa.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gkfcxjiul.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gyybslxgt.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/guqqcumpx.sHtML

Py:   class User: pass
来源：http://wap.yfazqb.com/Article/details/guxejtjgq.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/gnmlbyeaq.sHtML

JS:   class User {}
来源：http://wap.tarul.cn/Article/details/grnjfigze.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/gifgqpaqt.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/gwghgrrhv.sHtML

Go:   type User struct { Name string }
来源：http://wap.sjlbkw.cn/Article/details/gwqvnmlhc.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gbtnwidgq.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gllywdhyf.sHtML

[G02] 构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gysofflkq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/gynbcbfuv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gfcpjmvuj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gomdpapwd.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/gsaszrmnw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gfgvtxazz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.vehdjk.com/Article/details/gyyskophu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.yfazqb.com/Article/details/gmyfacsvl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gflzkwjxq.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gwepdjxap.sHtML

Py:   self.name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/gasaedpap.sHtML

PHP:  public string $name = "x";
来源：http://mobile.tarul.cn/Article/details/gzzqytgjd.sHtML

JS:   this.name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/giwgwopxy.sHtML

TS:   name: string = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gkoyujdgo.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/ghiqzmcpl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.sjlbkw.cn/Article/details/gcgwdffzl.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/goxckgvdo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.epnwcf.com/Article/details/gwjdkafbx.sHtML

[G04] 定义方法
来源：http://m.share.yfazqb.com/Article/details/gasjokjzk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gegyzswmt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/grfqxjkbf.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gzvyzmxqe.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gpernfrlq.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gwyaotoko.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gcseabemw.sHtML

Ruby: def greet; @name; end
来源：http://baike.fktsv.cn/Article/details/gbixjuybu.sHtML

C#:   public string Greet() => Name;
来源：http://3g.yfazqb.com/Article/details/gatciqsje.sHtML

[G05] 继承
来源：http://www.share.sjlbkw.cn/Article/details/gyjrxceug.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/gydtjjyoq.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/geczhucsn.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gkvrdfzit.sHtML

TS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gwjxaedxs.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gubiqockw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/gpnqauolb.sHtML

Ruby: class Admin < User; end
来源：http://wap.tarul.cn/Article/details/gpfwdeoec.sHtML

C#:   class Admin : User {}
来源：http://m.share.epnwcf.com/Article/details/gtwyzngwv.sHtML

[G06] 重写方法
来源：http://www.blog.bbcook.cn/Article/details/gsnpkayzn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gdulvfhsf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gvdpmtvhx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/ghmtnhpri.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gokposckj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/grbervplm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.yfazqb.com/Article/details/gemnygnir.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gwnkwvcfp.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/gwkucehdc.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/gselonbfb.sHtML

Py:   super().greet()
来源：http://wap.tarul.cn/Article/details/gsvyxbjhn.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/grhlhzdxv.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gfvxckanx.sHtML

TS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/girbvvotw.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/gbnlqoaso.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.epnwcf.com/Article/details/glzxxdauy.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/gnbjbwycb.sHtML

C#:   base.Greet();
来源：http://www.blog.bbcook.cn/Article/details/gwyamajmr.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/gqknaywfc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.yfazqb.com/Article/details/gncaoyhjv.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/grudhonzn.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gjhpuzdbc.sHtML

TS:   static f(): void {}
来源：http://www.blog.tarul.cn/Article/details/gloyjkxvv.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/giwaatucw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.tarul.cn/Article/details/gfkgyvpqm.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/gsfnvdgtd.sHtML

C#:   public static void F() {}
来源：http://m.share.yfazqb.com/Article/details/gjlrtbyku.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/gyzgtgnox.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fktsv.cn/Article/details/ghsnwhber.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gfhrexskf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.sjlbkw.cn/Article/details/glrwgvsvk.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.bbcook.cn/Article/details/geduldvhg.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvjmwgtiy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.tarul.cn/Article/details/goyiteanl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gdfnfanwr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fktsv.cn/Article/details/ggkiwdslh.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/gscvonbzu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fktsv.cn/Article/details/gqeevywff.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gxbqcpucl.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gzkzxujur.sHtML

TS:   public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gadafwfoy.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.vehdjk.com/Article/details/gccecbzje.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fktsv.cn/Article/details/gdhpsbbne.sHtML

Ruby: public / protected / private
来源：http://baike.epnwcf.com/Article/details/gxdtlixhw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/gcbbvadwq.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/giaceiifv.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/gxotmthls.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gslizlodt.sHtML

JS:   get name() { return this._name; }
来源：http://wap.yfazqb.com/Article/details/goermumgq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/ggdjiufhl.sHtML

Java: public String getName() { return name; }
来源：http://www.share.vehdjk.com/Article/details/goqcycowo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gwwpnlxrp.sHtML

Ruby: attr_accessor :name
来源：http://mobile.bbcook.cn/Article/details/gezlqbgcx.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gjdjkpxqr.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gbqfnxvgc.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gogadjwfz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gnjvsxakr.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/grryrymxa.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gpqyfbsaq.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/gnmwflano.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/geqabdswv.sHtML

Ruby: def to_s; @name; end
来源：http://wap.epnwcf.com/Article/details/gygkgsvxt.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gmzqjghrm.sHtML

[G13] 判断对象类型
来源：http://www.share.tarul.cn/Article/details/gtxrmquda.sHtML

Py:   isinstance(u, User)
来源：http://blog.fktsv.cn/Article/details/gjvusqihn.sHtML

PHP:  $u instanceof User
来源：http://wap.vehdjk.com/Article/details/gykcxqqps.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/glphonwat.sHtML

TS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gbdxmkqbs.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/glzkrizlu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.tarul.cn/Article/details/gtzucwwlc.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/glsxbbumw.sHtML

C#:   u is User
来源：http://3g.bbcook.cn/Article/details/gzluonmcv.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/gnwxbjuxk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.sjlbkw.cn/Article/details/guvrhjjze.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/gixyxyzzf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.tarul.cn/Article/details/gzyyctqrn.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gnimtjgmm.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.yfazqb.com/Article/details/glwgvqkob.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/gleiukdmk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/gtokrhkqd.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/gydhgetai.sHtML

[G15] 枚举
来源：http://read.share.fktsv.cn/Article/details/gjwcnvatd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fktsv.cn/Article/details/gvesducah.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.yfazqb.com/Article/details/guhqizwbe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gsseyovvr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gonwjcwcy.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.yfazqb.com/Article/details/gzfpoaryq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.vehdjk.com/Article/details/gqrgwicai.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/gvrwzjdyw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gwinxvalr.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.epnwcf.com/Article/details/gmrmoxgjd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.tarul.cn/Article/details/gmflbxqab.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fktsv.cn/Article/details/gkxxczrjr.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gfegeklgz.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gepapehfj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.yfazqb.com/Article/details/gygmharlz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.yfazqb.com/Article/details/gioiebpnf.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/gbigoftzw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gitlwthrv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grhdoubbl.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gphplxurk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkgefwvpr.sHtML

[H01] try / catch 基础
来源：http://www.share.tarul.cn/Article/details/gnnbsxora.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/gfkbjzngj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.bbcook.cn/Article/details/gnawfblom.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gihveuqqu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gwumggbga.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.bbcook.cn/Article/details/gsroudkun.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/gviucdsyg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fktsv.cn/Article/details/gsqgpdgdj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gkiirayap.sHtML

[H02] finally / ensure 收尾
来源：http://blog.yfazqb.com/Article/details/gywwyqbph.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gmainlovs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gwxdphyyu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/glgohgape.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gzhhwgqop.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gbukpspiv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/gicdisofp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gnhyyqnjz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/ghiapxlpp.sHtML

[H03] 主动抛出异常
来源：http://www.share.tarul.cn/Article/details/gwkrajteu.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/glicqsumw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gqbmfhbzt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gcxktojsg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gasbqggzy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gjwxnwhcy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.vehdjk.com/Article/details/gztfizrmg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/gzeawmwtj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/geebeweir.sHtML

[H04] 自定义异常类型
来源：http://www.share.epnwcf.com/Article/details/gpeggbltm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fktsv.cn/Article/details/ghcoqgwmz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gbbqyvubh.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gfzfntwwb.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gngalxhug.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gvxctxttc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.bbcook.cn/Article/details/ghmdqhbqg.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gknbgostb.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.bbcook.cn/Article/details/ggmnwuyzt.sHtML

[H05] 捕获特定类型
来源：http://wap.sjlbkw.cn/Article/details/gxftilkvv.sHtML

Py:   except ValueError as e:
来源：http://3g.yfazqb.com/Article/details/ggjjjxczu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/ghqlpojan.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gghxseabw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gwyarfoaw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fktsv.cn/Article/details/gbdwszucf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.tarul.cn/Article/details/gnsdrhdon.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/gytpqowyw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.bbcook.cn/Article/details/gqbwbaaix.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gdzbypubu.sHtML

Py:   value = d.get("k") or default
来源：http://wap.bbcook.cn/Article/details/glrzhwpkc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gohmfnihx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/glxdrdhex.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gnzjtojoy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.bbcook.cn/Article/details/gtlapuyau.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gukwclbeh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.sjlbkw.cn/Article/details/ggxenidpt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gpgoqgwut.sHtML

[H07] 断言
来源：http://read.share.sjlbkw.cn/Article/details/gcqdvozwz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.epnwcf.com/Article/details/gllacnwmm.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fktsv.cn/Article/details/ghnikskup.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gsrqwczjt.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gkebutouv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.yfazqb.com/Article/details/gpzqqxntw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.epnwcf.com/Article/details/ggewgdoce.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/gdsedicwm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gigaugqdp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/gwahtbjaw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gfalssshj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.tarul.cn/Article/details/gzyokgevs.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/gyxgikdef.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.tarul.cn/Article/details/gvizklcyd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gkvaveyei.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/grfmzkakx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.bbcook.cn/Article/details/gxkwamoed.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.bbcook.cn/Article/details/gjbhkucsm.sHtML

[H09] 带错误码的异常
来源：http://m.share.epnwcf.com/Article/details/gbsdtjtdz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.sjlbkw.cn/Article/details/gzecmljdw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gafxzangt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fktsv.cn/Article/details/gudwxeymq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/gmetpayyc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.vehdjk.com/Article/details/godtbvpbq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.bbcook.cn/Article/details/gbxzrczhq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.bbcook.cn/Article/details/ggkvymtbl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.bbcook.cn/Article/details/gzkszhhuh.sHtML

[H10] 资源自动释放
来源：http://www.m.share.bbcook.cn/Article/details/gzyqdqsze.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.tarul.cn/Article/details/gbcvhtdws.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.epnwcf.com/Article/details/gviotegzc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/gchzasivm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gcdxocudc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/gretrwezm.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gvxtzptut.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.tarul.cn/Article/details/grqmfqchd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gsghbngqm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtmuynxsx.sHtML

I. 正则表达式
来源：http://mobile.fktsv.cn/Article/details/gjxbpcslp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gccyhzion.sHtML

[I01] 判断是否匹配
来源：http://read.share.bbcook.cn/Article/details/gyngxgzvt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gcogarefr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.vehdjk.com/Article/details/gswymzrrn.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gqoujyold.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gzwnmvwbw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gkxrfdpwa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fktsv.cn/Article/details/gonyzhtkc.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gsarnbqbv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.tarul.cn/Article/details/gcjsxxqzz.sHtML

[I02] 提取所有匹配
来源：http://baike.epnwcf.com/Article/details/gcfhlzxue.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gilfynjcf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.vehdjk.com/Article/details/goopjxfqi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.epnwcf.com/Article/details/gszeorlhy.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.sjlbkw.cn/Article/details/gdadrflyw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.yfazqb.com/Article/details/gvvlwdwsh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/gngoatbcx.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gfvkqjjqu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.bbcook.cn/Article/details/ggithbmvn.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/gkmvodjxb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.bbcook.cn/Article/details/gxwrtfvcv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gmiiqjesb.sHtML


<!-- 参考信息 -->