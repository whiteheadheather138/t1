代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gndkkmvec.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gfxdrokik.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gpeazcaxv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.tarul.cn/Article/details/gjbvbielf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gyokxkbwk.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gpltvvout.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gxpltavun.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gixidwihv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gudbxobzj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gqagycumj.sHtML

[F11] 复制与移动文件
来源：http://read.share.vehdjk.com/Article/details/gtqmmugdn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gyfacizmp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/grgdsrsgv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gkmrazmcr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/guhehilne.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.epnwcf.com/Article/details/gouwvyagh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/gxuxhuixp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gcmxavjoi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/giiwjytim.sHtML

[F12] CSV 读写
来源：http://wap.epnwcf.com/Article/details/gycgbbyfe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fktsv.cn/Article/details/gxepyktsa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fktsv.cn/Article/details/gjnpbhvou.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.tarul.cn/Article/details/gxuokczym.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/guepujfkk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gflmnzexm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/gtaylcefs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/gigvxppkh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.epnwcf.com/Article/details/gkresfvbm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/geauksdel.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gnqqrpwkg.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjsesfrxv.sHtML

[G01] 定义类
来源：http://mobile.yfazqb.com/Article/details/gerpgcyxj.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/gvbvkizbw.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/godncltgv.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gjqxryqui.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/glubshlzf.sHtML

Java: class User {}
来源：http://blog.tarul.cn/Article/details/gggjcybfl.sHtML

Go:   type User struct { Name string }
来源：http://www.share.bbcook.cn/Article/details/gtwvcvghy.sHtML

Ruby: class User; end
来源：http://mobile.tarul.cn/Article/details/gicdwtjeg.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/gtggoidea.sHtML

[G02] 构造函数
来源：http://wap.fktsv.cn/Article/details/ggvixsuwo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.sjlbkw.cn/Article/details/gviioymst.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gkmwnbftx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gnufficxd.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.tarul.cn/Article/details/glvseeekf.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gpulgpkjq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.bbcook.cn/Article/details/gjdxawqcm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gcrdzwevv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gyjvzkdtt.sHtML

[G03] 实例属性
来源：http://3g.vehdjk.com/Article/details/gzvwmliwx.sHtML

Py:   self.name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gvsxzjqrj.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/goizxwnoe.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/gpotfcaea.sHtML

TS:   name: string = "x";
来源：http://3g.sjlbkw.cn/Article/details/ghoqacnbe.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/gphfofhkd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gbhltzyvt.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/giearfbdq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/gkmdwiwck.sHtML

[G04] 定义方法
来源：http://read.share.epnwcf.com/Article/details/gqohfxsrf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.vehdjk.com/Article/details/gsgdpngxv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/grnirysgp.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gpkfldrgr.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gwgcepixf.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/glgbajvqf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/graprywrs.sHtML

Ruby: def greet; @name; end
来源：http://www.share.bbcook.cn/Article/details/gtmpvfppn.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gymiktpul.sHtML

[G05] 继承
来源：http://m.share.yfazqb.com/Article/details/grkqgxnih.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gftaqboak.sHtML

PHP:  class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gubxbhzdf.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gwhfwxpek.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gcfhadzis.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/galtoqdnw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fktsv.cn/Article/details/grmzdrqsm.sHtML

Ruby: class Admin < User; end
来源：http://blog.fktsv.cn/Article/details/gczbzteen.sHtML

C#:   class Admin : User {}
来源：http://wap.fktsv.cn/Article/details/gifitobfu.sHtML

[G06] 重写方法
来源：http://wap.epnwcf.com/Article/details/gubmjffpq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/gggexihtq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gkstevrzl.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/geupbprmu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gmldzvmwb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gkyfkhvmk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.epnwcf.com/Article/details/gzniiycmq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.sjlbkw.cn/Article/details/gzgbaodcy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/gryhuwklk.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/ggnnzmsab.sHtML

Py:   super().greet()
来源：http://wap.tarul.cn/Article/details/gmtmunmcd.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/gezuupxlp.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gdinsuqaj.sHtML

TS:   super.greet();
来源：http://blog.fktsv.cn/Article/details/guhvmnlkv.sHtML

Java: super.greet();
来源：http://blog.vehdjk.com/Article/details/gmylvskwn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gquybkhyd.sHtML

Ruby: super
来源：http://read.share.vehdjk.com/Article/details/gvhojxwlr.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gbxykkzeh.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gfrcpwrya.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.vehdjk.com/Article/details/gzhphvlym.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/gduapnprk.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/gvwbmrzdh.sHtML

TS:   static f(): void {}
来源：http://read.share.epnwcf.com/Article/details/giothzuue.sHtML

Java: static void f() {}
来源：http://www.share.tarul.cn/Article/details/gtfdzltdd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fktsv.cn/Article/details/gtzcvveks.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/gjdzvafrc.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/gcmixaljm.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/gkheelnck.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/gwetggrwk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.yfazqb.com/Article/details/gwucoyhia.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.sjlbkw.cn/Article/details/gavzyycnp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gtmdlwbhz.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gotlyrbif.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gkjypqjdf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.epnwcf.com/Article/details/gkhaztsor.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.bbcook.cn/Article/details/guhyfrsxy.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/grtmppwkt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.epnwcf.com/Article/details/gbbwhzcmg.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gqfqhwppc.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.tarul.cn/Article/details/gdoylndkg.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gpzvrjlcs.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.yfazqb.com/Article/details/gjlfrrmmt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gdqeycutu.sHtML

Ruby: public / protected / private
来源：http://mobile.tarul.cn/Article/details/gzfvnmnkd.sHtML

C#:   public / protected / private / internal
来源：http://m.share.bbcook.cn/Article/details/gfocaxark.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/glzzowofg.sHtML

Py:   @property 与 @x.setter
来源：http://wap.sjlbkw.cn/Article/details/gfbcdmbqq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/grggzmgpc.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/godvytann.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gsjtjwtcz.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gzwzdiseu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gafktdvki.sHtML

Ruby: attr_accessor :name
来源：http://read.share.epnwcf.com/Article/details/giwpdszib.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/gsnlguhyy.sHtML

[G12] 对象转字符串
来源：http://mobile.fktsv.cn/Article/details/guyxvawqj.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gbmkoqdel.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gewpeeqnt.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gsywivnmw.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gjptgxslt.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.epnwcf.com/Article/details/gcjyynfva.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gnkimvmfn.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fktsv.cn/Article/details/gxplcegxw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/ghvdmqiwz.sHtML

[G13] 判断对象类型
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlohoosd.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/gkizikqpw.sHtML

PHP:  $u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/geweiozkk.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/guxvedxta.sHtML

TS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/ghcueqovy.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/gxpqgkyvf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/gymulqwpm.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/gexwjbcem.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/guvwttskw.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/glwboycaj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fktsv.cn/Article/details/gwdcbwwgy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/gqflgdnhp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fktsv.cn/Article/details/gptsghyyj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fktsv.cn/Article/details/gmhevuvba.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fktsv.cn/Article/details/ggvmmlfau.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gfajhlanz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/gpukuoama.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.tarul.cn/Article/details/gpclddokp.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gejdcuvsp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gshtnizep.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.vehdjk.com/Article/details/gvyfhpbxo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.vehdjk.com/Article/details/gzsxuseis.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gfohojdwn.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.yfazqb.com/Article/details/gcebckpvw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/ghnjssrdm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/ghkczevaj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gsuxesntg.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.yfazqb.com/Article/details/gnixwmobs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/ghtmnriff.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fktsv.cn/Article/details/gadlekqeb.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gdyoxzhjf.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gjhhtsaio.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/ggmbslrtm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gozfxawle.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/gctgvowww.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gpmyqvudx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/goccbcgki.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gjmmvirjp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnkjvzgsm.sHtML

[H01] try / catch 基础
来源：http://baike.vehdjk.com/Article/details/gacsovpqr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.tarul.cn/Article/details/gqmaxlzud.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gzxlsrgzf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gbxhyhcra.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gxdzfmumx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/ganmjmaxs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/gecfrkkxw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fktsv.cn/Article/details/gatxutgaf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gfkacldon.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.bbcook.cn/Article/details/gmxuxzelg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gyomuebbc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gfcphypow.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gyboiwlwu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gxsnkizxy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gyegjufpb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.bbcook.cn/Article/details/gzdbsrlhb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.bbcook.cn/Article/details/gvtlbdlct.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.bbcook.cn/Article/details/guxledpdy.sHtML

[H03] 主动抛出异常
来源：http://www.share.epnwcf.com/Article/details/gppezpypd.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.yfazqb.com/Article/details/gbkwdfamh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gxgkexahh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gecrcuhvh.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gcomqwcuh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gwlqwhhvb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/gxipqysdf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fktsv.cn/Article/details/gxdbcvwzp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gtavjuwzv.sHtML

[H04] 自定义异常类型
来源：http://read.share.vehdjk.com/Article/details/gzyyeuxkd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.bbcook.cn/Article/details/gkwjrrrow.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gftfbmzpj.sHtML

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gzkneogpq.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gsxbphrdc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gdimubzpy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/ggbgyywhj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.yfazqb.com/Article/details/gilgcxurr.sHtML

C#:   class MyException : Exception {}
来源：http://baike.tarul.cn/Article/details/guovfztkp.sHtML

[H05] 捕获特定类型
来源：http://mobile.sjlbkw.cn/Article/details/gvksmzhae.sHtML

Py:   except ValueError as e:
来源：http://wap.yfazqb.com/Article/details/gryogmzrg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.tarul.cn/Article/details/gddfsyatx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gpokwazmb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gkfazajka.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gzlynhdob.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.tarul.cn/Article/details/gationgnu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.yfazqb.com/Article/details/gxmxqkjvp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.tarul.cn/Article/details/gauyyouvy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/gdkrkobze.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.epnwcf.com/Article/details/gmosaqdxf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gqqjkrerd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gxakagduv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gedrekicp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.epnwcf.com/Article/details/gghdtgxwz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.yfazqb.com/Article/details/gzaolbqhc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/gevguurpr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gfncqxqmi.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gcjugcmsx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.bbcook.cn/Article/details/gjagkpwsq.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gdalnoyts.sHtML

JS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gesilylsm.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/glukqlzar.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/gnzrraurj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/gysdbhzce.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/gpcdsgtbz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gvlevllva.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.vehdjk.com/Article/details/gnvmfhrqm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/gbzdcmdwc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.tarul.cn/Article/details/gwqdqekci.sHtML

JS:   e.message;  e.stack
来源：http://wap.sjlbkw.cn/Article/details/gpsmqljzd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.sjlbkw.cn/Article/details/gnpcbycxt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gksamhzrj.sHtML

Go:   err.Error()
来源：http://mobile.yfazqb.com/Article/details/gejyxsluz.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/gphjrydnp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fktsv.cn/Article/details/gsjzqnwwn.sHtML

[H09] 带错误码的异常
来源：http://www.blog.bbcook.cn/Article/details/gvagnhybx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/gnrhetluf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.sjlbkw.cn/Article/details/gykzjlpso.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fktsv.cn/Article/details/gdihuhovc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gdvsfykyb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.vehdjk.com/Article/details/grwrcrmpb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gunbonxcs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.epnwcf.com/Article/details/gieqivuoq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.yfazqb.com/Article/details/gfojkhmjn.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/gvwbnsylh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.epnwcf.com/Article/details/gdcdnqmun.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.epnwcf.com/Article/details/gmriuzbct.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gvlfkkcwd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gibflyejv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.bbcook.cn/Article/details/gztfwoits.sHtML

Go:   defer f.Close()
来源：http://www.m.share.yfazqb.com/Article/details/gnlsjxphk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fktsv.cn/Article/details/guzqwulju.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/gqqfxjqqw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtyqdbbuz.sHtML

I. 正则表达式
来源：http://mobile.bbcook.cn/Article/details/gvolcraov.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/goputfcvu.sHtML

[I01] 判断是否匹配
来源：http://mobile.bbcook.cn/Article/details/gytpcsbqt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/girciczpb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gkladtyva.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gnyjhpxdt.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gkomqlakg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gzhndncpf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fktsv.cn/Article/details/gbstdgnmd.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/grjzhfljw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gppjpxbmf.sHtML

[I02] 提取所有匹配
来源：http://blog.fktsv.cn/Article/details/gujkgtekz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gwhswdwns.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/gsnurhxry.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gpeibyyya.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbmqespu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gufkqntii.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.epnwcf.com/Article/details/gkidyzbrr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gjvgeylac.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gvrvbkpgh.sHtML

[I03] 提取捕获分组
来源：http://mobile.tarul.cn/Article/details/gecwrdjyz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.yfazqb.com/Article/details/geyvrrpen.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gtlszynda.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/gjvzhbpim.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.bbcook.cn/Article/details/gebyudcwc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.bbcook.cn/Article/details/gjpokdeod.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.bbcook.cn/Article/details/ghinjvkps.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.bbcook.cn/Article/details/gpwgdswmt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.bbcook.cn/Article/details/gfxssqnpl.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/gemniusba.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gzvnugbsa.sHtML


<!-- 参考信息 -->