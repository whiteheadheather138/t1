代发 wailian999

Ruby: File.delete("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gzqqqsbqv.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/ggimkoopi.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/gybcifzsi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gmqtudaeo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gajkkuoyu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gvhgcyjoq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/ggjxztfxm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.epnwcf.com/Article/details/gkntwtsaa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.sjlbkw.cn/Article/details/gxmanlvke.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.tarul.cn/Article/details/gwyjcroat.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/gpogqoisx.sHtML

[F08] 遍历目录
来源：http://www.share.sjlbkw.cn/Article/details/gfjwandjo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.epnwcf.com/Article/details/gthveixbs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gogtgtaij.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/glpcxukzg.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/glfdfkqgw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gjbrqxdta.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.vehdjk.com/Article/details/gcpbwbcll.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.tarul.cn/Article/details/ghhktjozw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.vehdjk.com/Article/details/gwmapkqow.sHtML

[F09] 获取文件大小
来源：http://blog.sjlbkw.cn/Article/details/ggebbkjrc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.tarul.cn/Article/details/gmhhzzbxz.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gbhegewbk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gbxrejdpl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gisjxcpdq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gcxooywrp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.bbcook.cn/Article/details/gcomjpege.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gzcqcamcb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gadupnkip.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.bbcook.cn/Article/details/glkmkkvwr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gkpvqtqha.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.epnwcf.com/Article/details/godewsxcx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ggghtahrk.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gyfafprsc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.bbcook.cn/Article/details/gyabmoxkx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gizstewah.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gufomgrus.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gjncdylhb.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gdeqidldi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gumqtisyg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/glqivspux.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gsaufljzw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gvpfavwke.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/goqdchrbx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/geuhzutwu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gokvcxosm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.tarul.cn/Article/details/gojgjykhc.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/gkvjramvc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.bbcook.cn/Article/details/gjtjjvqim.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/geetlnuoh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.epnwcf.com/Article/details/gvdguqmsm.sHtML

TS:   // 同上
来源：http://read.share.epnwcf.com/Article/details/glwdefebr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gulfsxwjq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.tarul.cn/Article/details/gblezoxoh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/grbftutsz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/gvnmipriq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggpdsxspu.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gjmwejldd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gvpvnrkev.sHtML

[G01] 定义类
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlzmeigi.sHtML

Py:   class User: pass
来源：http://blog.yfazqb.com/Article/details/gjmwyevvi.sHtML

PHP:  class User {}
来源：http://baike.fktsv.cn/Article/details/glsnezszl.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gsnmjswwd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gzjkmhrjs.sHtML

Java: class User {}
来源：http://www.blog.epnwcf.com/Article/details/gpcnjkeae.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gvyljjffr.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/glxamdgqx.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gzmpxgyoq.sHtML

[G02] 构造函数
来源：http://baike.bbcook.cn/Article/details/gfzcxmxgu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gbxhlhhpj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gknwegwnn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/ggnsnvfrd.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gtjevxspr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gncrsvcwh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.epnwcf.com/Article/details/ggfyopopc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.yfazqb.com/Article/details/gytfxnrel.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.bbcook.cn/Article/details/gkgnsbuzc.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/gfgjlswyt.sHtML

Py:   self.name = "x"
来源：http://read.share.tarul.cn/Article/details/gvdanlbep.sHtML

PHP:  public string $name = "x";
来源：http://mobile.bbcook.cn/Article/details/grwxhoojo.sHtML

JS:   this.name = "x";
来源：http://blog.tarul.cn/Article/details/giddlwbxg.sHtML

TS:   name: string = "x";
来源：http://www.share.epnwcf.com/Article/details/ggjleitrm.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gsowblvan.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.epnwcf.com/Article/details/gfizqqwci.sHtML

Ruby: @name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/guzitound.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.bbcook.cn/Article/details/gemcabcsz.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gwquinooj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gayezcvtu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gclogqiis.sHtML

JS:   greet() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/grvgwsmik.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gmecdxtxm.sHtML

Java: String greet() { return name; }
来源：http://baike.tarul.cn/Article/details/gjydrcnsq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gzbfjppyb.sHtML

Ruby: def greet; @name; end
来源：http://3g.sjlbkw.cn/Article/details/gjkxelnup.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fktsv.cn/Article/details/gaababzfj.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gvslrpkvl.sHtML

Py:   class Admin(User): pass
来源：http://mobile.epnwcf.com/Article/details/gloskoktb.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/geyovskax.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gbyevajzi.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gfigqxlas.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/geqqlnguk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.vehdjk.com/Article/details/gojkdbwmp.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.vehdjk.com/Article/details/grycuzjiv.sHtML

C#:   class Admin : User {}
来源：http://3g.vehdjk.com/Article/details/gtfbvlcfi.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/ghtiimezy.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.epnwcf.com/Article/details/gbpzweknw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gjopzfjul.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gzakyxtte.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gmnhursxn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/glvqyotjp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/ggykstnes.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gwshidnzj.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/govsqmcrf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fktsv.cn/Article/details/gkexzbaqf.sHtML

Py:   super().greet()
来源：http://www.blog.tarul.cn/Article/details/gkagixpvi.sHtML

PHP:  parent::greet();
来源：http://m.share.sjlbkw.cn/Article/details/gcnguvliw.sHtML

JS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gdxykptja.sHtML

TS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gukkrlybs.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gaqugebli.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fktsv.cn/Article/details/gnuzlrfjw.sHtML

Ruby: super
来源：http://blog.tarul.cn/Article/details/gpakupwhd.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/giukrylgu.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/guacdtmvt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.yfazqb.com/Article/details/gyknsacpt.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/grlidkygf.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/gxeccshcl.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/gcejgaspk.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/gsguhydcb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gdatqbjfr.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gvocbxlgl.sHtML

C#:   public static void F() {}
来源：http://3g.bbcook.cn/Article/details/ghbieesej.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gwavgzvcn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.tarul.cn/Article/details/gldrwikcf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gnprpxmsl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.tarul.cn/Article/details/gbhshvaeu.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fktsv.cn/Article/details/gdibtqnjv.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/gphbobomc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gbtuhrlke.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gbqvkpkoi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gkhurlytp.sHtML

[G10] 访问控制
来源：http://3g.yfazqb.com/Article/details/gciijqbca.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.yfazqb.com/Article/details/gtulhaiyn.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/gfsnvpkum.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.sjlbkw.cn/Article/details/gvwjcjzcl.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/ghvxsuniv.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/grfrxbpbi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.bbcook.cn/Article/details/gpaihgxyt.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/ggykdxqdr.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gokwbfesp.sHtML

[G11] getter / setter
来源：http://read.share.sjlbkw.cn/Article/details/ghfmfhkby.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.sjlbkw.cn/Article/details/gyegzsbgm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gvkjtzgbs.sHtML

JS:   get name() { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gmswufhub.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gyuwtgvga.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/gbijpagod.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gptlmgzyi.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.tarul.cn/Article/details/gjiuvydsd.sHtML

C#:   public string Name { get; set; }
来源：http://wap.vehdjk.com/Article/details/gajshsaqr.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/gwdwenifi.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.vehdjk.com/Article/details/grdwjhwhh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gkgbbvmno.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdrlvzhw.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gavcxesvq.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/gucfcehpe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/grxacywyx.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.yfazqb.com/Article/details/gpplfunmx.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/gmmcjuliz.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gdnjtnbjt.sHtML

Py:   isinstance(u, User)
来源：http://m.share.sjlbkw.cn/Article/details/ghkznomts.sHtML

PHP:  $u instanceof User
来源：http://www.share.tarul.cn/Article/details/gtmbilzbd.sHtML

JS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gzczigznt.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gosmlracf.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gixirtqej.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.yfazqb.com/Article/details/ghptobyzv.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/gcqnnfvta.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gnfjzxidm.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/gzxisqzfi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/gefweybhi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/gxberzjwj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fktsv.cn/Article/details/gudbadyyv.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gpqtkqrru.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvyfhsues.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gdlnyqhrv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/gabhumpax.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.tarul.cn/Article/details/gwaqqibdu.sHtML

[G15] 枚举
来源：http://www.m.share.bbcook.cn/Article/details/gzrclnula.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.tarul.cn/Article/details/gigclhwxw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.epnwcf.com/Article/details/gjcaapver.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.bbcook.cn/Article/details/gqvrbqejf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gzkqlgprq.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.bbcook.cn/Article/details/gsikfhexs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.yfazqb.com/Article/details/gidumfuqu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.tarul.cn/Article/details/gtntywwlw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gazuhqyyu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.epnwcf.com/Article/details/gznesakpx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.tarul.cn/Article/details/gykdvyehx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/ghyvlhneo.sHtML

JS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/gxnoxtyxw.sHtML

TS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gkeuihzlk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gkkpzvmak.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.bbcook.cn/Article/details/gksyxxrrk.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.epnwcf.com/Article/details/gvugpwnhd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/ggtpaysoi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxygukusg.sHtML

H. 异常与错误处理
来源：http://blog.vehdjk.com/Article/details/gcqmyqyrv.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gksitfvnv.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gtnbypwsi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/gkucaiajz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fktsv.cn/Article/details/gesrmpwvi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gbtdofgns.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gwembmqnl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/genaktbiv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.epnwcf.com/Article/details/gktetpixm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/gvvsslolo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.yfazqb.com/Article/details/gnxikjoxk.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fktsv.cn/Article/details/gdavfesja.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.bbcook.cn/Article/details/ggownpelw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gjcablxel.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gqfwmlitf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjszgdhry.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gpzrnqexm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/grjhrpbby.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gflwdhlrs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gqnrortmz.sHtML

[H03] 主动抛出异常
来源：http://m.share.vehdjk.com/Article/details/gmqujgvwj.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/gsdnffvhz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gwtnctwsu.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gffspscxm.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/ggfunszpl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/ggmumosch.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/ghnskthvr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/ginkepsjv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/ggmrzbabj.sHtML

[H04] 自定义异常类型
来源：http://wap.epnwcf.com/Article/details/gjnabfwpa.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.vehdjk.com/Article/details/gxwvafbls.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gurezalmy.sHtML

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gaeufslkc.sHtML

TS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gyjowehfp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/glslpjnok.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.tarul.cn/Article/details/gnupxhpha.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.sjlbkw.cn/Article/details/gncbgerfs.sHtML

C#:   class MyException : Exception {}
来源：http://wap.sjlbkw.cn/Article/details/gtvqpdtcf.sHtML

[H05] 捕获特定类型
来源：http://wap.vehdjk.com/Article/details/ggkdzusmn.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/gllgkckgw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.sjlbkw.cn/Article/details/gpfnhwixw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gzbrvlzit.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gljqtgiyg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.yfazqb.com/Article/details/gamqvuwtk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gbcqrdzat.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.vehdjk.com/Article/details/gbvtfgejq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.sjlbkw.cn/Article/details/gevugeztu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.tarul.cn/Article/details/glhzqvmri.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.sjlbkw.cn/Article/details/gylhmcbic.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gqvvynyal.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gjqesdqxd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gyexsjycy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.yfazqb.com/Article/details/glkisijpq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.bbcook.cn/Article/details/gphpcrzhs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.yfazqb.com/Article/details/gotsbdkaz.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.epnwcf.com/Article/details/gjlkasxtg.sHtML

[H07] 断言
来源：http://blog.tarul.cn/Article/details/gxswdgior.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.yfazqb.com/Article/details/gfjuaxtkf.sHtML

PHP:  assert($x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gszlnpwfs.sHtML

JS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gbxnqvnkj.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gmmprwdhx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.epnwcf.com/Article/details/gvnuqhogg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.bbcook.cn/Article/details/glgwwcyjq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.vehdjk.com/Article/details/gqoorqxss.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gkaqgxpgl.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/giqniqkdt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.epnwcf.com/Article/details/giohrfeum.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/gjkqdkxrt.sHtML

JS:   e.message;  e.stack
来源：http://m.share.tarul.cn/Article/details/gdcbdjczp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.sjlbkw.cn/Article/details/gknfdyqro.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gszhxifik.sHtML

Go:   err.Error()
来源：http://baike.fktsv.cn/Article/details/gqealoojm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/glzfdsasm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.sjlbkw.cn/Article/details/gprjnpbco.sHtML

[H09] 带错误码的异常
来源：http://wap.tarul.cn/Article/details/gpisswnvz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.yfazqb.com/Article/details/gjpoutcwc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.tarul.cn/Article/details/gboowrvhd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.epnwcf.com/Article/details/gddwbsqxz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.yfazqb.com/Article/details/goagpkcaz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.yfazqb.com/Article/details/gspozopts.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gwzokdvlf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.sjlbkw.cn/Article/details/gumjkffuk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.bbcook.cn/Article/details/gcmxxxoii.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/gjdqcgewh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.epnwcf.com/Article/details/gbbpsnume.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.epnwcf.com/Article/details/gesrpvjhq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/glsfobprq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/grqpaeyia.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/gzqwazppv.sHtML

Go:   defer f.Close()
来源：http://read.share.vehdjk.com/Article/details/gsqpgazqf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.epnwcf.com/Article/details/goxzrrddh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gvcuoapmd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/giehkjalg.sHtML

I. 正则表达式
来源：http://www.share.sjlbkw.cn/Article/details/giegqcxfq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcgpbruvx.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/gbbdixhyn.sHtML


<!-- 参考信息 -->