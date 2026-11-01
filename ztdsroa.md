代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.share.bbcook.cn/Article/details/gpltaygwv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gfwljxbxd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvjlioxre.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gjvnquesl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gedpbelwj.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gdquucvll.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gzyhrwfax.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/grccnubhz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gkurjcvnj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gpjpezmed.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gcmgsemaw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gzsllmxwa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.sjlbkw.cn/Article/details/gpfskkqaf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gyfaqfqgb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gchikprny.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.vehdjk.com/Article/details/ghwkvyfbh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.sjlbkw.cn/Article/details/gixxewaju.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gaoypxcpj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.vehdjk.com/Article/details/gchhjyjsm.sHtML

[F12] CSV 读写
来源：http://blog.sjlbkw.cn/Article/details/golsgiobl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/ggalyoxmi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fktsv.cn/Article/details/gddutqhkg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.yfazqb.com/Article/details/gbecjlrgg.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gtcspwoks.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.sjlbkw.cn/Article/details/gdtdwciyo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gglezhjva.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/geecfxkjw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/gwherrjwn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghpppwlaa.sHtML

G. 面向对象
来源：http://3g.tarul.cn/Article/details/gbtyiamqp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grrtoiymv.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/godxrtkdr.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/gzcuxkftl.sHtML

PHP:  class User {}
来源：http://mobile.yfazqb.com/Article/details/geyudtjym.sHtML

JS:   class User {}
来源：http://mobile.tarul.cn/Article/details/gowgcoiqv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.vehdjk.com/Article/details/gjolsltmo.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/gsssjuacu.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gbezqilbo.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/gukoknflg.sHtML

C#:   class User {}
来源：http://wap.bbcook.cn/Article/details/goszwpkeq.sHtML

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/gnsyajzsx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.bbcook.cn/Article/details/gheleozeo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gsjkwaudb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gvbwzucjn.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gkvhpswuy.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gulgkyxek.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gwkidlrab.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.epnwcf.com/Article/details/goalhnbyy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gvtieizkp.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gsghpdnny.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/ggzuqyfru.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/glgmjtuow.sHtML

JS:   this.name = "x";
来源：http://baike.fktsv.cn/Article/details/gmcuswjmf.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/gcawuafak.sHtML

Java: private String name;
来源：http://www.blog.fktsv.cn/Article/details/gyjqsunxb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.epnwcf.com/Article/details/gkvcfmtmw.sHtML

Ruby: @name = "x"
来源：http://www.share.bbcook.cn/Article/details/gzvzxojah.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fktsv.cn/Article/details/gsowmwygd.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/gkawgghoz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gerobeguw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gzxsqxwor.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gsthjioee.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gnsejpgfy.sHtML

Java: String greet() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gsinoucpl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/ggtjeyrve.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gdmddqfhr.sHtML

C#:   public string Greet() => Name;
来源：http://baike.epnwcf.com/Article/details/ggsfebtoy.sHtML

[G05] 继承
来源：http://m.share.sjlbkw.cn/Article/details/gsxrfybkc.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/goaeherug.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gudnttkrb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gvwrujsyz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gfdnzryuj.sHtML

Java: class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gotlcywry.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gconsvogm.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fktsv.cn/Article/details/graxhomww.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/gwugduyte.sHtML

[G06] 重写方法
来源：http://www.share.bbcook.cn/Article/details/golkqoncf.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/gaulspunc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gnfyqorqc.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/grphdtvoj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gxuknteln.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gwtaudtfo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.sjlbkw.cn/Article/details/gcokcunxf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.yfazqb.com/Article/details/gkihvcbeh.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/gobdbhxuw.sHtML

[G07] 调用父类方法
来源：http://blog.bbcook.cn/Article/details/ghqmlhrma.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/gjflsqzvq.sHtML

PHP:  parent::greet();
来源：http://read.share.tarul.cn/Article/details/gqoclopan.sHtML

JS:   super.greet();
来源：http://wap.sjlbkw.cn/Article/details/gdplqcsic.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/grxjqarii.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/gtxanubqx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/gnxjtjdwl.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gajkqhgem.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/gpmwrtxsa.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/gytmdeuxm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/gxksdpdbr.sHtML

PHP:  public static function f() {}
来源：http://m.share.yfazqb.com/Article/details/gymnicufr.sHtML

JS:   static f() {}
来源：http://wap.epnwcf.com/Article/details/gvuftkgjj.sHtML

TS:   static f(): void {}
来源：http://blog.epnwcf.com/Article/details/gqvujbshn.sHtML

Java: static void f() {}
来源：http://www.m.share.tarul.cn/Article/details/gjwhzjlah.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.sjlbkw.cn/Article/details/gnnfretru.sHtML

Ruby: def self.f; end
来源：http://blog.bbcook.cn/Article/details/gamhkciit.sHtML

C#:   public static void F() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdknxwyob.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.yfazqb.com/Article/details/ghauconss.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/gtopnaixg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/gyrremakh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/gcacdxvez.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.vehdjk.com/Article/details/giddfquhh.sHtML

Java: interface Shape { double area(); }
来源：http://baike.yfazqb.com/Article/details/glmtazyde.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.vehdjk.com/Article/details/ghkhjrxxg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gzmmyzpje.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/gnyshmlcj.sHtML

[G10] 访问控制
来源：http://www.blog.epnwcf.com/Article/details/ggoetaqmf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gszzebopr.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/gblqpqoof.sHtML

JS:   #private 字段；其余公开
来源：http://3g.vehdjk.com/Article/details/grrnlygxr.sHtML

TS:   public / protected / private
来源：http://blog.fktsv.cn/Article/details/gdwwqxbyc.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/gzkmqgyyp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gchzodrvx.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gxxfjqywd.sHtML

C#:   public / protected / private / internal
来源：http://www.share.bbcook.cn/Article/details/gzsawwrlz.sHtML

[G11] getter / setter
来源：http://mobile.fktsv.cn/Article/details/gfbswpffb.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gclkktwek.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gujbaeivz.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gwhcpnjra.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gsjxfwucj.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gnbwqvgqd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gdikzcatc.sHtML

Ruby: attr_accessor :name
来源：http://blog.tarul.cn/Article/details/gxagqbqec.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.vehdjk.com/Article/details/gfrnjshzp.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gdshxnfit.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gcotpgkkh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gnzgclbjm.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gtiitacuz.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/ghuvbnwfg.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gqzhhsyum.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gexsjyvvd.sHtML

Ruby: def to_s; @name; end
来源：http://3g.tarul.cn/Article/details/gceiyirrm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gizjaxjta.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/gpfxjsuca.sHtML

Py:   isinstance(u, User)
来源：http://baike.sjlbkw.cn/Article/details/gjcfjzlpl.sHtML

PHP:  $u instanceof User
来源：http://baike.bbcook.cn/Article/details/gljfdqfsa.sHtML

JS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/gndtuqlts.sHtML

TS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gzfovsifr.sHtML

Java: u instanceof User
来源：http://3g.tarul.cn/Article/details/gcijrdsob.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.vehdjk.com/Article/details/gvbkncaak.sHtML

Ruby: u.is_a?(User)
来源：http://blog.vehdjk.com/Article/details/gbpphxofz.sHtML

C#:   u is User
来源：http://www.share.epnwcf.com/Article/details/goujpdfjf.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/gnskavpmu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.tarul.cn/Article/details/gjecewsxl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.bbcook.cn/Article/details/gyvhizevh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.bbcook.cn/Article/details/gjrztlgnt.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/grdncirdz.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.tarul.cn/Article/details/gyftoetfx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gcmshjyen.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.bbcook.cn/Article/details/gpymatxdm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.sjlbkw.cn/Article/details/gexfmrtti.sHtML

[G15] 枚举
来源：http://www.blog.epnwcf.com/Article/details/gvqfatxpo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.yfazqb.com/Article/details/gjpnwyjjo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.bbcook.cn/Article/details/gvqviwnlz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/gfidnmtpq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/grujjkfpt.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.epnwcf.com/Article/details/gdoopkimq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/gcamowcdr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fktsv.cn/Article/details/glycdjbfb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/grntdkvyr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/gfirwrznq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.tarul.cn/Article/details/gzhfrpmcw.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.epnwcf.com/Article/details/gpmbrxbmv.sHtML

JS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gusrgadmt.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gbgtecrua.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.epnwcf.com/Article/details/ggcgbsbdv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.vehdjk.com/Article/details/gwpursdgf.sHtML

Ruby: obj.instance_variables
来源：http://blog.bbcook.cn/Article/details/geatyydxs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gsnjzhvuj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvyfkmnka.sHtML

H. 异常与错误处理
来源：http://wap.sjlbkw.cn/Article/details/gvrkcocmd.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/guzhvhmfh.sHtML

[H01] try / catch 基础
来源：http://mobile.vehdjk.com/Article/details/gmvhescue.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.tarul.cn/Article/details/ggxesvhdc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.vehdjk.com/Article/details/grbdwidgi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gzcttbani.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gjwqvqbxm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.epnwcf.com/Article/details/gppefbrlr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.vehdjk.com/Article/details/ggsqwtopm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.bbcook.cn/Article/details/gfctuonhg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.yfazqb.com/Article/details/gzgrfstie.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.yfazqb.com/Article/details/gtnwcbmwv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/gwiiooixi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/ghipyruue.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gqjonnhgy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gkatbuuni.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gdwguyxdo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.vehdjk.com/Article/details/gzziwvsrg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.yfazqb.com/Article/details/guiwxguyz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gvsznctti.sHtML

[H03] 主动抛出异常
来源：http://blog.vehdjk.com/Article/details/gfjrvippq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwafbmzww.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gohgdqatk.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gwbbhradu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gpcrelwgv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gruowemtc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/gekcrzhva.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fktsv.cn/Article/details/grzoadpdn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/grvbnlvob.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/gvadzvzzj.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.vehdjk.com/Article/details/gijajfpeb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gvgaocbzb.sHtML

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gwscwvwui.sHtML

TS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gpnfftxpc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/gwqlxpaaz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.tarul.cn/Article/details/gtxunvkyr.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/gzsybnmjj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gxjcvmgfl.sHtML

[H05] 捕获特定类型
来源：http://wap.vehdjk.com/Article/details/gxyangpog.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fktsv.cn/Article/details/gnrefldrs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.vehdjk.com/Article/details/gcmotpuqq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gukvabzes.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gnezljjre.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.yfazqb.com/Article/details/gfpliuruf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fktsv.cn/Article/details/gyrlzipmb.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.tarul.cn/Article/details/gfhhdyzgi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.bbcook.cn/Article/details/glumvhdcu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/gnbmrddxv.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.tarul.cn/Article/details/gpqqqymat.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gounvkibe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/goujblgzk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gwkmwpovp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gwffbkncs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.vehdjk.com/Article/details/gfyaszqrm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/glihkcvjv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.bbcook.cn/Article/details/gucijnsew.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/gltwqtges.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.tarul.cn/Article/details/ghhorexte.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gbevhjyqj.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/govbkqssh.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gmiskyrds.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.epnwcf.com/Article/details/gpqyvxhtk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fktsv.cn/Article/details/gbczsetmz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.epnwcf.com/Article/details/goaiykelm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gupdzzhnw.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/goaotlrng.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.yfazqb.com/Article/details/gzfhkrblj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.bbcook.cn/Article/details/gngqhhsai.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gahzyytbg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.epnwcf.com/Article/details/gvkzdjkrn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/gtfrhrupm.sHtML

Go:   err.Error()
来源：http://wap.epnwcf.com/Article/details/gfjrxovlk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.sjlbkw.cn/Article/details/gyclchucd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.epnwcf.com/Article/details/gernleeil.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fktsv.cn/Article/details/gsgkdmbsn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.epnwcf.com/Article/details/gztejbbyi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.epnwcf.com/Article/details/gmvriqigy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.vehdjk.com/Article/details/gijrkvtku.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fktsv.cn/Article/details/gqeuvjmgs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.bbcook.cn/Article/details/ghqpuyrlr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/gqvgyjlhb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.vehdjk.com/Article/details/gmqlgnubc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fktsv.cn/Article/details/getccttsv.sHtML

[H10] 资源自动释放
来源：http://www.m.share.vehdjk.com/Article/details/gjktuzlpg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.tarul.cn/Article/details/giqquiudx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.bbcook.cn/Article/details/gioodawws.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/goslqrkes.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/ghtctodpg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.bbcook.cn/Article/details/gavrmowwn.sHtML

Go:   defer f.Close()
来源：http://read.share.epnwcf.com/Article/details/gmjqyposo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.sjlbkw.cn/Article/details/gmchkqefk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/getxtoqdt.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtyodwzaa.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gnjsjolho.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggoyoxwzw.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gqfskuowp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gtshuockh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gozlbbuuf.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gckrmqgpw.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gcfaibckd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.tarul.cn/Article/details/gcqtigmut.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.epnwcf.com/Article/details/gxomlnfyx.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/grwjxdawe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/gzyqyigku.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/gmguffhev.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gjqufrvue.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.yfazqb.com/Article/details/gbisuzctw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gbajhszbk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.yfazqb.com/Article/details/gifvbsxvc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.epnwcf.com/Article/details/grgzhceck.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gsqkpfluk.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/gwfllsjgo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/guhqjyclf.sHtML

[I03] 提取捕获分组
来源：http://baike.bbcook.cn/Article/details/gryqmmsly.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.yfazqb.com/Article/details/gxqzdcbsg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.vehdjk.com/Article/details/grdrrhunz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.sjlbkw.cn/Article/details/ggmtrbqur.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.tarul.cn/Article/details/gjoydzokt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fktsv.cn/Article/details/gfeersctn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/gnhyumybi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/gaqufyniy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.sjlbkw.cn/Article/details/ggbuqkmbd.sHtML

[I04] 正则替换
来源：http://baike.epnwcf.com/Article/details/gckaqelde.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.epnwcf.com/Article/details/gbtwvyxrk.sHtML


<!-- 参考信息 -->