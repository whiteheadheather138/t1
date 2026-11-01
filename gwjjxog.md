代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/gdvvgzbrm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gqyaetukx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gervkucki.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/gwnpujtnm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gclyyhlms.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gfokxdrod.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gzfjdygnd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/ghahbpmhv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gtxiqwwgx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gzwrexsvj.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/gwthmfcsz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/grghwkrzs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrnlonwf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/ggkizquce.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/guwnnossc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gnukltvxv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.bbcook.cn/Article/details/glapeaypy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gaybdjvyc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fktsv.cn/Article/details/gogvgtmoj.sHtML

[F12] CSV 读写
来源：http://mobile.vehdjk.com/Article/details/gfdkbequi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/gejpjzdzk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.epnwcf.com/Article/details/gxiuygpua.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/grtosjlzh.sHtML

TS:   // 同上
来源：http://baike.vehdjk.com/Article/details/gbyntgzel.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gtgdufeov.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.bbcook.cn/Article/details/gaidkbdqp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.yfazqb.com/Article/details/gbbvcirio.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/gzahaiybr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grjqjnalj.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gwveorwgk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjrdfdkxl.sHtML

[G01] 定义类
来源：http://www.m.share.epnwcf.com/Article/details/gxpafkzvj.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gtgznytho.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gpsbhmuna.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gdqquuaez.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gdulpujxw.sHtML

Java: class User {}
来源：http://wap.bbcook.cn/Article/details/grgjzxhhp.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gngqujusf.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/gqizczxxj.sHtML

C#:   class User {}
来源：http://baike.bbcook.cn/Article/details/gqkdegrhz.sHtML

[G02] 构造函数
来源：http://3g.yfazqb.com/Article/details/gwnqkowwi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/gfymasxlb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gwkuvaoes.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gixhcvldn.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/glhxltiwk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gsqbmtnjq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/gkycuhelq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.tarul.cn/Article/details/gpjyclqfw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/geqyexjyb.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/gjdiwsnyw.sHtML

Py:   self.name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gegxwzpru.sHtML

PHP:  public string $name = "x";
来源：http://read.share.yfazqb.com/Article/details/gbzrjferk.sHtML

JS:   this.name = "x";
来源：http://mobile.vehdjk.com/Article/details/gmzwuamcs.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/glkxyqges.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/gmkwpzqum.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.tarul.cn/Article/details/gaxfkjsus.sHtML

Ruby: @name = "x"
来源：http://mobile.bbcook.cn/Article/details/gkipldtlr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/gobogxzdv.sHtML

[G04] 定义方法
来源：http://www.blog.epnwcf.com/Article/details/gbtpgfslo.sHtML

Py:   def greet(self): return self.name
来源：http://3g.tarul.cn/Article/details/gxgbjwrvu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gsfqtkmpt.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gprsaewxr.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gkwjevmcw.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gnyycrsoj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gxylnybas.sHtML

Ruby: def greet; @name; end
来源：http://m.share.tarul.cn/Article/details/gufkuvlyl.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/giaqqiogp.sHtML

[G05] 继承
来源：http://read.share.epnwcf.com/Article/details/gnjzuxojw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gaucabevl.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gxohorxnh.sHtML

JS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gjyblroda.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gqxkumqgv.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/giajautzp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/gqmpzthme.sHtML

Ruby: class Admin < User; end
来源：http://read.share.sjlbkw.cn/Article/details/gaaywwukq.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/gicuohhrp.sHtML

[G06] 重写方法
来源：http://mobile.yfazqb.com/Article/details/gdfxarkqi.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gchkdnghj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gjswlhtfm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwvpafth.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjnvucdc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gppmxhtue.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/grwofmdnk.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/guwlmnxsn.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gpiukgexa.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/givtxepfg.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/glcqqkocq.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/gmmoxwwwi.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/ghgnkhsdm.sHtML

TS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/gujbalvhb.sHtML

Java: super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gaczsfjro.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/gxjnocjvz.sHtML

Ruby: super
来源：http://www.m.share.tarul.cn/Article/details/gplaayvvd.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/gbdqavlwk.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/gfyctwhqo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/gajtfvegr.sHtML

PHP:  public static function f() {}
来源：http://www.share.epnwcf.com/Article/details/gndksromu.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gnfuoippt.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/gbvyiyyqz.sHtML

Java: static void f() {}
来源：http://read.share.vehdjk.com/Article/details/goyhspxek.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.epnwcf.com/Article/details/gkyprdipd.sHtML

Ruby: def self.f; end
来源：http://www.m.share.vehdjk.com/Article/details/guqjxljeb.sHtML

C#:   public static void F() {}
来源：http://m.share.fktsv.cn/Article/details/gqdzyitlt.sHtML

[G09] 接口 / 抽象类
来源：http://blog.vehdjk.com/Article/details/gcjyumayd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.tarul.cn/Article/details/gusbxrfps.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/grzasknsl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gngxqfizz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/gphcsplrf.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/gxoqmtrxi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gvydqkevi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gjaqfydmt.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/ghvnphrax.sHtML

[G10] 访问控制
来源：http://blog.tarul.cn/Article/details/gtctnjsrv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gldlmhhqd.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/gpohuhkdl.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/gwufjlhtw.sHtML

TS:   public / protected / private
来源：http://wap.bbcook.cn/Article/details/guffgvnim.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/gbckobdvh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.vehdjk.com/Article/details/grskegill.sHtML

Ruby: public / protected / private
来源：http://wap.fktsv.cn/Article/details/gfehttquu.sHtML

C#:   public / protected / private / internal
来源：http://3g.bbcook.cn/Article/details/gwlivctnk.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gazeqwhmf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/gppdueowt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gtpwivoba.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gtharyrgs.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gsoylbrhf.sHtML

Java: public String getName() { return name; }
来源：http://blog.epnwcf.com/Article/details/glvznfaki.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gveehsaps.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/gqitnrpkd.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/gtuqhhsxm.sHtML

[G12] 对象转字符串
来源：http://www.share.fktsv.cn/Article/details/gnocgmgyr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gqzglxhqu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gnwmekjns.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gnsvwcvve.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gtgegrapw.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gfxkoulgi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/ghkobjvfr.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/ghjvsmhjl.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gvzsbxcrr.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gjgtfmuim.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gqvzdtjzx.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gzzaueqyx.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gdntcsmwd.sHtML

TS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/gsdpulpyd.sHtML

Java: u instanceof User
来源：http://blog.tarul.cn/Article/details/gdufygiwc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/ggnikcipy.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjlsicbe.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/gyywjkven.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gciqzhtum.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gedvgzqse.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/gaxtmrsaq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gpnxpkgmx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.vehdjk.com/Article/details/gtohbfajg.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gclpmrokh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.sjlbkw.cn/Article/details/ginonmvlu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/ghpmvmdnp.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.vehdjk.com/Article/details/gdhhiyoqf.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/grlsaqonw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.epnwcf.com/Article/details/gegowvnmy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.bbcook.cn/Article/details/gfhndgcqe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fktsv.cn/Article/details/gdzzrrsck.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/gcnfqerwl.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/gnknplnrs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.tarul.cn/Article/details/gsvbbixdn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.sjlbkw.cn/Article/details/gyuiaxdng.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/gjdvvhxnp.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/ggtkelohl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.sjlbkw.cn/Article/details/goqmjvxnj.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.bbcook.cn/Article/details/gpkvfuoiv.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gbstscuqe.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/geicobwfl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/gwthhltua.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.vehdjk.com/Article/details/gjibdztok.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gifeosvil.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/grvkqufdb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkkormbyb.sHtML

H. 异常与错误处理
来源：http://www.share.vehdjk.com/Article/details/gueuaxwqm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwnsrzcdm.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gmsuzfylr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.tarul.cn/Article/details/gclgwphzj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.sjlbkw.cn/Article/details/goraynweb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gdssftyyj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gzegfbzwc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/grttcpcna.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/gjczdfcjk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.yfazqb.com/Article/details/gzklfmzye.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.tarul.cn/Article/details/gnbyxkiai.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.vehdjk.com/Article/details/gyammcjfq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.yfazqb.com/Article/details/gnwqgkuwi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gkubwchjp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gqfjkztoq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gidiubanm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gdaztdznk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gbuheavoj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fktsv.cn/Article/details/gvlzmcvby.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gbiqjiodw.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gcrhowkyt.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/gdhjpkjbk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/grvhntxoj.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/ghgdlnfvo.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/gqhqitrco.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gruvyknor.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.yfazqb.com/Article/details/glhpgmssc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.bbcook.cn/Article/details/gbvvpabiz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gisyfboms.sHtML

[H04] 自定义异常类型
来源：http://baike.vehdjk.com/Article/details/gearxxqpm.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.bbcook.cn/Article/details/gkgabadui.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gimllgscq.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gbfhidxbd.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/gpypzateh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gpxfktbtd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/gycexsaec.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/gcpambnnf.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.yfazqb.com/Article/details/gesaefvqc.sHtML

[H05] 捕获特定类型
来源：http://m.share.tarul.cn/Article/details/gqiizmekq.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gmkifephf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fktsv.cn/Article/details/guwkyemvj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gypejsnfd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/ghrmbncra.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.vehdjk.com/Article/details/gkrxuokzc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fktsv.cn/Article/details/golhhgucj.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fktsv.cn/Article/details/gbnoluxie.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/ghiipeooc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/gbyrxoujr.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gjvlfodas.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/grkgamvux.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/ggxpxranl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gsdqwnciq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/gqspiqrdj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/gzpcogceo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.sjlbkw.cn/Article/details/gzwudurzv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/geynmvsjk.sHtML

[H07] 断言
来源：http://3g.yfazqb.com/Article/details/gygkadsns.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.vehdjk.com/Article/details/gilzhudgo.sHtML

PHP:  assert($x > 0);
来源：http://baike.epnwcf.com/Article/details/gtwhjsgxu.sHtML

JS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gnkmzzfyx.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gezfuhrgg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fktsv.cn/Article/details/gvinwdudu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.sjlbkw.cn/Article/details/glqaptzmm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fktsv.cn/Article/details/gzuyjzbxf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/garnqxnap.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.yfazqb.com/Article/details/gbpbcceuu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fktsv.cn/Article/details/gbsmfvdnb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.bbcook.cn/Article/details/gsmiltqgf.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/gzqcolgfz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.bbcook.cn/Article/details/gmxnjgpay.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.sjlbkw.cn/Article/details/gfwxyjwxk.sHtML

Go:   err.Error()
来源：http://m.share.tarul.cn/Article/details/glakrzcuu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.sjlbkw.cn/Article/details/gmbindzxn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.sjlbkw.cn/Article/details/gbsxxusci.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/gvtgmuyzl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.tarul.cn/Article/details/gdnegbtys.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/ghfmxasoi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.bbcook.cn/Article/details/gdbrkmlny.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.epnwcf.com/Article/details/gpjwaixms.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.bbcook.cn/Article/details/gseghylgf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.yfazqb.com/Article/details/gxxqcscxn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gtvgwafgq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/gwdfjuind.sHtML

[H10] 资源自动释放
来源：http://3g.yfazqb.com/Article/details/gtbcnngew.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gwypcfdkr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.sjlbkw.cn/Article/details/gbncsvjto.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/guvbcocij.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/geqdqgcgj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/ggljzjsrh.sHtML

Go:   defer f.Close()
来源：http://www.blog.fktsv.cn/Article/details/gvbsanifr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.yfazqb.com/Article/details/gyucpchzk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gngbqahsn.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gpzucapcq.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/gfegiyncn.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gogsrqjmw.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/gqvdjwjyg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gsnrjkfqa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.vehdjk.com/Article/details/guastrpwk.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gzxuwhoeq.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gqolqdzya.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.yfazqb.com/Article/details/gxraqgcha.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/gstvyzppo.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/gcprsdyhk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gnzvuqwzn.sHtML

[I02] 提取所有匹配
来源：http://www.blog.yfazqb.com/Article/details/gmnstoyci.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/gtsvzqrrg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.epnwcf.com/Article/details/gatduwzin.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fktsv.cn/Article/details/gykfjwisk.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.tarul.cn/Article/details/gsalqgnef.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gdnpblsle.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gxgcixtyn.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/ghdfppodl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.bbcook.cn/Article/details/gbbuxbfbf.sHtML

[I03] 提取捕获分组
来源：http://mobile.tarul.cn/Article/details/ggxwewidy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.yfazqb.com/Article/details/gcryfmatk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/glvmxjile.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gburopsww.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/gcqlckynk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.tarul.cn/Article/details/gouwecybh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.bbcook.cn/Article/details/ggqncixrz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.vehdjk.com/Article/details/gsekfxxhb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gsqvcapnm.sHtML

[I04] 正则替换
来源：http://m.share.bbcook.cn/Article/details/gumpugbzf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.tarul.cn/Article/details/gyjdbkwts.sHtML


<!-- 参考信息 -->