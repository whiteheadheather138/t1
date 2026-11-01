代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gmvtsekqc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/gitfzhdfm.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/gsmuqccxj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.vehdjk.com/Article/details/gjijeqpuo.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gfuqjbrbe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gtqnvcrgp.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fktsv.cn/Article/details/gzmlikzel.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gdsuotmyf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/grqlzlzph.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gxuejdter.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/gybuffkdj.sHtML

Ruby: File.size("a.txt")
来源：http://wap.vehdjk.com/Article/details/ghiphmrpu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/geswwixfa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.yfazqb.com/Article/details/gexxnwluj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gzdzgbywx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.yfazqb.com/Article/details/gixyesdiy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gbizybsks.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gmbvwzioh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.epnwcf.com/Article/details/ggocbfqqk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/ghhdvpqhi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/giqsekwam.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gverjxzvf.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/goguosscv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gnsxhislm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.vehdjk.com/Article/details/gcexevdey.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gbqtgxarc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gejbbxgvs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.epnwcf.com/Article/details/gvhsgzodw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.bbcook.cn/Article/details/gzlfdpcwq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gdnrpyhnr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.epnwcf.com/Article/details/gkejouzzx.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/gfuikyrpe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/gcdafxwth.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/gjjrgvhxp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.tarul.cn/Article/details/gpvdczqgi.sHtML

TS:   // 同上
来源：http://3g.epnwcf.com/Article/details/gfmrlugux.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gdmfbyfjv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.yfazqb.com/Article/details/guoovnqqc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/gprlmgblv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.tarul.cn/Article/details/gzcfzdqiy.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxjbnflvn.sHtML

G. 面向对象
来源：http://baike.sjlbkw.cn/Article/details/gndpotlcz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwhcryjki.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/gbmtzbzxq.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gwjdjqaaz.sHtML

PHP:  class User {}
来源：http://wap.tarul.cn/Article/details/grvbimhpm.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gzkswgocs.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.sjlbkw.cn/Article/details/gurcpqocx.sHtML

Java: class User {}
来源：http://www.share.bbcook.cn/Article/details/groxgdjvd.sHtML

Go:   type User struct { Name string }
来源：http://read.share.epnwcf.com/Article/details/gbgwjpidp.sHtML

Ruby: class User; end
来源：http://mobile.tarul.cn/Article/details/gjfurvodj.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/goutcdzvw.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/ggbyexasr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.tarul.cn/Article/details/gnncwmaar.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.sjlbkw.cn/Article/details/gxcifabic.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gogeachde.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.sjlbkw.cn/Article/details/glxmmeiuj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gtxqytylk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.sjlbkw.cn/Article/details/gbfqdftvt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/gpnchxcmb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.yfazqb.com/Article/details/gcqxrytix.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gdgtybbif.sHtML

Py:   self.name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gqezzboua.sHtML

PHP:  public string $name = "x";
来源：http://mobile.yfazqb.com/Article/details/gctykptlp.sHtML

JS:   this.name = "x";
来源：http://blog.sjlbkw.cn/Article/details/ggmiilhbq.sHtML

TS:   name: string = "x";
来源：http://www.blog.yfazqb.com/Article/details/geleodcmp.sHtML

Java: private String name;
来源：http://www.blog.yfazqb.com/Article/details/gliucdjhe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gldexkfot.sHtML

Ruby: @name = "x"
来源：http://blog.sjlbkw.cn/Article/details/goyquggww.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.epnwcf.com/Article/details/gtehgvvuz.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gblwwokgh.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gcakfcakn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gorkdsdcz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gicxbknmr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gtxcgvykk.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gpjlngugg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gzqbkdthd.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gquudkzcf.sHtML

C#:   public string Greet() => Name;
来源：http://3g.yfazqb.com/Article/details/gpnroyxfv.sHtML

[G05] 继承
来源：http://baike.epnwcf.com/Article/details/gmyaskwss.sHtML

Py:   class Admin(User): pass
来源：http://m.share.vehdjk.com/Article/details/gwgpozmvl.sHtML

PHP:  class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gznhoptkv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gvyzxhklt.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gyolatuwg.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gbixnhczz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gksbfhros.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/ghyivdznh.sHtML

C#:   class Admin : User {}
来源：http://www.share.bbcook.cn/Article/details/gcqboielu.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/ggasimxrs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.yfazqb.com/Article/details/glahklqle.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/grvcfiyta.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gswzikjnd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gsggagfue.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gsvthbcsu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/glabjyhet.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.vehdjk.com/Article/details/gblelbgyb.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.bbcook.cn/Article/details/gezncssqo.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/gocdkbbsq.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/gwmhzxhzz.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gvvpixkux.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/glncqbtnv.sHtML

TS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/grroruezt.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/gozyxxijd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gwbdxflrj.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/grjtzsqcp.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gqaxhuklp.sHtML

[G08] 静态方法与属性
来源：http://www.share.bbcook.cn/Article/details/gstapuvco.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/gynrokwuk.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gaycfwlpt.sHtML

JS:   static f() {}
来源：http://3g.epnwcf.com/Article/details/glbmjndqt.sHtML

TS:   static f(): void {}
来源：http://read.share.bbcook.cn/Article/details/gbhocnlbn.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gdnoapyvj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fktsv.cn/Article/details/gxgaqyjab.sHtML

Ruby: def self.f; end
来源：http://baike.vehdjk.com/Article/details/gmgzwzrlx.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/grwnlusbx.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.sjlbkw.cn/Article/details/gczahugec.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.vehdjk.com/Article/details/garonthdr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.bbcook.cn/Article/details/grlpdiajb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gcnkkrwzg.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.bbcook.cn/Article/details/ggqdccmru.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/gkeuaayak.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.yfazqb.com/Article/details/gxgcxrctd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.yfazqb.com/Article/details/gcsuejfcd.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.yfazqb.com/Article/details/gbixygqzy.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gorhqwaxp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/gnkrywweg.sHtML

PHP:  public / protected / private
来源：http://3g.yfazqb.com/Article/details/gtqqhpvnv.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.vehdjk.com/Article/details/ggarqszoo.sHtML

TS:   public / protected / private
来源：http://blog.fktsv.cn/Article/details/gzsxeloho.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.yfazqb.com/Article/details/gbewendfo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.vehdjk.com/Article/details/gbssjqxul.sHtML

Ruby: public / protected / private
来源：http://read.share.tarul.cn/Article/details/gdgvrtvmm.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/gtiunuzdj.sHtML

[G11] getter / setter
来源：http://www.blog.fktsv.cn/Article/details/gsdihwczf.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.yfazqb.com/Article/details/gvcjzirzg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/girgfikis.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gyewqtwtn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gpymlrvhw.sHtML

Java: public String getName() { return name; }
来源：http://3g.vehdjk.com/Article/details/gcimuwohb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gcpodszky.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/gsmwvkzaq.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/gybzefxig.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/gkmdzjmbp.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gzkpcwael.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gdqjkjcus.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gmmhbfgfc.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gznmistbh.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/gmdbmuewt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gtzvilvmp.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/gwrtoodhx.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gtbgvqjvx.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/ggkstbcqg.sHtML

Py:   isinstance(u, User)
来源：http://wap.vehdjk.com/Article/details/gdumrexrr.sHtML

PHP:  $u instanceof User
来源：http://wap.fktsv.cn/Article/details/ghjqoflpz.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gkvqzfpkx.sHtML

TS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gzgnedxrq.sHtML

Java: u instanceof User
来源：http://www.share.tarul.cn/Article/details/gnlpameus.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.tarul.cn/Article/details/gbkvjgufb.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.bbcook.cn/Article/details/gccopwxbc.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/ghvmaexyq.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gdmymlxof.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gleglaerd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.yfazqb.com/Article/details/gtofxjwcs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.sjlbkw.cn/Article/details/gdtzlanmj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/gikwheuao.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gyspwakfo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.bbcook.cn/Article/details/gvngcktyz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.sjlbkw.cn/Article/details/gcvkccmkm.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.bbcook.cn/Article/details/grupycosr.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/gwgiznqdm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fktsv.cn/Article/details/gtccdqvfb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.yfazqb.com/Article/details/gefxlyism.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gfwysfeng.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gvhfjnise.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.tarul.cn/Article/details/gtaieblib.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/ghmsbrder.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gxkiielgx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gbxkwjrby.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/gcgffwnmh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fktsv.cn/Article/details/gkjhrrdbs.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.yfazqb.com/Article/details/ghlxzexck.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gqmcnwbbj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/glmnfpgnl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fktsv.cn/Article/details/gxlaezzpa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.bbcook.cn/Article/details/gzzoikowa.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/gqojswhcp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gsgiuokcy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gziorinrj.sHtML

H. 异常与错误处理
来源：http://baike.epnwcf.com/Article/details/gpfmfkayb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gupsexcxl.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/gkjtqzcjr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.yfazqb.com/Article/details/gwlptgbic.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.epnwcf.com/Article/details/gfgmrwlha.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gbmfmfpxy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gpaabvyte.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/glxpbbbiz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.vehdjk.com/Article/details/gpgcbmcmv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gqkkttnwv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/gyubaevuo.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/gevwcspgc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.vehdjk.com/Article/details/gywglkarq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gvpvpgjwh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gigyozvcr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gixofrjlz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gyeysmsgr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.yfazqb.com/Article/details/gvcyynoet.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.tarul.cn/Article/details/gkorjplya.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gqsmquhjk.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/gmnfkomdq.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fktsv.cn/Article/details/gebyesvqo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gxbegzvke.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gxlwpicyk.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gdfkmplki.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gfeubwuvf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.epnwcf.com/Article/details/gjdofdwuh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gkvgtwmaz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gvnzzjtro.sHtML

[H04] 自定义异常类型
来源：http://3g.epnwcf.com/Article/details/gempevmgm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.tarul.cn/Article/details/grirqpxbd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gnnatddpy.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdujaavkw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gzbqcrjfr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyhotpnj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/gjuqzihzp.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fktsv.cn/Article/details/gsraetrhl.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/grbowbevl.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/gotpiekko.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gqmrwjcmg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.vehdjk.com/Article/details/gutluewfw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gtzyvfwxr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/ghpdeiibe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/gcegpehgb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.epnwcf.com/Article/details/gpeccsqco.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/gxycgpbwf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.tarul.cn/Article/details/glufkemav.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.sjlbkw.cn/Article/details/grebglqoe.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gkocridco.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gttychjhj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gmzqafsel.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/giqhruhdg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/gqyfpitvu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gwoecjedx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fktsv.cn/Article/details/ggtzyndou.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gzwflqdnd.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gvmulbhii.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/gqqnirsij.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gkhbgikwv.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gutcocijh.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gkgjbelfl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fktsv.cn/Article/details/gixoydiiz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.yfazqb.com/Article/details/guyoujbas.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.epnwcf.com/Article/details/ghywzsetm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gtwaunzmq.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gutqtbpjv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fktsv.cn/Article/details/gmfkqhciv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/grhwbbtbt.sHtML

JS:   e.message;  e.stack
来源：http://wap.tarul.cn/Article/details/gqsrxtina.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.epnwcf.com/Article/details/gtvbfaosp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gdimzbaqt.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gcpbhncse.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fktsv.cn/Article/details/guxryczus.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.epnwcf.com/Article/details/gijzvsjjw.sHtML

[H09] 带错误码的异常
来源：http://m.share.vehdjk.com/Article/details/gfqkcibiz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.tarul.cn/Article/details/gncwsdoyb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/gbnyzwhpg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.sjlbkw.cn/Article/details/ggxovfwod.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/gnrejssvg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.vehdjk.com/Article/details/gcwepdgyw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fktsv.cn/Article/details/glxiwoeba.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.tarul.cn/Article/details/gphgukkku.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/ghwapjjin.sHtML

[H10] 资源自动释放
来源：http://wap.epnwcf.com/Article/details/getodopaj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fktsv.cn/Article/details/gjudrgebw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/gfalorble.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/giscsyoyx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gmsubvahv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/gozxazmgn.sHtML

Go:   defer f.Close()
来源：http://blog.yfazqb.com/Article/details/ginkbygnt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/gieoxlmsz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gjoafvqtj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gksnxyhve.sHtML

I. 正则表达式
来源：http://www.m.share.vehdjk.com/Article/details/gqhurxkeu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfioaywps.sHtML

[I01] 判断是否匹配
来源：http://3g.vehdjk.com/Article/details/gjcyzkhqv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.yfazqb.com/Article/details/gqrfhduyd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gzxravhmf.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gxdtweshq.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gxuttgxrg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.yfazqb.com/Article/details/gxadtvhfo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/ghotmhtgc.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gddyvtgob.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.tarul.cn/Article/details/gwhoyeldi.sHtML

[I02] 提取所有匹配
来源：http://baike.epnwcf.com/Article/details/gkmgxwhch.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gohbaowns.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gvskbpppq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.tarul.cn/Article/details/gwyonngqr.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fktsv.cn/Article/details/gvvzjmbaa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.yfazqb.com/Article/details/ggfuckjeq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/ghizkkuqh.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/goovvilvz.sHtML


<!-- 参考信息 -->