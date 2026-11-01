代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gxrnmnyjl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gldknlrct.sHtML

Ruby: Dir.children("dir")
来源：http://3g.epnwcf.com/Article/details/gwfnipiyj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/gbjhodqkc.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gtphibagt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gmussnsuh.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gavnsxmyv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/guqyjooac.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gwztjvqqi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/glgxofwpt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/gpthedskq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.tarul.cn/Article/details/ggldivrsf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.vehdjk.com/Article/details/glyzznvli.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.bbcook.cn/Article/details/gargfboga.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gsgvskcxz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/gxkxkeuur.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gitfychws.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gtczocnep.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gsppuexux.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gfbhmawbv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gzxifxsvb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/grqcjdhxn.sHtML

[F11] 复制与移动文件
来源：http://read.share.vehdjk.com/Article/details/gmhmvsemy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gipkeoxfn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fktsv.cn/Article/details/geufefwqd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gcouybqnm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/glkjeysdr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.bbcook.cn/Article/details/gmqamnzsj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.tarul.cn/Article/details/goldrzsbk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gvvjkzuiw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gqjlyfbje.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/gdqnlplfw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/gwurkmnls.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/gzzluyery.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.sjlbkw.cn/Article/details/ghoepxycb.sHtML

TS:   // 同上
来源：http://baike.bbcook.cn/Article/details/gxgbghmxp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.vehdjk.com/Article/details/gagfdylpi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/grplhkjdf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gzjhcsxfz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.yfazqb.com/Article/details/gkupsyzoj.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnyadgpzd.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gdohwxxpu.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkgtciudy.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/gbvqpqzww.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gkauvjojz.sHtML

PHP:  class User {}
来源：http://www.share.vehdjk.com/Article/details/gublmzwoy.sHtML

JS:   class User {}
来源：http://read.share.tarul.cn/Article/details/gncyohpqm.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/govrpixds.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gqhcdword.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/guuuixmhx.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/gzhgjhiso.sHtML

C#:   class User {}
来源：http://wap.tarul.cn/Article/details/gupulwgha.sHtML

[G02] 构造函数
来源：http://baike.vehdjk.com/Article/details/gftqqmrej.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.sjlbkw.cn/Article/details/gepnbyqoj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/gnrmhmxem.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gncnfjcvq.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gfmpbwffp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/goqutejqz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gyitwolhj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/gfqfdwjfy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.vehdjk.com/Article/details/gxduwrhwq.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/gimcforet.sHtML

Py:   self.name = "x"
来源：http://3g.epnwcf.com/Article/details/gtvorzdap.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/garqclezo.sHtML

JS:   this.name = "x";
来源：http://wap.yfazqb.com/Article/details/gyuzjkpcp.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gbhdislwo.sHtML

Java: private String name;
来源：http://wap.vehdjk.com/Article/details/gbwwhpjxz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gaajvlsyc.sHtML

Ruby: @name = "x"
来源：http://wap.vehdjk.com/Article/details/gionkakcz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gbyrfwqkd.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/gqdymhrrk.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/giugzhdud.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gxwjkfzzz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gekmkbzcl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gfsecwyei.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gnjgvtyro.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/glyewluvi.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/ghtlpqsyg.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/giiuejnoh.sHtML

[G05] 继承
来源：http://mobile.fktsv.cn/Article/details/gdqaswoda.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/grmyoecor.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gbbtgsval.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/ggnfrgyny.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gjbtcrgdd.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gjezujdmr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gfojlsazj.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gaftfvgvc.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gzkfdxbsd.sHtML

[G06] 重写方法
来源：http://blog.tarul.cn/Article/details/gjxkzfuvj.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.bbcook.cn/Article/details/ghoxrlceh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gpzpexqop.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gkvepdufs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gimwnkkie.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/grdgmjybl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gardpslpj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/geggayfwc.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fktsv.cn/Article/details/gwvtnteol.sHtML

[G07] 调用父类方法
来源：http://blog.vehdjk.com/Article/details/gzwinuzes.sHtML

Py:   super().greet()
来源：http://www.share.bbcook.cn/Article/details/gcejnvlvj.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gxramvzmk.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gukfigdtw.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gksnkrrpb.sHtML

Java: super.greet();
来源：http://www.share.bbcook.cn/Article/details/gwxmchpgf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.vehdjk.com/Article/details/glosvmsdx.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gqyvxfuvo.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/gdisaomeh.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtwpnhor.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/gbzsacigc.sHtML

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/gpjeehevm.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/gixpmwsiw.sHtML

TS:   static f(): void {}
来源：http://mobile.epnwcf.com/Article/details/gbqhrbcli.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/gipbwrowd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.tarul.cn/Article/details/gtwrxedho.sHtML

Ruby: def self.f; end
来源：http://www.m.share.vehdjk.com/Article/details/gchfppnnr.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/gclqdevro.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/gukqokmqg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fktsv.cn/Article/details/gvdynxdub.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gttokfqvq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.sjlbkw.cn/Article/details/gibxdogea.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.epnwcf.com/Article/details/gishztarn.sHtML

Java: interface Shape { double area(); }
来源：http://3g.bbcook.cn/Article/details/gjitwiddd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fktsv.cn/Article/details/gvtgqxest.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.sjlbkw.cn/Article/details/gtyqbvfnn.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.vehdjk.com/Article/details/gtksxygnn.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/gtncybubj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/gfzjcvyjm.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gaobfrbaf.sHtML

JS:   #private 字段；其余公开
来源：http://wap.yfazqb.com/Article/details/gdrwohlcv.sHtML

TS:   public / protected / private
来源：http://wap.yfazqb.com/Article/details/guhtfoogo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.sjlbkw.cn/Article/details/gslhfjfkc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/grolrcsob.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gvpbqhdcv.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/gnazzdnoo.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/grhpmzhfw.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.sjlbkw.cn/Article/details/gwfcfsqqv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gtaqblqkg.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gouzigttf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gaskcroyo.sHtML

Java: public String getName() { return name; }
来源：http://wap.fktsv.cn/Article/details/gdrylwghb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gbtliwbcu.sHtML

Ruby: attr_accessor :name
来源：http://blog.fktsv.cn/Article/details/gtfwvjguj.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.tarul.cn/Article/details/gyjgmerfq.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/guuoiadup.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gkfmbxnoz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gpxlnqzhw.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gmwryytfn.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gbzvqkzfy.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.epnwcf.com/Article/details/gojualhvb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gasvicoah.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fktsv.cn/Article/details/gwavsenya.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gzoxwbdnd.sHtML

[G13] 判断对象类型
来源：http://www.blog.epnwcf.com/Article/details/gzxohrpdi.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/guhiiakai.sHtML

PHP:  $u instanceof User
来源：http://3g.epnwcf.com/Article/details/gxzxfaoey.sHtML

JS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/gggytwrcr.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/ggiskgrig.sHtML

Java: u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gwppbcqjm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.yfazqb.com/Article/details/gebtbaikt.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/guxiyjgby.sHtML

C#:   u is User
来源：http://mobile.yfazqb.com/Article/details/galmrkipd.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/goaqdoyzk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/grnimklsy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.bbcook.cn/Article/details/gjtfqolfj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/ghxtueyzp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.yfazqb.com/Article/details/gfsnpgxrb.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/gluhbpacv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.tarul.cn/Article/details/gcijscikt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.sjlbkw.cn/Article/details/gdwacxkrj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fktsv.cn/Article/details/gpzdhrnld.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/ghjcgmzrr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.bbcook.cn/Article/details/ggefqebsq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gyovldlsr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gndagsxuh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gbgtbopbs.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gpohvfwzt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.vehdjk.com/Article/details/gcavobnlt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gthdtceqy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gscqgbray.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.tarul.cn/Article/details/gxheoinui.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.vehdjk.com/Article/details/gmreqnnlr.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/gvmaywsbc.sHtML

JS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gfktqvmtm.sHtML

TS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gwzonlzir.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/gsemivjpd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.sjlbkw.cn/Article/details/ghtwfubob.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/gtaszlztz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gizvnqklr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gpkopayqc.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/ghwiuefhe.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gosrptlde.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gpryzagcp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.yfazqb.com/Article/details/gkprgecgg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.epnwcf.com/Article/details/granpvguo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gwjjpmbiv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/ggzjbusxz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.tarul.cn/Article/details/gsyvgbyyo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fktsv.cn/Article/details/ggyvcjdux.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.sjlbkw.cn/Article/details/gsztnkgmg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fktsv.cn/Article/details/ggegivlgg.sHtML

[H02] finally / ensure 收尾
来源：http://3g.epnwcf.com/Article/details/gyvwunaed.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fktsv.cn/Article/details/gekipfbvm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/goeuxbens.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gpzwixwmb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gdvqdqcwc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/ghiigroxn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.sjlbkw.cn/Article/details/gzlumptxk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gbskixysz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gwbkqwtdn.sHtML

[H03] 主动抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gqsrdayoy.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.vehdjk.com/Article/details/gbrbnoplb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gxiztrvpq.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gbmyfsrpu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gybtflich.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gycyrduqr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.vehdjk.com/Article/details/gpulmhqeo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/gftggpwcu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gekogwiks.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gotjwrfsg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gmeegotkk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gvkgjvpex.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gshbbxeix.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gucupwube.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/gtxddjqpt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.bbcook.cn/Article/details/gergcdzwo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.bbcook.cn/Article/details/gdanpjyms.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/goiyhqxxt.sHtML

[H05] 捕获特定类型
来源：http://wap.fktsv.cn/Article/details/grpxalgtx.sHtML

Py:   except ValueError as e:
来源：http://baike.tarul.cn/Article/details/grbqskaab.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.yfazqb.com/Article/details/gjmjzuumd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/ghoeicztb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gtsepbece.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.tarul.cn/Article/details/gmsmnxxsi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/gdbuspibj.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/grgzepubc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/gbjewbfzl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.yfazqb.com/Article/details/gkjcdxmpy.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gjmoqsqdr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gtjrovzwx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsmtvsxc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/gewpppdmu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.epnwcf.com/Article/details/geftrkcar.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.sjlbkw.cn/Article/details/gxpwrwwok.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/giquysatp.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/gxtuvskch.sHtML

[H07] 断言
来源：http://www.share.sjlbkw.cn/Article/details/gzowuhtna.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.vehdjk.com/Article/details/gqbvaemtp.sHtML

PHP:  assert($x > 0);
来源：http://wap.tarul.cn/Article/details/gjvmckwgb.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gbqynkhsf.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gtljdkcdv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.vehdjk.com/Article/details/gefcfybvq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.sjlbkw.cn/Article/details/gsjzleslw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.vehdjk.com/Article/details/gjbzqtdxl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/govpdkgds.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gvagcdmpk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.sjlbkw.cn/Article/details/grnxhgedf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.bbcook.cn/Article/details/ghffppaxe.sHtML

JS:   e.message;  e.stack
来源：http://baike.tarul.cn/Article/details/ghlhklxnk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.bbcook.cn/Article/details/gtnftipxk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.tarul.cn/Article/details/ghywfglrt.sHtML

Go:   err.Error()
来源：http://3g.vehdjk.com/Article/details/gnsyibhya.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.tarul.cn/Article/details/gmwzgpeim.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.tarul.cn/Article/details/gifynnfpd.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/gmrwcpebx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/gdyfazteg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/grmuhdmce.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/gfzmggmyh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.vehdjk.com/Article/details/gvtaqwkog.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gmfbijjdj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.epnwcf.com/Article/details/gopwgauas.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.epnwcf.com/Article/details/giestizau.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.sjlbkw.cn/Article/details/gkrwvaukv.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gnofivway.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.yfazqb.com/Article/details/ggbqirjbz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.bbcook.cn/Article/details/girkanzwm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gjmcfmrsl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gnzpcgjec.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/glbsdhwuh.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/glbcxxhqv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/ghyuovohz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/grzfyjyjr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmqayjndr.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/gnilwxpoc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkntpizmo.sHtML

[I01] 判断是否匹配
来源：http://baike.vehdjk.com/Article/details/gtwgnrrno.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/giyhyngkb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/giivzzesx.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/gsbgvrwzl.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gcrysjzej.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.vehdjk.com/Article/details/gxrquruyw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.vehdjk.com/Article/details/gbkwnkadb.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gkctexbil.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gihudbbsl.sHtML

[I02] 提取所有匹配
来源：http://read.share.yfazqb.com/Article/details/gsaxdnrcw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.yfazqb.com/Article/details/gcpqzmcye.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.epnwcf.com/Article/details/gpeaimics.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/gkkrzbhav.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/goqizezyz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/gddwjbogb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fktsv.cn/Article/details/gfhxxgunp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gugfsjyhs.sHtML


<!-- 参考信息 -->