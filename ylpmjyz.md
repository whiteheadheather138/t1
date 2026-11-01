代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gyusuwkkc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gumhjphbd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gssqjgood.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gwgfkbdus.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gcvvzxxfh.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gkkkvbxlm.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gbhhuxkxa.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gfuvokola.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gcfjuuekb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gfqnojbij.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gggdbsdum.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gphlyxdss.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.tarul.cn/Article/details/ghbmuuyef.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.tarul.cn/Article/details/gsiycseya.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/grjzrcoek.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.yfazqb.com/Article/details/gnmieamcz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gkjiapbvc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/ggngwpbji.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gjgxqgljr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gldeubttx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.sjlbkw.cn/Article/details/gieekftiz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gzsccwbqc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gxoypjcux.sHtML

[F08] 遍历目录
来源：http://m.share.sjlbkw.cn/Article/details/gegfrxkie.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.epnwcf.com/Article/details/glqgohrcw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.sjlbkw.cn/Article/details/groleswqi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gozsqdayi.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/glykarsck.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/ghycycssl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.tarul.cn/Article/details/gnurmkqyr.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fktsv.cn/Article/details/gzjljoaxq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gqetdaodw.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gmkjchvsh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/gkrkytchk.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.epnwcf.com/Article/details/grylzogyc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gcgeapaqg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gcsuwexbe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/goejjnlhc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.vehdjk.com/Article/details/gbednumpy.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/grduusdjq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.epnwcf.com/Article/details/gcdgverds.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.yfazqb.com/Article/details/gcobwkluw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gnxsozcvp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/ghntygghb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gvvdhplxw.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gbumeoxmm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fktsv.cn/Article/details/gfqxyezbr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gtmknzufd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gpmdrnfpw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gokpgehwk.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gylekyfia.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gffdkodom.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.sjlbkw.cn/Article/details/gaxpezdwb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gxsjtjfsl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/geabvsuzm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/glgoeuhgf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.yfazqb.com/Article/details/gjfsuzpba.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/ghvpfsfvt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.sjlbkw.cn/Article/details/gwkkbqkfq.sHtML

[F12] CSV 读写
来源：http://blog.yfazqb.com/Article/details/gdmjrviec.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/gefpbtesv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.vehdjk.com/Article/details/gosxqyhop.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/gcannqooc.sHtML

TS:   // 同上
来源：http://blog.yfazqb.com/Article/details/glvcklavw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.vehdjk.com/Article/details/gvgtnfewj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.tarul.cn/Article/details/geyuadvts.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gvjdwfpnn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/gpjgbkrhu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvlmzdpar.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/gghkwbphg.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsarjrnzq.sHtML

[G01] 定义类
来源：http://blog.tarul.cn/Article/details/goatjorwz.sHtML

Py:   class User: pass
来源：http://m.share.sjlbkw.cn/Article/details/geltljdbd.sHtML

PHP:  class User {}
来源：http://wap.yfazqb.com/Article/details/gtqwvcjel.sHtML

JS:   class User {}
来源：http://blog.vehdjk.com/Article/details/gkrlvsfnp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/glmsiotgf.sHtML

Java: class User {}
来源：http://mobile.fktsv.cn/Article/details/gdpqnqllx.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/gsdljdyhk.sHtML

Ruby: class User; end
来源：http://www.m.share.yfazqb.com/Article/details/gfjytoapi.sHtML

C#:   class User {}
来源：http://wap.epnwcf.com/Article/details/gechtvdhi.sHtML

[G02] 构造函数
来源：http://mobile.tarul.cn/Article/details/gdehhtmzm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fktsv.cn/Article/details/glpvfefwh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gsceqriwy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gazmfkhff.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/gizfhqcku.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/ggrfweooj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gxshbszsa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/gdjvthvbf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gmpjsjzof.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/gnexwxmre.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/gwxyxoswz.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/ghgcufvzz.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/gioyoirex.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/gsrxbzroc.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gczgzmaai.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/guvrwxzmv.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gbajayhmr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.yfazqb.com/Article/details/gsczrfckj.sHtML

[G04] 定义方法
来源：http://baike.bbcook.cn/Article/details/gupctevwn.sHtML

Py:   def greet(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gwhaofinw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gpatyicnj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/ggraknotg.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gurtlaszb.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gtdfjpbue.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gynpqnawd.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gyrxbtfmx.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gahnwegzn.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gipjgddkw.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/gupxkkcff.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gqfuzstgk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gopbnetmf.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/geqczxvwo.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gyvcgsojv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/gnwlxmbln.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gtxokkjsz.sHtML

C#:   class Admin : User {}
来源：http://read.share.sjlbkw.cn/Article/details/gidnrwuia.sHtML

[G06] 重写方法
来源：http://www.blog.bbcook.cn/Article/details/gchaxqmis.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/gqnrdtopo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gfbjscpod.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gttdtuddz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gkzvnbbme.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gtfbolusk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gvtdjfszd.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.yfazqb.com/Article/details/gnvyrcpow.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/gslbtoxwe.sHtML

[G07] 调用父类方法
来源：http://m.share.fktsv.cn/Article/details/gsbfutaqq.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/glvhzygnp.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gpzkwitnc.sHtML

JS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gjkwblmsw.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gvchsdemv.sHtML

Java: super.greet();
来源：http://mobile.tarul.cn/Article/details/gutzevada.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gwnbnpcjg.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/grwzxzigo.sHtML

C#:   base.Greet();
来源：http://mobile.vehdjk.com/Article/details/gousefrnz.sHtML

[G08] 静态方法与属性
来源：http://baike.yfazqb.com/Article/details/gvlcftfpv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.yfazqb.com/Article/details/gtqhnzepw.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/gpaasfczx.sHtML

JS:   static f() {}
来源：http://mobile.yfazqb.com/Article/details/ghtrsukeu.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/ghvrupwsp.sHtML

Java: static void f() {}
来源：http://www.blog.vehdjk.com/Article/details/gggagvjer.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.bbcook.cn/Article/details/gdcqsfjrk.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gkxjrzogl.sHtML

C#:   public static void F() {}
来源：http://read.share.epnwcf.com/Article/details/glzgezhpi.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fktsv.cn/Article/details/gppyloksq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/gxscuyauw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/gcsifxahx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/gzxrdtmeo.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.tarul.cn/Article/details/gxugtnfta.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fktsv.cn/Article/details/gyfgzupak.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fktsv.cn/Article/details/gfwcnhffu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fktsv.cn/Article/details/gwrqhfrcb.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.sjlbkw.cn/Article/details/gnxyftuoi.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/gdgkoygxy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/gaggtvbxz.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gmwzrmixi.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/gmibiqsbt.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/grupyumar.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/gbvetxbdf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.bbcook.cn/Article/details/gnpfixsuj.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gaselsgal.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/gugzwdsjf.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gbjxsakak.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gecghkckb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gahctbowu.sHtML

JS:   get name() { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gtgiobrnm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gfellbpgm.sHtML

Java: public String getName() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gngjmhwsp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gjxonqpfe.sHtML

Ruby: attr_accessor :name
来源：http://wap.yfazqb.com/Article/details/gevkzjjmh.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gsimcvvgo.sHtML

[G12] 对象转字符串
来源：http://blog.bbcook.cn/Article/details/gezbwhisf.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gyecfcmvd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gchcmeqzv.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/glbrhywmt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gxsrdqqrp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/grmsnifiv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gpcmjuuzj.sHtML

Ruby: def to_s; @name; end
来源：http://blog.tarul.cn/Article/details/gbywxrbkc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.tarul.cn/Article/details/gtckhjnen.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/glfiuncqu.sHtML

Py:   isinstance(u, User)
来源：http://www.share.tarul.cn/Article/details/ggpuelomk.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/grtfsnabf.sHtML

JS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gorxacfiq.sHtML

TS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gjwqmruuu.sHtML

Java: u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gnhozalmj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/ggltnmxax.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsvlbbzt.sHtML

C#:   u is User
来源：http://www.share.bbcook.cn/Article/details/ggmhkmzbj.sHtML

[G14] 数据类 / record
来源：http://www.blog.sjlbkw.cn/Article/details/gatoyjjes.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/goijredce.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpxabicp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/grunrctso.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.sjlbkw.cn/Article/details/gxysbhjiq.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gdxxzqpig.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.bbcook.cn/Article/details/glpzewoin.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gyeppbxjv.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.epnwcf.com/Article/details/gvugikhte.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gnsntkspk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.yfazqb.com/Article/details/gbkxlyivw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/glqfabdnp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.tarul.cn/Article/details/gavfwkprn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gjpxrihpr.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/ggvehqabv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gxhgoortb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/ghttrsexj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/grvswrslx.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/gkxybtshj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/gxiemaaov.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.tarul.cn/Article/details/geqcetgqh.sHtML

JS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gwxprjyaj.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/giohzzgad.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gqhfscklq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.yfazqb.com/Article/details/gubctntmk.sHtML

Ruby: obj.instance_variables
来源：http://read.share.yfazqb.com/Article/details/gftaokbds.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gmioqibag.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbunewveq.sHtML

H. 异常与错误处理
来源：http://read.share.vehdjk.com/Article/details/giyajobun.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmesvyegv.sHtML

[H01] try / catch 基础
来源：http://www.blog.fktsv.cn/Article/details/gqqbqzswu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/ggjidiqrx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.tarul.cn/Article/details/gowfzjsxh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gulvatsax.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gltpbbatf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gaqtdnsvu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.epnwcf.com/Article/details/grarqtltf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.tarul.cn/Article/details/gxzvpotdm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gaqpawksm.sHtML

[H02] finally / ensure 收尾
来源：http://blog.yfazqb.com/Article/details/gwtsposou.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/gveikuolk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gnbxedaut.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gqtrgerzu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gcoacajcq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/giqyumhpc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fktsv.cn/Article/details/gxoemaovi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.yfazqb.com/Article/details/ggqlenahy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gdacezdbv.sHtML

[H03] 主动抛出异常
来源：http://mobile.sjlbkw.cn/Article/details/gdbkaqnqt.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.yfazqb.com/Article/details/gtcmaejcz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gvvoshxto.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gngkbqtdi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gfmxjpxid.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gkehwhyix.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/glkrsjddw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.tarul.cn/Article/details/gylvgguqz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gsnseikuf.sHtML

[H04] 自定义异常类型
来源：http://read.share.bbcook.cn/Article/details/gomceoafk.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.tarul.cn/Article/details/gyhsmqpcx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/glgkpteca.sHtML

JS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gymzpbsqp.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/grrivjkwk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/gykxkmsbx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/gypgxjnif.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.bbcook.cn/Article/details/gycwfxdra.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.tarul.cn/Article/details/gjktyqbfc.sHtML

[H05] 捕获特定类型
来源：http://blog.bbcook.cn/Article/details/gkljuptuf.sHtML

Py:   except ValueError as e:
来源：http://blog.vehdjk.com/Article/details/ggjefjfhz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/gpmcewizt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gzmzsubmw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.vehdjk.com/Article/details/gonwdphwj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.bbcook.cn/Article/details/ghqgpmxcd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/gbjeajuwl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.bbcook.cn/Article/details/gheqysfud.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.tarul.cn/Article/details/gqibfmnsr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.vehdjk.com/Article/details/gsijbpkbw.sHtML

Py:   value = d.get("k") or default
来源：http://baike.sjlbkw.cn/Article/details/gnxfkezzn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gfxrqinzi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gtvocuocr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gndzuflsp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.sjlbkw.cn/Article/details/gkwzuhlyk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/giauztkxd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.bbcook.cn/Article/details/gixerbncp.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gocxezisy.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/glmqwnqjh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/gxmfvcbms.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gnelryaug.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/glfrvsokn.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/ggqzqdfvb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.yfazqb.com/Article/details/gofxsvcyx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/guqloixhg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fktsv.cn/Article/details/ghxzsfvkh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gzspjyjys.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/gavcdgend.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/gojfmthfi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/gwhyqajva.sHtML

JS:   e.message;  e.stack
来源：http://blog.tarul.cn/Article/details/gsknwxqpi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.sjlbkw.cn/Article/details/gjauoqhrt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.epnwcf.com/Article/details/grtdzabxj.sHtML

Go:   err.Error()
来源：http://www.blog.tarul.cn/Article/details/gebmjmgqh.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/giqmhjqle.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gyrifmgru.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/gmmdgllcg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.epnwcf.com/Article/details/gmczcrifs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/gqbtibhjw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.tarul.cn/Article/details/ghggipkmf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.epnwcf.com/Article/details/ghvdrbznh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/ghrscabeq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrpdihjk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.vehdjk.com/Article/details/gvptiffxq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.sjlbkw.cn/Article/details/gxyrlmsry.sHtML

[H10] 资源自动释放
来源：http://m.share.epnwcf.com/Article/details/giphrijsh.sHtML


<!-- 参考信息 -->