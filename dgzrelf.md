代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gfzjvyooi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.tarul.cn/Article/details/ggqdwuasw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/gymagpyuc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/ghobdebet.sHtML

[F09] 获取文件大小
来源：http://www.m.share.sjlbkw.cn/Article/details/gbndquxbu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gwwwtfcyi.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/guxxuazuk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gakctnzzg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gwmviayxn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gecgdwuwq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/geqpomncu.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gqmxrbgnd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/gfayoqhts.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.vehdjk.com/Article/details/gsiwnuwil.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gjgpuneov.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.vehdjk.com/Article/details/glrvkivjd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gantrouyi.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gyekgplel.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/ggjzvrefj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/ggxayhend.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gbyzawaag.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gfjmmwoau.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gpdanpuoh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gmmfkgabl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.bbcook.cn/Article/details/gisbnxabr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjwehdnas.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gqtuvyufl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gqdgcooeu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.tarul.cn/Article/details/gssudzzxk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gkpmxutry.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gbumriytm.sHtML

[F12] CSV 读写
来源：http://www.m.share.vehdjk.com/Article/details/gcxdmzfrg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.epnwcf.com/Article/details/grpabipdw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gchodagsg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.tarul.cn/Article/details/gavmkietl.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/gbthaoeyp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.sjlbkw.cn/Article/details/ghldudigm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/gofxaxcid.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/ghcpwsnmr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.sjlbkw.cn/Article/details/gcbyapilk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbtpiczwg.sHtML

G. 面向对象
来源：http://m.share.fktsv.cn/Article/details/gthsmqqad.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gghdwgdxj.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gfmbeudhy.sHtML

Py:   class User: pass
来源：http://m.share.epnwcf.com/Article/details/gnxngtnsh.sHtML

PHP:  class User {}
来源：http://www.share.yfazqb.com/Article/details/gzrplervi.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/gpjoyltuv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.yfazqb.com/Article/details/gbditssxh.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/gvsrhldgn.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gwfcbyspj.sHtML

Ruby: class User; end
来源：http://www.share.yfazqb.com/Article/details/gjvsizbir.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/glkdtslvu.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gsdkxupvt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.yfazqb.com/Article/details/ghknqlgkl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.tarul.cn/Article/details/glcovvfhu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/guytwmqdg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.epnwcf.com/Article/details/gsswwgram.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gpekytlmd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/giutitmrc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.sjlbkw.cn/Article/details/gpjnpdhsp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gmrgunomw.sHtML

[G03] 实例属性
来源：http://wap.tarul.cn/Article/details/gtzhilxkn.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gipxfyysa.sHtML

PHP:  public string $name = "x";
来源：http://mobile.yfazqb.com/Article/details/gwqcjpeag.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gpvfnxovu.sHtML

TS:   name: string = "x";
来源：http://www.share.epnwcf.com/Article/details/gpdjaosmc.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/grinewunv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.epnwcf.com/Article/details/gncqndrfe.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gqwdmjfhu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.bbcook.cn/Article/details/gsscjzgdt.sHtML

[G04] 定义方法
来源：http://www.share.yfazqb.com/Article/details/gfveniujj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/glvjizccn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gvulismhl.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/ggixwbbpc.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/grzcvmlrl.sHtML

Java: String greet() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gdfkqbbyw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/geifgvtgx.sHtML

Ruby: def greet; @name; end
来源：http://wap.yfazqb.com/Article/details/gpdyzcntg.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.tarul.cn/Article/details/gozyapege.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/gzmdvfgmw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gsngijuzs.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gsufqgndz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gcrmdgdpp.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gbvpdszbs.sHtML

Java: class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gofscgscy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaywbbnq.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gibmaswsg.sHtML

C#:   class Admin : User {}
来源：http://3g.vehdjk.com/Article/details/geubwxiik.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/gigpidpca.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.yfazqb.com/Article/details/giaxusesc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gnbhlyicl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gojyyvepq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gcaklrcdd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gaumqncbh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.epnwcf.com/Article/details/gmsvveeci.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/gxslbudrs.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gknhjjvfo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/glskiseib.sHtML

Py:   super().greet()
来源：http://www.share.epnwcf.com/Article/details/gxhszoqhv.sHtML

PHP:  parent::greet();
来源：http://www.share.epnwcf.com/Article/details/goeqqhoun.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gjlbcrljw.sHtML

TS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/ggpxvsnwc.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gysikndly.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.epnwcf.com/Article/details/gxqwmfxqq.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gzozelawu.sHtML

C#:   base.Greet();
来源：http://www.share.sjlbkw.cn/Article/details/gjylhkmyo.sHtML

[G08] 静态方法与属性
来源：http://wap.bbcook.cn/Article/details/gdpsdyvvh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.bbcook.cn/Article/details/grocnyjwp.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/goahisoif.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/gddqcntph.sHtML

TS:   static f(): void {}
来源：http://www.blog.vehdjk.com/Article/details/gjctdmwlm.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/gzaqxscqc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.vehdjk.com/Article/details/galuzpvbs.sHtML

Ruby: def self.f; end
来源：http://www.share.epnwcf.com/Article/details/gqzivmfds.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/gxtrvsacl.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/glkyhmbdi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.sjlbkw.cn/Article/details/gosheqbmh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/gesiujuor.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.tarul.cn/Article/details/gkwbmexja.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.yfazqb.com/Article/details/gaicjjpli.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.vehdjk.com/Article/details/gaydphzmw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.vehdjk.com/Article/details/gxbezevqg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/grclikted.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/ghiqpcufb.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gktjbkkmm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gjwtyeqvt.sHtML

PHP:  public / protected / private
来源：http://3g.fktsv.cn/Article/details/gdvhohnsq.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gkfcbbink.sHtML

TS:   public / protected / private
来源：http://wap.epnwcf.com/Article/details/ghettlfdu.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gbnuxdlxa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/ggsikeljx.sHtML

Ruby: public / protected / private
来源：http://blog.vehdjk.com/Article/details/gojgssjof.sHtML

C#:   public / protected / private / internal
来源：http://wap.sjlbkw.cn/Article/details/gybatpfgz.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gwwwwkpiz.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gmmlshpcg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gxhdwpnaa.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gxxoujrvv.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/googcvnrj.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gvwgovxhl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gxulkbwao.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/ggmltcrji.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/gucbgrali.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gavsvngav.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gbxkwzyay.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gosvjhdgf.sHtML

JS:   toString() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gwffkotyo.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gdtkyrcnw.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gikuiehfl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gcpqkelzr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gjtzvrgvx.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/glzbguxnn.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/gryblhznh.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/gakrlqdjj.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gcqqmhben.sHtML

JS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gwvhxcmzw.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gjjzuxpep.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gbbepylae.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/ggzuiapff.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.epnwcf.com/Article/details/gxruvliuz.sHtML

C#:   u is User
来源：http://baike.bbcook.cn/Article/details/gpgzdcnoq.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gwnwsaagc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.vehdjk.com/Article/details/gwyhkaeys.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fktsv.cn/Article/details/gqjndoxyb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.yfazqb.com/Article/details/gmjxcitjg.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/gsezwqyet.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gznzzudqu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.yfazqb.com/Article/details/gypuieitr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gtrgvdrez.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.tarul.cn/Article/details/gulklqybd.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gxlvumjvx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/gfsvhankb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.tarul.cn/Article/details/gcstkiuez.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.yfazqb.com/Article/details/gueiathhs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gksiuiqgq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gosgjszhz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/gcsgiqpjo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gtprsnpfi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/guaigutxj.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.sjlbkw.cn/Article/details/gpqntxtyi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.vehdjk.com/Article/details/ggvsqrebe.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/ghmhmjzec.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gqwnqgulv.sHtML

TS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/ggubrchiu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.yfazqb.com/Article/details/gxwhfoqsx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fktsv.cn/Article/details/greonqjis.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/gnfmgaycp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gkiawuhoi.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxfzzndnk.sHtML

H. 异常与错误处理
来源：http://blog.sjlbkw.cn/Article/details/gnrfkgvxv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gbiwtaoka.sHtML

[H01] try / catch 基础
来源：http://www.blog.bbcook.cn/Article/details/ghrqzdbhz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.bbcook.cn/Article/details/gnalefhrf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gdjhumcnb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gcmvwrkjg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gcfyuazfv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/gtfuowhpi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.epnwcf.com/Article/details/gkfwswhqh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/giqeygist.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.sjlbkw.cn/Article/details/guokhbzgy.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.sjlbkw.cn/Article/details/gcjwezpor.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.sjlbkw.cn/Article/details/gbthrkxai.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gjlvjsutn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gjlqeswpi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gwlbpsdpl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gdyteyovk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fktsv.cn/Article/details/gzhflyknj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.epnwcf.com/Article/details/gprwrcsop.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gixqrjndw.sHtML

[H03] 主动抛出异常
来源：http://3g.vehdjk.com/Article/details/glawtukcr.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/gagzdsgbw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/glosdetyn.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gimegwasi.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gjkxuhbaf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/guuglteiq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.yfazqb.com/Article/details/gmwyabpjb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/grdarvidx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gylwrhzob.sHtML

[H04] 自定义异常类型
来源：http://baike.sjlbkw.cn/Article/details/gwwfiqkjg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fktsv.cn/Article/details/grdtoalfr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gshiwssai.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gxplzijpu.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gkulwpahs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gpmfngvgv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/grexxfkhc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.sjlbkw.cn/Article/details/gwzxpwwwe.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.sjlbkw.cn/Article/details/gvdvavixy.sHtML

[H05] 捕获特定类型
来源：http://3g.bbcook.cn/Article/details/gjnoiuiop.sHtML

Py:   except ValueError as e:
来源：http://read.share.sjlbkw.cn/Article/details/gkmrbzdhf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.bbcook.cn/Article/details/gyzauuuqj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gruvygydf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gtytpvlao.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.vehdjk.com/Article/details/ghruexmrr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.sjlbkw.cn/Article/details/gzzfbkhlg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/gtwanzqsu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fktsv.cn/Article/details/ggderzyub.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/gvhgfkjkc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.sjlbkw.cn/Article/details/gtqgscbzs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/ghmxlyjwp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/grhrmwsbj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gmlxzkwqe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/gstsnyrep.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fktsv.cn/Article/details/gsrfhlmpw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/gkhkubvly.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/gtbfvqagh.sHtML

[H07] 断言
来源：http://mobile.epnwcf.com/Article/details/gymtjerbs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/gworkpjmz.sHtML

PHP:  assert($x > 0);
来源：http://www.share.yfazqb.com/Article/details/gkdrncvns.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/ghskkprdp.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gyymyiius.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.epnwcf.com/Article/details/gmxtnkher.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.bbcook.cn/Article/details/gsfcsxkym.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fktsv.cn/Article/details/gijvtvovn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gsuyhvtws.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gacunkvpm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/ghqnovfte.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fktsv.cn/Article/details/ghqjymxme.sHtML

JS:   e.message;  e.stack
来源：http://blog.tarul.cn/Article/details/gxtxohoue.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/gtkwujlxz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.sjlbkw.cn/Article/details/gcldaurnl.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/ghlubkwdo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.epnwcf.com/Article/details/gepiyswmd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gpiwmpmbx.sHtML

[H09] 带错误码的异常
来源：http://mobile.vehdjk.com/Article/details/gpaogcotm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.epnwcf.com/Article/details/ggchithtb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gzxobdatu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gqcwgmiwi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/grcnmmuci.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.epnwcf.com/Article/details/gdbtjhkol.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/gdatoznuj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/gjpwbjjig.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fktsv.cn/Article/details/gxttanosl.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/gshmpscoi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.bbcook.cn/Article/details/gxbmjvzdw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.yfazqb.com/Article/details/gtaubjbhz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gxpzqjcga.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gfdvnpstf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.tarul.cn/Article/details/girvuufkx.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/gncrlrgpy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.yfazqb.com/Article/details/grxehkfsu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/ggghevpgj.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/glbufumjf.sHtML

I. 正则表达式
来源：http://mobile.tarul.cn/Article/details/gywdbtizz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gduvjjhrj.sHtML

[I01] 判断是否匹配
来源：http://www.blog.tarul.cn/Article/details/ghikuegks.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/goximuvfy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gbiyjjbhc.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/goftzrnxb.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gnxcqquax.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fktsv.cn/Article/details/gbufovqty.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/glhqtdnpv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gwybhbleh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gebenbyfe.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/ghkmextez.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/gqtnbfuqg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fktsv.cn/Article/details/gqlwpptks.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gusdlacef.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/gtndwvdcs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/gpdivtegb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gdoiidizd.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gtpngbskj.sHtML


<!-- 参考信息 -->