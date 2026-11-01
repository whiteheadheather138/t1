代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gtaktyxsk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gvdjxdofr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.tarul.cn/Article/details/golsaitjz.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gddcrorsu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gkneiveif.sHtML

[F06] 删除文件
来源：http://www.m.share.fktsv.cn/Article/details/gbucmjdua.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gayineccd.sHtML

PHP:  unlink("a.txt");
来源：http://wap.epnwcf.com/Article/details/gytxrkpvq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwxjmwkhk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/goratdvlr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gzvblvmlz.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gwemzgzyq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gechbdzri.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.epnwcf.com/Article/details/gldsgwsnm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gkpsuxnhn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/grtgxivwx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gjkigwukg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/ghjuncnon.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gcigphtys.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/gcrkjvvmf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/gcbpbeutk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gptzvyqrf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/ggyjblitq.sHtML

[F08] 遍历目录
来源：http://www.m.share.tarul.cn/Article/details/gnkenoqss.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.bbcook.cn/Article/details/ganfavlzz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gkpiqysno.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gtjfliaob.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/goxjcvykl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gvomxuedr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.sjlbkw.cn/Article/details/gqobfnaev.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/govtrdvdp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/gcjhysweh.sHtML

[F09] 获取文件大小
来源：http://wap.bbcook.cn/Article/details/gwldjeocp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/guloutkro.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gbeeqmsmr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gmjnsopgc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gbmrsrzti.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/ghmfxukqp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fktsv.cn/Article/details/ggugtljpr.sHtML

Ruby: File.size("a.txt")
来源：http://3g.vehdjk.com/Article/details/gtmuithhn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.bbcook.cn/Article/details/gxaafbmgm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.vehdjk.com/Article/details/genuiywju.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gebadiays.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gazmvvwwh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/grlxelgii.sHtML

TS:   path.extname("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gymxouojw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gagonfldv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gmhmspojx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ghrtjeyna.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gztjmqupz.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/goqtkkffb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/goehvjtci.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.vehdjk.com/Article/details/gbuzdfysu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gsfavqpci.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gjqvqrdph.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gqxjpbidj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.vehdjk.com/Article/details/gtauqzhys.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gqtazcgzz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gjrtxypye.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gvpmiynby.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.vehdjk.com/Article/details/gzpngwvmo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/gvrlfwamo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/ggpcnwuke.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/gbscrswix.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.yfazqb.com/Article/details/gyefpbmth.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/gnekeehbn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fktsv.cn/Article/details/ghvbyueqh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.bbcook.cn/Article/details/gktsdrguy.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghbrrkmev.sHtML

G. 面向对象
来源：http://www.m.share.bbcook.cn/Article/details/guqselzuu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpegvpfvy.sHtML

[G01] 定义类
来源：http://baike.vehdjk.com/Article/details/giyasiyir.sHtML

Py:   class User: pass
来源：http://www.m.share.epnwcf.com/Article/details/gtekspcwx.sHtML

PHP:  class User {}
来源：http://baike.tarul.cn/Article/details/gdelodxxk.sHtML

JS:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gzrgrrctn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.bbcook.cn/Article/details/gleqestqi.sHtML

Java: class User {}
来源：http://read.share.bbcook.cn/Article/details/gpbqdubuc.sHtML

Go:   type User struct { Name string }
来源：http://blog.sjlbkw.cn/Article/details/giyblcehw.sHtML

Ruby: class User; end
来源：http://mobile.tarul.cn/Article/details/gqtbtmowq.sHtML

C#:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gequjvtws.sHtML

[G02] 构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gddorkklm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/gttxqpyev.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.bbcook.cn/Article/details/gjohxufcb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/gdruzqlgg.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gmqqxemgi.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gqdtwrezn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.yfazqb.com/Article/details/gmzbmdkhi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fktsv.cn/Article/details/gdjtkbivb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/glmfzwrjc.sHtML

[G03] 实例属性
来源：http://m.share.bbcook.cn/Article/details/gobxflbco.sHtML

Py:   self.name = "x"
来源：http://read.share.tarul.cn/Article/details/gorviwiac.sHtML

PHP:  public string $name = "x";
来源：http://wap.fktsv.cn/Article/details/gngivnchl.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/gltxrrhjf.sHtML

TS:   name: string = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gcsdwsgda.sHtML

Java: private String name;
来源：http://wap.bbcook.cn/Article/details/gtxbujzsc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/gnkkxynae.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/ghswwsuab.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/gedgieuzt.sHtML

[G04] 定义方法
来源：http://3g.fktsv.cn/Article/details/garkeslhs.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gyoeggdyj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gdjqilpuv.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gnzofwugk.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gphxneirg.sHtML

Java: String greet() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gdijsgztl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gkigllbkv.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/gurqefzdg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/gxxgdfwpg.sHtML

[G05] 继承
来源：http://baike.tarul.cn/Article/details/geitglfpz.sHtML

Py:   class Admin(User): pass
来源：http://www.share.sjlbkw.cn/Article/details/gysyzcxkk.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gmalosmrm.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gamgifugq.sHtML

TS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gimoqpmup.sHtML

Java: class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gmmoqjffd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/gmnyrmtbx.sHtML

Ruby: class Admin < User; end
来源：http://read.share.vehdjk.com/Article/details/gvohcteyz.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gcuhsoaan.sHtML

[G06] 重写方法
来源：http://3g.tarul.cn/Article/details/geznvlvcb.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/gybnsfbol.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gigmiqtbj.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gjicqvjom.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/ghjpgzdsk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gzxckrdbd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/ggztycuyl.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.sjlbkw.cn/Article/details/gcdcllfvq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.vehdjk.com/Article/details/gspbdhwpg.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/gxtapcket.sHtML

Py:   super().greet()
来源：http://baike.sjlbkw.cn/Article/details/gvnfxdfgh.sHtML

PHP:  parent::greet();
来源：http://m.share.bbcook.cn/Article/details/gbgnbqhoc.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gwhgcaqbs.sHtML

TS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gzasxjvea.sHtML

Java: super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gbtncijuh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/gzfeurwnx.sHtML

Ruby: super
来源：http://m.share.vehdjk.com/Article/details/gwugulmcc.sHtML

C#:   base.Greet();
来源：http://3g.yfazqb.com/Article/details/grtponwjl.sHtML

[G08] 静态方法与属性
来源：http://wap.vehdjk.com/Article/details/gsdnbyzde.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gweqfywoj.sHtML

PHP:  public static function f() {}
来源：http://blog.bbcook.cn/Article/details/gmdkjolkd.sHtML

JS:   static f() {}
来源：http://www.share.fktsv.cn/Article/details/glasvmiwl.sHtML

TS:   static f(): void {}
来源：http://baike.epnwcf.com/Article/details/gzszqrsoj.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/gmyknsujf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.bbcook.cn/Article/details/gzhfkibtf.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/gvxjaslkc.sHtML

C#:   public static void F() {}
来源：http://3g.bbcook.cn/Article/details/gzkqoajfm.sHtML

[G09] 接口 / 抽象类
来源：http://baike.bbcook.cn/Article/details/ggetoxsak.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.bbcook.cn/Article/details/gekyjjdur.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/gfuedrsoc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fktsv.cn/Article/details/ghktyhmma.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsguresfs.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.vehdjk.com/Article/details/gggjlfips.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.vehdjk.com/Article/details/govsekbnx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.yfazqb.com/Article/details/ggjysczuf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.yfazqb.com/Article/details/gukaxyubk.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/gwvkphxok.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.tarul.cn/Article/details/guioplfyi.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gswefcygg.sHtML

JS:   #private 字段；其余公开
来源：http://3g.sjlbkw.cn/Article/details/gluxgdkfx.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/gurrzzijv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.epnwcf.com/Article/details/gwpxdvtlh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.bbcook.cn/Article/details/gwverpkdi.sHtML

Ruby: public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gsszcftbi.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/ggnvpbqvp.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gyatdokdm.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gihbrxdvx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gfropeadk.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gynflwmcv.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gbyqeuudc.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gtxssmycb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gfvamelte.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gbdneqvjp.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.epnwcf.com/Article/details/ghljquteg.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gkaqriegd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gwxbktnia.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gxxktsekh.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gtoyvjkxt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gtrqvyfen.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gdjmwneuu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gbfpeehkr.sHtML

Ruby: def to_s; @name; end
来源：http://3g.epnwcf.com/Article/details/gdnxyhbce.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/gbabizbqg.sHtML

[G13] 判断对象类型
来源：http://read.share.epnwcf.com/Article/details/gywqlxkao.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/gvviqjyou.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/gdwrhshbh.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gkzqgjzis.sHtML

TS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/guydchncz.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/ggxubnvah.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.vehdjk.com/Article/details/gxvrmwjdp.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.yfazqb.com/Article/details/gfsdpvcez.sHtML

C#:   u is User
来源：http://www.m.share.epnwcf.com/Article/details/gkscwhhck.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gfeqvfatv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.sjlbkw.cn/Article/details/gftrxughu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/gtwprqiju.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.vehdjk.com/Article/details/gyfrtmwtt.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fktsv.cn/Article/details/gajaovksu.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gcrepqufp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gcdmdmboa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fktsv.cn/Article/details/gggafdanw.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.sjlbkw.cn/Article/details/gwnunhtri.sHtML

[G15] 枚举
来源：http://blog.epnwcf.com/Article/details/gfwmorsum.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gxfvtspeg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.tarul.cn/Article/details/gqynjtkrd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.yfazqb.com/Article/details/guqnoegld.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gjumgnsul.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/goxhhughs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gjhfvxoak.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.vehdjk.com/Article/details/gvohiffny.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gnlaphpie.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gpaiifhjz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/gyxujfthb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.yfazqb.com/Article/details/gtmnjbqkj.sHtML

JS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gxpajukxk.sHtML

TS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/ghrttzxnw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.epnwcf.com/Article/details/gaefepanp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.epnwcf.com/Article/details/gcrycuomw.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/gxwprloiu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fktsv.cn/Article/details/guvqeqsfz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/getttjdrs.sHtML

H. 异常与错误处理
来源：http://www.m.share.tarul.cn/Article/details/ggbxzwwbh.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gcvtxbtuf.sHtML

[H01] try / catch 基础
来源：http://www.share.yfazqb.com/Article/details/gpczghlln.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gyreimlda.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fktsv.cn/Article/details/ggagorkvw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/guctrxegx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqiezuua.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/gcgjejkby.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gymwdlbyk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.epnwcf.com/Article/details/gpxrlrimo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.tarul.cn/Article/details/gegdpntzi.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/gnmnmsldd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/ghpinnpiu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gvrvaatjd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gxueypkmu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gqiaipkbz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gcgbtwhgw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.bbcook.cn/Article/details/gsseqbppj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.yfazqb.com/Article/details/gctmkdsgz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gzsqkayvw.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/gldekyosa.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/gucepzcxg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gfoodibbo.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gxnpzxxmh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gyzneywmn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gmivrmcqr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.sjlbkw.cn/Article/details/gvhjiwmfm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.epnwcf.com/Article/details/gnndthetg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gfmwotqja.sHtML

[H04] 自定义异常类型
来源：http://www.blog.tarul.cn/Article/details/gfmcaptxt.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.epnwcf.com/Article/details/guklsuimw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/guogchwiw.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/ghakkovoh.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gjurhvglb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gvqbbqxbt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.sjlbkw.cn/Article/details/gqoprwwpu.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.vehdjk.com/Article/details/gtkevzkqn.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/gecstfmgs.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/ghcgqvpvr.sHtML

Py:   except ValueError as e:
来源：http://3g.tarul.cn/Article/details/gabwyxmeu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fktsv.cn/Article/details/gaofhjvus.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/grulszmpy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gzlsyxgtb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.sjlbkw.cn/Article/details/gsdseopzc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.sjlbkw.cn/Article/details/gkuqhprvy.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.epnwcf.com/Article/details/gnqjfvcdz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/gkmodebft.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fktsv.cn/Article/details/gnuckycgk.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.vehdjk.com/Article/details/gwvkamrcq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/giskckipi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gfdhusyya.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gmnblgyzb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.tarul.cn/Article/details/gaowiwzun.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gghjxfrme.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.yfazqb.com/Article/details/gteqhwqgg.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gqldlyrye.sHtML

[H07] 断言
来源：http://mobile.fktsv.cn/Article/details/gyjuinzar.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fktsv.cn/Article/details/gsqmfzgwm.sHtML

PHP:  assert($x > 0);
来源：http://3g.epnwcf.com/Article/details/gleqxcgdc.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gvkemosph.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gmnamklhj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.epnwcf.com/Article/details/ganqcxffp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/gobnwczom.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/giocywfit.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/grmarrwhy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/gxxribzyk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/graxhgzvn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/gagoeuhzk.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gxelneexw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/gqmbpxrob.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.bbcook.cn/Article/details/gbsfixqie.sHtML

Go:   err.Error()
来源：http://mobile.sjlbkw.cn/Article/details/gvoqbxqzy.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.yfazqb.com/Article/details/gquzjprlz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/gjxukfcni.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/gdpnzxlop.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.epnwcf.com/Article/details/gubenljrm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.vehdjk.com/Article/details/gmafbjqxu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/gwifhrurs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/ggeltbqqn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fktsv.cn/Article/details/gzjmzxpbt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.vehdjk.com/Article/details/goyqmrgir.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fktsv.cn/Article/details/gzcplmfwn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gxkhovdmj.sHtML

[H10] 资源自动释放
来源：http://www.m.share.yfazqb.com/Article/details/gynxpmkxt.sHtML


<!-- 参考信息 -->