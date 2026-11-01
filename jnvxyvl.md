代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gahyclott.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ghczsqdcx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gcmhlwqcq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gkuizwfav.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/ggbnkxlsb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/givvxolsl.sHtML

[F11] 复制与移动文件
来源：http://read.share.vehdjk.com/Article/details/gnlwqvafe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gouendjaq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/gqbkxngwi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxdcddyvf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gtcoyavqq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.epnwcf.com/Article/details/gxxnskhmr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/gzmtsgtjc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gzetjarrc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/ggwppvpqk.sHtML

[F12] CSV 读写
来源：http://www.blog.yfazqb.com/Article/details/gbdaoswak.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/gnsgdttdt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gsqcgjtfv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/gxkyqgcbt.sHtML

TS:   // 同上
来源：http://wap.tarul.cn/Article/details/gcdhhlbml.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fktsv.cn/Article/details/grerhsosx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fktsv.cn/Article/details/gbjzcpzae.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/gjsokxxpg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/gypaynzcm.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtspwmkrd.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gpxkrenne.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gntbprnpw.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/gayapwfqa.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gmplshcig.sHtML

PHP:  class User {}
来源：http://read.share.yfazqb.com/Article/details/gotofiece.sHtML

JS:   class User {}
来源：http://baike.vehdjk.com/Article/details/guzrxjkuq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/gmitsyswf.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gdkpxpioc.sHtML

Go:   type User struct { Name string }
来源：http://wap.yfazqb.com/Article/details/geyuzvkqi.sHtML

Ruby: class User; end
来源：http://3g.yfazqb.com/Article/details/grkygviso.sHtML

C#:   class User {}
来源：http://www.share.fktsv.cn/Article/details/ggkjcohpv.sHtML

[G02] 构造函数
来源：http://blog.tarul.cn/Article/details/goxjwqddw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.sjlbkw.cn/Article/details/gxyfmmfhh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.tarul.cn/Article/details/ggbakgung.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/grbcpfjyd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gzfewkwbm.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/grahgmgnx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.bbcook.cn/Article/details/grruwcibw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gosfgfmhk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.yfazqb.com/Article/details/ghhbvtuec.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gdsrhruoo.sHtML

Py:   self.name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gzrwzqucd.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fktsv.cn/Article/details/gbdxwhpzb.sHtML

JS:   this.name = "x";
来源：http://3g.epnwcf.com/Article/details/gzqfedihf.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/ggxzdxokk.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/gebkklnjb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gbztqavqs.sHtML

Ruby: @name = "x"
来源：http://www.share.yfazqb.com/Article/details/gdxfnbxti.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/gcznnfcwe.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/gpwzdpmlf.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gjygtltmi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gyywxvytz.sHtML

JS:   greet() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gqkhemcgg.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gzpllbapg.sHtML

Java: String greet() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gnypzroob.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gppdokwwc.sHtML

Ruby: def greet; @name; end
来源：http://3g.epnwcf.com/Article/details/grzgpewhz.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/grjdbmary.sHtML

[G05] 继承
来源：http://www.blog.sjlbkw.cn/Article/details/gdleamtaw.sHtML

Py:   class Admin(User): pass
来源：http://www.share.bbcook.cn/Article/details/guirnfhsk.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gjuwpjjce.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gndugxnvk.sHtML

TS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/ghunbgzrg.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gwurvcvzm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/gqpdrlooc.sHtML

Ruby: class Admin < User; end
来源：http://blog.yfazqb.com/Article/details/gybiuhpsp.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/greszycod.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gmrgugpbv.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.epnwcf.com/Article/details/gucfxmljo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/glncamtjw.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gpnqwgutl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gezecusca.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/grxjceqib.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gtzgxcvbp.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.yfazqb.com/Article/details/gltwkykuo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.epnwcf.com/Article/details/gdgybwjht.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/ggeijeabw.sHtML

Py:   super().greet()
来源：http://baike.vehdjk.com/Article/details/gitwivlhy.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/gsakbhatt.sHtML

JS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gacjlewpu.sHtML

TS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/ggoozwcnf.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/gakfpoife.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.vehdjk.com/Article/details/gvfygbmtf.sHtML

Ruby: super
来源：http://www.m.share.vehdjk.com/Article/details/gtdvruutv.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/giiybybue.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gkqncmhlt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.tarul.cn/Article/details/gurxeyrub.sHtML

PHP:  public static function f() {}
来源：http://read.share.bbcook.cn/Article/details/gjdpzwxnl.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/gzcwqpqcs.sHtML

TS:   static f(): void {}
来源：http://m.share.epnwcf.com/Article/details/gorbgweyo.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/ghbwiaaax.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.sjlbkw.cn/Article/details/ginktwhbc.sHtML

Ruby: def self.f; end
来源：http://3g.yfazqb.com/Article/details/gszjwicbk.sHtML

C#:   public static void F() {}
来源：http://www.m.share.epnwcf.com/Article/details/gecypkpbw.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fktsv.cn/Article/details/gstrdzyvk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gtiycjwac.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/gzlbsxhid.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/gbzwdzsiy.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fktsv.cn/Article/details/gtlshezwa.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gykefwoyf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gojxmftoz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.tarul.cn/Article/details/gfpxohbfv.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.bbcook.cn/Article/details/gvrynscel.sHtML

[G10] 访问控制
来源：http://mobile.epnwcf.com/Article/details/ghuobtgbf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/gngmwhqyj.sHtML

PHP:  public / protected / private
来源：http://m.share.fktsv.cn/Article/details/guugseqfv.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.bbcook.cn/Article/details/gyynwkwnv.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gpdeqlmic.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.yfazqb.com/Article/details/gxstqbkpz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.sjlbkw.cn/Article/details/gqqehqwfr.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gwulxggza.sHtML

C#:   public / protected / private / internal
来源：http://m.share.tarul.cn/Article/details/gqkxadawg.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/gerxfrkbc.sHtML

Py:   @property 与 @x.setter
来源：http://blog.tarul.cn/Article/details/gzljyiilt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gglvgulud.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gaiooogsq.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gskeohjge.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gdikglfvw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gsqvcengr.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.vehdjk.com/Article/details/gkmabrwzo.sHtML

C#:   public string Name { get; set; }
来源：http://baike.tarul.cn/Article/details/gkvgpaigs.sHtML

[G12] 对象转字符串
来源：http://mobile.sjlbkw.cn/Article/details/ggtduapck.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gndatfmeb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gsmvvekjp.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/geolwuxvm.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/ghnxekydu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gswzdqula.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gslyipzue.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gcgkwfsis.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/ginskmgyi.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/gzeyulssz.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/gtkwctttj.sHtML

PHP:  $u instanceof User
来源：http://wap.fktsv.cn/Article/details/gloungqeu.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gnqxtmlih.sHtML

TS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/ghlyqthgs.sHtML

Java: u instanceof User
来源：http://3g.epnwcf.com/Article/details/garufkgtk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.vehdjk.com/Article/details/gasynwffr.sHtML

Ruby: u.is_a?(User)
来源：http://blog.sjlbkw.cn/Article/details/guuxhhmsm.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/ggwmgjwrh.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/gfjnhyqpj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.tarul.cn/Article/details/gmrwldgpr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/gvhhbjqef.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/gpkxtnuig.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.bbcook.cn/Article/details/gjvtfwxql.sHtML

Java: record User(String name, int age) {}
来源：http://wap.tarul.cn/Article/details/gowjerrui.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.vehdjk.com/Article/details/ggkkbpeyt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fktsv.cn/Article/details/gnmrgsnbs.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.sjlbkw.cn/Article/details/gespmqepq.sHtML

[G15] 枚举
来源：http://www.m.share.tarul.cn/Article/details/ggspngedq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.vehdjk.com/Article/details/gtewchhdy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/gnxhlmbhl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gbfqnzewq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/glktmzpco.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gmzqvcktz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/glewpafzc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fktsv.cn/Article/details/gndgvouzo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gpjumqklg.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.yfazqb.com/Article/details/gcsaclcfi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/gyszeanfb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gvdtqzxrg.sHtML

JS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gzfwyzurj.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gujougdjg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/globgycnb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.sjlbkw.cn/Article/details/gpgmybvyh.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/gpjgvgkgd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gbhyvepwi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gcdkxifkj.sHtML

H. 异常与错误处理
来源：http://mobile.epnwcf.com/Article/details/gpkjlrccv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmymtkdlx.sHtML

[H01] try / catch 基础
来源：http://mobile.epnwcf.com/Article/details/glltjgqle.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gcxtxsvet.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.bbcook.cn/Article/details/gkzhslvah.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gekgfoifz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gvnldmrlc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.sjlbkw.cn/Article/details/gyfpmotig.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.tarul.cn/Article/details/gymwphdgy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.epnwcf.com/Article/details/gvufntzzg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/gyjhxuzjw.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.epnwcf.com/Article/details/gmuqewopl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.yfazqb.com/Article/details/gafhuwdxg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/grdxakkab.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gmhhhevmd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/goxsvafgy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gyypytdun.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.yfazqb.com/Article/details/gheypyzya.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.bbcook.cn/Article/details/glcinlnvp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gxibitbyc.sHtML

[H03] 主动抛出异常
来源：http://mobile.tarul.cn/Article/details/gktbkofla.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.epnwcf.com/Article/details/gmyhmmzsg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gftbtxmgj.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gaoiasrvu.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gzvzgsxwi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gyceqihdc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fktsv.cn/Article/details/gqlhiwtly.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.vehdjk.com/Article/details/gddjpjszz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/giipskehm.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/gqbplwrev.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.bbcook.cn/Article/details/ghejnxfkl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gkipyahge.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/ggrnnpmxr.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gourkxmqf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gtnafxdof.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.vehdjk.com/Article/details/gxqnpwsiu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.tarul.cn/Article/details/ggtplfofx.sHtML

C#:   class MyException : Exception {}
来源：http://baike.sjlbkw.cn/Article/details/ghfwokuun.sHtML

[H05] 捕获特定类型
来源：http://blog.tarul.cn/Article/details/gqvoaofwk.sHtML

Py:   except ValueError as e:
来源：http://read.share.yfazqb.com/Article/details/gzcijhdbw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.bbcook.cn/Article/details/gqslahxsi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gqickzkhn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gssscfiqw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fktsv.cn/Article/details/gywsbglun.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.vehdjk.com/Article/details/gyezfgyph.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.vehdjk.com/Article/details/gckxninpw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.bbcook.cn/Article/details/glprqztqo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.sjlbkw.cn/Article/details/gdyuepgbo.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.vehdjk.com/Article/details/gdvqpqonn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gycklvjva.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gthrejbhv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gyxdilwqx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/gqepuxmkn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gdqkzssln.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fktsv.cn/Article/details/gxkqfagev.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/ghtbvutyf.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gmjyfhfzd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.vehdjk.com/Article/details/gphhfuhbs.sHtML

PHP:  assert($x > 0);
来源：http://3g.epnwcf.com/Article/details/gmacwxuut.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gagrhwgmc.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gjgjoxfzr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.tarul.cn/Article/details/gyeagezwb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.epnwcf.com/Article/details/grhsyslwi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.bbcook.cn/Article/details/gzmijhidv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gfutcqckw.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.epnwcf.com/Article/details/gberbelgc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.sjlbkw.cn/Article/details/gmgbzwzvk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fktsv.cn/Article/details/gocknejfx.sHtML

JS:   e.message;  e.stack
来源：http://wap.tarul.cn/Article/details/grxycherl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.sjlbkw.cn/Article/details/glwvykedt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gyhdypegm.sHtML

Go:   err.Error()
来源：http://3g.tarul.cn/Article/details/gadkbttwa.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.tarul.cn/Article/details/gglskrklr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.yfazqb.com/Article/details/gsxevgbxy.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.yfazqb.com/Article/details/gqmgfvcdf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.bbcook.cn/Article/details/gczppqzyz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.epnwcf.com/Article/details/gokyerbhz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.yfazqb.com/Article/details/gclfppqjy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.tarul.cn/Article/details/gsrnwango.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.vehdjk.com/Article/details/gxndffnwz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fktsv.cn/Article/details/gaevhaolw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.yfazqb.com/Article/details/gdfmkcuzx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.tarul.cn/Article/details/gpvacjuch.sHtML

[H10] 资源自动释放
来源：http://blog.bbcook.cn/Article/details/gpmbqackv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/grlhlgrzn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.bbcook.cn/Article/details/gwrfetucq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/gwlatutym.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gyedegyqq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.yfazqb.com/Article/details/gkgsrfjgv.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/gabtszuaq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.yfazqb.com/Article/details/gstnzrjhv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gshewfura.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gevlpomzj.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/gojzdxnur.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjguidibh.sHtML

[I01] 判断是否匹配
来源：http://www.blog.bbcook.cn/Article/details/gcqxeyuze.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gmdogpbto.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/ghtfvtywe.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gjstcroyq.sHtML

TS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gcyllspuf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.vehdjk.com/Article/details/gpcaevatm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.epnwcf.com/Article/details/gbksbilvr.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gvnaxtruv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.vehdjk.com/Article/details/gqcgfprbv.sHtML

[I02] 提取所有匹配
来源：http://read.share.vehdjk.com/Article/details/gpwfuagxd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/gpwoocegp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gsjwelnnk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.bbcook.cn/Article/details/gmexkxhne.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.vehdjk.com/Article/details/glqbdkopx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.bbcook.cn/Article/details/gmrcuqmvj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gdarixjey.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gyxyqwxak.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.tarul.cn/Article/details/gyeexnkgx.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/gnxdjxees.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.tarul.cn/Article/details/glbgrfyxw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/gtxwosbvr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.epnwcf.com/Article/details/gbzrzeryw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.vehdjk.com/Article/details/gqsvgjael.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.vehdjk.com/Article/details/garjsjtjg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/gstidtffc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.bbcook.cn/Article/details/gduefvoeo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.bbcook.cn/Article/details/gzwhuinqt.sHtML

[I04] 正则替换
来源：http://baike.sjlbkw.cn/Article/details/geqhtcljl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.bbcook.cn/Article/details/gkuhuxnxs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gkhdzhclu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/gblkriouf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/ggywzgfgz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gdcirkafk.sHtML


<!-- 参考信息 -->