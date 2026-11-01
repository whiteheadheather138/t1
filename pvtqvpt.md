代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/guokfdoet.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fktsv.cn/Article/details/gsrrxnmoo.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gtmtlakqs.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gdfeyohid.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gbwopzxta.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.bbcook.cn/Article/details/gfqxwqern.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/glkdryfgg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gqerntcbl.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gnprecdua.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gtjexnekl.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gncdrxikn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gksrrznbm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gqednouet.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gkncjawkh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/gakoefcpa.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.tarul.cn/Article/details/gjxrgmnco.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.vehdjk.com/Article/details/gxwwgjvcl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.tarul.cn/Article/details/gupqymudd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gtreitmfr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gqznbqauh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gzuplsxig.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gylxbnoed.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gyfosbvpw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/geutvvoje.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gwrgjoirm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfzlykxyb.sHtML

[F11] 复制与移动文件
来源：http://blog.tarul.cn/Article/details/gjnctamuc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gtafzczkp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.tarul.cn/Article/details/gmjjgywxp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gwyopgkwv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/giaecsxut.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/gjhohyzaq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.bbcook.cn/Article/details/gwincvzjz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gydlxayeo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gmapidopd.sHtML

[F12] CSV 读写
来源：http://3g.fktsv.cn/Article/details/gradhypsq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gqftwiexy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/gatkbeuaz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gcynqrfxu.sHtML

TS:   // 同上
来源：http://www.blog.epnwcf.com/Article/details/glpmltswd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/gmsvwyugq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/gdjfxlvap.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gvhmvlwfj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.bbcook.cn/Article/details/gzihbgkgq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkbbxedcy.sHtML

G. 面向对象
来源：http://baike.bbcook.cn/Article/details/gjwyyinvl.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/godjjyrgf.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/gcbbpvban.sHtML

Py:   class User: pass
来源：http://blog.sjlbkw.cn/Article/details/grrplztfc.sHtML

PHP:  class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gibumthxb.sHtML

JS:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/gnqoycecb.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.sjlbkw.cn/Article/details/gduqjdiwy.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/giuwdrumb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.bbcook.cn/Article/details/guqgrutst.sHtML

Ruby: class User; end
来源：http://www.blog.epnwcf.com/Article/details/glntjyipi.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gidartvqm.sHtML

[G02] 构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gotyozzmb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fktsv.cn/Article/details/gxjsppijk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/guyiblzex.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/giialsbrq.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/gczcqjsqf.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/goddpdmjz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.epnwcf.com/Article/details/gcfqcptkr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/gltyzzpdn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.bbcook.cn/Article/details/gjbqapqtb.sHtML

[G03] 实例属性
来源：http://m.share.sjlbkw.cn/Article/details/gjvftuaqd.sHtML

Py:   self.name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gpusxtblv.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/ghzygrvkq.sHtML

JS:   this.name = "x";
来源：http://read.share.yfazqb.com/Article/details/ghhhinznx.sHtML

TS:   name: string = "x";
来源：http://m.share.tarul.cn/Article/details/gamjlyimc.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/ghxezejmm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gtsuvoqau.sHtML

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/girqqhcij.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.yfazqb.com/Article/details/gkzanfbpw.sHtML

[G04] 定义方法
来源：http://read.share.yfazqb.com/Article/details/gtwahbhla.sHtML

Py:   def greet(self): return self.name
来源：http://blog.vehdjk.com/Article/details/gzoefkwjh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gewckfmnl.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gygecxxje.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gvtaoyxjb.sHtML

Java: String greet() { return name; }
来源：http://blog.fktsv.cn/Article/details/guvxqzwhx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gyxdtvjfd.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gzscogqkh.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fktsv.cn/Article/details/guqvdngfa.sHtML

[G05] 继承
来源：http://mobile.vehdjk.com/Article/details/goreaimib.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/gmasctbqz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gyanioolp.sHtML

JS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gdsgunmqk.sHtML

TS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gddxizgwi.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gfdsnfayh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.tarul.cn/Article/details/gogaohvvd.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.tarul.cn/Article/details/gayqpqhjb.sHtML

C#:   class Admin : User {}
来源：http://m.share.epnwcf.com/Article/details/gjfibfeeu.sHtML

[G06] 重写方法
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbecdkgz.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/gciattdar.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gbtgrgnck.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gxhqyhqxm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/glccapwhh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gxmusurva.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fktsv.cn/Article/details/geqcbaaeo.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fktsv.cn/Article/details/gqxnhwqui.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.epnwcf.com/Article/details/gfnnwgqiw.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/gdczenpbe.sHtML

Py:   super().greet()
来源：http://www.m.share.vehdjk.com/Article/details/gyghzghzs.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/gonmuolzc.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkguanix.sHtML

TS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/ghmnhmyrj.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/gcxxnbgcg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/gplquseug.sHtML

Ruby: super
来源：http://www.blog.bbcook.cn/Article/details/gdkorjqbv.sHtML

C#:   base.Greet();
来源：http://3g.sjlbkw.cn/Article/details/gdpliccml.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/gevgsvbyj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.tarul.cn/Article/details/gfphrdxrs.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/gimqpviza.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/gyzkftbmq.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gyvrwxkgu.sHtML

Java: static void f() {}
来源：http://www.blog.vehdjk.com/Article/details/gauttglwb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.bbcook.cn/Article/details/gozpfvhlt.sHtML

Ruby: def self.f; end
来源：http://blog.bbcook.cn/Article/details/gsfbqvxdc.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/gyujfjofa.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gfzcvnywq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.tarul.cn/Article/details/giwwqyysg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gvquiurkp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/ggvifhbre.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.bbcook.cn/Article/details/giwtaqbtc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.epnwcf.com/Article/details/gllvjhxhi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.yfazqb.com/Article/details/gnetyrspd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gvtqxbnuh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/gmgfwsiop.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/gbwdacbor.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.vehdjk.com/Article/details/gjxlnitop.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gunanhfyo.sHtML

JS:   #private 字段；其余公开
来源：http://blog.bbcook.cn/Article/details/gkjguepko.sHtML

TS:   public / protected / private
来源：http://3g.epnwcf.com/Article/details/gpyysvskx.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/gcxgozitd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.epnwcf.com/Article/details/gmxhrgewn.sHtML

Ruby: public / protected / private
来源：http://wap.yfazqb.com/Article/details/gldzpgvjr.sHtML

C#:   public / protected / private / internal
来源：http://blog.epnwcf.com/Article/details/gaanrzjnm.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/gczdllbqo.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fktsv.cn/Article/details/gthwptzej.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gebaqttdg.sHtML

JS:   get name() { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gcojshjhl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gqktzwiwt.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gxvfcbrrd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gjlkaezcg.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gowhvpzcv.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbabjvzd.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/ggdovusfw.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gqwuxzjjg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gvvnfridv.sHtML

JS:   toString() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gpvmhnpxo.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gnpbpkhor.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gomukjlfx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/ggbtatavb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gdbonomcq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/giqurbweg.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/gqkpyusho.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/gsjpkfbcu.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/gcnrtzmjd.sHtML

JS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gsrteatfu.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/giipymkdy.sHtML

Java: u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gtivbbmyv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/gooflexqf.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gobjtdphd.sHtML

C#:   u is User
来源：http://3g.bbcook.cn/Article/details/gieaqdptm.sHtML

[G14] 数据类 / record
来源：http://wap.vehdjk.com/Article/details/gjssklvuw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.vehdjk.com/Article/details/gpisdxbmv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.epnwcf.com/Article/details/gisjewqyu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.epnwcf.com/Article/details/gsftcnbhx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/gwpaondus.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.epnwcf.com/Article/details/gqhfpqkxa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gctnykbps.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/glluttuha.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.sjlbkw.cn/Article/details/grsqsyhdl.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/ggnzjvbev.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gzuadrvym.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fktsv.cn/Article/details/ggtobihly.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fktsv.cn/Article/details/gfjyfdqfo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gaxltyidw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/gpjknpgna.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fktsv.cn/Article/details/ggotoqyhq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.epnwcf.com/Article/details/gqxzgkewe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gqnlveizz.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/gkqstsagk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.vehdjk.com/Article/details/ghbuvhtcy.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.sjlbkw.cn/Article/details/gbxeofibp.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gascqytbm.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gzevnyhqs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.tarul.cn/Article/details/gniicxvcq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.epnwcf.com/Article/details/grxesvxry.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/geipzmzsg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gddqyokqq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdtyaddpg.sHtML

H. 异常与错误处理
来源：http://blog.vehdjk.com/Article/details/gzelfchyb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkinxrizu.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/guylwyigr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.epnwcf.com/Article/details/guybarngs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gbrwrxywf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/ganjpjikg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gocpajgax.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.vehdjk.com/Article/details/gvaxuwogn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.tarul.cn/Article/details/gsemtqafm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/gdvoavbnq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.bbcook.cn/Article/details/gqlvgrpor.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/ggebysvqo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gyxhksyjv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gkchaoxyu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gsfvlowjs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gznelhvly.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gprocggbv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.vehdjk.com/Article/details/gftabudfs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/gwbsbraie.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gjrmoqrci.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gschbzrwz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fktsv.cn/Article/details/gthzwqfkt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gzvamkcpm.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gbtzupuby.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gpbclfmjm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gpmxspeve.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.vehdjk.com/Article/details/gsmygprqv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.vehdjk.com/Article/details/gbdskyquu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gvpshienz.sHtML

[H04] 自定义异常类型
来源：http://www.blog.epnwcf.com/Article/details/gppjdgteh.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.tarul.cn/Article/details/gplyxsduu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/glzaisrmf.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gsckngjko.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gqnfpjzwx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gzetyjcea.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.tarul.cn/Article/details/glwcijqfk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.vehdjk.com/Article/details/ggiwcrsbg.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gcwrlwbto.sHtML

[H05] 捕获特定类型
来源：http://wap.tarul.cn/Article/details/gzstcitcd.sHtML

Py:   except ValueError as e:
来源：http://3g.bbcook.cn/Article/details/gkrbraahe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.vehdjk.com/Article/details/gseflypwj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gcbqvotnu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gebwnyfak.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.tarul.cn/Article/details/gfrcsmvlr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.yfazqb.com/Article/details/gugoddbut.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/gtklafgkd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/golojddyk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gosybagiz.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.vehdjk.com/Article/details/giahxiprj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gprygfxzr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gpxcycliy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gkdmuargw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.tarul.cn/Article/details/gomclhdkd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.vehdjk.com/Article/details/gpyfuphvq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.tarul.cn/Article/details/gytwbtfln.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.yfazqb.com/Article/details/gsvvtasqk.sHtML

[H07] 断言
来源：http://3g.fktsv.cn/Article/details/glmnfsjls.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.yfazqb.com/Article/details/gxqyvarps.sHtML

PHP:  assert($x > 0);
来源：http://www.share.yfazqb.com/Article/details/gnnwfgeaz.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gvhmffuyp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gkhlcorow.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gjyqamcnz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.bbcook.cn/Article/details/gyrtgwesd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.bbcook.cn/Article/details/gcjznewuy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gkcbwhhvy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.tarul.cn/Article/details/gbwnxauwx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmjcwmgs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.sjlbkw.cn/Article/details/gonybqhum.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fktsv.cn/Article/details/gscajnixq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.tarul.cn/Article/details/giptanwqz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.yfazqb.com/Article/details/gmjumnvew.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/gdedppado.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.sjlbkw.cn/Article/details/gkdifpfll.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fktsv.cn/Article/details/gzdjunbuk.sHtML

[H09] 带错误码的异常
来源：http://3g.vehdjk.com/Article/details/gjlkfchvo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.tarul.cn/Article/details/glaywxcpc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gattpkmci.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/gwntfzzox.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.yfazqb.com/Article/details/gxtmarnxs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gewcbmryl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gzabomqda.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.bbcook.cn/Article/details/gznjcibgt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.yfazqb.com/Article/details/genmdmwps.sHtML

[H10] 资源自动释放
来源：http://wap.epnwcf.com/Article/details/gkmyyooqr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.bbcook.cn/Article/details/gphpzybva.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fktsv.cn/Article/details/gpwtmdrou.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/gprlkitug.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/gbpqnhndd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/gvssrzeor.sHtML

Go:   defer f.Close()
来源：http://mobile.epnwcf.com/Article/details/gbqmizikk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.sjlbkw.cn/Article/details/gxjdbvpuy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/gcqqwwjsc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkrezpaan.sHtML

I. 正则表达式
来源：http://www.blog.tarul.cn/Article/details/ghoiosavg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gixsvxxdi.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/gofijmstu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gwqieypht.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/guxvokavf.sHtML

JS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gmfdnafxx.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gbmizubnk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.yfazqb.com/Article/details/ghukztgue.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.vehdjk.com/Article/details/gnlxhbujc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gdysmjcbq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.epnwcf.com/Article/details/ggmfbkzko.sHtML

[I02] 提取所有匹配
来源：http://read.share.bbcook.cn/Article/details/gmbzkacsv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gtnfqvlxz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.epnwcf.com/Article/details/gfirfnfei.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.tarul.cn/Article/details/ghbudakzw.sHtML


<!-- 参考信息 -->