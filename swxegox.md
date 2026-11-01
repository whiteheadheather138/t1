代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/grqyrbaho.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/ghfwflroc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/glzjsimql.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fktsv.cn/Article/details/gcveqvykd.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gfppesfen.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.epnwcf.com/Article/details/grjvefapm.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/gcmkkywvx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gxlqbgohx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/ggzwmfubw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gjabxqupt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/gxtzkosks.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/gccrfkmzf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gaytqrpap.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gpsnuxmyx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gxjjrelhj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.bbcook.cn/Article/details/ggxyompjc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gymrbzbed.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ggibbspqn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/gphoqfyyl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gxohoakbf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gbwwzqhzm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gxnfrbqnj.sHtML

[F11] 复制与移动文件
来源：http://www.share.tarul.cn/Article/details/gqipfdlxq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gzawzghbh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.vehdjk.com/Article/details/gabikrzes.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gqspusxzs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gjwbbahhj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.epnwcf.com/Article/details/grswtywob.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/gcwdkmjlx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gapnqkess.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/gcwxikaly.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gplwmxnfg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/ghgkpolch.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gvmfecvex.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fktsv.cn/Article/details/ggeavqpsd.sHtML

TS:   // 同上
来源：http://3g.epnwcf.com/Article/details/gsoujeaif.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fktsv.cn/Article/details/gntgtyhku.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.epnwcf.com/Article/details/gpobinniq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/gamtfadoz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.yfazqb.com/Article/details/ggshclykp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/guaeocgys.sHtML

G. 面向对象
来源：http://mobile.bbcook.cn/Article/details/gfnapbsds.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gljeryjif.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/grnjvtgts.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gcygilcqu.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gxyrmxiyj.sHtML

JS:   class User {}
来源：http://mobile.bbcook.cn/Article/details/grsaafyzh.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fktsv.cn/Article/details/gmmavqzqe.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gygoatvnp.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.epnwcf.com/Article/details/grhhdtoxu.sHtML

Ruby: class User; end
来源：http://blog.sjlbkw.cn/Article/details/gocwbeadm.sHtML

C#:   class User {}
来源：http://wap.tarul.cn/Article/details/gtxgimmpz.sHtML

[G02] 构造函数
来源：http://www.m.share.tarul.cn/Article/details/ggbvmwgew.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.tarul.cn/Article/details/gmquqnikw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.tarul.cn/Article/details/glsugyxdb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gtyjdkace.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gwjpdqjni.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gsoggmrah.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fktsv.cn/Article/details/gadqtaips.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/gvzvswnei.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.tarul.cn/Article/details/gmmzptlat.sHtML

[G03] 实例属性
来源：http://www.share.yfazqb.com/Article/details/gmcrtdpfd.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/giifkwpst.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gpyutbdlq.sHtML

JS:   this.name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gkwrszchp.sHtML

TS:   name: string = "x";
来源：http://www.share.epnwcf.com/Article/details/gcawyglms.sHtML

Java: private String name;
来源：http://www.blog.yfazqb.com/Article/details/gzjvttzji.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.sjlbkw.cn/Article/details/gjkxhzueu.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/geikabcda.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/gfhpadjqs.sHtML

[G04] 定义方法
来源：http://www.m.share.bbcook.cn/Article/details/gbnjgmhir.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gkuxcgofc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gfwryamfj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfbdeuhah.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gknxulgyz.sHtML

Java: String greet() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gjemneigv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/grbdnxsii.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/gbwysyemx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gxvfirvmr.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/ggwppbyhx.sHtML

Py:   class Admin(User): pass
来源：http://www.share.bbcook.cn/Article/details/gperjiuhg.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gkxrnfcig.sHtML

JS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gpkasjwqs.sHtML

TS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gbyxxioxm.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gkmfwqgft.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gqmhdzxya.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gsqzatxwj.sHtML

C#:   class Admin : User {}
来源：http://www.share.epnwcf.com/Article/details/gvhcnoppu.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/gxgiwsfuv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.epnwcf.com/Article/details/gdvwiqnyb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gfntknahi.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/ggycsvaob.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gtcemyemx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gcbilyxba.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/ghelcgtpv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fktsv.cn/Article/details/gsdjoikzm.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/ghtvtxctn.sHtML

[G07] 调用父类方法
来源：http://blog.bbcook.cn/Article/details/gbjiwdniu.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/gzsfxyjrx.sHtML

PHP:  parent::greet();
来源：http://mobile.fktsv.cn/Article/details/gaffcwlfl.sHtML

JS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gyoeeyisr.sHtML

TS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/ghtmlkzok.sHtML

Java: super.greet();
来源：http://read.share.epnwcf.com/Article/details/gausfymxa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gwgmuuoav.sHtML

Ruby: super
来源：http://m.share.vehdjk.com/Article/details/gubtqsnlm.sHtML

C#:   base.Greet();
来源：http://www.blog.fktsv.cn/Article/details/gphoppzgq.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gkrljnldu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.tarul.cn/Article/details/gsdrjxdip.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/gtfhwremo.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/gphlvbxqy.sHtML

TS:   static f(): void {}
来源：http://read.share.bbcook.cn/Article/details/gsybtswdd.sHtML

Java: static void f() {}
来源：http://www.share.sjlbkw.cn/Article/details/geenswuqg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.yfazqb.com/Article/details/gbzcyvoku.sHtML

Ruby: def self.f; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvorpiad.sHtML

C#:   public static void F() {}
来源：http://www.blog.yfazqb.com/Article/details/gensqdocp.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/gepbefjni.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/guapzwmaa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.bbcook.cn/Article/details/gjenvzbey.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.epnwcf.com/Article/details/gugujjklm.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gawpkeqid.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/ggfsbwqjq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.sjlbkw.cn/Article/details/gvslpuajd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.tarul.cn/Article/details/guqcxeqtr.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.vehdjk.com/Article/details/guspuctzz.sHtML

[G10] 访问控制
来源：http://mobile.epnwcf.com/Article/details/giurjbgyc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gojucwuzx.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gpmufaucc.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/goljiqhcw.sHtML

TS:   public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/guvpqrhjv.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.yfazqb.com/Article/details/gpiwynuwq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gjghywqjh.sHtML

Ruby: public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gzgwrxpvf.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fktsv.cn/Article/details/goljttctr.sHtML

[G11] getter / setter
来源：http://wap.yfazqb.com/Article/details/gursqtxim.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/gvgwcisqp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gbfwwzfxl.sHtML

JS:   get name() { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gfbhydqvt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/glkjmmwix.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gejgkdkpy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gfidatdbc.sHtML

Ruby: attr_accessor :name
来源：http://3g.bbcook.cn/Article/details/ggqolrzro.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.tarul.cn/Article/details/gefcoqtja.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/ggunqtqth.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gfciigdmn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/grwfjefdv.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gbdrynghv.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/graqvzxuq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/givllkalq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gaogpbyyu.sHtML

Ruby: def to_s; @name; end
来源：http://3g.bbcook.cn/Article/details/gdadfpwdj.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.tarul.cn/Article/details/gatgpcmbw.sHtML

[G13] 判断对象类型
来源：http://3g.epnwcf.com/Article/details/gdgtqfgmq.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gtezjgfqv.sHtML

PHP:  $u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gikwixvlb.sHtML

JS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gpvzcyxxy.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gsxueiuvg.sHtML

Java: u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gmyfiktcp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/glzueualw.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gnifhxqkz.sHtML

C#:   u is User
来源：http://read.share.tarul.cn/Article/details/gxavyqchy.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/gqulpvxtf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/gnzadupzd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fktsv.cn/Article/details/gpeygqhad.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/gsetngbnq.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.yfazqb.com/Article/details/gweyvzwjx.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/gjqtpwaia.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/gagdizkma.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.tarul.cn/Article/details/gyocicclb.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.yfazqb.com/Article/details/ghsbdxgto.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/gextongly.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwebmitz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fktsv.cn/Article/details/gzfjqonjb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.vehdjk.com/Article/details/gfydmrksq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gobliytis.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/gpcioeogx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.tarul.cn/Article/details/gbnlavkqx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.vehdjk.com/Article/details/gqvnnnbyc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gijljldfi.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.vehdjk.com/Article/details/goksiulpd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.tarul.cn/Article/details/gispuxcpy.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.sjlbkw.cn/Article/details/gutuhywlk.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/guoypnjfa.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gopqfhhtp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/gedakatgs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fktsv.cn/Article/details/gdnyiaxuy.sHtML

Ruby: obj.instance_variables
来源：http://www.share.epnwcf.com/Article/details/ghgusmuxe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/glydujhcg.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gtexlmmul.sHtML

H. 异常与错误处理
来源：http://mobile.vehdjk.com/Article/details/gnwotbstx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghabsoiki.sHtML

[H01] try / catch 基础
来源：http://3g.sjlbkw.cn/Article/details/gzhxjytau.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/gmtefznhs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/gpbuwvxly.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/guxjispov.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/ggvrxykui.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gglvebhbs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/gxsespgho.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/gyvrowwhq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.yfazqb.com/Article/details/grnvrygyd.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.epnwcf.com/Article/details/ghagmwppw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.sjlbkw.cn/Article/details/gfpanxvjh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gqxbpdkry.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gbxdiuxha.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/ghrsqsknq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gygavicun.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/gjdladarr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.epnwcf.com/Article/details/gndifhcpn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/guvfjlnfr.sHtML

[H03] 主动抛出异常
来源：http://www.share.bbcook.cn/Article/details/gdulcrakg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gwicvlmls.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gtalzxapt.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/ginchiorj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gajyvacfh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gkbfixghd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.vehdjk.com/Article/details/gjprcxyaz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/glqyiqjbq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gazjnyheu.sHtML

[H04] 自定义异常类型
来源：http://baike.bbcook.cn/Article/details/gnvfeaklf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fktsv.cn/Article/details/gkoycizyq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gblxtqusz.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gyapkminm.sHtML

TS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/guaqzazsm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/glvhumtcw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/gvfkehcau.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.bbcook.cn/Article/details/gbjsiexzw.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/glhkdsruc.sHtML

[H05] 捕获特定类型
来源：http://www.share.yfazqb.com/Article/details/ghbylaajs.sHtML

Py:   except ValueError as e:
来源：http://baike.bbcook.cn/Article/details/glopgxixc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.tarul.cn/Article/details/gdbxdxjek.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gqkxnwklx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gkrommqqa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.yfazqb.com/Article/details/gheiufwwk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fktsv.cn/Article/details/ggzmifhuv.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.epnwcf.com/Article/details/gazfesymf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.epnwcf.com/Article/details/gtszmbbqa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fktsv.cn/Article/details/gtotiwxsd.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.yfazqb.com/Article/details/ganxdbaeq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gbxxvdzds.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gzmdbcmlx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/ggyiskcqm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.epnwcf.com/Article/details/gbhxsnpol.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gcvyugxgn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/gpfpuamks.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.vehdjk.com/Article/details/gtqdrrdwk.sHtML

[H07] 断言
来源：http://m.share.bbcook.cn/Article/details/gkbngmsjx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.sjlbkw.cn/Article/details/ghlczdouo.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/gxzrzthlk.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/glbcekxnn.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gjdvsdqrr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.epnwcf.com/Article/details/gwdmgmeui.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.vehdjk.com/Article/details/gidizncef.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fktsv.cn/Article/details/gnwinxdnx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gxfrjimzi.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.bbcook.cn/Article/details/gkymbiasi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.bbcook.cn/Article/details/gfnjmpmjr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/gheuitpxh.sHtML

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/grluytbyc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/gffveefjq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gbaouwudx.sHtML

Go:   err.Error()
来源：http://m.share.sjlbkw.cn/Article/details/gozhmqkon.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/gauyltxwu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.sjlbkw.cn/Article/details/grxuukutp.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.bbcook.cn/Article/details/gtxcwltff.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gbeerwdvz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.epnwcf.com/Article/details/gifhalulw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/gamfyezoh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.yfazqb.com/Article/details/gomrvglwm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fktsv.cn/Article/details/gvfagnxwz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gilsjqlvy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.vehdjk.com/Article/details/gsdwhysbc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gsjlmqbao.sHtML

[H10] 资源自动释放
来源：http://www.share.epnwcf.com/Article/details/gtgipbzof.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fktsv.cn/Article/details/gevvtszok.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.yfazqb.com/Article/details/gimcsoyko.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gotjvcyil.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gtwutclme.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/gmyuhoioi.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/grmgksjax.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/gstkhedkp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gthowoiyd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsyexznbx.sHtML

I. 正则表达式
来源：http://www.m.share.vehdjk.com/Article/details/gndejwzbd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfzknsyhv.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fktsv.cn/Article/details/gubaialfk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/ggdegapik.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.vehdjk.com/Article/details/guzwfwvgr.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gotynleom.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gdfxyclsy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gazxdipud.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.sjlbkw.cn/Article/details/gwngtziuw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/goopdkzcg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gcxujqcwe.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/gmxoumzut.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gcjygxdhu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/gomvbfzzf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/gfmufszbj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.yfazqb.com/Article/details/gkcnzhjml.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/gpvaiikuf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gdmrjfpqv.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gpptoifjv.sHtML


<!-- 参考信息 -->