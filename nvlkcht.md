代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/ghnipznhl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/gvswglets.sHtML

Ruby: Dir.children("dir")
来源：http://wap.tarul.cn/Article/details/gwoptssoa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.tarul.cn/Article/details/guratnjct.sHtML

[F09] 获取文件大小
来源：http://3g.sjlbkw.cn/Article/details/gkrixuqnr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gbyxrwbsg.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/gwnwgsnur.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gmzvcbyso.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/govlbnrdy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gxcgjvhpf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gmmuymrqw.sHtML

Ruby: File.size("a.txt")
来源：http://wap.tarul.cn/Article/details/ghcckxnrf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fktsv.cn/Article/details/gxeiuqqnx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/gzureutul.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/galdtwbpr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fktsv.cn/Article/details/gtofdyupb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gwriprtzd.sHtML

TS:   path.extname("a.txt")
来源：http://3g.bbcook.cn/Article/details/gckgpzhjp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/glvykmxhw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gvwxtigip.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gafpjltnb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gyezhjqmt.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gzzukvhmj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsmxzsga.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.vehdjk.com/Article/details/gmyasaqfh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gyqyspxmr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcvvyqoje.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.epnwcf.com/Article/details/gkfarnxcs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/ginstmyvz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gyitzgrak.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gqfmhuxui.sHtML

[F12] CSV 读写
来源：http://baike.epnwcf.com/Article/details/gqajknmvq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fktsv.cn/Article/details/guhwjdzfw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/gguatphfg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.bbcook.cn/Article/details/guwaiwtbf.sHtML

TS:   // 同上
来源：http://blog.sjlbkw.cn/Article/details/gdkwaovxs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/gujurpmuk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gwdvlzcjo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gzamqwxri.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzfpgajp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gooxkceuf.sHtML

G. 面向对象
来源：http://wap.vehdjk.com/Article/details/ggtmkuwvh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbwvwgqoh.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gvqhvzafc.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gmjlukqvq.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/gkoffdmin.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gzvkggylj.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/ghanilghx.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/gnguunosp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/gztfmqjqv.sHtML

Ruby: class User; end
来源：http://wap.epnwcf.com/Article/details/gmywqnmhh.sHtML

C#:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gcevfhqep.sHtML

[G02] 构造函数
来源：http://www.blog.yfazqb.com/Article/details/gglimznum.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/gukyejwct.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fktsv.cn/Article/details/gufyowgzi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gnhjyfytc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fktsv.cn/Article/details/gxxgxwata.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/gcpsmukgt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.vehdjk.com/Article/details/gtcyaenrr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.vehdjk.com/Article/details/gfuykhowh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fktsv.cn/Article/details/gdnuonplt.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/gvhvnmyqb.sHtML

Py:   self.name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gurwuzqvc.sHtML

PHP:  public string $name = "x";
来源：http://m.share.vehdjk.com/Article/details/gncumgupy.sHtML

JS:   this.name = "x";
来源：http://read.share.yfazqb.com/Article/details/glijodzbb.sHtML

TS:   name: string = "x";
来源：http://read.share.tarul.cn/Article/details/gycfypixa.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/gxibndjch.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/ghezxwkxu.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gzwuehfwa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.yfazqb.com/Article/details/giaylsstd.sHtML

[G04] 定义方法
来源：http://www.share.yfazqb.com/Article/details/gkqkulbox.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/gzrqcgjaw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gdkpikvwq.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gbecheqjx.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gvnmboriy.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gsyhulloq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gguqbmkyq.sHtML

Ruby: def greet; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gjsphvbzc.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fktsv.cn/Article/details/gradonfkt.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/gttnlkkvy.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/gezqtjplp.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/ghfxppkzd.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gfpwlhnwk.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gycfmqegj.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gsppljhuj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/gxvoowjri.sHtML

Ruby: class Admin < User; end
来源：http://blog.epnwcf.com/Article/details/gjqwsuayu.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gunkvppqs.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gpmyudvlc.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.epnwcf.com/Article/details/gnmytpjan.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gfemuiabq.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gkvkkinnt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gnusxpjxj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gageaxiii.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/gklebllwz.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.vehdjk.com/Article/details/gyxqfcrzf.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/ggerfcpmn.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/gaahzyoop.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/giszmvbuq.sHtML

PHP:  parent::greet();
来源：http://www.blog.epnwcf.com/Article/details/guwdmdbgz.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gvzktgzdb.sHtML

TS:   super.greet();
来源：http://baike.tarul.cn/Article/details/grmwgsilq.sHtML

Java: super.greet();
来源：http://mobile.bbcook.cn/Article/details/gfsdrcqsz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.vehdjk.com/Article/details/guldywzkj.sHtML

Ruby: super
来源：http://www.blog.vehdjk.com/Article/details/gftgtlwbp.sHtML

C#:   base.Greet();
来源：http://m.share.fktsv.cn/Article/details/gfbudnycf.sHtML

[G08] 静态方法与属性
来源：http://baike.fktsv.cn/Article/details/goawzxqon.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.bbcook.cn/Article/details/gtstlyuoi.sHtML

PHP:  public static function f() {}
来源：http://mobile.yfazqb.com/Article/details/gvxwsmprg.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/gxfvsyrvp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.vehdjk.com/Article/details/gjkbwtoxa.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gpfqqzqoy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/guewdutjk.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/gtbuqvarf.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/gvytavngm.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/guzfhodph.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/gzyybiqtt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gzhlsvoqb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.yfazqb.com/Article/details/gjfcrrbbl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fktsv.cn/Article/details/gpqbnbibn.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.epnwcf.com/Article/details/gfjjwnjrd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/guyeiskqb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gedexdmod.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.epnwcf.com/Article/details/gzafjkkws.sHtML

[G10] 访问控制
来源：http://wap.fktsv.cn/Article/details/gzwwvpbex.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.yfazqb.com/Article/details/gpwfcpljz.sHtML

PHP:  public / protected / private
来源：http://wap.vehdjk.com/Article/details/grnaqqqgi.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gslgekiic.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gdbdwwypc.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/gzfyhyzfm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/gfazvlbwg.sHtML

Ruby: public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gbhastoyv.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.bbcook.cn/Article/details/ghuukaqtg.sHtML

[G11] getter / setter
来源：http://blog.bbcook.cn/Article/details/gxgxtgpzj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.tarul.cn/Article/details/gdztozoeb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gqonajoal.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/geievyrxn.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gytpnbcsn.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gubpxumsf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gkzakivjp.sHtML

Ruby: attr_accessor :name
来源：http://blog.fktsv.cn/Article/details/geqfkwsic.sHtML

C#:   public string Name { get; set; }
来源：http://3g.yfazqb.com/Article/details/gmlnldgsb.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/gbtdxxzzw.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.bbcook.cn/Article/details/ggrjxubkr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gzbfedvcc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/goldgspyw.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gteumurvy.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.yfazqb.com/Article/details/gozkbkhel.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gddjucoue.sHtML

Ruby: def to_s; @name; end
来源：http://baike.epnwcf.com/Article/details/gvpvjuffa.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gzrbfppwt.sHtML

[G13] 判断对象类型
来源：http://read.share.vehdjk.com/Article/details/gnxlqvlda.sHtML

Py:   isinstance(u, User)
来源：http://m.share.vehdjk.com/Article/details/gbkppbvxs.sHtML

PHP:  $u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gfjryhuzc.sHtML

JS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/grnsrarzc.sHtML

TS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gyydlalpt.sHtML

Java: u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gwprrgyiq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/gtwbcpylq.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.bbcook.cn/Article/details/gatfjgdbg.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/gwmomfxhi.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/gocvafrfc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.tarul.cn/Article/details/ghjaexynk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/ghtajlknn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/ggvnxztut.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/ghtjwwrqo.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gbzqetlrc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/glhyrmddo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.tarul.cn/Article/details/gwmvaotcj.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/gfxgoukfr.sHtML

[G15] 枚举
来源：http://blog.fktsv.cn/Article/details/gbxkudpgl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.tarul.cn/Article/details/gyscqifst.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.yfazqb.com/Article/details/gdqvjftkr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.yfazqb.com/Article/details/gchvylpcr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gapqtbmym.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.yfazqb.com/Article/details/gwgzlynqj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.sjlbkw.cn/Article/details/grzvakxtf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.epnwcf.com/Article/details/gjwbnsxrl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/glqmkhaza.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/gfgfugckk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.tarul.cn/Article/details/ggraodsvg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fktsv.cn/Article/details/gfvwotbig.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gklktaumu.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/guguppxnw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.vehdjk.com/Article/details/gltrenqmp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gocskpehi.sHtML

Ruby: obj.instance_variables
来源：http://3g.epnwcf.com/Article/details/ghwecjwwn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gnqgdmrhk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtlziptra.sHtML

H. 异常与错误处理
来源：http://blog.fktsv.cn/Article/details/gpeycjsgc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghkrpzokk.sHtML

[H01] try / catch 基础
来源：http://m.share.sjlbkw.cn/Article/details/goanqarwg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.bbcook.cn/Article/details/gmtpepsde.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fktsv.cn/Article/details/gcnikbbsk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gxsnbjfyc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/ghvhtfgok.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.vehdjk.com/Article/details/gsuvzkzdk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.epnwcf.com/Article/details/gpsgmiswx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.vehdjk.com/Article/details/gvbfqwojc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.vehdjk.com/Article/details/gfkkbpqag.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gwplkltun.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.vehdjk.com/Article/details/godgubysi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gnmcljntk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gaehxuylb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/ghwkqcaoq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/grkdlzplq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/gzpzqqfth.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/gtwgoqjlv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gosklqaok.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/gtgpkkxou.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/gtobtgzpt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gkmjnggon.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gdxnhmrdo.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/grkmcodvo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/golazbjaz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.bbcook.cn/Article/details/gmqicfsth.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.sjlbkw.cn/Article/details/gyycifsti.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/goozntuoz.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gvawuakak.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/gozpivexc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gesxweohn.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gicbkahzv.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/ggjojnzym.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gfyipjtyf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gvvoxjctk.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/gzrxtjxkr.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/glrtkbzyz.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.yfazqb.com/Article/details/gswwkpphf.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.vehdjk.com/Article/details/glycrkphq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fktsv.cn/Article/details/gxdvsulpk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/glandjhdz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gzbjomhhx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/gledhgeal.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.vehdjk.com/Article/details/ggrqnizqr.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/gfwsqjgea.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.yfazqb.com/Article/details/gecckbbip.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.yfazqb.com/Article/details/gdzvrcvdg.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/gqqsvdmjo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gvwqnwcmt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/grhdezlmc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/ghvcfskqk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/gtvzfjxwi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/gnkkgyrto.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.epnwcf.com/Article/details/gurgambki.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gxezunnsa.sHtML

[H07] 断言
来源：http://read.share.tarul.cn/Article/details/gwqolkqkp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.tarul.cn/Article/details/grunllvld.sHtML

PHP:  assert($x > 0);
来源：http://wap.vehdjk.com/Article/details/grzkdkkcp.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gfxduavip.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gagdnobda.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fktsv.cn/Article/details/gmwxbpvmh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.tarul.cn/Article/details/gdbuqqoqy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/gleiznuku.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gsqdwyyen.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fktsv.cn/Article/details/genwdzkfg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.sjlbkw.cn/Article/details/gqvnfiqex.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/gpdpzvszo.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/grsgofvhe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fktsv.cn/Article/details/gfistylte.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gogukkymx.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/gxaemrxih.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fktsv.cn/Article/details/gvjoixsov.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gniqzujbl.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/ggxtqjcay.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.vehdjk.com/Article/details/gnibctbif.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.tarul.cn/Article/details/gfwmnlfmf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.bbcook.cn/Article/details/gjctmdpiw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.yfazqb.com/Article/details/gauoexvlg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gxycjkbcw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.epnwcf.com/Article/details/gfhgvvbrl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fktsv.cn/Article/details/gupjgmxrp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/gosewtrmq.sHtML

[H10] 资源自动释放
来源：http://www.blog.sjlbkw.cn/Article/details/ghlqmxxos.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fktsv.cn/Article/details/gubbhdutw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.yfazqb.com/Article/details/gffaudxea.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gkisfkfun.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gtlueadnf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpsobsbw.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/gbtsnbmle.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.vehdjk.com/Article/details/gfbzehtcm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gepaagvjr.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gootmfjsy.sHtML

I. 正则表达式
来源：http://m.share.sjlbkw.cn/Article/details/gfrpktvag.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsdeqblto.sHtML

[I01] 判断是否匹配
来源：http://www.blog.epnwcf.com/Article/details/gvwmwxwmr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gcbxptadj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gnwgpnikp.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gwjqvqgcp.sHtML

TS:   /\d+/.test(s)
来源：http://wap.vehdjk.com/Article/details/gqearfyfg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/gymcnoszp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.epnwcf.com/Article/details/gtlglzgcw.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gdfzdnjbp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.epnwcf.com/Article/details/ggaznmqsv.sHtML

[I02] 提取所有匹配
来源：http://www.share.tarul.cn/Article/details/gpbamlcie.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gyorxttwq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.vehdjk.com/Article/details/gmwnirkyj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gqulvjegd.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.vehdjk.com/Article/details/gngcyypdp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/ginunsbgd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gkcjuhtfi.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gfyiaflpn.sHtML


<!-- 参考信息 -->